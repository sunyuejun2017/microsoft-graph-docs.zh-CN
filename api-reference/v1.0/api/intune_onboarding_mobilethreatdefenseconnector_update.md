# <a name="update-mobilethreatdefenseconnector"></a><span data-ttu-id="52a26-101">更新 mobileThreatDefenseConnector</span><span class="sxs-lookup"><span data-stu-id="52a26-101">Update mobileThreatDefenseConnector</span></span>

> <span data-ttu-id="52a26-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="52a26-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="52a26-103">更新 [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="52a26-103">Update the properties of a [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="52a26-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="52a26-104">Prerequisites</span></span>
<span data-ttu-id="52a26-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="52a26-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="52a26-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="52a26-107">Permission type</span></span>|<span data-ttu-id="52a26-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="52a26-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="52a26-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="52a26-109">Delegated (work or school account)</span></span>|<span data-ttu-id="52a26-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52a26-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="52a26-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="52a26-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="52a26-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="52a26-112">Not supported.</span></span>|
|<span data-ttu-id="52a26-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="52a26-113">Application</span></span>|<span data-ttu-id="52a26-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="52a26-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="52a26-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="52a26-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="52a26-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="52a26-116">Request headers</span></span>
|<span data-ttu-id="52a26-117">标头</span><span class="sxs-lookup"><span data-stu-id="52a26-117">Header</span></span>|<span data-ttu-id="52a26-118">值</span><span class="sxs-lookup"><span data-stu-id="52a26-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="52a26-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="52a26-119">Authorization</span></span>|<span data-ttu-id="52a26-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="52a26-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="52a26-121">Accept</span><span class="sxs-lookup"><span data-stu-id="52a26-121">Accept</span></span>|<span data-ttu-id="52a26-122">application/json</span><span class="sxs-lookup"><span data-stu-id="52a26-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="52a26-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="52a26-123">Request body</span></span>
<span data-ttu-id="52a26-124">在请求正文中，提供 [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="52a26-124">In the request body, supply a JSON representation for the [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md) object.</span></span>

<span data-ttu-id="52a26-125">下表显示了创建 [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="52a26-125">The following table shows the properties that are required when you create the [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md).</span></span>

|<span data-ttu-id="52a26-126">属性</span><span class="sxs-lookup"><span data-stu-id="52a26-126">Property</span></span>|<span data-ttu-id="52a26-127">类型</span><span class="sxs-lookup"><span data-stu-id="52a26-127">Type</span></span>|<span data-ttu-id="52a26-128">说明</span><span class="sxs-lookup"><span data-stu-id="52a26-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="52a26-129">id</span><span class="sxs-lookup"><span data-stu-id="52a26-129">id</span></span>|<span data-ttu-id="52a26-130">String</span><span class="sxs-lookup"><span data-stu-id="52a26-130">String</span></span>|<span data-ttu-id="52a26-131">尚未记录</span><span class="sxs-lookup"><span data-stu-id="52a26-131">Not yet documented</span></span>|
|<span data-ttu-id="52a26-132">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="52a26-132">lastHeartbeatDateTime</span></span>|<span data-ttu-id="52a26-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="52a26-133">DateTimeOffset</span></span>|<span data-ttu-id="52a26-134">从数据同步合作伙伴接收到上一个检测信号的日期/时间</span><span class="sxs-lookup"><span data-stu-id="52a26-134">DateTime of last Heartbeat recieved from the Data Sync Partner</span></span>|
|<span data-ttu-id="52a26-135">partnerState</span><span class="sxs-lookup"><span data-stu-id="52a26-135">partnerState</span></span>|<span data-ttu-id="52a26-136">String</span><span class="sxs-lookup"><span data-stu-id="52a26-136">String</span></span>|<span data-ttu-id="52a26-137">此帐户数据同步合作伙伴状态可能的值为：`unavailable`、`available`、`enabled`、`unresponsive`。</span><span class="sxs-lookup"><span data-stu-id="52a26-137">Data Sync Partner state for this account Possible values are: `unavailable`, `available`, `enabled`, `unresponsive`.</span></span>|
|<span data-ttu-id="52a26-138">androidEnabled</span><span class="sxs-lookup"><span data-stu-id="52a26-138">androidEnabled</span></span>|<span data-ttu-id="52a26-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="52a26-139">Boolean</span></span>|<span data-ttu-id="52a26-140">对于 Android 设备，设置在合规性评估期间是否应使用来自数据同步合作伙伴的数据</span><span class="sxs-lookup"><span data-stu-id="52a26-140">For Android, set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="52a26-141">iosEnabled</span><span class="sxs-lookup"><span data-stu-id="52a26-141">iosEnabled</span></span>|<span data-ttu-id="52a26-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="52a26-142">Boolean</span></span>|<span data-ttu-id="52a26-143">对于 iOS 设备，获取或设置在合规性评估期间是否应使用来自数据同步合作伙伴的数据</span><span class="sxs-lookup"><span data-stu-id="52a26-143">For IOS, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="52a26-144">androidDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="52a26-144">androidDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="52a26-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="52a26-145">Boolean</span></span>|<span data-ttu-id="52a26-146">对于 Android 设备，设置 Intune 是否必须在使设备兼容之前接收来自数据同步合作伙伴的数据</span><span class="sxs-lookup"><span data-stu-id="52a26-146">For Android, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="52a26-147">iosDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="52a26-147">iosDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="52a26-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="52a26-148">Boolean</span></span>|<span data-ttu-id="52a26-149">对于 iOS 设备，设置 Intune 是否必须在使设备兼容之前接收来自数据同步合作伙伴的数据</span><span class="sxs-lookup"><span data-stu-id="52a26-149">For IOS, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="52a26-150">partnerUnsupportedOsVersionBlocked</span><span class="sxs-lookup"><span data-stu-id="52a26-150">partnerUnsupportedOsVersionBlocked</span></span>|<span data-ttu-id="52a26-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="52a26-151">Boolean</span></span>|<span data-ttu-id="52a26-152">获取或设置是否阻止不符合数据同步合作伙伴最低版本要求的启用平台上的设备</span><span class="sxs-lookup"><span data-stu-id="52a26-152">Get or set whether to block devices on the enabled platforms that do not meet the minimum version requirements of the Data Sync Partner</span></span>|
|<span data-ttu-id="52a26-153">partnerUnresponsivenessThresholdInDays</span><span class="sxs-lookup"><span data-stu-id="52a26-153">partnerUnresponsivenessThresholdInDays</span></span>|<span data-ttu-id="52a26-154">Int32</span><span class="sxs-lookup"><span data-stu-id="52a26-154">Int32</span></span>|<span data-ttu-id="52a26-155">获取或设置每个租户允许此合作伙伴集成不响应的天数</span><span class="sxs-lookup"><span data-stu-id="52a26-155">Get or Set days the per tenant tolerance to unresponsiveness for this partner integration</span></span>|



## <a name="response"></a><span data-ttu-id="52a26-156">响应</span><span class="sxs-lookup"><span data-stu-id="52a26-156">Response</span></span>
<span data-ttu-id="52a26-157">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="52a26-157">If successful, this method returns a `200 OK` response code and an updated [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="52a26-158">示例</span><span class="sxs-lookup"><span data-stu-id="52a26-158">Example</span></span>
### <a name="request"></a><span data-ttu-id="52a26-159">请求</span><span class="sxs-lookup"><span data-stu-id="52a26-159">Request</span></span>
<span data-ttu-id="52a26-160">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="52a26-160">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
Content-type: application/json
Content-length: 347

{
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "available",
  "androidEnabled": true,
  "iosEnabled": true,
  "androidDeviceBlockedOnMissingPartnerData": true,
  "iosDeviceBlockedOnMissingPartnerData": true,
  "partnerUnsupportedOsVersionBlocked": true,
  "partnerUnresponsivenessThresholdInDays": 6
}
```

### <a name="response"></a><span data-ttu-id="52a26-161">响应</span><span class="sxs-lookup"><span data-stu-id="52a26-161">Response</span></span>
<span data-ttu-id="52a26-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="52a26-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 463

{
  "@odata.type": "#microsoft.graph.mobileThreatDefenseConnector",
  "id": "e4bede14-de14-e4be-14de-bee414debee4",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "available",
  "androidEnabled": true,
  "iosEnabled": true,
  "androidDeviceBlockedOnMissingPartnerData": true,
  "iosDeviceBlockedOnMissingPartnerData": true,
  "partnerUnsupportedOsVersionBlocked": true,
  "partnerUnresponsivenessThresholdInDays": 6
}
```


