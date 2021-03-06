<a id="plannerbuckettaskboardtaskformat-resource-type" class="xliff"></a>

# plannerBucketTaskBoardTaskFormat 资源类型

**plannerBucketTaskBoardTaskFormat** 资源表示用于在“任务板”的“存储桶”视图（由被分配到的存储桶中的任务组成的视图）下正确呈现任务的信息。每个[任务](plannertask.md)均将有一个与其相关联的 **plannerBucketTaskBoardTaskFormat** 对象。


<a id="methods" class="xliff"></a>

## 方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[Get plannerBucketTaskBoardTaskFormat](../api/plannerbuckettaskboardtaskformat_get.md) | [plannerBucketTaskBoardTaskFormat](plannerbuckettaskboardtaskformat.md) |读取 **plannerBucketTaskBoardTaskFormat** 对象的属性和关系。|
|[Update](../api/plannerbuckettaskboardtaskformat_update.md) | [plannerBucketTaskBoardTaskFormat](plannerbuckettaskboardtaskformat.md)  |更新 **plannerBucketTaskBoardTaskFormat** 对象 |

<a id="properties" class="xliff"></a>

## 属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|id|String| 只读。资源的 ID。长度为 28 个字符，区分大小写。[格式验证](planner_identifiers_disclaimer.md)在服务上完成。|
|orderHint|String|用于对任务板存储桶视图中的任务进行排序的提示。[此处](planner_order_hint_format.md)概述了此格式。|

<a id="relationships" class="xliff"></a>

## 关系
无


<a id="json-representation" class="xliff"></a>

## JSON 表示形式
下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerBucketTaskBoardTaskFormat"
}-->

```json
{
  "id": "String (identifier)",
  "orderHint": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerBucketTaskBoardTaskFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->