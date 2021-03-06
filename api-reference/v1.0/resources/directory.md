# <a name="directory-resource-type-deleted-items"></a>目录资源类型（已删除的项目）

表示目录中已删除的项目。 删除某个项目后，它会被添加到已删除项目“容器”中。 已删除的项目将保留最多 30 天的还原时间。 30 天后，这些项目将永久删除。

目前，已删除的项目功能仅支持用于 Office 365 [groups](group.md) 和 [users](users.md)。

## <a name="methods"></a>方法

| 方法         | 返回类型 | 说明 |
|:---------------|:------------|:------------|
|[Get deleted item](../api/directory_deleteditems_get.md) | [directoryObject](directoryobject.md) | 获取已删除项目的属性。 |
|[Restore deleted item](../api/directory_deleteditems_restore.md) |[directoryObject](directoryobject.md)| 还原最近删除的项目。 |
|[List deleted items](../api/directory_deleteditems_list.md) |[directoryObject](directoryobject.md) 集合| 获取最近删除的项目列表。 |
|[Permanently delete an item](../api/directory_deleteditems_delete.md) | 无 | 永久删除项目。 |

## <a name="properties"></a>属性
| 属性   | 类型 |说明|
|:---------------|:--------|:----------|
|id|String| 对象的唯一标识符；例如，12345678-9abc-def0-1234-56789abcde。 键。 不可为 null。 只读。|

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|DeletedItems|[directoryObject](directoryobject.md) 集合| 最近删除的项目。 只读。 可为 Null。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.directory"
}-->

```json
{
  "id": "String (identifier)"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directory resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->