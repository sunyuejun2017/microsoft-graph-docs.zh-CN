# <a name="create-androidlobapp"></a><span data-ttu-id="b101d-101">创建 androidLobApp</span><span class="sxs-lookup"><span data-stu-id="b101d-101">Create androidLobApp</span></span>

> <span data-ttu-id="b101d-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="b101d-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b101d-103">创建新的 [androidLobApp](../resources/intune_apps_androidlobapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b101d-103">Create a new [plannerBucket](../resources/intune_apps_androidlobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b101d-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="b101d-104">Prerequisites</span></span>
<span data-ttu-id="b101d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="b101d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b101d-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="b101d-107">Permission type</span></span>|<span data-ttu-id="b101d-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b101d-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b101d-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b101d-109">Delegated (work or school account)</span></span>|<span data-ttu-id="b101d-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b101d-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b101d-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b101d-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b101d-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="b101d-112">Not supported.</span></span>|
|<span data-ttu-id="b101d-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="b101d-113">Application</span></span>|<span data-ttu-id="b101d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b101d-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b101d-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b101d-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="b101d-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="b101d-116">Request headers</span></span>
|<span data-ttu-id="b101d-117">标头</span><span class="sxs-lookup"><span data-stu-id="b101d-117">Header</span></span>|<span data-ttu-id="b101d-118">值</span><span class="sxs-lookup"><span data-stu-id="b101d-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b101d-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="b101d-119">Authorization</span></span>|<span data-ttu-id="b101d-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b101d-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="b101d-121">Accept</span><span class="sxs-lookup"><span data-stu-id="b101d-121">Accept</span></span>|<span data-ttu-id="b101d-122">application/json</span><span class="sxs-lookup"><span data-stu-id="b101d-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b101d-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="b101d-123">Request body</span></span>
<span data-ttu-id="b101d-124">在请求正文中，提供 androidLobApp 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b101d-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="b101d-125">下表显示了创建 androidLobApp 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b101d-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="b101d-126">属性</span><span class="sxs-lookup"><span data-stu-id="b101d-126">Property</span></span>|<span data-ttu-id="b101d-127">类型</span><span class="sxs-lookup"><span data-stu-id="b101d-127">Type</span></span>|<span data-ttu-id="b101d-128">说明</span><span class="sxs-lookup"><span data-stu-id="b101d-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b101d-129">id</span><span class="sxs-lookup"><span data-stu-id="b101d-129">id</span></span>|<span data-ttu-id="b101d-130">String</span><span class="sxs-lookup"><span data-stu-id="b101d-130">String</span></span>|<span data-ttu-id="b101d-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b101d-131">Key of the setting.</span></span> <span data-ttu-id="b101d-132">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b101d-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="b101d-133">displayName</span><span class="sxs-lookup"><span data-stu-id="b101d-133">displayName</span></span>|<span data-ttu-id="b101d-134">String</span><span class="sxs-lookup"><span data-stu-id="b101d-134">String</span></span>|<span data-ttu-id="b101d-135">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="b101d-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="b101d-136">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b101d-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="b101d-137">description</span><span class="sxs-lookup"><span data-stu-id="b101d-137">description</span></span>|<span data-ttu-id="b101d-138">String</span><span class="sxs-lookup"><span data-stu-id="b101d-138">String</span></span>|<span data-ttu-id="b101d-139">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="b101d-139">The description of the app.</span></span> <span data-ttu-id="b101d-140">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b101d-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="b101d-141">publisher</span><span class="sxs-lookup"><span data-stu-id="b101d-141">Publisher</span></span>|<span data-ttu-id="b101d-142">String</span><span class="sxs-lookup"><span data-stu-id="b101d-142">String</span></span>|<span data-ttu-id="b101d-143">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="b101d-143">The name of the app.</span></span> <span data-ttu-id="b101d-144">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b101d-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="b101d-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="b101d-145">largeIcon</span></span>|[<span data-ttu-id="b101d-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="b101d-146">mimeContent</span></span>](../resources/intune_apps_mimecontent.md)|<span data-ttu-id="b101d-147">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="b101d-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="b101d-148">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b101d-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="b101d-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b101d-149">createdDateTime</span></span>|<span data-ttu-id="b101d-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b101d-150">DateTimeOffset</span></span>|<span data-ttu-id="b101d-151">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="b101d-151">The date and time when the page was created.</span></span> <span data-ttu-id="b101d-152">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b101d-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="b101d-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b101d-153">lastModifiedDateTime</span></span>|<span data-ttu-id="b101d-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b101d-154">DateTimeOffset</span></span>|<span data-ttu-id="b101d-155">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="b101d-155">The date and time when the attachment was last modified.</span></span> <span data-ttu-id="b101d-156">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b101d-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="b101d-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="b101d-157">isFeatured</span></span>|<span data-ttu-id="b101d-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="b101d-158">Boolean</span></span>|<span data-ttu-id="b101d-159">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b101d-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="b101d-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="b101d-160">privacyInformationUrl</span></span>|<span data-ttu-id="b101d-161">String</span><span class="sxs-lookup"><span data-stu-id="b101d-161">String</span></span>|<span data-ttu-id="b101d-162">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="b101d-162">The privacy statement Url.</span></span> <span data-ttu-id="b101d-163">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b101d-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="b101d-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="b101d-164">informationUrl</span></span>|<span data-ttu-id="b101d-165">String</span><span class="sxs-lookup"><span data-stu-id="b101d-165">String</span></span>|<span data-ttu-id="b101d-166">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="b101d-166">The more information Url.</span></span> <span data-ttu-id="b101d-167">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b101d-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="b101d-168">owner</span><span class="sxs-lookup"><span data-stu-id="b101d-168">owner</span></span>|<span data-ttu-id="b101d-169">String</span><span class="sxs-lookup"><span data-stu-id="b101d-169">String</span></span>|<span data-ttu-id="b101d-170">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="b101d-170">The owner of the timesheet.</span></span> <span data-ttu-id="b101d-171">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b101d-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="b101d-172">developer</span><span class="sxs-lookup"><span data-stu-id="b101d-172">developer</span></span>|<span data-ttu-id="b101d-173">String</span><span class="sxs-lookup"><span data-stu-id="b101d-173">String</span></span>|<span data-ttu-id="b101d-174">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="b101d-174">The name of the app.</span></span> <span data-ttu-id="b101d-175">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b101d-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="b101d-176">notes</span><span class="sxs-lookup"><span data-stu-id="b101d-176">notes</span></span>|<span data-ttu-id="b101d-177">String</span><span class="sxs-lookup"><span data-stu-id="b101d-177">String</span></span>|<span data-ttu-id="b101d-178">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="b101d-178">Notes for the app.</span></span> <span data-ttu-id="b101d-179">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="b101d-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="b101d-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="b101d-180">publishingState</span></span>|<span data-ttu-id="b101d-181">String</span><span class="sxs-lookup"><span data-stu-id="b101d-181">String</span></span>|<span data-ttu-id="b101d-182">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="b101d-182">The publishing state for the app.</span></span> <span data-ttu-id="b101d-183">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="b101d-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="b101d-184">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)。可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="b101d-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md) Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="b101d-185">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="b101d-185">committedContentVersion</span></span>|<span data-ttu-id="b101d-186">String</span><span class="sxs-lookup"><span data-stu-id="b101d-186">String</span></span>|<span data-ttu-id="b101d-187">内部提交的内容版本。</span><span class="sxs-lookup"><span data-stu-id="b101d-187">The internal committed content version.</span></span> <span data-ttu-id="b101d-188">继承自 [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="b101d-188">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="b101d-189">fileName</span><span class="sxs-lookup"><span data-stu-id="b101d-189">fileName</span></span>|<span data-ttu-id="b101d-190">String</span><span class="sxs-lookup"><span data-stu-id="b101d-190">String</span></span>|<span data-ttu-id="b101d-191">主 Lob 应用程序文件的名称。</span><span class="sxs-lookup"><span data-stu-id="b101d-191">The name of the main Lob application file.</span></span> <span data-ttu-id="b101d-192">继承自 [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="b101d-192">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="b101d-193">size</span><span class="sxs-lookup"><span data-stu-id="b101d-193">size</span></span>|<span data-ttu-id="b101d-194">Int64</span><span class="sxs-lookup"><span data-stu-id="b101d-194">Int64</span></span>|<span data-ttu-id="b101d-195">总大小，包括所有已上传文件。</span><span class="sxs-lookup"><span data-stu-id="b101d-195">The total size, including all uploaded files.</span></span> <span data-ttu-id="b101d-196">继承自 [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="b101d-196">Inherited from [mobileLobApp](../resources/intune_apps_mobilelobapp.md)</span></span>|
|<span data-ttu-id="b101d-197">packageId</span><span class="sxs-lookup"><span data-stu-id="b101d-197">PackageId</span></span>|<span data-ttu-id="b101d-198">String</span><span class="sxs-lookup"><span data-stu-id="b101d-198">String</span></span>|<span data-ttu-id="b101d-199">包标识符。</span><span class="sxs-lookup"><span data-stu-id="b101d-199">The package identifier.</span></span>|
|<span data-ttu-id="b101d-200">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="b101d-200">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="b101d-201">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="b101d-201">androidMinimumOperatingSystem</span></span>](../resources/intune_apps_androidminimumoperatingsystem.md)|<span data-ttu-id="b101d-202">最低适用操作系统的值。</span><span class="sxs-lookup"><span data-stu-id="b101d-202">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="b101d-203">versionName</span><span class="sxs-lookup"><span data-stu-id="b101d-203">versionName</span></span>|<span data-ttu-id="b101d-204">String</span><span class="sxs-lookup"><span data-stu-id="b101d-204">String</span></span>|<span data-ttu-id="b101d-205">Android 业务线 (LoB) 应用的版本名称。</span><span class="sxs-lookup"><span data-stu-id="b101d-205">The version name of Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="b101d-206">versionCode</span><span class="sxs-lookup"><span data-stu-id="b101d-206">versionCode</span></span>|<span data-ttu-id="b101d-207">String</span><span class="sxs-lookup"><span data-stu-id="b101d-207">String</span></span>|<span data-ttu-id="b101d-208">Android 业务线 (LoB) 应用的版本代码。</span><span class="sxs-lookup"><span data-stu-id="b101d-208">The version code of Android Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="b101d-209">响应</span><span class="sxs-lookup"><span data-stu-id="b101d-209">Response</span></span>
<span data-ttu-id="b101d-210">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [androidLobApp](../resources/intune_apps_androidlobapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b101d-210">If successful, this method returns a `201 Created` response code and a [ListItemVersion](../resources/intune_apps_androidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b101d-211">示例</span><span class="sxs-lookup"><span data-stu-id="b101d-211">Example</span></span>
### <a name="request"></a><span data-ttu-id="b101d-212">请求</span><span class="sxs-lookup"><span data-stu-id="b101d-212">Request</span></span>
<span data-ttu-id="b101d-213">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b101d-213">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1139

{
  "@odata.type": "#microsoft.graph.androidLobApp",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "publishingState": "processing",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "packageId": "Package Id value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value"
}
```

### <a name="response"></a><span data-ttu-id="b101d-214">响应</span><span class="sxs-lookup"><span data-stu-id="b101d-214">Response</span></span>
<span data-ttu-id="b101d-p118">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b101d-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1247

{
  "@odata.type": "#microsoft.graph.androidLobApp",
  "id": "4b9a27d0-27d0-4b9a-d027-9a4bd0279a4b",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "publishingState": "processing",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "packageId": "Package Id value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value"
}
```


