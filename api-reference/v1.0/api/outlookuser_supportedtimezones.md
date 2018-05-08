# <a name="outlookuser-supportedtimezones"></a><span data-ttu-id="572c5-101">outlookUser: supportedTimeZones</span><span class="sxs-lookup"><span data-stu-id="572c5-101">outlookUser: supportedTimeZones</span></span>

<span data-ttu-id="572c5-102">获取用户支持的时区列表，就像在用户的邮箱服务器上配置的那样。</span><span class="sxs-lookup"><span data-stu-id="572c5-102">Get the list of time zones that are supported for the user, as configured on the user's mailbox server.</span></span>

<span data-ttu-id="572c5-103">可以显式指定以 Windows 时区格式返回时区，或者以 [Internet 号码分配局 (IANA) 时区](http://www.iana.org/time-zones)（也称为“Olson 时区”）格式返回。</span><span class="sxs-lookup"><span data-stu-id="572c5-103">You can explicitly specify to have time zones returned in the Windows time zone format or  [Internet Assigned Numbers Authority (IANA) time zone](http://www.iana.org/time-zones) (also known as Olson time zone) format.</span></span> <span data-ttu-id="572c5-104">Windows 时区是默认格式。</span><span class="sxs-lookup"><span data-stu-id="572c5-104">The Windows format is the default.</span></span>

<span data-ttu-id="572c5-105">在设置 Outlook 客户端时，用户从此受支持的列表中选择首选时区。</span><span class="sxs-lookup"><span data-stu-id="572c5-105">When setting up an Outlook client, the user selects the preferred time zone from this supported list.</span></span> <span data-ttu-id="572c5-106">随后可以通过[获取用户的邮箱设置](user_get_mailboxsettings.md)获取首选时区。</span><span class="sxs-lookup"><span data-stu-id="572c5-106">You can subsequently get the preferred time zone by [getting the user's mailbox settings](user_get_mailboxsettings.md).</span></span>


## <a name="permissions"></a><span data-ttu-id="572c5-107">权限</span><span class="sxs-lookup"><span data-stu-id="572c5-107">Permissions</span></span>
<span data-ttu-id="572c5-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="572c5-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="572c5-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="572c5-110">Permission type</span></span>      | <span data-ttu-id="572c5-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="572c5-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="572c5-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="572c5-112">Delegated (work or school account)</span></span> | <span data-ttu-id="572c5-113">User.Read、User.ReadBasic.All</span><span class="sxs-lookup"><span data-stu-id="572c5-113">User.Read, User.ReadBasic.All</span></span>    |
|<span data-ttu-id="572c5-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="572c5-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="572c5-115">User.Read</span><span class="sxs-lookup"><span data-stu-id="572c5-115">User.Read</span></span>    |
|<span data-ttu-id="572c5-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="572c5-116">Application</span></span> | <span data-ttu-id="572c5-117">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="572c5-117">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="572c5-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="572c5-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/supportedTimeZones
GET /users/{id|userPrincipalName}/outlook/supportedTimeZones

GET /me/outlook/supportedTimeZones(TimeZoneStandard=microsoft.graph.timeZoneStandard'{timezone_format}')
GET /users/{id|userPrincipalName}/outlook/supportedTimeZones(TimeZoneStandard=microsoft.graph.timeZoneStandard'{timezone_format}')
```
## <a name="request-headers"></a><span data-ttu-id="572c5-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="572c5-119">Request headers</span></span>
| <span data-ttu-id="572c5-120">名称</span><span class="sxs-lookup"><span data-stu-id="572c5-120">Name</span></span>       | <span data-ttu-id="572c5-121">类型</span><span class="sxs-lookup"><span data-stu-id="572c5-121">Type</span></span> | <span data-ttu-id="572c5-122">说明</span><span class="sxs-lookup"><span data-stu-id="572c5-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="572c5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="572c5-123">Authorization</span></span>  | <span data-ttu-id="572c5-124">string</span><span class="sxs-lookup"><span data-stu-id="572c5-124">string</span></span>  | <span data-ttu-id="572c5-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="572c5-p104">Bearer {token}. Required.</span></span> |


## <a name="parameters"></a><span data-ttu-id="572c5-127">参数</span><span class="sxs-lookup"><span data-stu-id="572c5-127">Parameters</span></span>
| <span data-ttu-id="572c5-128">函数参数</span><span class="sxs-lookup"><span data-stu-id="572c5-128">Function parameter</span></span>       | <span data-ttu-id="572c5-129">类型</span><span class="sxs-lookup"><span data-stu-id="572c5-129">Type</span></span> | <span data-ttu-id="572c5-130">说明</span><span class="sxs-lookup"><span data-stu-id="572c5-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="572c5-131">TimeZoneStandard</span><span class="sxs-lookup"><span data-stu-id="572c5-131">TimeZoneStandard</span></span>  | <span data-ttu-id="572c5-132">String</span><span class="sxs-lookup"><span data-stu-id="572c5-132">String</span></span>  | <span data-ttu-id="572c5-133">时区格式。</span><span class="sxs-lookup"><span data-stu-id="572c5-133">A time zone format.</span></span> <span data-ttu-id="572c5-134">支持的值：`Windows` 和 `Iana`。</span><span class="sxs-lookup"><span data-stu-id="572c5-134">Valid values are `Windows` and `Iana`.</span></span> <span data-ttu-id="572c5-135">可选。</span><span class="sxs-lookup"><span data-stu-id="572c5-135">Optional.</span></span> |


## <a name="request-body"></a><span data-ttu-id="572c5-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="572c5-136">Request body</span></span>
<span data-ttu-id="572c5-137">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="572c5-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="572c5-138">响应</span><span class="sxs-lookup"><span data-stu-id="572c5-138">Response</span></span>
<span data-ttu-id="572c5-139">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [timeZoneInformation](../resources/timezoneinformation.md) 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="572c5-139">If successful, this method returns a `200 OK` response code and collection of [directoryRole](../resources/timezoneinformation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="572c5-140">示例</span><span class="sxs-lookup"><span data-stu-id="572c5-140">Example</span></span>

##### <a name="request-1"></a><span data-ttu-id="572c5-141">请求 1</span><span class="sxs-lookup"><span data-stu-id="572c5-141">Request 1</span></span>
<span data-ttu-id="572c5-142">以下示例未指定 `timeZoneStandard` 参数，并获取以 Windows 时区格式表示的受支持的时区列表。</span><span class="sxs-lookup"><span data-stu-id="572c5-142">The following example does not specify the `timeZoneStandard` parameter, and gets the list of supported time zones represented in the Windows time zone format.</span></span> 
<!-- {
  "blockType": "request",
  "name": "user_supportedtimezones_default"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/outlook/supportedTimeZones
```

##### <a name="response-1"></a><span data-ttu-id="572c5-143">响应 1</span><span class="sxs-lookup"><span data-stu-id="572c5-143">Response 1</span></span>
<span data-ttu-id="572c5-144">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="572c5-144">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "name": "user_supportedtimezones_default",
  "truncated": true,
  "@odata.type": "microsoft.graph.timeZoneInformation",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Collection(microsoft.graph.timeZoneInformation)",
  "value":[
    {
      "alias":"Dateline Standard Time",
      "displayName":"(UTC-12:00) International Date Line West"
    },
    {
      "alias":"Samoa Standard Time",
      "displayName":"(UTC+13:00) Samoa"
    },
    {
       "alias":"UTC-11",
       "displayName":"(UTC-11:00) Coordinated Universal Time-11"
    },
    {
      "alias":"Aleutian Standard Time",
      "displayName":"(UTC-10:00) Aleutian Islands"
    }
  ]
}
```

##### <a name="request-2"></a><span data-ttu-id="572c5-145">请求 2</span><span class="sxs-lookup"><span data-stu-id="572c5-145">Request 2</span></span>
<span data-ttu-id="572c5-146">以下示例指定 `TimeZoneStandard` 参数的 `Iana`，并获取以 IANA 格式表示的受支持的时区列表。</span><span class="sxs-lookup"><span data-stu-id="572c5-146">The following example specifies `Iana` for the `TimeZoneStandard` parameter, and gets the list of supported time zones represented in IANA format.</span></span> 

<!-- {
  "blockType": "request",
  "name": "user_supportedtimezones_iana"
} -->

```http
GET https://graph.microsoft.com/v1.0/me/outlook/supportedTimeZones(TimeZoneStandard=microsoft.graph.timeZoneStandard'Iana')
```

##### <a name="response-2"></a><span data-ttu-id="572c5-147">响应 2</span><span class="sxs-lookup"><span data-stu-id="572c5-147">Response 2</span></span>
<span data-ttu-id="572c5-148">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="572c5-148">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "name": "user_supportedtimezones_iana",
  "truncated": true,
  "@odata.type": "microsoft.graph.timeZoneInformation",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Collection(microsoft.graph.timeZoneInformation)",
  "value":[
    {
      "alias":"Etc/GMT+12",
      "displayName":"Etc/GMT+12"
    },
    {
      "alias":"US/Samoa",
      "displayName":"US/Samoa"
    },
    {
      "alias":"Etc/GMT+11",
      "displayName":"Etc/GMT+11"
    },
    {
      "alias":"US/Aleutian",
      "displayName":"US/Aleutian"
    }
  ]
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: supportedTimeZones",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->