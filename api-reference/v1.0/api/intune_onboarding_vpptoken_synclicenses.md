# <a name="synclicenses-action"></a><span data-ttu-id="6b65f-101">syncLicenses 操作</span><span class="sxs-lookup"><span data-stu-id="6b65f-101">syncLicenses action</span></span>

> <span data-ttu-id="6b65f-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="6b65f-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6b65f-103">同步与特定 appleVolumePurchaseProgramToken 关联的许可证</span><span class="sxs-lookup"><span data-stu-id="6b65f-103">Syncs licenses associated with a specific appleVolumePurchaseProgramToken</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6b65f-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="6b65f-104">Prerequisites</span></span>
<span data-ttu-id="6b65f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="6b65f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="6b65f-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="6b65f-107">Permission type</span></span>|<span data-ttu-id="6b65f-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6b65f-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6b65f-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6b65f-109">Delegated (work or school account)</span></span>|<span data-ttu-id="6b65f-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b65f-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="6b65f-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6b65f-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6b65f-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="6b65f-112">Not supported.</span></span>|
|<span data-ttu-id="6b65f-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="6b65f-113">Application</span></span>|<span data-ttu-id="6b65f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="6b65f-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6b65f-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6b65f-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/vppTokens/{vppTokenId}/syncLicenses
```

## <a name="request-headers"></a><span data-ttu-id="6b65f-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="6b65f-116">Request headers</span></span>
|<span data-ttu-id="6b65f-117">标头</span><span class="sxs-lookup"><span data-stu-id="6b65f-117">Header</span></span>|<span data-ttu-id="6b65f-118">值</span><span class="sxs-lookup"><span data-stu-id="6b65f-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6b65f-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="6b65f-119">Authorization</span></span>|<span data-ttu-id="6b65f-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6b65f-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6b65f-121">Accept</span><span class="sxs-lookup"><span data-stu-id="6b65f-121">Accept</span></span>|<span data-ttu-id="6b65f-122">application/json</span><span class="sxs-lookup"><span data-stu-id="6b65f-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6b65f-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="6b65f-123">Request body</span></span>
<span data-ttu-id="6b65f-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6b65f-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6b65f-125">响应</span><span class="sxs-lookup"><span data-stu-id="6b65f-125">Response</span></span>
<span data-ttu-id="6b65f-126">如果成功，此操作会在响应正文中返回 `200 OK` 响应代码和 [vppToken](../resources/intune_onboarding_vpptoken.md)。</span><span class="sxs-lookup"><span data-stu-id="6b65f-126">If successful, this action returns a  response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6b65f-127">示例</span><span class="sxs-lookup"><span data-stu-id="6b65f-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="6b65f-128">请求</span><span class="sxs-lookup"><span data-stu-id="6b65f-128">Request</span></span>
<span data-ttu-id="6b65f-129">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6b65f-129">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/vppTokens/{vppTokenId}/syncLicenses
```

### <a name="response"></a><span data-ttu-id="6b65f-130">响应</span><span class="sxs-lookup"><span data-stu-id="6b65f-130">Response</span></span>
<span data-ttu-id="6b65f-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6b65f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 619

{
  "value": {
    "@odata.type": "#microsoft.graph.vppToken",
    "id": "9ceb2f92-2f92-9ceb-922f-eb9c922feb9c",
    "organizationName": "Organization Name value",
    "vppTokenAccountType": "education",
    "appleId": "Apple Id value",
    "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
    "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
    "token": "Token value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "state": "valid",
    "lastSyncStatus": "inProgress",
    "automaticallyUpdateApps": true,
    "countryOrRegion": "Country Or Region value"
  }
}
```


