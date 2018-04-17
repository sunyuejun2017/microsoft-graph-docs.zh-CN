# <a name="create-windows10compliancepolicy"></a><span data-ttu-id="3373f-101">创建 windows10CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="3373f-101">Create windows10CompliancePolicy</span></span>

> <span data-ttu-id="3373f-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="3373f-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3373f-103">创建新的 [windows10CompliancePolicy](../resources/intune_deviceconfig_windows10compliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3373f-103">Create a new [plannerBucket](../resources/intune_deviceconfig_windows10compliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3373f-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="3373f-104">Prerequisites</span></span>
<span data-ttu-id="3373f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="3373f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="3373f-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="3373f-107">Permission type</span></span>|<span data-ttu-id="3373f-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="3373f-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3373f-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3373f-109">Delegated (work or school account)</span></span>|<span data-ttu-id="3373f-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3373f-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3373f-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3373f-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3373f-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="3373f-112">Not supported.</span></span>|
|<span data-ttu-id="3373f-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="3373f-113">Application</span></span>|<span data-ttu-id="3373f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="3373f-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3373f-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3373f-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="3373f-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="3373f-116">Request headers</span></span>
|<span data-ttu-id="3373f-117">标头</span><span class="sxs-lookup"><span data-stu-id="3373f-117">Header</span></span>|<span data-ttu-id="3373f-118">值</span><span class="sxs-lookup"><span data-stu-id="3373f-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3373f-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="3373f-119">Authorization</span></span>|<span data-ttu-id="3373f-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3373f-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="3373f-121">Accept</span><span class="sxs-lookup"><span data-stu-id="3373f-121">Accept</span></span>|<span data-ttu-id="3373f-122">application/json</span><span class="sxs-lookup"><span data-stu-id="3373f-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3373f-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="3373f-123">Request body</span></span>
<span data-ttu-id="3373f-124">在请求正文中，提供 windows10CompliancePolicy 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3373f-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="3373f-125">下表显示创建 windows10CompliancePolicy 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="3373f-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="3373f-126">属性</span><span class="sxs-lookup"><span data-stu-id="3373f-126">Property</span></span>|<span data-ttu-id="3373f-127">类型</span><span class="sxs-lookup"><span data-stu-id="3373f-127">Type</span></span>|<span data-ttu-id="3373f-128">说明</span><span class="sxs-lookup"><span data-stu-id="3373f-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3373f-129">id</span><span class="sxs-lookup"><span data-stu-id="3373f-129">id</span></span>|<span data-ttu-id="3373f-130">String</span><span class="sxs-lookup"><span data-stu-id="3373f-130">String</span></span>|<span data-ttu-id="3373f-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="3373f-131">Key of the setting.</span></span> <span data-ttu-id="3373f-132">继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="3373f-132">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="3373f-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3373f-133">createdDateTime</span></span>|<span data-ttu-id="3373f-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3373f-134">DateTimeOffset</span></span>|<span data-ttu-id="3373f-135">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="3373f-135">DateTime the object was created.</span></span> <span data-ttu-id="3373f-136">继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="3373f-136">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="3373f-137">description</span><span class="sxs-lookup"><span data-stu-id="3373f-137">description</span></span>|<span data-ttu-id="3373f-138">String</span><span class="sxs-lookup"><span data-stu-id="3373f-138">String</span></span>|<span data-ttu-id="3373f-139">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="3373f-139">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3373f-140">继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="3373f-140">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="3373f-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3373f-141">lastModifiedDateTime</span></span>|<span data-ttu-id="3373f-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3373f-142">DateTimeOffset</span></span>|<span data-ttu-id="3373f-143">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="3373f-143">Indicates the date the object was last modified.</span></span> <span data-ttu-id="3373f-144">继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="3373f-144">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="3373f-145">displayName</span><span class="sxs-lookup"><span data-stu-id="3373f-145">displayName</span></span>|<span data-ttu-id="3373f-146">String</span><span class="sxs-lookup"><span data-stu-id="3373f-146">String</span></span>|<span data-ttu-id="3373f-147">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="3373f-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3373f-148">继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="3373f-148">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="3373f-149">version</span><span class="sxs-lookup"><span data-stu-id="3373f-149">version</span></span>|<span data-ttu-id="3373f-150">Int32</span><span class="sxs-lookup"><span data-stu-id="3373f-150">Int32</span></span>|<span data-ttu-id="3373f-151">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="3373f-151">Version of the device configuration.</span></span> <span data-ttu-id="3373f-152">继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="3373f-152">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="3373f-153">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="3373f-153">passwordRequired</span></span>|<span data-ttu-id="3373f-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="3373f-154">Boolean</span></span>|<span data-ttu-id="3373f-155">需要密码才可解锁 Windows 设备。</span><span class="sxs-lookup"><span data-stu-id="3373f-155">Require a password to unlock Windows device.</span></span>|
|<span data-ttu-id="3373f-156">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="3373f-156">passwordBlockSimple</span></span>|<span data-ttu-id="3373f-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="3373f-157">Boolean</span></span>|<span data-ttu-id="3373f-158">指示是否阻止简单密码。</span><span class="sxs-lookup"><span data-stu-id="3373f-158">Indicates whether or not to block simple password.</span></span>|
|<span data-ttu-id="3373f-159">passwordRequiredToUnlockFromIdle</span><span class="sxs-lookup"><span data-stu-id="3373f-159">passwordRequiredToUnlockFromIdle</span></span>|<span data-ttu-id="3373f-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="3373f-160">Boolean</span></span>|<span data-ttu-id="3373f-161">需要密码才可解锁空闲设备。</span><span class="sxs-lookup"><span data-stu-id="3373f-161">Require a password to unlock an idle device.</span></span>|
|<span data-ttu-id="3373f-162">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="3373f-162">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="3373f-163">Int32</span><span class="sxs-lookup"><span data-stu-id="3373f-163">Int32</span></span>|<span data-ttu-id="3373f-164">在需要密码之前不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="3373f-164">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="3373f-165">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="3373f-165">passwordExpirationDays</span></span>|<span data-ttu-id="3373f-166">Int32</span><span class="sxs-lookup"><span data-stu-id="3373f-166">Int32</span></span>|<span data-ttu-id="3373f-167">密码过期天数。</span><span class="sxs-lookup"><span data-stu-id="3373f-167">The password expiration in days.</span></span>|
|<span data-ttu-id="3373f-168">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="3373f-168">passwordMinimumLength</span></span>|<span data-ttu-id="3373f-169">Int32</span><span class="sxs-lookup"><span data-stu-id="3373f-169">Int32</span></span>|<span data-ttu-id="3373f-170">密码最短长度。</span><span class="sxs-lookup"><span data-stu-id="3373f-170">The minimum password length.</span></span>|
|<span data-ttu-id="3373f-171">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="3373f-171">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="3373f-172">Int32</span><span class="sxs-lookup"><span data-stu-id="3373f-172">Int32</span></span>|<span data-ttu-id="3373f-173">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="3373f-173">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="3373f-174">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="3373f-174">passwordRequiredType</span></span>|<span data-ttu-id="3373f-175">String</span><span class="sxs-lookup"><span data-stu-id="3373f-175">String</span></span>|<span data-ttu-id="3373f-176">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="3373f-176">The required password type.</span></span> <span data-ttu-id="3373f-177">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="3373f-177">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="3373f-178">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="3373f-178">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="3373f-179">Int32</span><span class="sxs-lookup"><span data-stu-id="3373f-179">Int32</span></span>|<span data-ttu-id="3373f-180">防止重复使用的先前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="3373f-180">The number of previous passwords to prevent re-use of.</span></span>|
|<span data-ttu-id="3373f-181">requireHealthyDeviceReport</span><span class="sxs-lookup"><span data-stu-id="3373f-181">requireHealthyDeviceReport</span></span>|<span data-ttu-id="3373f-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="3373f-182">Boolean</span></span>|<span data-ttu-id="3373f-183">要求设备由 Windows 设备运行状况证明报告为正常。</span><span class="sxs-lookup"><span data-stu-id="3373f-183">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="3373f-184">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="3373f-184">osMinimumVersion</span></span>|<span data-ttu-id="3373f-185">String</span><span class="sxs-lookup"><span data-stu-id="3373f-185">String</span></span>|<span data-ttu-id="3373f-186">最低 Windows 10 版本。</span><span class="sxs-lookup"><span data-stu-id="3373f-186">Minimum Windows 10 version.</span></span>|
|<span data-ttu-id="3373f-187">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="3373f-187">osMaximumVersion</span></span>|<span data-ttu-id="3373f-188">String</span><span class="sxs-lookup"><span data-stu-id="3373f-188">String</span></span>|<span data-ttu-id="3373f-189">最高 Windows 10 版本。</span><span class="sxs-lookup"><span data-stu-id="3373f-189">Maximum Windows 10 version.</span></span>|
|<span data-ttu-id="3373f-190">mobileOsMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="3373f-190">mobileOsMinimumVersion</span></span>|<span data-ttu-id="3373f-191">String</span><span class="sxs-lookup"><span data-stu-id="3373f-191">String</span></span>|<span data-ttu-id="3373f-192">最低 Windows Phone 版本。</span><span class="sxs-lookup"><span data-stu-id="3373f-192">Minimum Windows Phone version.</span></span>|
|<span data-ttu-id="3373f-193">mobileOsMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="3373f-193">mobileOsMaximumVersion</span></span>|<span data-ttu-id="3373f-194">String</span><span class="sxs-lookup"><span data-stu-id="3373f-194">String</span></span>|<span data-ttu-id="3373f-195">最高 Windows Phone 版本。</span><span class="sxs-lookup"><span data-stu-id="3373f-195">Maximum Windows Phone version.</span></span>|
|<span data-ttu-id="3373f-196">earlyLaunchAntiMalwareDriverEnabled</span><span class="sxs-lookup"><span data-stu-id="3373f-196">earlyLaunchAntiMalwareDriverEnabled</span></span>|<span data-ttu-id="3373f-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="3373f-197">Boolean</span></span>|<span data-ttu-id="3373f-198">要求设备由 Windows 设备运行状况证明报告为正常 - 提前启动反恶意驱动程序已启用。</span><span class="sxs-lookup"><span data-stu-id="3373f-198">Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.</span></span>|
|<span data-ttu-id="3373f-199">bitLockerEnabled</span><span class="sxs-lookup"><span data-stu-id="3373f-199">bitLockerEnabled</span></span>|<span data-ttu-id="3373f-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="3373f-200">Boolean</span></span>|<span data-ttu-id="3373f-201">要求设备由 Windows 设备运行状况证明报告为正常 - bit locker 已启用。</span><span class="sxs-lookup"><span data-stu-id="3373f-201">Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled</span></span>|
|<span data-ttu-id="3373f-202">secureBootEnabled</span><span class="sxs-lookup"><span data-stu-id="3373f-202">secureBootEnabled</span></span>|<span data-ttu-id="3373f-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="3373f-203">Boolean</span></span>|<span data-ttu-id="3373f-204">要求设备由 Windows 设备运行状况证明报告为正常 - 安全启动已启用。</span><span class="sxs-lookup"><span data-stu-id="3373f-204">Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.</span></span>|
|<span data-ttu-id="3373f-205">codeIntegrityEnabled</span><span class="sxs-lookup"><span data-stu-id="3373f-205">codeIntegrityEnabled</span></span>|<span data-ttu-id="3373f-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="3373f-206">Boolean</span></span>|<span data-ttu-id="3373f-207">要求设备由 Windows 设备运行状况证明报告为正常。</span><span class="sxs-lookup"><span data-stu-id="3373f-207">Require devices to be reported as healthy by Windows Device Health Attestation.</span></span>|
|<span data-ttu-id="3373f-208">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="3373f-208">storageRequireEncryption</span></span>|<span data-ttu-id="3373f-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="3373f-209">Boolean</span></span>|<span data-ttu-id="3373f-210">要求对 Windows 设备加密。</span><span class="sxs-lookup"><span data-stu-id="3373f-210">Require encryption on windows devices.</span></span>|



## <a name="response"></a><span data-ttu-id="3373f-211">响应</span><span class="sxs-lookup"><span data-stu-id="3373f-211">Response</span></span>
<span data-ttu-id="3373f-212">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [windows10CompliancePolicy](../resources/intune_deviceconfig_windows10compliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3373f-212">If successful, this method returns a `201 Created` response code and a [directoryObject](../resources/intune_deviceconfig_windows10compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3373f-213">示例</span><span class="sxs-lookup"><span data-stu-id="3373f-213">Example</span></span>
### <a name="request"></a><span data-ttu-id="3373f-214">请求</span><span class="sxs-lookup"><span data-stu-id="3373f-214">Request</span></span>
<span data-ttu-id="3373f-215">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3373f-215">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 1018

{
  "@odata.type": "#microsoft.graph.windows10CompliancePolicy",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordRequiredToUnlockFromIdle": true,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "requireHealthyDeviceReport": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "mobileOsMinimumVersion": "Mobile Os Minimum Version value",
  "mobileOsMaximumVersion": "Mobile Os Maximum Version value",
  "earlyLaunchAntiMalwareDriverEnabled": true,
  "bitLockerEnabled": true,
  "secureBootEnabled": true,
  "codeIntegrityEnabled": true,
  "storageRequireEncryption": true
}
```

### <a name="response"></a><span data-ttu-id="3373f-216">响应</span><span class="sxs-lookup"><span data-stu-id="3373f-216">Response</span></span>
<span data-ttu-id="3373f-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3373f-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1126

{
  "@odata.type": "#microsoft.graph.windows10CompliancePolicy",
  "id": "2919ae62-ae62-2919-62ae-192962ae1929",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordRequiredToUnlockFromIdle": true,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "requireHealthyDeviceReport": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "mobileOsMinimumVersion": "Mobile Os Minimum Version value",
  "mobileOsMaximumVersion": "Mobile Os Maximum Version value",
  "earlyLaunchAntiMalwareDriverEnabled": true,
  "bitLockerEnabled": true,
  "secureBootEnabled": true,
  "codeIntegrityEnabled": true,
  "storageRequireEncryption": true
}
```


