# <a name="onenote-resource-type"></a>Onenote 资源类型

适用于 Onenote 资源的入口点。

所有通过 Microsoft Graph API 对 OneNote 服务的调用都使用此服务根 URL：

```
https://graph.microsoft.com/{version}/{location}/onenote/ 
```

位置可以是 Office 365 或消费者版 OneDrive 上的用户笔记本，还可以是 Office 365 上的组笔记本或 SharePoint 站点托管的团队笔记本。 

**用户笔记本** 要访问消费者版 OneDrive 或 OneDrive for Business 上的个人笔记本，请使用下列 URL 之一：

```
https://graph.microsoft.com/{version}/me/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{userPrincipalName}/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

**组笔记本** 要访问组所有的笔记本，请使用下列服务根 URL：

```
https://graph.microsoft.com/{version}/groups/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
**SharePoint 站点笔记本** 要访问 SharePoint 团队网站所有的笔记本，请使用下列服务根 URL：

```
https://graph.microsoft.com/{version}/sites/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
## <a name="authorization"></a>授权

有关使用 OneNote API 所需权限的信息，请参阅 [Notes permissions](../../../concepts/permissions_reference.md#notes-permissions)。


## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|笔记本|[笔记本](notebook.md)集合|用户或组所有的 OneNote 笔记本集合。只读。可为 NULL。|
|操作|[操作](onenoteoperation.md)集合 |OneNote 操作状态。不支持获取操作集合，但如果响应中返回 `Operation-Location` 标头，可以获取长时间运行的操作的状态。只读。可为 NULL。|
|页面|[页面](page.md)集合|用户或组所有的全部 OneNote 笔记本中的页面。只读。可为 NULL。|
|资源|[资源](resource.md)集合 |OneNote 页面中的图像和其他文件资源。不支持获取资源集合，但可以[获取特定资源的二进制内容](resource.md)。只读。可为 NULL。|
|sectionGroups|[SectionGroup](sectiongroup.md) 集合|用户或组所有的全部 OneNote 笔记本中的分区组。只读。可为 NULL。|
|节|[节](section.md)集合|用户或组所有的全部 OneNote 笔记本中的节。只读。可为 Null。|

## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[创建笔记本](../api/onenote_post_notebooks.md) |[笔记本](notebook.md)| 通过发布到笔记本集合创建笔记本。|
|[列出笔记本](../api/onenote_list_notebooks.md) |[笔记本](notebook.md)集合| 获取笔记本的集合。|
|[创建页面](../api/onenote_post_pages.md) |[页面](page.md)| 通过发布到页面集合创建页面。|
|[列出页面](../api/onenote_list_pages.md) |[页面](page.md)集合| 获取页面的集合。|
|[列出分区组](../api/onenote_list_sectiongroups.md) |[SectionGroup](sectiongroup.md) 集合| 获取分区组的集合。|
|[列出节](../api/onenote_list_sections.md) |[节](section.md)集合| 获取节的集合。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenote resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
