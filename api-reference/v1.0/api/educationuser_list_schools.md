# <a name="list-schools"></a><span data-ttu-id="f37e2-101">列出学校</span><span class="sxs-lookup"><span data-stu-id="f37e2-101">List schools</span></span>

<span data-ttu-id="f37e2-102">检索用户所在的学校列表。</span><span class="sxs-lookup"><span data-stu-id="f37e2-102">Retrieve a list of licenseDetails objects for a user.</span></span>

><span data-ttu-id="f37e2-103">**注意：**如果使用委派令牌，成员只能看到有关自己学校的信息。</span><span class="sxs-lookup"><span data-stu-id="f37e2-103">**Note:** If the delegated token is used, members can only see information about their own schools.</span></span> <span data-ttu-id="f37e2-104">在这种情况下，使用 `...beta/education/me/schools` 资源。</span><span class="sxs-lookup"><span data-stu-id="f37e2-104">Use the `...beta/education/me/schools` resource in this case.</span></span>

## <a name="permissions"></a><span data-ttu-id="f37e2-105">权限</span><span class="sxs-lookup"><span data-stu-id="f37e2-105">Permissions</span></span>
<span data-ttu-id="f37e2-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="f37e2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f37e2-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="f37e2-108">Permission type</span></span>      | <span data-ttu-id="f37e2-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f37e2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f37e2-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f37e2-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="f37e2-111">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="f37e2-111">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="f37e2-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f37e2-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="f37e2-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="f37e2-113">Not supported.</span></span>  |
|<span data-ttu-id="f37e2-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="f37e2-114">Application</span></span> | <span data-ttu-id="f37e2-115">EduRoster.Read.All、EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f37e2-115">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="f37e2-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f37e2-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/me/schools
GET /education/users/{id}/schools
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f37e2-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f37e2-117">Optional query parameters</span></span>
<span data-ttu-id="f37e2-118">此方法支持 [OData 查询参数](http://graph.microsoft.io/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f37e2-118">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f37e2-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="f37e2-119">Request headers</span></span>
| <span data-ttu-id="f37e2-120">标头</span><span class="sxs-lookup"><span data-stu-id="f37e2-120">Header</span></span>       | <span data-ttu-id="f37e2-121">值</span><span class="sxs-lookup"><span data-stu-id="f37e2-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f37e2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f37e2-122">Authorization</span></span>  | <span data-ttu-id="f37e2-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f37e2-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f37e2-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="f37e2-125">Request body</span></span>
<span data-ttu-id="f37e2-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f37e2-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="f37e2-127">响应</span><span class="sxs-lookup"><span data-stu-id="f37e2-127">Response</span></span>
<span data-ttu-id="f37e2-128">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [educationSchool](../resources/educationschool.md) 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="f37e2-128">If successful, this method returns a `200 OK` response code and collection of [groupSettingTemplate](../resources/educationschool.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f37e2-129">示例</span><span class="sxs-lookup"><span data-stu-id="f37e2-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f37e2-130">请求</span><span class="sxs-lookup"><span data-stu-id="f37e2-130">Request</span></span>
<span data-ttu-id="f37e2-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f37e2-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_schools"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/me/schools
```
##### <a name="response"></a><span data-ttu-id="f37e2-132">响应</span><span class="sxs-lookup"><span data-stu-id="f37e2-132">Response</span></span>
<span data-ttu-id="f37e2-133">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f37e2-133">The following is an example of the response.</span></span> 

><span data-ttu-id="f37e2-p104">**注意：**为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="f37e2-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSchool",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 345

{
  "value": [
    {
      "id": "10001",
      "displayName": "Contoso High School",
      "description": "Public 9-12 high school",
      "status": "active",
      "externalSource": "sis",
      "principalEmail": "amyr@contoso.com",
      "principalName": "Amy Roebuck",
      "externalPrincipalId": "14007",
      "highestGrade": "12",
      "lowestGrade": "9",
      "schoolNumber": "10001",
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
      "externalId": "10001",
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