# <a name="reportroot-getskypeforbusinessparticipantactivityminutecounts"></a><span data-ttu-id="753f0-101">reportRoot: getSkypeForBusinessParticipantActivityMinuteCounts</span><span class="sxs-lookup"><span data-stu-id="753f0-101">reportRoot: getSkypeForBusinessParticipantActivityMinuteCounts</span></span>

<span data-ttu-id="753f0-102">获取使用情况趋势，即组织中用户参与的会议会话的时长（以分钟为单位）和类型。</span><span class="sxs-lookup"><span data-stu-id="753f0-102">Get usage trends on the length in minutes and type of conference sessions that users from your organization participated in.</span></span> <span data-ttu-id="753f0-103">会议会话类型包括音频/视频。</span><span class="sxs-lookup"><span data-stu-id="753f0-103">Types of conference sessions include audio/video.</span></span>

> <span data-ttu-id="753f0-104">**注意：**若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Skype for Business 会议参与者活动](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b)。</span><span class="sxs-lookup"><span data-stu-id="753f0-104">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business conference participant activity](https://support.office.com/client/Skype-for-Business-Online-conference-participant-activity-c3c89995-65dd-4715-9e38-bb244c742c6b).</span></span>

## <a name="permissions"></a><span data-ttu-id="753f0-105">权限</span><span class="sxs-lookup"><span data-stu-id="753f0-105">Permissions</span></span>

<span data-ttu-id="753f0-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="753f0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="753f0-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="753f0-108">Permission type</span></span>                        | <span data-ttu-id="753f0-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="753f0-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="753f0-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="753f0-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="753f0-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="753f0-111">Not supported.</span></span>                           |
| <span data-ttu-id="753f0-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="753f0-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="753f0-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="753f0-113">Not supported.</span></span>                           |
| <span data-ttu-id="753f0-114">应用</span><span class="sxs-lookup"><span data-stu-id="753f0-114">Application</span></span>                            | <span data-ttu-id="753f0-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="753f0-115">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="753f0-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="753f0-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessParticipantActivityMinuteCounts(period='{period_value}')
```

## <a name="request-parameters"></a><span data-ttu-id="753f0-117">请求参数</span><span class="sxs-lookup"><span data-stu-id="753f0-117">Request parameters</span></span>

<span data-ttu-id="753f0-118">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="753f0-118">In the request URL, provide the following query parameter with a valid value.</span></span>

| <span data-ttu-id="753f0-119">参数</span><span class="sxs-lookup"><span data-stu-id="753f0-119">Parameter</span></span> | <span data-ttu-id="753f0-120">类型</span><span class="sxs-lookup"><span data-stu-id="753f0-120">Type</span></span>   | <span data-ttu-id="753f0-121">说明</span><span class="sxs-lookup"><span data-stu-id="753f0-121">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="753f0-122">period</span><span class="sxs-lookup"><span data-stu-id="753f0-122">period</span></span>    | <span data-ttu-id="753f0-123">string</span><span class="sxs-lookup"><span data-stu-id="753f0-123">string</span></span> | <span data-ttu-id="753f0-124">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="753f0-124">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="753f0-125">受支持的 {Period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="753f0-125">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="753f0-126">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="753f0-126">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="753f0-127">必需。</span><span class="sxs-lookup"><span data-stu-id="753f0-127">Required.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="753f0-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="753f0-128">Request headers</span></span>

| <span data-ttu-id="753f0-129">名称</span><span class="sxs-lookup"><span data-stu-id="753f0-129">Name</span></span>          | <span data-ttu-id="753f0-130">说明</span><span class="sxs-lookup"><span data-stu-id="753f0-130">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="753f0-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="753f0-131">Authorization</span></span> | <span data-ttu-id="753f0-p104">持有者{令牌}。必需。</span><span class="sxs-lookup"><span data-stu-id="753f0-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="753f0-134">If-None-Match</span><span class="sxs-lookup"><span data-stu-id="753f0-134">If-None-Match</span></span> | <span data-ttu-id="753f0-135">如果包含此请求头，且提供的 eTag 与文件中的当前标记一致，返回的是 `304 Not Modified` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="753f0-135">If this request header is included and the eTag provided matches the current tag on the file, a `304 Not Modified` response code is returned.</span></span> <span data-ttu-id="753f0-136">可选。</span><span class="sxs-lookup"><span data-stu-id="753f0-136">Optional.</span></span> |

## <a name="response"></a><span data-ttu-id="753f0-137">响应</span><span class="sxs-lookup"><span data-stu-id="753f0-137">Response</span></span>

<span data-ttu-id="753f0-138">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="753f0-138">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="753f0-139">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="753f0-139">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="753f0-140">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="753f0-140">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="753f0-141">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="753f0-141">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="753f0-142">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="753f0-142">Report Refresh Date</span></span>
- <span data-ttu-id="753f0-143">报表日期</span><span class="sxs-lookup"><span data-stu-id="753f0-143">Report Date</span></span>
- <span data-ttu-id="753f0-144">报表周期</span><span class="sxs-lookup"><span data-stu-id="753f0-144">Report Period</span></span>
- <span data-ttu-id="753f0-145">音频/视频</span><span class="sxs-lookup"><span data-stu-id="753f0-145">Audio/Video</span></span>

## <a name="example"></a><span data-ttu-id="753f0-146">示例</span><span class="sxs-lookup"><span data-stu-id="753f0-146">Example</span></span>

#### <a name="request"></a><span data-ttu-id="753f0-147">请求</span><span class="sxs-lookup"><span data-stu-id="753f0-147">Request</span></span>

<span data-ttu-id="753f0-148">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="753f0-148">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessparticipantactivityminutecounts"
}-->

```http
GET https://graph.microsoft.com/v1.0/reports/getSkypeForBusinessParticipantActivityMinuteCounts(period='D7')
```

#### <a name="response"></a><span data-ttu-id="753f0-149">响应</span><span class="sxs-lookup"><span data-stu-id="753f0-149">Response</span></span>

<span data-ttu-id="753f0-150">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="753f0-150">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="753f0-151">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="753f0-151">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,Audio/Video
```