<a id="plannerappliedcategories-resource-type" class="xliff"></a>

# plannerAppliedCategories 资源类型


**AppliedCategoriesCollection** 资源表示已应用于任务的类别（或标签）的集合。她是 [plannerTask](plannertask.md) 对象的组成部分。最多可向一个任务应用 6 个类别。类别说明，例如 `category1`、`category2` 等，是[计划详细信息](plannerplandetails.md)对象的组成部分。它是开放类型。

<a id="properties" class="xliff"></a>

## 属性
开放类型的属性可以由客户端定义。但是在这种情况下，在任务上应用相应的类别时客户端必须将 `category1`、`category2`、`category3`、`category4`、`category5` 和/或 `category6` 作为属性，且其值要为 `true` 布尔值。下面是一个示例。不应用这些类别时，则将属性值设置为 `false` 布尔值来自动删除属性。 

<a id="json-representation" class="xliff"></a>

## JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerAppliedCategories"
}-->

```json
{
  "String-value": true
}
```

示例： 

```json
{
  "category1": true,
  "category3": true,
  "category5": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerAppliedCategories resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->