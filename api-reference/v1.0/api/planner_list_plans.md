# <a name="list-plans"></a>列出计划

检索 **plannerplan** 对象列表。
### <a name="prerequisites"></a>先决条件
要执行此 API，需要以下**范围**： 

*Group.Read.All*

### <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
GET /planner/plans
```
### <a name="optional-query-parameters"></a>可选的查询参数
此方法要求指定所有者[筛选器](http://graph.microsoft.io/docs/overview/query_parameters)。

### <a name="request-headers"></a>请求标头
| 名称      |说明|
|:----------|:----------|
| Authorization  | Bearer <code>|

### <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。
### <a name="response"></a>响应
如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [plannerPlan](../resources/plannerplan.md) 对象集合。

此方法可以返回任何 [HTTP 状态代码](../../../concepts/errors.md)。应用应当为此方法处理的最常见的错误为 403 和 404 响应。有关这些错误的详细信息，请参阅[常见规划器错误情况](../resources/planner_overview.md#common-planner-error-conditions)。

### <a name="example"></a>示例
##### <a name="request"></a>请求
下面是一个请求示例。
<!-- {
  "blockType": "request",
  "name": "get_plans"
}-->
```http
GET https://graph.microsoft.com/v1.0/planner/plans
```
##### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerPlan",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 421

{
  "value": [
    {
      "createdBy": {
        "application": {
          "id": "95e27074-6c4a-447a-aa24-9d718a0b86fa"
        },
        "user": {
          "id": "ebf3b108-5234-4e22-b93d-656d7dae5874"
        }
      },
      "createdDateTime": "2015-03-30T18:36:49.2407981Z",
      "owner": "ebf3b108-5234-4e22-b93d-656d7dae5874",
      "title": "title-value",
      "id": "xqQg5FS2LkCp935s-FIFm2QAFkHM"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List plans",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->