# <a name="opentypeextension-resource-type-open-extensions"></a>openTypeExtension 资源类型（开放扩展）

借助开放扩展（旧称为“Office 365 数据扩展”），可以直接将泛型属性轻松添加到 Microsoft Graph 中的资源。 

开放扩展由 **openTypeExtension** 资源表示。 添加到资源的所有开放扩展都会显示在派生自 [extension](extension.md) 抽象类型的 **extensions** 导航属性中。 每个扩展都有 **extensionName** 属性（这是所有扩展的预定义唯一可写属性）和自定义数据。 

一种有助于确保扩展名称唯一性的方法是，使用反向域名系统 (DNS) 格式，此格式依赖_用户自己的域_。例如，`Com.Contoso.ContactInfo`。 请勿在扩展名称中使用 Microsoft 域（`Com.Microsoft` 或 `Com.OnMicrosoft`）。

开放扩展示例：[使用开放扩展向用户添加自定义数据](../../../concepts/extensibility_open_users.md)

一般可用性（GA: /v1.0 和 /beta）或预览版 (/beta) 对应版本中的以下资源支持开放扩展。

|资源 |版本 |
|:---------------|:-------|
| [管理单元](../../beta/resources/administrativeunit.md)  | 仅供预览 |
| [日历事件](event.md) | GA |
| 组[日历事件](event.md) | GA |
| 组对话线程[帖子](post.md) | GA |
| [设备](device.md) | GA |
| [组](group.md) | GA |
| [邮件](message.md) | GA |
| [组织](organization.md) | GA |
| [个人联系人](contact.md) | GA |
| [用户](user.md) | GA |

### <a name="use-open-extensions-for-outlook-resources-or-extended-properties"></a>使用开放扩展（针对 Outlook 资源）还是使用扩展属性？

开放扩展是大部分涉及存储和访问自定义数据的应用场景的推荐解决方案。不过，如果需要访问尚未通过 [Microsoft Graph API 元数据](http://developer.microsoft.com/en-us/graph/docs/overview/call_api)公开的 Outlook MAPI 属性的自定义数据，则可以使用[扩展属性及其 REST API](extended-properties-overview.md)。若要确认元数据公开了哪些属性，请访问 https://graph.microsoft.com/v1.0/$metadata。


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.opentypeextension"
}-->

```json
{
  "extensionName": "string",
  "id": "string (identifier)"
}

```

<br/>

## <a name="properties"></a>属性

|属性      |类型    |说明 |
|:---------------|:--------|:----------|
|extensionName|String|开放类型开放扩展的唯一文本标识符。必需。|
|id|String| 连接具有 **extensionName** 扩展类型的完全限定的标识符 。只读。|

## <a name="relationships"></a>关系

无


## <a name="methods"></a>方法

|方法        |返回类型 |说明 |
|:---------------|:--------|:----------|
|[Post](../api/opentypeextension_post_opentypeextension.md) | [openTypeExtension](opentypeextension.md)（在现有资源实例中），或包含 openTypeExtension 对象的新 [contact](../resources/contact.md)、[event](../resources/event.md) 或 [message](../resources/message.md)。 | 在现有的或新的资源实例中创建 openTypeExtension 对象。|
|[获取](../api/opentypeextension_get.md) | [openTypeExtension](opentypeextension.md) |读取 openTypeExtension 对象的属性和关系。|
|[更新](../api/opentypeextension_update.md) | [openTypeExtension](opentypeextension.md)   |更新 openTypeExtension 对象。 |
|[删除](../api/opentypeextension_delete.md) | 无 |删除 openTypeExtension 对象。 |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "openTypeExtension resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
