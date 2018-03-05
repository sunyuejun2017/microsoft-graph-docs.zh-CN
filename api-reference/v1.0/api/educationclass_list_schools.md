# <a name="list-schools"></a><span data-ttu-id="bfc77-101">列出学校</span><span class="sxs-lookup"><span data-stu-id="bfc77-101">List schools</span></span>

<span data-ttu-id="bfc77-102">检索教授该课程的学校列表。</span><span class="sxs-lookup"><span data-stu-id="bfc77-102">Retrieve a list of schools in which the class is taught.</span></span>

## <a name="permissions"></a><span data-ttu-id="bfc77-103">权限</span><span class="sxs-lookup"><span data-stu-id="bfc77-103">Permissions</span></span>
<span data-ttu-id="bfc77-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="bfc77-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="bfc77-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="bfc77-106">Permission type</span></span>      | <span data-ttu-id="bfc77-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bfc77-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bfc77-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bfc77-108">Delegated (work or school account)</span></span> |  <span data-ttu-id="bfc77-109">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="bfc77-109">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="bfc77-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bfc77-110">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="bfc77-111">不支持</span><span class="sxs-lookup"><span data-stu-id="bfc77-111">Not supported</span></span>  |
|<span data-ttu-id="bfc77-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="bfc77-112">Application</span></span> | <span data-ttu-id="bfc77-113">EduRoster.Read.All、EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bfc77-113">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="bfc77-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bfc77-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/schools
```
## <a name="optional-query-parameters"></a><span data-ttu-id="bfc77-115">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="bfc77-115">Optional query parameters</span></span>
<span data-ttu-id="bfc77-116">此方法支持 [OData 查询参数](http://graph.microsoft.io/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="bfc77-116">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bfc77-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="bfc77-117">Request headers</span></span>
| <span data-ttu-id="bfc77-118">标头</span><span class="sxs-lookup"><span data-stu-id="bfc77-118">Header</span></span>       | <span data-ttu-id="bfc77-119">值</span><span class="sxs-lookup"><span data-stu-id="bfc77-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="bfc77-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="bfc77-120">Authorization</span></span>  | <span data-ttu-id="bfc77-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bfc77-p102">Bearer {token}. Required.</span></span>  |


## <a name="request-body"></a><span data-ttu-id="bfc77-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="bfc77-123">Request body</span></span>
<span data-ttu-id="bfc77-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="bfc77-124">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="bfc77-125">响应</span><span class="sxs-lookup"><span data-stu-id="bfc77-125">Response</span></span>
<span data-ttu-id="bfc77-126">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [educationSchool](../resources/educationschool.md) 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="bfc77-126">If successful, this method returns a `200 OK` response code and collection of [groupSettingTemplate](../resources/educationschool.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bfc77-127">示例</span><span class="sxs-lookup"><span data-stu-id="bfc77-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bfc77-128">请求</span><span class="sxs-lookup"><span data-stu-id="bfc77-128">Request</span></span>
<span data-ttu-id="bfc77-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="bfc77-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_schools"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/classes/11014/schools
```
##### <a name="response"></a><span data-ttu-id="bfc77-130">响应</span><span class="sxs-lookup"><span data-stu-id="bfc77-130">Response</span></span>
<span data-ttu-id="bfc77-131">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="bfc77-131">The following is an example of the response.</span></span> 

><span data-ttu-id="bfc77-p103">**注意：**为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="bfc77-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSchool",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 892

{
  "value": [
    {
      "id": "10002",
      "displayName": "Fabrikam High School",
      "description": "Magnate school for the arts. Los Angeles School District",
      "status": "String",
      "externalSource": "String",
      "principalEmail": "AmyR@fabrikam.com",
      "principalName": "Amy Roebuck",
      "externalPrincipalId": "14007",
      "highestGrade": "12",
      "lowestGrade": "9",
      "schoolNumber": "10002",
      "address": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      },
      "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
      },
      "externalId": "10002",
      "fax": "+1 (253) 555-0101",
      "phone": "+1 (253) 555-0102",
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List schools",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->