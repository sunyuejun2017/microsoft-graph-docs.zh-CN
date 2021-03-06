#  <a name="use-delta-query-to-track-changes-in-microsoft-graph-data"></a>使用增量查询跟踪 Microsoft Graph 数据更改

Delta 查询使应用程序能够发现新创建、更新或删除的实体，无需使用每个请求对目标资源执行完全读取。Microsoft Graph 应用程序可以使用 delta 查询和本地数据存储高效地同步更改。

## <a name="use-delta-query-to-track-changes-in-a-resource-collection"></a>使用 delta 查询来跟踪资源集合的更改

通常的调用模式如下：

1.  应用程序首先对所需资源运行 delta 函数以调用 GET 请求。
2.  Microsoft Graph 发送一个包含已请求资源和[状态令牌](#state-tokens)的响应。

     a.如果返回了 `nextLink` URL，则会话中可能存在要检索的其他数据页面。应用程序继续使用 `nextLink` URL 发出请求以检索所有页面中的数据，直到响应中返回 `deltaLink` URL。

     b.如果返回了 `deltaLink` URL，则未返回关于资源现有状态的更多数据。为了执行以后的请求，应用程序使用 `deltaLink` URL 了解资源更改。
     
3.  当应用程序需要了解资源更改时，会使用步骤 2 中收到的 `deltaLink` URL 发出新请求。*可能*在完成步骤 2 或应用程序检查更改时立即发出此请求。
4.  Microsoft Graph 返回响应，描述自上一个请求以来的资源更改和 `nextLink` URL 或 `deltaLink` URL。

### <a name="state-tokens"></a>状态令牌

增量查询 GET 响应中始终返回 `nextLink` 或 `deltaLink` 响应头中指定的 URL。`nextLink` URL 包含的是 _skipToken_，`deltaLink` URL 包含的是 _deltaToken_。 

这些令牌对客户端不透明。以下是需要了解的详细信息：

- 每个令牌都反映状态，并表示一轮更改跟踪中的响应快照。 
- 状态令牌还会进行编码，并包括初始 delta 查询请求中指定的其他查询参数（如 `$select`）。因此，不需要在后续 delta 查询请求中重复这些操作。
- 执行增量查询时，可以将 `nextLink` 或 `deltaLink` URL 复制并应用到下一个 **delta** 函数调用，无需检查 URL 的内容（包括其状态令牌）。


### <a name="optional-query-parameters"></a>可选的查询参数

如果客户使用查询参数，则它必须在初始请求中指定。Microsoft Graph 自动将指定参数编码为响应中提供的 `nextLink` 或 `deltaLink`。调用应用程序只需预先指定其所需的查询参数一次。Microsoft Graph 将为所有后续请求自动添加指定参数。

对于用户和组，在使用某些查询参数时受到限制：

-   如果使用的是 `$select` 查询参数，则该参数表示客户倾向于仅跟踪 `$select` 语句中指定的属性或关系的更改。如果未选中的属性发生更改，则属性已更改的资源将不会出现在后续请求之后的 delta 响应中。
-   不支持 `$expand`。

对于用户和组 API，作用域筛选器允许按 objectId 跟踪对一个或多个特定用户或组所做的更改。例如，下面的请求：https://graph.microsoft.com/beta/groups/delta/?$filter= id eq '477e9fc6-5de7-4406-bb2a-7e5c83c9ae5f' or id eq '004d6a07-fe70-4b92-add5-e6e37b8acd8e' 返回对与在查询筛选器中指定的 ID 相匹配的组的更改。 

## <a name="resource-representation-in-the-delta-query-response"></a>delta 查询响应中的资源表示形式

-   在 delta 查询响应中，使用标准表示形式表示受支持资源的新建实例。

-   更新实例由它们的 **id** 表示，*至少*具有已更新的属性，但可能也包含其他属性。

-   用户和组的关系表示为对标准资源表示形式的注释。这些注释使用格式 `propertyName@delta`。注释包含在初始 delta 查询请求的响应内。

删除的实例使用其 **id** 和 `@removed` 对象表示。`@removed` 对象可能包含有关为何删除该实例的其他信息。例如，"@removed": {"reason": “changed”}。

可能的 @removed 原因可以是*已更改*或*已删除*。
- *已更改*表示该项已被删除，可以从 [deletedItems](../api-reference/beta/resources/directory.md) 恢复。
- *已删除*表示该项已被删除，无法恢复。

`@removed` 对象可以在初始 delta 查询响应和跟踪的 (deltaLink) 响应中返回。使用 delta 查询请求的客户端应能够处理响应中的这些对象。

## <a name="supported-resources"></a>支持的资源

目前，以下资源支持 delta 查询。

| **资源集合** | **API** |
|:------ | :------ |
| 主日历的日历视图（日期范围）中的事件 | [事件](../api-reference/v1.0/resources/event.md)资源的 [delta](../api-reference/v1.0/api/event_delta.md) 函数 |
| 组 | [组](../api-reference/v1.0/resources/group.md)资源的 [delta](../api-reference/v1.0/api/group_delta.md) 函数 |
| 邮件文件夹 | [邮件文件夹](../api-reference/v1.0/resources/mailFolder.md)资源的 [delta](../api-reference/v1.0/api/mailfolder_delta.md) 函数 |
| 文件夹中的邮件 | [邮件](../api-reference/v1.0/resources/message.md)资源的 [delta](../api-reference/v1.0/api/message_delta.md) 函数 | 
| 私人联系人文件夹 | [联系人文件夹](../api-reference/v1.0/resources/contactfolder.md)资源的 [delta](../api-reference/v1.0/api/contactfolder_delta.md) 函数 |
| 文件夹中的私人联系人 | [联系人](../api-reference/v1.0/resources/contact.md)资源的 [delta](../api-reference/v1.0/api/contact_delta.md) 函数 |
| 用户 | [用户](../api-reference/v1.0/resources/user.md)资源的 [delta](../api-reference/v1.0/api/user_delta.md) 函数 | 
| 驱动器项目\* | [driveItem](../api-reference/v1.0/resources/driveitem.md) 资源的 [delta](../api-reference/v1.0/api/driveitem_delta.md) 函数 |
| Planner 项目\*\* | [plannerUser](../api-reference/beta/resources/planneruser.md) 资源所有段的 [delta](../api-reference/beta/api/planneruser_list_delta.md) 函数（预览版） |

> \* OneDrive 资源的使用模式与其他支持资源类似，仅存在一些小的语法差异。为了与其他资源类型保持一致，适用于驱动器的 delta 查询今后将进行更新。若要详细了解现行语法，请参阅[跟踪驱动器更改](https://developer.microsoft.com/zh-CN/graph/docs/api-reference/v1.0/api/item_delta)。

> \*\* Planner 资源的使用模式与其他支持资源类似，仅存在些许差异。  有关详细信息，请参阅[跟踪 Planner 更改](../api-reference/beta/api/planneruser_list_delta.md)。

## <a name="prerequisites"></a>先决条件

在对某个特定资源执行 delta 查询时也需要读取该资源所需的相同[权限](./permissions_reference.md)。

## <a name="delta-query-request-examples"></a>delta 查询请求示例 

- [获取日历视图中事件的增量更改](../concepts/delta_query_events.md)
- [获取文件夹中邮件的增量更改](./delta_query_messages.md)
- [获取组的增量更改](./delta_query_groups.md)
- [获取用户的增量更改](./delta_query_users.md)
