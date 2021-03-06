<a id="plannerbucket-resource-type" class="xliff"></a>

# plannerBucket 资源类型

**plannerBucket** 资源表示 Office 365 计划中的任务的存储桶（或“自定义列”）。它包含在 [plannerPlan](plannerPlan.md) 之中，并且可能具有 [plannerTasks](plannerTask.md) 集合。



<a id="methods" class="xliff"></a>

## 方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[Get plannerBucket](../api/plannerbucket_get.md) | [plannerBucket](plannerbucket.md) |读取 **plannerBucket** 对象的属性和关系。|
|[List plannerTasks](../api/plannerbucket_list_tasks.md) |[plannerTask](plannertask.md) collection| 获取 **plannerTask** 对象集合。|
|[Create](../api/planner_post_buckets.md) | [plannerBucket](plannerbucket.md)   | 新建 **plannerBucket** 对象。 |
|[Update](../api/plannerbucket_update.md) | [plannerBucket](plannerbucket.md)   |更新 **plannerBucket** 对象。 |
|[Delete](../api/plannerbucket_delete.md) | 无 |删除 **plannerBucket** 对象。 |

<a id="properties" class="xliff"></a>

## 属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|id|String| 只读。存储桶 ID。长度为 28 个字符，区分大小写。[格式验证](planner_identifiers_disclaimer.md)在服务上完成。|
|name|String|存储桶的名称。|
|orderHint|String|提示用于为列表视图中的此类项目排序。[此处](planner_order_hint_format.md)概述了此格式。|
|planId|String|此存储桶所属的计划 ID。|

<a id="relationships" class="xliff"></a>

## 关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|tasks|[plannerTask](plannertask.md) collection| 只读。可为 NULL。存储桶中的任务集合。|

<a id="json-representation" class="xliff"></a>

## JSON 表示形式
下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerBucket"
}-->

```json
{
  "id": "String (identifier)",
  "name": "String",
  "orderHint": "String",
  "planId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerBucket resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->