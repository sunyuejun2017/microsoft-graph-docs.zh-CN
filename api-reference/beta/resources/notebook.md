# <a name="notebook-resource-type"></a>notebook 资源类型

OneNote 笔记本。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "sectionGroups",
    "sections"
  ],
  "@odata.type": "microsoft.graph.notebook"
}-->

```json
{
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "isDefault": true,
  "isShared": true,
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "links": {"@odata.type": "microsoft.graph.notebookLinks"},
  "displayName": "string",
  "sectionGroupsUrl": "string",
  "sectionsUrl": "string",
  "self": "string",
  "userRole": "String"
}

```
## <a name="properties"></a>属性
| 属性       | 类型    |说明|
|:---------------|:--------|:----------|
|createdBy|[identitySet](identityset.md)|识别创建项目的用户、设备和应用程序。只读。|
|createdDateTime|DateTimeOffset|笔记本的创建日期和时间。时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。只读。|
|id|String|笔记本的唯一标识符。只读。|
|isDefault|Boolean|指示其是否是用户的默认笔记本。只读。|
|isShared|Boolean|指示是否共享笔记本。如果为 true，则笔记本的内容可供除所有者之外的人员查看。只读。|
|lastModifiedBy|[identitySet](identityset.md)|识别创建项目的用户、设备和应用程序。只读。|
|lastModifiedDateTime|DateTimeOffset|上次修改笔记本的日期和时间。时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。只读。|
|links|[NotebookLinks](notebooklinks.md)|用于打开笔记本的链接。如果安装了 OneNote 本机客户端，则 `oneNoteClientURL` 链接将在其中打开笔记本。`oneNoteWebURL` 链接将在 OneNote Online 中打开笔记本。|
|displayName|String|笔记本的名称。|
|sectionGroupsUrl|String|`sectionGroups` 导航属性的 URL，其将返回笔记本中的所有分区组。只读。|
|sectionsUrl|String|`sections` 导航属性的 URL，其将返回笔记本中的所有分区。只读。|
|self|String|可以在其中获取关于笔记本的详细信息的终结点。只读。|
|userRole|String|可能的值是：`Owner`、`Contributor`、`Reader`、`None`。“所有者”表示对笔记本的所有者级别访问权限。“参与者”表示对笔记本的读写访问权限。“读者”表示对笔记本的只读访问权限。只读。|

## <a name="relationships"></a>关系
| 关系 | 类型    |说明|
|:---------------|:--------|:----------|
|sectionGroups|[SectionGroup](sectiongroup.md) collection|笔记本中的分区组。只读。可为 NULL。|
|sections|[Section](section.md) collection|笔记本中的分区。只读。可为 Null。|

## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[Get notebook](../api/notebook_get.md) | [Notebook](notebook.md) |读取笔记本的属性和关系。|
|[Create section group](../api/notebook_post_sectiongroups.md) |[SectionGroup](sectiongroup.md)| 通过发布到指定笔记本中的 sectionGroups 集合创建分区组。|
|[List section groups](../api/notebook_list_sectiongroups.md) |[SectionGroup](sectiongroup.md) collection| 获取指定笔记本中的分区组集合。|
|[Create section](../api/notebook_post_sections.md) |[Section](section.md)| 通过发布到指定笔记本中的分区集合创建分区。|
|[List sections](../api/notebook_list_sections.md) |[Section](section.md) collection| 获取指定笔记本中的分区集合。|
|[copyNotebook](../api/notebook_copynotebook.md)| 无 | 复制笔记本。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "notebook resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
