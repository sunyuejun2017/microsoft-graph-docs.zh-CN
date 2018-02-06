# <a name="reportroot-getskypeforbusinessactivityuserdetail"></a><span data-ttu-id="d5439-101">reportRoot: getSkypeForBusinessActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="d5439-101">reportRoot: getSkypeForBusinessActivityUserDetail</span></span>

<span data-ttu-id="d5439-102">获取用户执行的 Skype for Business 活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="d5439-102">Get details about Skype for Business activity by user.</span></span>

> <span data-ttu-id="d5439-103">**注意：**若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Skype for Business 活动](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424)。</span><span class="sxs-lookup"><span data-stu-id="d5439-103">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business activity](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span></span>

## <a name="permissions"></a><span data-ttu-id="d5439-104">权限</span><span class="sxs-lookup"><span data-stu-id="d5439-104">Permissions</span></span>

<span data-ttu-id="d5439-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="d5439-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="d5439-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="d5439-107">Permission type</span></span>                        | <span data-ttu-id="d5439-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d5439-108">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="d5439-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d5439-109">Delegated (work or school account)</span></span>     | <span data-ttu-id="d5439-110">不支持。</span><span class="sxs-lookup"><span data-stu-id="d5439-110">Not supported.</span></span>                           |
| <span data-ttu-id="d5439-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d5439-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d5439-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="d5439-112">Not supported.</span></span>                           |
| <span data-ttu-id="d5439-113">应用</span><span class="sxs-lookup"><span data-stu-id="d5439-113">Application</span></span>                            | <span data-ttu-id="d5439-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5439-114">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="d5439-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d5439-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessActivityUserDetail(period='{period_value}')
GET /reports/getSkypeForBusinessActivityUserDetail(date={date_value})
```

## <a name="request-parameters"></a><span data-ttu-id="d5439-116">请求参数</span><span class="sxs-lookup"><span data-stu-id="d5439-116">Request parameters</span></span>

<span data-ttu-id="d5439-117">在请求 URL 中，提供以下参数之一的有效值。</span><span class="sxs-lookup"><span data-stu-id="d5439-117">In the request URL, provide the following query parameter with a valid value.</span></span>

| <span data-ttu-id="d5439-118">参数</span><span class="sxs-lookup"><span data-stu-id="d5439-118">Parameter</span></span> | <span data-ttu-id="d5439-119">类型</span><span class="sxs-lookup"><span data-stu-id="d5439-119">Type</span></span>   | <span data-ttu-id="d5439-120">说明</span><span class="sxs-lookup"><span data-stu-id="d5439-120">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="d5439-121">period</span><span class="sxs-lookup"><span data-stu-id="d5439-121">period</span></span>    | <span data-ttu-id="d5439-122">string</span><span class="sxs-lookup"><span data-stu-id="d5439-122">string</span></span> | <span data-ttu-id="d5439-123">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="d5439-123">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="d5439-124">受支持的 {Period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="d5439-124">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="d5439-125">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="d5439-125">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="d5439-126">date</span><span class="sxs-lookup"><span data-stu-id="d5439-126">date</span></span>      | <span data-ttu-id="d5439-127">Date</span><span class="sxs-lookup"><span data-stu-id="d5439-127">Date</span></span>   | <span data-ttu-id="d5439-128">指定要查看用户在哪个日期执行的任何活动。</span><span class="sxs-lookup"><span data-stu-id="d5439-128">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="d5439-129">{date_value} 必须采用格式 YYYY-MM-DD。</span><span class="sxs-lookup"><span data-stu-id="d5439-129">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="d5439-130">因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。</span><span class="sxs-lookup"><span data-stu-id="d5439-130">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="d5439-131">**注意：**需要在 URL 中设置 period 或 date。</span><span class="sxs-lookup"><span data-stu-id="d5439-131">**Note:** You need to set either period or date in the URL.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d5439-132">请求头</span><span class="sxs-lookup"><span data-stu-id="d5439-132">Request headers</span></span>

| <span data-ttu-id="d5439-133">名称</span><span class="sxs-lookup"><span data-stu-id="d5439-133">Name</span></span>          | <span data-ttu-id="d5439-134">说明</span><span class="sxs-lookup"><span data-stu-id="d5439-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="d5439-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="d5439-135">Authorization</span></span> | <span data-ttu-id="d5439-p104">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="d5439-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d5439-138">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="d5439-138">If-None-Match</span></span> | <span data-ttu-id="d5439-139">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="d5439-139">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="d5439-140">可选。</span><span class="sxs-lookup"><span data-stu-id="d5439-140">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="d5439-141">响应</span><span class="sxs-lookup"><span data-stu-id="d5439-141">Response</span></span>

<span data-ttu-id="d5439-142">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="d5439-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="d5439-143">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="d5439-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="d5439-144">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="d5439-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="d5439-145">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="d5439-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="d5439-146">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="d5439-146">Report Refresh Date</span></span>
- <span data-ttu-id="d5439-147">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="d5439-147">User Principal Name</span></span>
- <span data-ttu-id="d5439-148">已删除</span><span class="sxs-lookup"><span data-stu-id="d5439-148">Is Deleted</span></span>
- <span data-ttu-id="d5439-149">删除日期</span><span class="sxs-lookup"><span data-stu-id="d5439-149">Deleted Date</span></span>
- <span data-ttu-id="d5439-150">上次活动日期</span><span class="sxs-lookup"><span data-stu-id="d5439-150">Last Activity Date</span></span>
- <span data-ttu-id="d5439-151">对等会话总数</span><span class="sxs-lookup"><span data-stu-id="d5439-151">Total Peer-to-peer Session Count</span></span>
- <span data-ttu-id="d5439-152">组织会议总数</span><span class="sxs-lookup"><span data-stu-id="d5439-152">Total Organized Conference Count</span></span>
- <span data-ttu-id="d5439-153">参与会议总数</span><span class="sxs-lookup"><span data-stu-id="d5439-153">Total Participated Conference Count</span></span>
- <span data-ttu-id="d5439-154">对等会话的上次活动日期</span><span class="sxs-lookup"><span data-stu-id="d5439-154">Peer-to-peer Last Activity Date</span></span>
- <span data-ttu-id="d5439-155">组织会议的上次活动日期</span><span class="sxs-lookup"><span data-stu-id="d5439-155">Organized Conference Last Activity Date</span></span>
- <span data-ttu-id="d5439-156">参与会议的上次活动日期</span><span class="sxs-lookup"><span data-stu-id="d5439-156">Participated Conference Last Activity Date</span></span>
- <span data-ttu-id="d5439-157">对等 IM 次数</span><span class="sxs-lookup"><span data-stu-id="d5439-157">Peer-to-peer IM Count</span></span>
- <span data-ttu-id="d5439-158">对等音频次数</span><span class="sxs-lookup"><span data-stu-id="d5439-158">Peer-to-peer Audio Count</span></span>
- <span data-ttu-id="d5439-159">对等音频分钟数</span><span class="sxs-lookup"><span data-stu-id="d5439-159">Peer-to-peer Audio Minutes</span></span>
- <span data-ttu-id="d5439-160">对等视频次数</span><span class="sxs-lookup"><span data-stu-id="d5439-160">Peer-to-peer Video Count</span></span>
- <span data-ttu-id="d5439-161">对等视频分钟数</span><span class="sxs-lookup"><span data-stu-id="d5439-161">Peer-to-peer Video Minutes</span></span>
- <span data-ttu-id="d5439-162">对等应用共享次数</span><span class="sxs-lookup"><span data-stu-id="d5439-162">Peer-to-peer App Sharing Count</span></span>
- <span data-ttu-id="d5439-163">对等文件传输次数</span><span class="sxs-lookup"><span data-stu-id="d5439-163">Peer-to-peer File Transfer Count</span></span>
- <span data-ttu-id="d5439-164">组织会议 - IM 次数</span><span class="sxs-lookup"><span data-stu-id="d5439-164">Organized Conference IM Count</span></span>
- <span data-ttu-id="d5439-165">组织会议 - 音频/视频次数</span><span class="sxs-lookup"><span data-stu-id="d5439-165">Organized Conference Audio/Video Count</span></span>
- <span data-ttu-id="d5439-166">组织会议 - 音频/视频分钟数</span><span class="sxs-lookup"><span data-stu-id="d5439-166">Organized Conference Audio/Video Minutes</span></span>
- <span data-ttu-id="d5439-167">组织会议 - 应用共享次数</span><span class="sxs-lookup"><span data-stu-id="d5439-167">Organized Conference App Sharing Count</span></span>
- <span data-ttu-id="d5439-168">组织会议 - Web 次数</span><span class="sxs-lookup"><span data-stu-id="d5439-168">Organized Conference Web Count</span></span>
- <span data-ttu-id="d5439-169">组织会议 - 第三方拨入/拨出次数</span><span class="sxs-lookup"><span data-stu-id="d5439-169">Organized Conference Dial-in/out 3rd Party Count</span></span>
- <span data-ttu-id="d5439-170">组织会议 - Microsoft 拨入/拨出次数</span><span class="sxs-lookup"><span data-stu-id="d5439-170">Organized Conference Dial-in/out Microsoft Count</span></span>
- <span data-ttu-id="d5439-171">组织会议 - Microsoft 拨入分钟数</span><span class="sxs-lookup"><span data-stu-id="d5439-171">Organized Conference Dial-in Microsoft Minutes</span></span>
- <span data-ttu-id="d5439-172">组织会议 - Microsoft 拨出分钟数</span><span class="sxs-lookup"><span data-stu-id="d5439-172">Organized Conference Dial-out Microsoft Minutes</span></span>
- <span data-ttu-id="d5439-173">参与会议 - IM 次数</span><span class="sxs-lookup"><span data-stu-id="d5439-173">Paricipated Conference IM Count</span></span>
- <span data-ttu-id="d5439-174">参与会议 - 音频/视频次数</span><span class="sxs-lookup"><span data-stu-id="d5439-174">Participated Conference Audio/Video Count</span></span>
- <span data-ttu-id="d5439-175">参与会议 - 音频/视频分钟数</span><span class="sxs-lookup"><span data-stu-id="d5439-175">Participated Conference Audio/Video Minutes</span></span>
- <span data-ttu-id="d5439-176">参与会议 - 应用共享次数</span><span class="sxs-lookup"><span data-stu-id="d5439-176">Participated Conference App Sharing Count</span></span>
- <span data-ttu-id="d5439-177">参与会议 - Web 次数</span><span class="sxs-lookup"><span data-stu-id="d5439-177">Participated Conference Web Count</span></span>
- <span data-ttu-id="d5439-178">参与会议 - 第三方拨入/拨出次数</span><span class="sxs-lookup"><span data-stu-id="d5439-178">Participated Conference Dial-in/out 3rd Party Count</span></span>
- <span data-ttu-id="d5439-179">分配的产品</span><span class="sxs-lookup"><span data-stu-id="d5439-179">Assigned Products</span></span>
- <span data-ttu-id="d5439-180">报表周期</span><span class="sxs-lookup"><span data-stu-id="d5439-180">Report Period</span></span>

## <a name="example"></a><span data-ttu-id="d5439-181">示例</span><span class="sxs-lookup"><span data-stu-id="d5439-181">Example</span></span>

#### <a name="request"></a><span data-ttu-id="d5439-182">请求</span><span class="sxs-lookup"><span data-stu-id="d5439-182">Request</span></span>

<span data-ttu-id="d5439-183">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d5439-183">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessactivityuserdetail"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessActivityUserDetail(period='D7')
```

#### <a name="response"></a><span data-ttu-id="d5439-184">响应</span><span class="sxs-lookup"><span data-stu-id="d5439-184">Response</span></span>

<span data-ttu-id="d5439-185">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d5439-185">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="d5439-186">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="d5439-186">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Is Deleted,Deleted Date,Last Activity Date,Total Peer-to-peer Session Count,Total Organized Conference Count,Total Participated Conference Count,Peer-to-peer Last Activity Date,Organized Conference Last Activity Date,Participated Conference Last Activity Date,Peer-to-peer IM Count,Peer-to-peer Audio Count,Peer-to-peer Audio Minutes,Peer-to-peer Video Count,Peer-to-peer Video Minutes,Peer-to-peer App Sharing Count,Peer-to-peer File Transfer Count,Organized Conference IM Count,Organized Conference Audio/Video Count,Organized Conference Audio/Video Minutes,Organized Conference App Sharing Count,Organized Conference Web Count,Organized Conference Dial-in/out 3rd Party Count,Organized Conference Dial-in/out Microsoft Count,Organized Conference Dial-in Microsoft Minutes,Organized Conference Dial-out Microsoft Minutes,Paricipated Conference IM Count,Participated Conference Audio/Video Count,Participated Conference Audio/Video Minutes,Participated Conference App Sharing Count,Participated Conference Web Count,Participated Conference Dial-in/out 3rd Party Count,Assigned Products,Report Period
```