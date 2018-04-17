# <a name="create-devicecompliancedevicestatus"></a><span data-ttu-id="0c2d7-101">创建 deviceComplianceDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="0c2d7-101">Create deviceComplianceDeviceStatus</span></span>

> <span data-ttu-id="0c2d7-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="0c2d7-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0c2d7-103">创建新的 [deviceComplianceDeviceStatus](../resources/intune_deviceconfig_devicecompliancedevicestatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0c2d7-103">Create a new [plannerBucket](../resources/intune_deviceconfig_devicecompliancedevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0c2d7-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="0c2d7-104">Prerequisites</span></span>
<span data-ttu-id="0c2d7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="0c2d7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0c2d7-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="0c2d7-107">Permission type</span></span>|<span data-ttu-id="0c2d7-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0c2d7-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0c2d7-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0c2d7-109">Delegated (work or school account)</span></span>|<span data-ttu-id="0c2d7-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c2d7-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0c2d7-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0c2d7-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0c2d7-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="0c2d7-112">Not supported.</span></span>|
|<span data-ttu-id="0c2d7-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="0c2d7-113">Application</span></span>|<span data-ttu-id="0c2d7-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="0c2d7-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0c2d7-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0c2d7-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="0c2d7-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="0c2d7-116">Request headers</span></span>
|<span data-ttu-id="0c2d7-117">标头</span><span class="sxs-lookup"><span data-stu-id="0c2d7-117">Header</span></span>|<span data-ttu-id="0c2d7-118">值</span><span class="sxs-lookup"><span data-stu-id="0c2d7-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0c2d7-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="0c2d7-119">Authorization</span></span>|<span data-ttu-id="0c2d7-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0c2d7-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="0c2d7-121">Accept</span><span class="sxs-lookup"><span data-stu-id="0c2d7-121">Accept</span></span>|<span data-ttu-id="0c2d7-122">application/json</span><span class="sxs-lookup"><span data-stu-id="0c2d7-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0c2d7-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="0c2d7-123">Request body</span></span>
<span data-ttu-id="0c2d7-124">在请求正文中，提供 deviceComplianceDeviceStatus 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0c2d7-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="0c2d7-125">下表显示创建 deviceComplianceDeviceStatus 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="0c2d7-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="0c2d7-126">属性</span><span class="sxs-lookup"><span data-stu-id="0c2d7-126">Property</span></span>|<span data-ttu-id="0c2d7-127">类型</span><span class="sxs-lookup"><span data-stu-id="0c2d7-127">Type</span></span>|<span data-ttu-id="0c2d7-128">说明</span><span class="sxs-lookup"><span data-stu-id="0c2d7-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c2d7-129">id</span><span class="sxs-lookup"><span data-stu-id="0c2d7-129">id</span></span>|<span data-ttu-id="0c2d7-130">String</span><span class="sxs-lookup"><span data-stu-id="0c2d7-130">String</span></span>|<span data-ttu-id="0c2d7-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="0c2d7-131">Key of the setting.</span></span>|
|<span data-ttu-id="0c2d7-132">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="0c2d7-132">deviceDisplayName</span></span>|<span data-ttu-id="0c2d7-133">String</span><span class="sxs-lookup"><span data-stu-id="0c2d7-133">String</span></span>|<span data-ttu-id="0c2d7-134">DevicePolicyStatus 的设备名称。</span><span class="sxs-lookup"><span data-stu-id="0c2d7-134">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="0c2d7-135">userName</span><span class="sxs-lookup"><span data-stu-id="0c2d7-135">UserName</span></span>|<span data-ttu-id="0c2d7-136">String</span><span class="sxs-lookup"><span data-stu-id="0c2d7-136">String</span></span>|<span data-ttu-id="0c2d7-137">报告的用户名</span><span class="sxs-lookup"><span data-stu-id="0c2d7-137">The User Name that is being reported</span></span>|
|<span data-ttu-id="0c2d7-138">deviceModel</span><span class="sxs-lookup"><span data-stu-id="0c2d7-138">deviceModel</span></span>|<span data-ttu-id="0c2d7-139">String</span><span class="sxs-lookup"><span data-stu-id="0c2d7-139">String</span></span>|<span data-ttu-id="0c2d7-140">报告的设备模型</span><span class="sxs-lookup"><span data-stu-id="0c2d7-140">The device model that is being reported</span></span>|
|<span data-ttu-id="0c2d7-141">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="0c2d7-141">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="0c2d7-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c2d7-142">DateTimeOffset</span></span>|<span data-ttu-id="0c2d7-143">设备符合性宽限期的到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="0c2d7-143">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="0c2d7-144">status</span><span class="sxs-lookup"><span data-stu-id="0c2d7-144">status</span></span>|<span data-ttu-id="0c2d7-145">String</span><span class="sxs-lookup"><span data-stu-id="0c2d7-145">String</span></span>|<span data-ttu-id="0c2d7-146">策略报告的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="0c2d7-146">Compliance status of the policy report.</span></span> <span data-ttu-id="0c2d7-147">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`。</span><span class="sxs-lookup"><span data-stu-id="0c2d7-147">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`.</span></span>|
|<span data-ttu-id="0c2d7-148">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="0c2d7-148">lastReportedDateTime</span></span>|<span data-ttu-id="0c2d7-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c2d7-149">DateTimeOffset</span></span>|<span data-ttu-id="0c2d7-150">策略报告的上次修改日期时间。</span><span class="sxs-lookup"><span data-stu-id="0c2d7-150">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="0c2d7-151">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="0c2d7-151">userPrincipalName</span></span>|<span data-ttu-id="0c2d7-152">String</span><span class="sxs-lookup"><span data-stu-id="0c2d7-152">String</span></span>|<span data-ttu-id="0c2d7-153">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="0c2d7-153">userPrincipalName</span></span>|



## <a name="response"></a><span data-ttu-id="0c2d7-154">响应</span><span class="sxs-lookup"><span data-stu-id="0c2d7-154">Response</span></span>
<span data-ttu-id="0c2d7-155">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和更新的 [deviceComplianceDeviceStatus](../resources/intune_deviceconfig_devicecompliancedevicestatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0c2d7-155">If successful, this method returns a `201 Created` response code and a [ListItemVersion](../resources/intune_deviceconfig_devicecompliancedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0c2d7-156">示例</span><span class="sxs-lookup"><span data-stu-id="0c2d7-156">Example</span></span>
### <a name="request"></a><span data-ttu-id="0c2d7-157">请求</span><span class="sxs-lookup"><span data-stu-id="0c2d7-157">Request</span></span>
<span data-ttu-id="0c2d7-158">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0c2d7-158">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses
Content-type: application/json
Content-length: 426

{
  "@odata.type": "#microsoft.graph.deviceComplianceDeviceStatus",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="0c2d7-159">响应</span><span class="sxs-lookup"><span data-stu-id="0c2d7-159">Response</span></span>
<span data-ttu-id="0c2d7-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0c2d7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 475

{
  "@odata.type": "#microsoft.graph.deviceComplianceDeviceStatus",
  "id": "c6c78124-8124-c6c7-2481-c7c62481c7c6",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "deviceModel": "Device Model value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```


