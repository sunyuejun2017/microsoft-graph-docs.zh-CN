# <a name="update-webapp"></a><span data-ttu-id="ad5ef-101">更新 webApp</span><span class="sxs-lookup"><span data-stu-id="ad5ef-101">Update webApp</span></span>

> <span data-ttu-id="ad5ef-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="ad5ef-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ad5ef-103">更新 [webApp](../resources/intune_apps_webapp.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ad5ef-103">Update the properties of a [calendar](../resources/intune_apps_webapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ad5ef-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="ad5ef-104">Prerequisites</span></span>
<span data-ttu-id="ad5ef-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="ad5ef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ad5ef-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="ad5ef-107">Permission type</span></span>|<span data-ttu-id="ad5ef-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ad5ef-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ad5ef-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ad5ef-109">Delegated (work or school account)</span></span>|<span data-ttu-id="ad5ef-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad5ef-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ad5ef-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ad5ef-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ad5ef-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="ad5ef-112">Not supported.</span></span>|
|<span data-ttu-id="ad5ef-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="ad5ef-113">Application</span></span>|<span data-ttu-id="ad5ef-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ad5ef-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ad5ef-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ad5ef-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="ad5ef-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="ad5ef-116">Request headers</span></span>
|<span data-ttu-id="ad5ef-117">标头</span><span class="sxs-lookup"><span data-stu-id="ad5ef-117">Header</span></span>|<span data-ttu-id="ad5ef-118">值</span><span class="sxs-lookup"><span data-stu-id="ad5ef-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ad5ef-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="ad5ef-119">Authorization</span></span>|<span data-ttu-id="ad5ef-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ad5ef-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="ad5ef-121">Accept</span><span class="sxs-lookup"><span data-stu-id="ad5ef-121">Accept</span></span>|<span data-ttu-id="ad5ef-122">application/json</span><span class="sxs-lookup"><span data-stu-id="ad5ef-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ad5ef-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="ad5ef-123">Request body</span></span>
<span data-ttu-id="ad5ef-124">在请求正文中，提供 [webApp](../resources/intune_apps_webapp.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ad5ef-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_apps_webapp.md) object.</span></span>

<span data-ttu-id="ad5ef-125">下表显示创建 [webApp](../resources/intune_apps_webapp.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ad5ef-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="ad5ef-126">属性</span><span class="sxs-lookup"><span data-stu-id="ad5ef-126">Property</span></span>|<span data-ttu-id="ad5ef-127">类型</span><span class="sxs-lookup"><span data-stu-id="ad5ef-127">Type</span></span>|<span data-ttu-id="ad5ef-128">说明</span><span class="sxs-lookup"><span data-stu-id="ad5ef-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ad5ef-129">id</span><span class="sxs-lookup"><span data-stu-id="ad5ef-129">id</span></span>|<span data-ttu-id="ad5ef-130">String</span><span class="sxs-lookup"><span data-stu-id="ad5ef-130">String</span></span>|<span data-ttu-id="ad5ef-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="ad5ef-131">Key of the setting.</span></span> <span data-ttu-id="ad5ef-132">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ad5ef-132">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ad5ef-133">displayName</span><span class="sxs-lookup"><span data-stu-id="ad5ef-133">displayName</span></span>|<span data-ttu-id="ad5ef-134">String</span><span class="sxs-lookup"><span data-stu-id="ad5ef-134">String</span></span>|<span data-ttu-id="ad5ef-135">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="ad5ef-135">The admin provided or imported title of the app.</span></span> <span data-ttu-id="ad5ef-136">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ad5ef-136">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ad5ef-137">description</span><span class="sxs-lookup"><span data-stu-id="ad5ef-137">description</span></span>|<span data-ttu-id="ad5ef-138">String</span><span class="sxs-lookup"><span data-stu-id="ad5ef-138">String</span></span>|<span data-ttu-id="ad5ef-139">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="ad5ef-139">The description of the app.</span></span> <span data-ttu-id="ad5ef-140">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ad5ef-140">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ad5ef-141">publisher</span><span class="sxs-lookup"><span data-stu-id="ad5ef-141">Publisher</span></span>|<span data-ttu-id="ad5ef-142">String</span><span class="sxs-lookup"><span data-stu-id="ad5ef-142">String</span></span>|<span data-ttu-id="ad5ef-143">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="ad5ef-143">The name of the app.</span></span> <span data-ttu-id="ad5ef-144">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ad5ef-144">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ad5ef-145">largeIcon</span><span class="sxs-lookup"><span data-stu-id="ad5ef-145">largeIcon</span></span>|[<span data-ttu-id="ad5ef-146">mimeContent</span><span class="sxs-lookup"><span data-stu-id="ad5ef-146">mimeContent</span></span>](../resources/intune_apps_mimecontent.md)|<span data-ttu-id="ad5ef-147">要显示在应用详细信息中并用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="ad5ef-147">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="ad5ef-148">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ad5ef-148">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ad5ef-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ad5ef-149">createdDateTime</span></span>|<span data-ttu-id="ad5ef-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ad5ef-150">DateTimeOffset</span></span>|<span data-ttu-id="ad5ef-151">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="ad5ef-151">The date and time when the page was created.</span></span> <span data-ttu-id="ad5ef-152">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ad5ef-152">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ad5ef-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ad5ef-153">lastModifiedDateTime</span></span>|<span data-ttu-id="ad5ef-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ad5ef-154">DateTimeOffset</span></span>|<span data-ttu-id="ad5ef-155">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="ad5ef-155">The date and time when the attachment was last modified.</span></span> <span data-ttu-id="ad5ef-156">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ad5ef-156">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ad5ef-157">isFeatured</span><span class="sxs-lookup"><span data-stu-id="ad5ef-157">isFeatured</span></span>|<span data-ttu-id="ad5ef-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad5ef-158">Boolean</span></span>|<span data-ttu-id="ad5ef-159">指示应用是否被管理员标记为特色的值。继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ad5ef-159">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ad5ef-160">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="ad5ef-160">privacyInformationUrl</span></span>|<span data-ttu-id="ad5ef-161">String</span><span class="sxs-lookup"><span data-stu-id="ad5ef-161">String</span></span>|<span data-ttu-id="ad5ef-162">隐私声明 URL。</span><span class="sxs-lookup"><span data-stu-id="ad5ef-162">The privacy statement Url.</span></span> <span data-ttu-id="ad5ef-163">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ad5ef-163">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ad5ef-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="ad5ef-164">informationUrl</span></span>|<span data-ttu-id="ad5ef-165">String</span><span class="sxs-lookup"><span data-stu-id="ad5ef-165">String</span></span>|<span data-ttu-id="ad5ef-166">详细信息 URL。</span><span class="sxs-lookup"><span data-stu-id="ad5ef-166">The more information Url.</span></span> <span data-ttu-id="ad5ef-167">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ad5ef-167">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ad5ef-168">owner</span><span class="sxs-lookup"><span data-stu-id="ad5ef-168">owner</span></span>|<span data-ttu-id="ad5ef-169">String</span><span class="sxs-lookup"><span data-stu-id="ad5ef-169">String</span></span>|<span data-ttu-id="ad5ef-170">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="ad5ef-170">The owner of the timesheet.</span></span> <span data-ttu-id="ad5ef-171">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ad5ef-171">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ad5ef-172">developer</span><span class="sxs-lookup"><span data-stu-id="ad5ef-172">developer</span></span>|<span data-ttu-id="ad5ef-173">String</span><span class="sxs-lookup"><span data-stu-id="ad5ef-173">String</span></span>|<span data-ttu-id="ad5ef-174">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="ad5ef-174">The name of the app.</span></span> <span data-ttu-id="ad5ef-175">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ad5ef-175">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ad5ef-176">notes</span><span class="sxs-lookup"><span data-stu-id="ad5ef-176">notes</span></span>|<span data-ttu-id="ad5ef-177">String</span><span class="sxs-lookup"><span data-stu-id="ad5ef-177">String</span></span>|<span data-ttu-id="ad5ef-178">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="ad5ef-178">Notes for the app.</span></span> <span data-ttu-id="ad5ef-179">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="ad5ef-179">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="ad5ef-180">publishingState</span><span class="sxs-lookup"><span data-stu-id="ad5ef-180">publishingState</span></span>|<span data-ttu-id="ad5ef-181">String</span><span class="sxs-lookup"><span data-stu-id="ad5ef-181">String</span></span>|<span data-ttu-id="ad5ef-182">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="ad5ef-182">The publishing state for the app.</span></span> <span data-ttu-id="ad5ef-183">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="ad5ef-183">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="ad5ef-184">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)。可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="ad5ef-184">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md) Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="ad5ef-185">appUrl</span><span class="sxs-lookup"><span data-stu-id="ad5ef-185">appUrl</span></span>|<span data-ttu-id="ad5ef-186">String</span><span class="sxs-lookup"><span data-stu-id="ad5ef-186">String</span></span>|<span data-ttu-id="ad5ef-187">Web 应用 URL。</span><span class="sxs-lookup"><span data-stu-id="ad5ef-187">The web app URL.</span></span>|
|<span data-ttu-id="ad5ef-188">useManagedBrowser</span><span class="sxs-lookup"><span data-stu-id="ad5ef-188">useManagedBrowser</span></span>|<span data-ttu-id="ad5ef-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="ad5ef-189">Boolean</span></span>|<span data-ttu-id="ad5ef-190">是否使用托管浏览器。</span><span class="sxs-lookup"><span data-stu-id="ad5ef-190">Whether or not to use managed browser.</span></span> <span data-ttu-id="ad5ef-191">此属性仅适用于 Android 和 iOS。</span><span class="sxs-lookup"><span data-stu-id="ad5ef-191">This property is only applicable for Android and IOS.</span></span>|



## <a name="response"></a><span data-ttu-id="ad5ef-192">响应</span><span class="sxs-lookup"><span data-stu-id="ad5ef-192">Response</span></span>
<span data-ttu-id="ad5ef-193">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [webApp](../resources/intune_apps_webapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ad5ef-193">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_apps_webapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ad5ef-194">示例</span><span class="sxs-lookup"><span data-stu-id="ad5ef-194">Example</span></span>
### <a name="request"></a><span data-ttu-id="ad5ef-195">请求</span><span class="sxs-lookup"><span data-stu-id="ad5ef-195">Request</span></span>
<span data-ttu-id="ad5ef-196">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ad5ef-196">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 664

{
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
  "appUrl": "https://example.com/appUrl/",
  "useManagedBrowser": true
}
```

### <a name="response"></a><span data-ttu-id="ad5ef-197">响应</span><span class="sxs-lookup"><span data-stu-id="ad5ef-197">Response</span></span>
<span data-ttu-id="ad5ef-p116">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ad5ef-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 817

{
  "@odata.type": "#microsoft.graph.webApp",
  "id": "4bdc5d30-5d30-4bdc-305d-dc4b305ddc4b",
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
  "appUrl": "https://example.com/appUrl/",
  "useManagedBrowser": true
}
```


