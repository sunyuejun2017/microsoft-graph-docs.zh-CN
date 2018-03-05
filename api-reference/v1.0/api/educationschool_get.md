# <a name="get-educationschool"></a><span data-ttu-id="00dfd-101">获取 educationSchool</span><span class="sxs-lookup"><span data-stu-id="00dfd-101">Get educationSchool</span></span>

<span data-ttu-id="00dfd-102">检索 school 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="00dfd-102">Retrieve the properties and relationships of charttitle object.</span></span>

## <a name="permissions"></a><span data-ttu-id="00dfd-103">权限</span><span class="sxs-lookup"><span data-stu-id="00dfd-103">Permissions</span></span>
<span data-ttu-id="00dfd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="00dfd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="00dfd-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="00dfd-106">Permission type</span></span>      | <span data-ttu-id="00dfd-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="00dfd-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="00dfd-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="00dfd-108">Delegated (work or school account)</span></span> |  <span data-ttu-id="00dfd-109">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="00dfd-109">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="00dfd-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="00dfd-110">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="00dfd-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="00dfd-111">Not supported.</span></span>  |
|<span data-ttu-id="00dfd-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="00dfd-112">Application</span></span> | <span data-ttu-id="00dfd-113">EduRoster.Read.All、EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00dfd-113">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="00dfd-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="00dfd-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/schools
GET /education/me/schools
GET /education/users/schools
```
## <a name="optional-query-parameters"></a><span data-ttu-id="00dfd-115">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="00dfd-115">Optional query parameters</span></span>
<span data-ttu-id="00dfd-116">此方法支持 [OData 查询参数](http://graph.microsoft.io/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="00dfd-116">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="00dfd-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="00dfd-117">Request headers</span></span>
| <span data-ttu-id="00dfd-118">标头</span><span class="sxs-lookup"><span data-stu-id="00dfd-118">Header</span></span>       | <span data-ttu-id="00dfd-119">值</span><span class="sxs-lookup"><span data-stu-id="00dfd-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="00dfd-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="00dfd-120">Authorization</span></span>  | <span data-ttu-id="00dfd-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="00dfd-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="00dfd-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="00dfd-123">Request body</span></span>
<span data-ttu-id="00dfd-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="00dfd-124">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="00dfd-125">响应</span><span class="sxs-lookup"><span data-stu-id="00dfd-125">Response</span></span>
<span data-ttu-id="00dfd-126">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [educationSchool](../resources/educationschool.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="00dfd-126">If successful, this method returns a `200 OK` response code and an [event](../resources/educationschool.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="00dfd-127">示例</span><span class="sxs-lookup"><span data-stu-id="00dfd-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="00dfd-128">请求</span><span class="sxs-lookup"><span data-stu-id="00dfd-128">Request</span></span>
<span data-ttu-id="00dfd-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="00dfd-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_educationschool"
}-->
```http
GET https://graph.microsoft.com/v1.0/education/schools/10001
```
##### <a name="response"></a><span data-ttu-id="00dfd-130">响应</span><span class="sxs-lookup"><span data-stu-id="00dfd-130">Response</span></span>
<span data-ttu-id="00dfd-131">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="00dfd-131">The following is an example of the response.</span></span> 

><span data-ttu-id="00dfd-p103">**注意：**为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="00dfd-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSchool"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 292

{
  "schoolPrincipalEmail": "AmyRoebuck@contoso.com",
  "schoolPrincipalName": "Amy Roebuck",
  "externalSchoolPrincipalId": "14007",
  "lowestGrade": "9",
  "highestGrade": "12"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get educationSchool",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->