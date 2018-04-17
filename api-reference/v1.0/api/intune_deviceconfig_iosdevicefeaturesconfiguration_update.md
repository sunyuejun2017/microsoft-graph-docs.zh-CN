# <a name="update-iosdevicefeaturesconfiguration"></a><span data-ttu-id="5dabb-101">更新 iosDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="5dabb-101">Update iosDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="5dabb-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="5dabb-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5dabb-103">更新 [iosDeviceFeaturesConfiguration](../resources/intune_deviceconfig_iosdevicefeaturesconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="5dabb-103">Update the properties of a [calendar](../resources/intune_deviceconfig_iosdevicefeaturesconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5dabb-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="5dabb-104">Prerequisites</span></span>
<span data-ttu-id="5dabb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="5dabb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5dabb-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="5dabb-107">Permission type</span></span>|<span data-ttu-id="5dabb-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="5dabb-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5dabb-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5dabb-109">Delegated (work or school account)</span></span>|<span data-ttu-id="5dabb-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5dabb-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5dabb-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5dabb-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5dabb-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="5dabb-112">Not supported.</span></span>|
|<span data-ttu-id="5dabb-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="5dabb-113">Application</span></span>|<span data-ttu-id="5dabb-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="5dabb-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5dabb-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5dabb-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="5dabb-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="5dabb-116">Request headers</span></span>
|<span data-ttu-id="5dabb-117">标头</span><span class="sxs-lookup"><span data-stu-id="5dabb-117">Header</span></span>|<span data-ttu-id="5dabb-118">值</span><span class="sxs-lookup"><span data-stu-id="5dabb-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5dabb-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="5dabb-119">Authorization</span></span>|<span data-ttu-id="5dabb-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="5dabb-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="5dabb-121">Accept</span><span class="sxs-lookup"><span data-stu-id="5dabb-121">Accept</span></span>|<span data-ttu-id="5dabb-122">application/json</span><span class="sxs-lookup"><span data-stu-id="5dabb-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5dabb-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="5dabb-123">Request body</span></span>
<span data-ttu-id="5dabb-124">在请求正文中，提供 [iosDeviceFeaturesConfiguration](../resources/intune_deviceconfig_iosdevicefeaturesconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5dabb-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_deviceconfig_iosdevicefeaturesconfiguration.md) object.</span></span>

