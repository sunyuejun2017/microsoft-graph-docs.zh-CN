# <a name="create-iosupdatedevicestatus"></a><span data-ttu-id="2a102-101">创建 iosUpdateDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="2a102-101">Create iosUpdateDeviceStatus</span></span>

> <span data-ttu-id="2a102-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="2a102-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2a102-103">创建新的 [iosUpdateDeviceStatus](../resources/intune_deviceconfig_iosupdatedevicestatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2a102-103">Create a new [plannerBucket](../resources/intune_deviceconfig_iosupdatedevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2a102-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="2a102-104">Prerequisites</span></span>
<span data-ttu-id="2a102-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="2a102-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2a102-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="2a102-107">Permission type</span></span>|<span data-ttu-id="2a102-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2a102-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2a102-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2a102-109">Delegated (work or school account)</span></span>|<span data-ttu-id="2a102-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a102-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2a102-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2a102-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2a102-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="2a102-112">Not supported.</span></span>|
|<span data-ttu-id="2a102-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="2a102-113">Application</span></span>|<span data-ttu-id="2a102-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="2a102-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2a102-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2a102-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/iosUpdateStatuses
```

## <a name="request-headers"></a><span data-ttu-id="2a102-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="2a102-116">Request headers</span></span>
|<span data-ttu-id="2a102-117">标头</span><span class="sxs-lookup"><span data-stu-id="2a102-117">Header</span></span>|<span data-ttu-id="2a102-118">值</span><span class="sxs-lookup"><span data-stu-id="2a102-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2a102-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="2a102-119">Authorization</span></span>|<span data-ttu-id="2a102-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2a102-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="2a102-121">Accept</span><span class="sxs-lookup"><span data-stu-id="2a102-121">Accept</span></span>|<span data-ttu-id="2a102-122">application/json</span><span class="sxs-lookup"><span data-stu-id="2a102-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2a102-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="2a102-123">Request body</span></span>
<span data-ttu-id="2a102-124">在请求正文中，提供 iosUpdateDeviceStatus 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2a102-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="2a102-125">下表显示了创建 iosUpdateDeviceStatus 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="2a102-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="2a102-126">属性</span><span class="sxs-lookup"><span data-stu-id="2a102-126">Property</span></span>|<span data-ttu-id="2a102-127">类型</span><span class="sxs-lookup"><span data-stu-id="2a102-127">Type</span></span>|<span data-ttu-id="2a102-128">说明</span><span class="sxs-lookup"><span data-stu-id="2a102-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2a102-129">id</span><span class="sxs-lookup"><span data-stu-id="2a102-129">id</span></span>|<span data-ttu-id="2a102-130">String</span><span class="sxs-lookup"><span data-stu-id="2a102-130">String</span></span>|<span data-ttu-id="2a102-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="2a102-131">Key of the setting.</span></span>|
|<span data-ttu-id="2a102-132">installStatus</span><span class="sxs-lookup"><span data-stu-id="2a102-132">installStatus</span></span>|<span data-ttu-id="2a102-133">String</span><span class="sxs-lookup"><span data-stu-id="2a102-133">String</span></span>|<span data-ttu-id="2a102-134">策略报告安装状态。</span><span class="sxs-lookup"><span data-stu-id="2a102-134">The installation status of the policy report.</span></span> <span data-ttu-id="2a102-135">可取值为：`success`、`available`、`idle`、`downloading`、`downloadFailed`、`downloadRequiresComputer`、`downloadInsufficientSpace`、`downloadInsufficientPower`、`downloadInsufficientNetwork`、`installing`、`installInsufficientSpace`、`installInsufficientPower`、`installPhoneCallInProgress`、`installFailed`、`notSupportedOperation`、`sharedDeviceUserLoggedInError`。</span><span class="sxs-lookup"><span data-stu-id="2a102-135">Possible values are: `success`, `available`, `idle`, `downloading`, `downloadFailed`, `downloadRequiresComputer`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installing`, `installInsufficientSpace`, `installInsufficientPower`, `installPhoneCallInProgress`, `installFailed`, `notSupportedOperation`, `sharedDeviceUserLoggedInError`.</span></span>|
|<span data-ttu-id="2a102-136">osVersion</span><span class="sxs-lookup"><span data-stu-id="2a102-136">osVersion</span></span>|<span data-ttu-id="2a102-137">String</span><span class="sxs-lookup"><span data-stu-id="2a102-137">String</span></span>|<span data-ttu-id="2a102-138">报告的设备版本。</span><span class="sxs-lookup"><span data-stu-id="2a102-138">The device version that is being reported.</span></span>|
|<span data-ttu-id="2a102-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="2a102-139">deviceId</span></span>|<span data-ttu-id="2a102-140">String</span><span class="sxs-lookup"><span data-stu-id="2a102-140">String</span></span>|<span data-ttu-id="2a102-141">报告的设备 ID。</span><span class="sxs-lookup"><span data-stu-id="2a102-141">The device id that is being reported.</span></span>|
|<span data-ttu-id="2a102-142">userId</span><span class="sxs-lookup"><span data-stu-id="2a102-142">userID</span></span>|<span data-ttu-id="2a102-143">String</span><span class="sxs-lookup"><span data-stu-id="2a102-143">String</span></span>|<span data-ttu-id="2a102-144">报告的用户 ID。</span><span class="sxs-lookup"><span data-stu-id="2a102-144">The User id that is being reported.</span></span>|
|<span data-ttu-id="2a102-145">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="2a102-145">deviceDisplayName</span></span>|<span data-ttu-id="2a102-146">String</span><span class="sxs-lookup"><span data-stu-id="2a102-146">String</span></span>|<span data-ttu-id="2a102-147">DevicePolicyStatus 的设备名。</span><span class="sxs-lookup"><span data-stu-id="2a102-147">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="2a102-148">userName</span><span class="sxs-lookup"><span data-stu-id="2a102-148">UserName</span></span>|<span data-ttu-id="2a102-149">String</span><span class="sxs-lookup"><span data-stu-id="2a102-149">String</span></span>|<span data-ttu-id="2a102-150">报告的用户名</span><span class="sxs-lookup"><span data-stu-id="2a102-150">The User Name that is being reported</span></span>|
|<span data-ttu-id="2a102-151">deviceModel</span><span class="sxs-lookup"><span data-stu-id="2a102-151">deviceModel</span></span>|<span data-ttu-id="2a102-152">String</span><span class="sxs-lookup"><span data-stu-id="2a102-152">String</span></span>|<span data-ttu-id="2a102-153">报告的设备模型</span><span class="sxs-lookup"><span data-stu-id="2a102-153">The device model that is being reported</span></span>|
|<span data-ttu-id="2a102-154">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="2a102-154">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="2a102-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2a102-155">DateTimeOffset</span></span>|<span data-ttu-id="2a102-156">设备符合性宽限期的到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="2a102-156">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="2a102-157">status</span><span class="sxs-lookup"><span data-stu-id="2a102-157">status</span></span>|<span data-ttu-id="2a102-158">String</span><span class="sxs-lookup"><span data-stu-id="2a102-158">String</span></span>|<span data-ttu-id="2a102-159">策略报告的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="2a102-159">Compliance status of the policy report.</span></span> <span data-ttu-id="2a102-160">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`。</span><span class="sxs-lookup"><span data-stu-id="2a102-160">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`.</span></span>|
|<span data-ttu-id="2a102-161">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="2a102-161">lastReportedDateTime</span></span>|<span data-ttu-id="2a102-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2a102-162">DateTimeOffset</span></span>|<span data-ttu-id="2a102-163">策略报告的上次修改日期时间。</span><span class="sxs-lookup"><span data-stu-id="2a102-163">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="2a102-164">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="2a102-164">userPrincipalName</span></span>|<span data-ttu-id="2a102-165">String</span><span class="sxs-lookup"><span data-stu-id="2a102-165">String</span></span>|<span data-ttu-id="2a102-166">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="2a102-166">userPrincipalName</span></span>|



## <a name="response"></a><span data-ttu-id="2a102-167">响应</span><span class="sxs-lookup"><span data-stu-id="2a102-167">Response</span></span>
<span data-ttu-id="2a102-168">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [iosUpdateDeviceStatus](../resources/intune_deviceconfig_iosupdatedevicestatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2a102-168">If successful, this method returns a `201 Created` response code and a [directoryObject](../resources/intune_deviceconfig_iosupdatedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2a102-169">示例</span><span class="sxs-lookup"><span data-stu-id="2a102-169">Example</span></span>
### <a name="request"></a><span data-ttu-id="2a102-170">请求</span><span class="sxs-lookup"><span data-stu-id="2a102-170">Request</span></span>
<span data-ttu-id="2a102-171">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2a102-171">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/iosUpdateStatuses
Content-type: application/json
Content-length: 552

{
  "@odata.type": "#microsoft.graph.iosUpdateDeviceStatus",
  "installStatus": "available",
  "osVersion": "Os Version value",
  "deviceId": "Device Id value",
  "userId": "User Id value",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="2a102-172">响应</span><span class="sxs-lookup"><span data-stu-id="2a102-172">Response</span></span>
<span data-ttu-id="2a102-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2a102-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 601

{
  "@odata.type": "#microsoft.graph.iosUpdateDeviceStatus",
  "id": "63a79499-9499-63a7-9994-a7639994a763",
  "installStatus": "available",
  "osVersion": "Os Version value",
  "deviceId": "Device Id value",
  "userId": "User Id value",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```


