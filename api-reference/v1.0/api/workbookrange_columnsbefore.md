# <a name="workbookrange-columnsbefore"></a><span data-ttu-id="01005-101">workbookRange: columnsBefore</span><span class="sxs-lookup"><span data-stu-id="01005-101">workbookRange: columnsBefore</span></span>

<span data-ttu-id="01005-102">获取给定范围左侧的一定数量的列。</span><span class="sxs-lookup"><span data-stu-id="01005-102">Gets a certain number of columns to the left of the given range.</span></span>

## <a name="permissions"></a><span data-ttu-id="01005-103">权限</span><span class="sxs-lookup"><span data-stu-id="01005-103">Permissions</span></span>
<span data-ttu-id="01005-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="01005-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="01005-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="01005-106">Permission type</span></span>      | <span data-ttu-id="01005-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="01005-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="01005-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="01005-108">Delegated (work or school account)</span></span> | <span data-ttu-id="01005-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="01005-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="01005-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="01005-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="01005-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="01005-111">Not supported.</span></span>    |
|<span data-ttu-id="01005-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="01005-112">Application</span></span> | <span data-ttu-id="01005-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="01005-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="01005-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="01005-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/columnsBefore(count=n)

```
## <a name="request-headers"></a><span data-ttu-id="01005-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="01005-115">Request headers</span></span>
| <span data-ttu-id="01005-116">名称</span><span class="sxs-lookup"><span data-stu-id="01005-116">Name</span></span>       | <span data-ttu-id="01005-117">说明</span><span class="sxs-lookup"><span data-stu-id="01005-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="01005-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="01005-118">Authorization</span></span>  | <span data-ttu-id="01005-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="01005-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="01005-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="01005-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="01005-p103">确定是否保留更改的工作簿会话 ID。可选。</span><span class="sxs-lookup"><span data-stu-id="01005-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="parameters"></a><span data-ttu-id="01005-124">参数</span><span class="sxs-lookup"><span data-stu-id="01005-124">Parameters</span></span>

| <span data-ttu-id="01005-125">参数</span><span class="sxs-lookup"><span data-stu-id="01005-125">Parameter</span></span>    | <span data-ttu-id="01005-126">类型</span><span class="sxs-lookup"><span data-stu-id="01005-126">Type</span></span>   |<span data-ttu-id="01005-127">说明</span><span class="sxs-lookup"><span data-stu-id="01005-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="01005-128">count</span><span class="sxs-lookup"><span data-stu-id="01005-128">count</span></span>|<span data-ttu-id="01005-129">Int32</span><span class="sxs-lookup"><span data-stu-id="01005-129">Int32</span></span>|<span data-ttu-id="01005-p104">生成的范围中要包含的列数。一般来说，使用正数可以在当前范围之外创建一个范围。也可以使用负数在当前范围之内创建一个范围。默认值为 1。</span><span class="sxs-lookup"><span data-stu-id="01005-p104">The number of columns to include in the resulting range. In general, use a positive number to create a range outside the current range. You can also use a negative number to create a range within the current range. The default value is 1</span></span>|

## <a name="request-body"></a><span data-ttu-id="01005-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="01005-134">Request body</span></span>

### <a name="response"></a><span data-ttu-id="01005-135">响应</span><span class="sxs-lookup"><span data-stu-id="01005-135">Response</span></span>
<span data-ttu-id="01005-136">如果成功，此方法在响应正文中返回 `200, OK` 响应代码和 [workbookRange](../resources/range.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="01005-136">If successful, this method returns `200, OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="01005-137">示例</span><span class="sxs-lookup"><span data-stu-id="01005-137">Example</span></span>
<span data-ttu-id="01005-138">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="01005-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="01005-139">请求</span><span class="sxs-lookup"><span data-stu-id="01005-139">Request</span></span>
<span data-ttu-id="01005-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="01005-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrange_columnsbefore"
}-->
```http
POST https://graph.microsoft.com/v1.0/drive/root/workbook/worksheets/{id}/range/columnsBefore(count=2)
```

##### <a name="response"></a><span data-ttu-id="01005-141">响应</span><span class="sxs-lookup"><span data-stu-id="01005-141">Response</span></span>
<span data-ttu-id="01005-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="01005-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.range"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 157

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnHidden": true,
  "columnIndex": 99
}
```