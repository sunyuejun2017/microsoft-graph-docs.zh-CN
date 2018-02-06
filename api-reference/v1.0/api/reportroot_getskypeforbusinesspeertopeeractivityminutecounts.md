# <a name="reportroot-getskypeforbusinesspeertopeeractivityminutecounts"></a><span data-ttu-id="b08b3-101">reportRoot: getSkypeForBusinessPeerToPeerActivityMinuteCounts</span><span class="sxs-lookup"><span data-stu-id="b08b3-101">reportRoot: getSkypeForBusinessPeerToPeerActivityMinuteCounts</span></span>

<span data-ttu-id="b08b3-102">获取使用情况趋势，即组织中召开的对等会话的时长（以分钟为单位）和类型。</span><span class="sxs-lookup"><span data-stu-id="b08b3-102">Get usage trends on the length in minutes and type of peer-to-peer sessions held in your organization.</span></span> <span data-ttu-id="b08b3-103">会话类型包括音频和视频。</span><span class="sxs-lookup"><span data-stu-id="b08b3-103">Types of sessions include audio and video.</span></span>

> <span data-ttu-id="b08b3-104">**注意：**若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Skype for Business 对等活动](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713)。</span><span class="sxs-lookup"><span data-stu-id="b08b3-104">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business peer-to-peer activity](https://support.office.com/client/Skype-for-Business-Online-peertopeer-activity-d3b2d569-4ee9-44b8-92bf-d518142f0713).</span></span>

## <a name="permissions"></a><span data-ttu-id="b08b3-105">权限</span><span class="sxs-lookup"><span data-stu-id="b08b3-105">Permissions</span></span>

<span data-ttu-id="b08b3-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="b08b3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="b08b3-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="b08b3-108">Permission type</span></span>                        | <span data-ttu-id="b08b3-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b08b3-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="b08b3-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b08b3-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="b08b3-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="b08b3-111">Not supported.</span></span>                           |
| <span data-ttu-id="b08b3-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b08b3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b08b3-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="b08b3-113">Not supported.</span></span>                           |
| <span data-ttu-id="b08b3-114">应用</span><span class="sxs-lookup"><span data-stu-id="b08b3-114">Application</span></span>                            | <span data-ttu-id="b08b3-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b08b3-115">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="b08b3-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b08b3-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessPeerToPeerActivityMinuteCounts(period='{period_value}')
```

## <a name="request-parameters"></a><span data-ttu-id="b08b3-117">请求参数</span><span class="sxs-lookup"><span data-stu-id="b08b3-117">Request parameters</span></span>

<span data-ttu-id="b08b3-118">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="b08b3-118">In the request URL, provide the following query parameter with a valid value.</span></span>

| <span data-ttu-id="b08b3-119">参数</span><span class="sxs-lookup"><span data-stu-id="b08b3-119">Parameter</span></span> | <span data-ttu-id="b08b3-120">类型</span><span class="sxs-lookup"><span data-stu-id="b08b3-120">Type</span></span>   | <span data-ttu-id="b08b3-121">说明</span><span class="sxs-lookup"><span data-stu-id="b08b3-121">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="b08b3-122">period</span><span class="sxs-lookup"><span data-stu-id="b08b3-122">period</span></span>    | <span data-ttu-id="b08b3-123">string</span><span class="sxs-lookup"><span data-stu-id="b08b3-123">string</span></span> | <span data-ttu-id="b08b3-124">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="b08b3-124">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="b08b3-125">受支持的 {Period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="b08b3-125">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="b08b3-126">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="b08b3-126">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="b08b3-127">必需。</span><span class="sxs-lookup"><span data-stu-id="b08b3-127">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="b08b3-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="b08b3-128">Request headers</span></span>

| <span data-ttu-id="b08b3-129">名称</span><span class="sxs-lookup"><span data-stu-id="b08b3-129">Name</span></span>          | <span data-ttu-id="b08b3-130">说明</span><span class="sxs-lookup"><span data-stu-id="b08b3-130">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="b08b3-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="b08b3-131">Authorization</span></span> | <span data-ttu-id="b08b3-p104">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="b08b3-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b08b3-134">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="b08b3-134">If-None-Match</span></span> | <span data-ttu-id="b08b3-135">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="b08b3-135">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="b08b3-136">可选。</span><span class="sxs-lookup"><span data-stu-id="b08b3-136">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="b08b3-137">响应</span><span class="sxs-lookup"><span data-stu-id="b08b3-137">Response</span></span>

<span data-ttu-id="b08b3-138">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="b08b3-138">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="b08b3-139">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="b08b3-139">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="b08b3-140">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="b08b3-140">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="b08b3-141">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="b08b3-141">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="b08b3-142">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="b08b3-142">Report Refresh Date</span></span>
- <span data-ttu-id="b08b3-143">报表日期</span><span class="sxs-lookup"><span data-stu-id="b08b3-143">Report Date</span></span>
- <span data-ttu-id="b08b3-144">报表周期</span><span class="sxs-lookup"><span data-stu-id="b08b3-144">Report Period</span></span>
- <span data-ttu-id="b08b3-145">音频</span><span class="sxs-lookup"><span data-stu-id="b08b3-145">Audio</span></span>
- <span data-ttu-id="b08b3-146">视频</span><span class="sxs-lookup"><span data-stu-id="b08b3-146">Video</span></span>

## <a name="example"></a><span data-ttu-id="b08b3-147">示例</span><span class="sxs-lookup"><span data-stu-id="b08b3-147">Example</span></span>

#### <a name="request"></a><span data-ttu-id="b08b3-148">请求</span><span class="sxs-lookup"><span data-stu-id="b08b3-148">Request</span></span>

<span data-ttu-id="b08b3-149">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b08b3-149">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinesspeertopeeractivityminutecounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessPeerToPeerActivityMinuteCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="b08b3-150">响应</span><span class="sxs-lookup"><span data-stu-id="b08b3-150">Response</span></span>

<span data-ttu-id="b08b3-151">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b08b3-151">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="b08b3-152">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="b08b3-152">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,Audio,Video
```