# <a name="update-androidmanagedappprotection"></a><span data-ttu-id="e6312-101">更新 androidManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="e6312-101">Update androidManagedAppProtection</span></span>

> <span data-ttu-id="e6312-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="e6312-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e6312-103">更新 [androidManagedAppProtection](../resources/intune_mam_androidmanagedappprotection.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e6312-103">Update the properties of a [calendar](../resources/intune_mam_androidmanagedappprotection.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e6312-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="e6312-104">Prerequisites</span></span>
<span data-ttu-id="e6312-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="e6312-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e6312-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="e6312-107">Permission type</span></span>|<span data-ttu-id="e6312-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e6312-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e6312-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e6312-109">Delegated (work or school account)</span></span>|<span data-ttu-id="e6312-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6312-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e6312-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e6312-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e6312-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="e6312-112">Not supported.</span></span>|
|<span data-ttu-id="e6312-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="e6312-113">Application</span></span>|<span data-ttu-id="e6312-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="e6312-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e6312-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e6312-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}
```

## <a name="request-headers"></a><span data-ttu-id="e6312-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="e6312-116">Request headers</span></span>
|<span data-ttu-id="e6312-117">标头</span><span class="sxs-lookup"><span data-stu-id="e6312-117">Header</span></span>|<span data-ttu-id="e6312-118">值</span><span class="sxs-lookup"><span data-stu-id="e6312-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e6312-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="e6312-119">Authorization</span></span>|<span data-ttu-id="e6312-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e6312-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="e6312-121">Accept</span><span class="sxs-lookup"><span data-stu-id="e6312-121">Accept</span></span>|<span data-ttu-id="e6312-122">application/json</span><span class="sxs-lookup"><span data-stu-id="e6312-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e6312-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="e6312-123">Request body</span></span>
<span data-ttu-id="e6312-124">在请求正文中，提供 [androidManagedAppProtection](../resources/intune_mam_androidmanagedappprotection.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e6312-124">In the request body, supply a JSON representation of [Attachment](../resources/intune_mam_androidmanagedappprotection.md) object.</span></span>

<span data-ttu-id="e6312-125">下表显示了创建 [androidManagedAppProtection](../resources/intune_mam_androidmanagedappprotection.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e6312-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="e6312-126">属性</span><span class="sxs-lookup"><span data-stu-id="e6312-126">Property</span></span>|<span data-ttu-id="e6312-127">类型</span><span class="sxs-lookup"><span data-stu-id="e6312-127">Type</span></span>|<span data-ttu-id="e6312-128">说明</span><span class="sxs-lookup"><span data-stu-id="e6312-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e6312-129">displayName</span><span class="sxs-lookup"><span data-stu-id="e6312-129">displayName</span></span>|<span data-ttu-id="e6312-130">String</span><span class="sxs-lookup"><span data-stu-id="e6312-130">String</span></span>|<span data-ttu-id="e6312-131">策略显示名称。</span><span class="sxs-lookup"><span data-stu-id="e6312-131">Policy display name.</span></span> <span data-ttu-id="e6312-132">继承自 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="e6312-132">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="e6312-133">description</span><span class="sxs-lookup"><span data-stu-id="e6312-133">description</span></span>|<span data-ttu-id="e6312-134">String</span><span class="sxs-lookup"><span data-stu-id="e6312-134">String</span></span>|<span data-ttu-id="e6312-135">策略的说明。</span><span class="sxs-lookup"><span data-stu-id="e6312-135">The policy's description.</span></span> <span data-ttu-id="e6312-136">继承自 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="e6312-136">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="e6312-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e6312-137">createdDateTime</span></span>|<span data-ttu-id="e6312-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e6312-138">DateTimeOffset</span></span>|<span data-ttu-id="e6312-139">创建策略的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="e6312-139">The date and time when the page was created.</span></span> <span data-ttu-id="e6312-140">继承自 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="e6312-140">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="e6312-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e6312-141">lastModifiedDateTime</span></span>|<span data-ttu-id="e6312-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e6312-142">DateTimeOffset</span></span>|<span data-ttu-id="e6312-143">上次修改策略的时间。</span><span class="sxs-lookup"><span data-stu-id="e6312-143">Last time the policy was modified.</span></span> <span data-ttu-id="e6312-144">继承自 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="e6312-144">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="e6312-145">id</span><span class="sxs-lookup"><span data-stu-id="e6312-145">id</span></span>|<span data-ttu-id="e6312-146">String</span><span class="sxs-lookup"><span data-stu-id="e6312-146">String</span></span>|<span data-ttu-id="e6312-147">实体的键。</span><span class="sxs-lookup"><span data-stu-id="e6312-147">Key of the setting.</span></span> <span data-ttu-id="e6312-148">继承自 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="e6312-148">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="e6312-149">version</span><span class="sxs-lookup"><span data-stu-id="e6312-149">version</span></span>|<span data-ttu-id="e6312-150">String</span><span class="sxs-lookup"><span data-stu-id="e6312-150">String</span></span>|<span data-ttu-id="e6312-151">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="e6312-151">Version of the entity.</span></span> <span data-ttu-id="e6312-152">继承自 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span><span class="sxs-lookup"><span data-stu-id="e6312-152">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="e6312-153">periodOfflineBeforeAccessCheck</span><span class="sxs-lookup"><span data-stu-id="e6312-153">periodOfflineBeforeAccessCheck</span></span>|<span data-ttu-id="e6312-154">Duration</span><span class="sxs-lookup"><span data-stu-id="e6312-154">Duration</span></span>|<span data-ttu-id="e6312-155">设备未连接到 Internet 时在该时间段后检查访问权限。</span><span class="sxs-lookup"><span data-stu-id="e6312-155">The period after which access is checked when the device is not connected to the internet.</span></span> <span data-ttu-id="e6312-156">继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="e6312-156">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="e6312-157">periodOnlineBeforeAccessCheck</span><span class="sxs-lookup"><span data-stu-id="e6312-157">periodOnlineBeforeAccessCheck</span></span>|<span data-ttu-id="e6312-158">Duration</span><span class="sxs-lookup"><span data-stu-id="e6312-158">Duration</span></span>|<span data-ttu-id="e6312-159">设备连接到 Internet 时在该时间段后检查访问权限。</span><span class="sxs-lookup"><span data-stu-id="e6312-159">The period after which access is checked when the device is connected to the internet.</span></span> <span data-ttu-id="e6312-160">继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="e6312-160">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="e6312-161">allowedInboundDataTransferSources</span><span class="sxs-lookup"><span data-stu-id="e6312-161">allowedInboundDataTransferSources</span></span>|<span data-ttu-id="e6312-162">String</span><span class="sxs-lookup"><span data-stu-id="e6312-162">String</span></span>|<span data-ttu-id="e6312-163">允许传输其中的数据的源。</span><span class="sxs-lookup"><span data-stu-id="e6312-163">Sources from which data is allowed to be transferred.</span></span> <span data-ttu-id="e6312-164">继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)。可取值为：`allApps`、`managedApps`、`none`。</span><span class="sxs-lookup"><span data-stu-id="e6312-164">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md) Possible values are: `allApps`, `managedApps`, `none`.</span></span>|
|<span data-ttu-id="e6312-165">allowedOutboundDataTransferDestinations</span><span class="sxs-lookup"><span data-stu-id="e6312-165">allowedOutboundDataTransferDestinations</span></span>|<span data-ttu-id="e6312-166">String</span><span class="sxs-lookup"><span data-stu-id="e6312-166">String</span></span>|<span data-ttu-id="e6312-167">允许向其传输数据的目标。</span><span class="sxs-lookup"><span data-stu-id="e6312-167">Destinations to which data is allowed to be transferred.</span></span> <span data-ttu-id="e6312-168">继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)。可取值为：`allApps`、`managedApps`、`none`。</span><span class="sxs-lookup"><span data-stu-id="e6312-168">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md) Possible values are: `allApps`, `managedApps`, `none`.</span></span>|
|<span data-ttu-id="e6312-169">organizationalCredentialsRequired</span><span class="sxs-lookup"><span data-stu-id="e6312-169">organizationalCredentialsRequired</span></span>|<span data-ttu-id="e6312-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="e6312-170">Boolean</span></span>|<span data-ttu-id="e6312-171">指示是否需要组织凭据才能使用应用。</span><span class="sxs-lookup"><span data-stu-id="e6312-171">Indicates whether organizational credentials are required for app use.</span></span> <span data-ttu-id="e6312-172">继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="e6312-172">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="e6312-173">allowedOutboundClipboardSharingLevel</span><span class="sxs-lookup"><span data-stu-id="e6312-173">allowedOutboundClipboardSharingLevel</span></span>|<span data-ttu-id="e6312-174">String</span><span class="sxs-lookup"><span data-stu-id="e6312-174">String</span></span>|<span data-ttu-id="e6312-175">可以在托管设备上的应用之间共享剪贴板的级别。</span><span class="sxs-lookup"><span data-stu-id="e6312-175">The level to which the clipboard may be shared between apps on the managed device.</span></span> <span data-ttu-id="e6312-176">继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)。可取值为：`allApps`、`managedAppsWithPasteIn`、`managedApps`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="e6312-176">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md) Possible values are: `allApps`, `managedAppsWithPasteIn`, `managedApps`, `blocked`.</span></span>|
|<span data-ttu-id="e6312-177">dataBackupBlocked</span><span class="sxs-lookup"><span data-stu-id="e6312-177">dataBackupBlocked</span></span>|<span data-ttu-id="e6312-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="e6312-178">Boolean</span></span>|<span data-ttu-id="e6312-179">指示是否阻止备份托管应用的数据。</span><span class="sxs-lookup"><span data-stu-id="e6312-179">Indicates whether the backup of a managed app's data is blocked.</span></span> <span data-ttu-id="e6312-180">继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="e6312-180">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="e6312-181">deviceComplianceRequired</span><span class="sxs-lookup"><span data-stu-id="e6312-181">deviceComplianceRequired</span></span>|<span data-ttu-id="e6312-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="e6312-182">Boolean</span></span>|<span data-ttu-id="e6312-183">指示是否需要设备符合性。</span><span class="sxs-lookup"><span data-stu-id="e6312-183">Indicates whether device compliance is required.</span></span> <span data-ttu-id="e6312-184">继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="e6312-184">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="e6312-185">managedBrowserToOpenLinksRequired</span><span class="sxs-lookup"><span data-stu-id="e6312-185">managedBrowserToOpenLinksRequired</span></span>|<span data-ttu-id="e6312-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="e6312-186">Boolean</span></span>|<span data-ttu-id="e6312-187">指示是否应在托管浏览器应用中打开 Internet 链接。</span><span class="sxs-lookup"><span data-stu-id="e6312-187">Indicates whether internet links should be opened in the managed browser app.</span></span> <span data-ttu-id="e6312-188">继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="e6312-188">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="e6312-189">saveAsBlocked</span><span class="sxs-lookup"><span data-stu-id="e6312-189">saveAsBlocked</span></span>|<span data-ttu-id="e6312-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="e6312-190">Boolean</span></span>|<span data-ttu-id="e6312-191">指示用户是否可以使用“另存为”菜单项保存受保护文件的副本。</span><span class="sxs-lookup"><span data-stu-id="e6312-191">Indicates whether users may use the "Save As" menu item to save a copy of protected files.</span></span> <span data-ttu-id="e6312-192">继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="e6312-192">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="e6312-193">periodOfflineBeforeWipeIsEnforced</span><span class="sxs-lookup"><span data-stu-id="e6312-193">periodOfflineBeforeWipeIsEnforced</span></span>|<span data-ttu-id="e6312-194">Duration</span><span class="sxs-lookup"><span data-stu-id="e6312-194">Duration</span></span>|<span data-ttu-id="e6312-195">在擦除所有托管数据之前，允许应用保持从 Internet 断开连接的时间量。</span><span class="sxs-lookup"><span data-stu-id="e6312-195">The amount of time an app is allowed to remain disconnected from the internet before all managed data it is wiped.</span></span> <span data-ttu-id="e6312-196">继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="e6312-196">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="e6312-197">pinRequired</span><span class="sxs-lookup"><span data-stu-id="e6312-197">pinRequired</span></span>|<span data-ttu-id="e6312-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="e6312-198">Boolean</span></span>|<span data-ttu-id="e6312-199">指示是否需要应用级 PIN。</span><span class="sxs-lookup"><span data-stu-id="e6312-199">Indicates whether an app-level pin is required.</span></span> <span data-ttu-id="e6312-200">继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="e6312-200">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="e6312-201">maximumPinRetries</span><span class="sxs-lookup"><span data-stu-id="e6312-201">maximumPinRetries</span></span>|<span data-ttu-id="e6312-202">Int32</span><span class="sxs-lookup"><span data-stu-id="e6312-202">Int32</span></span>|<span data-ttu-id="e6312-203">在擦除托管应用之前，不正确 PIN 重新尝试的最大尝试次数。</span><span class="sxs-lookup"><span data-stu-id="e6312-203">Maximum number of incorrect pin retry attempts before the managed app is wiped.</span></span> <span data-ttu-id="e6312-204">继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="e6312-204">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="e6312-205">simplePinBlocked</span><span class="sxs-lookup"><span data-stu-id="e6312-205">simplePinBlocked</span></span>|<span data-ttu-id="e6312-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="e6312-206">Boolean</span></span>|<span data-ttu-id="e6312-207">指示是否阻止 simplePin。</span><span class="sxs-lookup"><span data-stu-id="e6312-207">Indicates whether simplePin is blocked.</span></span> <span data-ttu-id="e6312-208">继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="e6312-208">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="e6312-209">minimumPinLength</span><span class="sxs-lookup"><span data-stu-id="e6312-209">minimumPinLength</span></span>|<span data-ttu-id="e6312-210">Int32</span><span class="sxs-lookup"><span data-stu-id="e6312-210">Int32</span></span>|<span data-ttu-id="e6312-211">PinRequired 设置为 True 时应用级 PIN 所需的最小 PIN 长度。继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="e6312-211">Minimum pin length required for an app-level pin if PinRequired is set to True Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="e6312-212">pinCharacterSet</span><span class="sxs-lookup"><span data-stu-id="e6312-212">pinCharacterSet</span></span>|<span data-ttu-id="e6312-213">String</span><span class="sxs-lookup"><span data-stu-id="e6312-213">String</span></span>|<span data-ttu-id="e6312-214">PinRequired 设置为 True 时可用于应用级 PIN 的字符集。</span><span class="sxs-lookup"><span data-stu-id="e6312-214">Character set which may be used for an app-level pin if PinRequired is set to True.</span></span> <span data-ttu-id="e6312-215">继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)。可取值为：`numeric`、`alphanumericAndSymbol`。</span><span class="sxs-lookup"><span data-stu-id="e6312-215">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md) Possible values are: `numeric`, `alphanumericAndSymbol`.</span></span>|
|<span data-ttu-id="e6312-216">periodBeforePinReset</span><span class="sxs-lookup"><span data-stu-id="e6312-216">periodBeforePinReset</span></span>|<span data-ttu-id="e6312-217">Duration</span><span class="sxs-lookup"><span data-stu-id="e6312-217">Duration</span></span>|<span data-ttu-id="e6312-218">TimePeriod，如果 PinRequired 设置为 True，必须在此之前重置所有级别的 PIN。</span><span class="sxs-lookup"><span data-stu-id="e6312-218">TimePeriod before the all-level pin must be reset if PinRequired is set to True.</span></span> <span data-ttu-id="e6312-219">继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="e6312-219">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="e6312-220">allowedDataStorageLocations</span><span class="sxs-lookup"><span data-stu-id="e6312-220">allowedDataStorageLocations</span></span>|<span data-ttu-id="e6312-221">String 集合</span><span class="sxs-lookup"><span data-stu-id="e6312-221">String collection</span></span>|<span data-ttu-id="e6312-222">用户可能存储托管数据的数据存储位置。</span><span class="sxs-lookup"><span data-stu-id="e6312-222">Data storage locations where a user may store managed data.</span></span> <span data-ttu-id="e6312-223">继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)。可取值为：`oneDriveForBusiness`、`sharePoint`、`localStorage`。</span><span class="sxs-lookup"><span data-stu-id="e6312-223">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md) Possible values are: `oneDriveForBusiness`, `sharePoint`, `localStorage`.</span></span>|
|<span data-ttu-id="e6312-224">contactSyncBlocked</span><span class="sxs-lookup"><span data-stu-id="e6312-224">contactSyncBlocked</span></span>|<span data-ttu-id="e6312-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="e6312-225">Boolean</span></span>|<span data-ttu-id="e6312-226">指示联系人是否可以同步到用户的设备。</span><span class="sxs-lookup"><span data-stu-id="e6312-226">Indicates whether contacts can be synced to the user's device.</span></span> <span data-ttu-id="e6312-227">继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="e6312-227">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="e6312-228">printBlocked</span><span class="sxs-lookup"><span data-stu-id="e6312-228">printBlocked</span></span>|<span data-ttu-id="e6312-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="e6312-229">Boolean</span></span>|<span data-ttu-id="e6312-230">指示是否允许从托管应用进行打印。</span><span class="sxs-lookup"><span data-stu-id="e6312-230">Indicates whether printing is allowed from managed apps.</span></span> <span data-ttu-id="e6312-231">继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="e6312-231">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="e6312-232">fingerprintBlocked</span><span class="sxs-lookup"><span data-stu-id="e6312-232">fingerprintBlocked</span></span>|<span data-ttu-id="e6312-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="e6312-233">Boolean</span></span>|<span data-ttu-id="e6312-234">指示如果 PinRequired 设置为 True，是否允许使用指纹读取器代替 PIN。</span><span class="sxs-lookup"><span data-stu-id="e6312-234">Indicates whether use of the fingerprint reader is allowed in place of a pin if PinRequired is set to True.</span></span> <span data-ttu-id="e6312-235">继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="e6312-235">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="e6312-236">disableAppPinIfDevicePinIsSet</span><span class="sxs-lookup"><span data-stu-id="e6312-236">disableAppPinIfDevicePinIsSet</span></span>|<span data-ttu-id="e6312-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="e6312-237">Boolean</span></span>|<span data-ttu-id="e6312-238">指示如果设置了设备 PIN，是否需要使用应用 PIN。</span><span class="sxs-lookup"><span data-stu-id="e6312-238">Indicates whether use of the app pin is required if the device pin is set.</span></span> <span data-ttu-id="e6312-239">继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="e6312-239">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="e6312-240">minimumRequiredOsVersion</span><span class="sxs-lookup"><span data-stu-id="e6312-240">minimumRequiredOsVersion</span></span>|<span data-ttu-id="e6312-241">String</span><span class="sxs-lookup"><span data-stu-id="e6312-241">String</span></span>|<span data-ttu-id="e6312-242">低于指定版本的版本将阻止托管应用访问公司数据。</span><span class="sxs-lookup"><span data-stu-id="e6312-242">Versions less than the specified version will block the managed app from accessing company data.</span></span> <span data-ttu-id="e6312-243">继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="e6312-243">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="e6312-244">minimumWarningOsVersion</span><span class="sxs-lookup"><span data-stu-id="e6312-244">minimumWarningOsVersion</span></span>|<span data-ttu-id="e6312-245">String</span><span class="sxs-lookup"><span data-stu-id="e6312-245">String</span></span>|<span data-ttu-id="e6312-246">低于指定版本的版本将导致托管应用访问公司数据时出现警告消息。</span><span class="sxs-lookup"><span data-stu-id="e6312-246">Versions less than the specified version will result in warning message on the managed app from accessing company data.</span></span> <span data-ttu-id="e6312-247">继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="e6312-247">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="e6312-248">minimumRequiredAppVersion</span><span class="sxs-lookup"><span data-stu-id="e6312-248">minimumRequiredAppVersion</span></span>|<span data-ttu-id="e6312-249">String</span><span class="sxs-lookup"><span data-stu-id="e6312-249">String</span></span>|<span data-ttu-id="e6312-250">低于指定版本的版本将阻止托管应用访问公司数据。</span><span class="sxs-lookup"><span data-stu-id="e6312-250">Versions less than the specified version will block the managed app from accessing company data.</span></span> <span data-ttu-id="e6312-251">继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="e6312-251">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="e6312-252">minimumWarningAppVersion</span><span class="sxs-lookup"><span data-stu-id="e6312-252">minimumWarningAppVersion</span></span>|<span data-ttu-id="e6312-253">String</span><span class="sxs-lookup"><span data-stu-id="e6312-253">String</span></span>|<span data-ttu-id="e6312-254">低于指定版本的版本将导致托管应用出现警告消息。</span><span class="sxs-lookup"><span data-stu-id="e6312-254">Versions less than the specified version will result in warning message on the managed app.</span></span> <span data-ttu-id="e6312-255">继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="e6312-255">Inherited from [managedAppProtection](../resources/intune_mam_managedappprotection.md)</span></span>|
|<span data-ttu-id="e6312-256">isAssigned</span><span class="sxs-lookup"><span data-stu-id="e6312-256">isAssigned</span></span>|<span data-ttu-id="e6312-257">Boolean</span><span class="sxs-lookup"><span data-stu-id="e6312-257">Boolean</span></span>|<span data-ttu-id="e6312-258">指示策略是否部署到任何包含组。</span><span class="sxs-lookup"><span data-stu-id="e6312-258">Indicates if the policy is deployed to any inclusion groups or not.</span></span> <span data-ttu-id="e6312-259">继承自 [targetedManagedAppProtection](../resources/intune_mam_targetedmanagedappprotection.md)</span><span class="sxs-lookup"><span data-stu-id="e6312-259">Inherited from [targetedManagedAppProtection](../resources/intune_mam_targetedmanagedappprotection.md)</span></span>|
|<span data-ttu-id="e6312-260">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="e6312-260">screenCaptureBlocked</span></span>|<span data-ttu-id="e6312-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="e6312-261">Boolean</span></span>|<span data-ttu-id="e6312-262">指示托管用户是否可以对托管应用进行屏幕截图</span><span class="sxs-lookup"><span data-stu-id="e6312-262">Indicates whether a managed user can take screen captures of managed apps</span></span>|
|<span data-ttu-id="e6312-263">disableAppEncryptionIfDeviceEncryptionIsEnabled</span><span class="sxs-lookup"><span data-stu-id="e6312-263">disableAppEncryptionIfDeviceEncryptionIsEnabled</span></span>|<span data-ttu-id="e6312-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="e6312-264">Boolean</span></span>|<span data-ttu-id="e6312-265">启用此设置后，如果启用设备级加密，则应用级加密将被禁用</span><span class="sxs-lookup"><span data-stu-id="e6312-265">When this setting is enabled, app level encryption is disabled if device level encryption is enabled</span></span>|
|<span data-ttu-id="e6312-266">encryptAppData</span><span class="sxs-lookup"><span data-stu-id="e6312-266">encryptAppData</span></span>|<span data-ttu-id="e6312-267">Boolean</span><span class="sxs-lookup"><span data-stu-id="e6312-267">Boolean</span></span>|<span data-ttu-id="e6312-268">指示是否应加密托管应用的应用程序数据</span><span class="sxs-lookup"><span data-stu-id="e6312-268">Indicates whether application data for managed apps should be encrypted</span></span>|
|<span data-ttu-id="e6312-269">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="e6312-269">deployedAppCount</span></span>|<span data-ttu-id="e6312-270">Int32</span><span class="sxs-lookup"><span data-stu-id="e6312-270">Int32</span></span>|<span data-ttu-id="e6312-271">当前策略部署到的应用的数量。</span><span class="sxs-lookup"><span data-stu-id="e6312-271">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="e6312-272">minimumRequiredPatchVersion</span><span class="sxs-lookup"><span data-stu-id="e6312-272">minimumRequiredPatchVersion</span></span>|<span data-ttu-id="e6312-273">String</span><span class="sxs-lookup"><span data-stu-id="e6312-273">String</span></span>|<span data-ttu-id="e6312-274">定义用户可以获得对应用的安全访问权限所需的最早的必需 Android 安全修补程序级别。</span><span class="sxs-lookup"><span data-stu-id="e6312-274">Define the oldest required Android security patch level a user can have to gain secure access to the app.</span></span>|
|<span data-ttu-id="e6312-275">minimumWarningPatchVersion</span><span class="sxs-lookup"><span data-stu-id="e6312-275">minimumWarningPatchVersion</span></span>|<span data-ttu-id="e6312-276">String</span><span class="sxs-lookup"><span data-stu-id="e6312-276">String</span></span>|<span data-ttu-id="e6312-277">定义用户可以获得对应用的安全访问权限所需的最早推荐 Android 安全修补程序级别。</span><span class="sxs-lookup"><span data-stu-id="e6312-277">Define the oldest recommended Android security patch level a user can have for secure access to the app.</span></span>|



## <a name="response"></a><span data-ttu-id="e6312-278">响应</span><span class="sxs-lookup"><span data-stu-id="e6312-278">Response</span></span>
<span data-ttu-id="e6312-279">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [androidManagedAppProtection](../resources/intune_mam_androidmanagedappprotection.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e6312-279">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_mam_androidmanagedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e6312-280">示例</span><span class="sxs-lookup"><span data-stu-id="e6312-280">Example</span></span>
### <a name="request"></a><span data-ttu-id="e6312-281">请求</span><span class="sxs-lookup"><span data-stu-id="e6312-281">Request</span></span>
<span data-ttu-id="e6312-282">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e6312-282">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}
Content-type: application/json
Content-length: 1690

{
  "displayName": "Display Name value",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": "Version value",
  "periodOfflineBeforeAccessCheck": "-PT17.1357909S",
  "periodOnlineBeforeAccessCheck": "PT35.0018757S",
  "allowedInboundDataTransferSources": "managedApps",
  "allowedOutboundDataTransferDestinations": "managedApps",
  "organizationalCredentialsRequired": true,
  "allowedOutboundClipboardSharingLevel": "managedAppsWithPasteIn",
  "dataBackupBlocked": true,
  "deviceComplianceRequired": true,
  "managedBrowserToOpenLinksRequired": true,
  "saveAsBlocked": true,
  "periodOfflineBeforeWipeIsEnforced": "-PT3M22.1587532S",
  "pinRequired": true,
  "maximumPinRetries": 1,
  "simplePinBlocked": true,
  "minimumPinLength": 0,
  "pinCharacterSet": "alphanumericAndSymbol",
  "periodBeforePinReset": "PT3M29.6631862S",
  "allowedDataStorageLocations": [
    "sharePoint"
  ],
  "contactSyncBlocked": true,
  "printBlocked": true,
  "fingerprintBlocked": true,
  "disableAppPinIfDevicePinIsSet": true,
  "minimumRequiredOsVersion": "Minimum Required Os Version value",
  "minimumWarningOsVersion": "Minimum Warning Os Version value",
  "minimumRequiredAppVersion": "Minimum Required App Version value",
  "minimumWarningAppVersion": "Minimum Warning App Version value",
  "isAssigned": true,
  "screenCaptureBlocked": true,
  "disableAppEncryptionIfDeviceEncryptionIsEnabled": true,
  "encryptAppData": true,
  "deployedAppCount": 0,
  "minimumRequiredPatchVersion": "Minimum Required Patch Version value",
  "minimumWarningPatchVersion": "Minimum Warning Patch Version value"
}
```

### <a name="response"></a><span data-ttu-id="e6312-283">响应</span><span class="sxs-lookup"><span data-stu-id="e6312-283">Response</span></span>
<span data-ttu-id="e6312-p134">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e6312-p134">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1864

{
  "@odata.type": "#microsoft.graph.androidManagedAppProtection",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "id": "cf517ced-7ced-cf51-ed7c-51cfed7c51cf",
  "version": "Version value",
  "periodOfflineBeforeAccessCheck": "-PT17.1357909S",
  "periodOnlineBeforeAccessCheck": "PT35.0018757S",
  "allowedInboundDataTransferSources": "managedApps",
  "allowedOutboundDataTransferDestinations": "managedApps",
  "organizationalCredentialsRequired": true,
  "allowedOutboundClipboardSharingLevel": "managedAppsWithPasteIn",
  "dataBackupBlocked": true,
  "deviceComplianceRequired": true,
  "managedBrowserToOpenLinksRequired": true,
  "saveAsBlocked": true,
  "periodOfflineBeforeWipeIsEnforced": "-PT3M22.1587532S",
  "pinRequired": true,
  "maximumPinRetries": 1,
  "simplePinBlocked": true,
  "minimumPinLength": 0,
  "pinCharacterSet": "alphanumericAndSymbol",
  "periodBeforePinReset": "PT3M29.6631862S",
  "allowedDataStorageLocations": [
    "sharePoint"
  ],
  "contactSyncBlocked": true,
  "printBlocked": true,
  "fingerprintBlocked": true,
  "disableAppPinIfDevicePinIsSet": true,
  "minimumRequiredOsVersion": "Minimum Required Os Version value",
  "minimumWarningOsVersion": "Minimum Warning Os Version value",
  "minimumRequiredAppVersion": "Minimum Required App Version value",
  "minimumWarningAppVersion": "Minimum Warning App Version value",
  "isAssigned": true,
  "screenCaptureBlocked": true,
  "disableAppEncryptionIfDeviceEncryptionIsEnabled": true,
  "encryptAppData": true,
  "deployedAppCount": 0,
  "minimumRequiredPatchVersion": "Minimum Required Patch Version value",
  "minimumWarningPatchVersion": "Minimum Warning Patch Version value"
}
```