<span data-ttu-id="5dabb-125">下表显示创建 [iosDeviceFeaturesConfiguration](../resources/intune_deviceconfig_iosdevicefeaturesconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="5dabb-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="5dabb-126">属性</span><span class="sxs-lookup"><span data-stu-id="5dabb-126">Property</span></span>|<span data-ttu-id="5dabb-127">类型</span><span class="sxs-lookup"><span data-stu-id="5dabb-127">Type</span></span>|<span data-ttu-id="5dabb-128">说明</span><span class="sxs-lookup"><span data-stu-id="5dabb-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5dabb-129">id</span><span class="sxs-lookup"><span data-stu-id="5dabb-129">id</span></span>|<span data-ttu-id="5dabb-130">String</span><span class="sxs-lookup"><span data-stu-id="5dabb-130">String</span></span>|<span data-ttu-id="5dabb-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="5dabb-131">Key of the setting.</span></span> <span data-ttu-id="5dabb-132">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5dabb-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5dabb-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5dabb-133">lastModifiedDateTime</span></span>|<span data-ttu-id="5dabb-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5dabb-134">DateTimeOffset</span></span>|<span data-ttu-id="5dabb-135">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="5dabb-135">Indicates the date the object was last modified.</span></span> <span data-ttu-id="5dabb-136">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5dabb-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5dabb-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5dabb-137">createdDateTime</span></span>|<span data-ttu-id="5dabb-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5dabb-138">DateTimeOffset</span></span>|<span data-ttu-id="5dabb-139">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="5dabb-139">DateTime the object was created.</span></span> <span data-ttu-id="5dabb-140">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5dabb-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5dabb-141">description</span><span class="sxs-lookup"><span data-stu-id="5dabb-141">description</span></span>|<span data-ttu-id="5dabb-142">String</span><span class="sxs-lookup"><span data-stu-id="5dabb-142">String</span></span>|<span data-ttu-id="5dabb-143">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="5dabb-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5dabb-144">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5dabb-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5dabb-145">displayName</span><span class="sxs-lookup"><span data-stu-id="5dabb-145">displayName</span></span>|<span data-ttu-id="5dabb-146">String</span><span class="sxs-lookup"><span data-stu-id="5dabb-146">String</span></span>|<span data-ttu-id="5dabb-147">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="5dabb-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5dabb-148">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5dabb-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5dabb-149">version</span><span class="sxs-lookup"><span data-stu-id="5dabb-149">version</span></span>|<span data-ttu-id="5dabb-150">Int32</span><span class="sxs-lookup"><span data-stu-id="5dabb-150">Int32</span></span>|<span data-ttu-id="5dabb-151">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="5dabb-151">Version of the device configuration.</span></span> <span data-ttu-id="5dabb-152">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5dabb-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5dabb-153">assetTagTemplate</span><span class="sxs-lookup"><span data-stu-id="5dabb-153">assetTagTemplate</span></span>|<span data-ttu-id="5dabb-154">String</span><span class="sxs-lookup"><span data-stu-id="5dabb-154">String</span></span>|<span data-ttu-id="5dabb-155">设备的资产标签信息，显示在登录窗口和锁定屏幕上。</span><span class="sxs-lookup"><span data-stu-id="5dabb-155">Asset tag information for the device, displayed on the login window and lock screen.</span></span>|
|<span data-ttu-id="5dabb-156">lockScreenFootnote</span><span class="sxs-lookup"><span data-stu-id="5dabb-156">lockScreenFootnote</span></span>|<span data-ttu-id="5dabb-157">String</span><span class="sxs-lookup"><span data-stu-id="5dabb-157">String</span></span>|<span data-ttu-id="5dabb-158">显示在登录窗口和锁定屏幕上的脚注。</span><span class="sxs-lookup"><span data-stu-id="5dabb-158">A footnote displayed on the login window and lock screen.</span></span> <span data-ttu-id="5dabb-159">在 iOS 9.3.1 及更高版本中可用。</span><span class="sxs-lookup"><span data-stu-id="5dabb-159">Available in iOS 9.3.1 and later.</span></span>|
|<span data-ttu-id="5dabb-160">homeScreenDockIcons</span><span class="sxs-lookup"><span data-stu-id="5dabb-160">homeScreenDockIcons</span></span>|<span data-ttu-id="5dabb-161">[iosHomeScreenItem](../resources/intune_deviceconfig_ioshomescreenitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5dabb-161">[iosHomeScreenItem](../resources/intune_deviceconfig_ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="5dabb-162">主屏幕 Dock 上显示的应用和文件夹的列表。</span><span class="sxs-lookup"><span data-stu-id="5dabb-162">A list of app and folders to appear on the Home Screen Dock.</span></span> <span data-ttu-id="5dabb-163">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="5dabb-163">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="5dabb-164">homeScreenPages</span><span class="sxs-lookup"><span data-stu-id="5dabb-164">homeScreenPages</span></span>|<span data-ttu-id="5dabb-165">[iosHomeScreenPage](../resources/intune_deviceconfig_ioshomescreenpage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5dabb-165">[iosHomeScreenPage](../resources/intune_deviceconfig_ioshomescreenpage.md) collection</span></span>|<span data-ttu-id="5dabb-166">主屏幕上的页面的列表。</span><span class="sxs-lookup"><span data-stu-id="5dabb-166">A list of pages on the Home Screen.</span></span> <span data-ttu-id="5dabb-167">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="5dabb-167">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="5dabb-168">notificationSettings</span><span class="sxs-lookup"><span data-stu-id="5dabb-168">notificationSettings</span></span>|<span data-ttu-id="5dabb-169">[iosNotificationSettings](../resources/intune_deviceconfig_iosnotificationsettings.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5dabb-169">[iosNotificationSettings](../resources/intune_deviceconfig_iosnotificationsettings.md) collection</span></span>|<span data-ttu-id="5dabb-170">每个捆绑 ID 的通知设置。仅适用于监督模式下的设备（iOS 9.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="5dabb-170">Notification settings for each bundle id. Applicable to devices in supervised mode only (iOS 9.3 and later).</span></span> <span data-ttu-id="5dabb-171">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="5dabb-171">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="5dabb-172">响应</span><span class="sxs-lookup"><span data-stu-id="5dabb-172">Response</span></span>
<span data-ttu-id="5dabb-173">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [iosDeviceFeaturesConfiguration](../resources/intune_deviceconfig_iosdevicefeaturesconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5dabb-173">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_deviceconfig_iosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5dabb-174">示例</span><span class="sxs-lookup"><span data-stu-id="5dabb-174">Example</span></span>
### <a name="request"></a><span data-ttu-id="5dabb-175">请求</span><span class="sxs-lookup"><span data-stu-id="5dabb-175">Request</span></span>
<span data-ttu-id="5dabb-176">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5dabb-176">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1983

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "assetTagTemplate": "Asset Tag Template value",
  "lockScreenFootnote": "Lock Screen Footnote value",
  "homeScreenDockIcons": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenFolder",
      "displayName": "Display Name value",
      "pages": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
          "displayName": "Display Name value",
          "apps": [
            {
              "@odata.type": "microsoft.graph.iosHomeScreenApp",
              "displayName": "Display Name value",
              "bundleID": "Bundle ID value"
            }
          ]
        }
      ]
    }
  ],
  "homeScreenPages": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenPage",
      "displayName": "Display Name value",
      "icons": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenFolder",
          "displayName": "Display Name value",
          "pages": [
            {
              "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
              "displayName": "Display Name value",
              "apps": [
                {
                  "@odata.type": "microsoft.graph.iosHomeScreenApp",
                  "displayName": "Display Name value",
                  "bundleID": "Bundle ID value"
                }
              ]
            }
          ]
        }
      ]
    }
  ],
  "notificationSettings": [
    {
      "@odata.type": "microsoft.graph.iosNotificationSettings",
      "bundleID": "Bundle ID value",
      "appName": "App Name value",
      "publisher": "Publisher value",
      "enabled": true,
      "showInNotificationCenter": true,
      "showOnLockScreen": true,
      "alertType": "banner",
      "badgesEnabled": true,
      "soundsEnabled": true
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="5dabb-177">响应</span><span class="sxs-lookup"><span data-stu-id="5dabb-177">Response</span></span>
<span data-ttu-id="5dabb-p112">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5dabb-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2160

{
  "@odata.type": "#microsoft.graph.iosDeviceFeaturesConfiguration",
  "id": "651e0ab3-0ab3-651e-b30a-1e65b30a1e65",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "assetTagTemplate": "Asset Tag Template value",
  "lockScreenFootnote": "Lock Screen Footnote value",
  "homeScreenDockIcons": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenFolder",
      "displayName": "Display Name value",
      "pages": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
          "displayName": "Display Name value",
          "apps": [
            {
              "@odata.type": "microsoft.graph.iosHomeScreenApp",
              "displayName": "Display Name value",
              "bundleID": "Bundle ID value"
            }
          ]
        }
      ]
    }
  ],
  "homeScreenPages": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenPage",
      "displayName": "Display Name value",
      "icons": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenFolder",
          "displayName": "Display Name value",
          "pages": [
            {
              "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
              "displayName": "Display Name value",
              "apps": [
                {
                  "@odata.type": "microsoft.graph.iosHomeScreenApp",
                  "displayName": "Display Name value",
                  "bundleID": "Bundle ID value"
                }
              ]
            }
          ]
        }
      ]
    }
  ],
  "notificationSettings": [
    {
      "@odata.type": "microsoft.graph.iosNotificationSettings",
      "bundleID": "Bundle ID value",
      "appName": "App Name value",
      "publisher": "Publisher value",
      "enabled": true,
      "showInNotificationCenter": true,
      "showOnLockScreen": true,
      "alertType": "banner",
      "badgesEnabled": true,
      "soundsEnabled": true
    }
  ]
}
```


