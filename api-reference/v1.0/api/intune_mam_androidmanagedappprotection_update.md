# <a name="update-androidmanagedappprotection"></a>更新 androidManagedAppProtection

> **注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

更新 [androidManagedAppProtection](../resources/intune_mam_androidmanagedappprotection.md) 对象的属性。
## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。

|权限类型|权限（从最高特权到最低特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementApps.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|不支持。|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|Accept|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [androidManagedAppProtection](../resources/intune_mam_androidmanagedappprotection.md) 对象的 JSON 表示形式。

下表显示了创建 [androidManagedAppProtection](../resources/intune_mam_androidmanagedappprotection.md) 时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|displayName|String|策略显示名称。 继承自 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)|
|description|String|策略的说明。 继承自 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)|
|createdDateTime|DateTimeOffset|创建策略的日期和时间。 继承自 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改策略的时间。 继承自 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)|
|id|String|实体的键。 继承自 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)|
|version|String|实体的版本。 继承自 [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)|
|periodOfflineBeforeAccessCheck|Duration|设备未连接到 Internet 时在该时间段后检查访问权限。 继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)|
|periodOnlineBeforeAccessCheck|Duration|设备连接到 Internet 时在该时间段后检查访问权限。 继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)|
|allowedInboundDataTransferSources|String|允许传输其中的数据的源。 继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)。可取值为：`allApps`、`managedApps`、`none`。|
|allowedOutboundDataTransferDestinations|String|允许向其传输数据的目标。 继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)。可取值为：`allApps`、`managedApps`、`none`。|
|organizationalCredentialsRequired|Boolean|指示是否需要组织凭据才能使用应用。 继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)|
|allowedOutboundClipboardSharingLevel|String|可以在托管设备上的应用之间共享剪贴板的级别。 继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)。可取值为：`allApps`、`managedAppsWithPasteIn`、`managedApps`、`blocked`。|
|dataBackupBlocked|Boolean|指示是否阻止备份托管应用的数据。 继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)|
|deviceComplianceRequired|Boolean|指示是否需要设备符合性。 继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)|
|managedBrowserToOpenLinksRequired|Boolean|指示是否应在托管浏览器应用中打开 Internet 链接。 继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)|
|saveAsBlocked|Boolean|指示用户是否可以使用“另存为”菜单项保存受保护文件的副本。 继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)|
|periodOfflineBeforeWipeIsEnforced|Duration|在擦除所有托管数据之前，允许应用保持从 Internet 断开连接的时间量。 继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)|
|pinRequired|Boolean|指示是否需要应用级 PIN。 继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)|
|maximumPinRetries|Int32|在擦除托管应用之前，不正确 PIN 重新尝试的最大尝试次数。 继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)|
|simplePinBlocked|Boolean|指示是否阻止 simplePin。 继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)|
|minimumPinLength|Int32|PinRequired 设置为 True 时应用级 PIN 所需的最小 PIN 长度。继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)|
|pinCharacterSet|String|PinRequired 设置为 True 时可用于应用级 PIN 的字符集。 继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)。可取值为：`numeric`、`alphanumericAndSymbol`。|
|periodBeforePinReset|Duration|PinRequired 设置为 True 时，在此时间段之后必须重置所有级别的 PIN。
 继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)|
|allowedDataStorageLocations|String 集合|用户可能存储托管数据的数据存储位置。 继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)。可取值为：`oneDriveForBusiness`、`sharePoint`、`localStorage`。|
|contactSyncBlocked|Boolean|指示联系人是否可以同步到用户的设备。 继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)|
|printBlocked|Boolean|指示是否允许从托管应用进行打印。 继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)|
|fingerprintBlocked|Boolean|指示如果 PinRequired 设置为 True，是否允许使用指纹读取器代替 PIN。 继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)|
|disableAppPinIfDevicePinIsSet|Boolean|指示如果设置了设备 PIN，是否需要使用应用 PIN。 继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)|
|minimumRequiredOsVersion|String|低于指定版本的版本将阻止托管应用访问公司数据。 继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)|
|minimumWarningOsVersion|String|低于指定版本的版本将导致托管应用访问公司数据时出现警告消息。 继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)|
|minimumRequiredAppVersion|String|低于指定版本的版本将阻止托管应用访问公司数据。 继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)|
|minimumWarningAppVersion|String|低于指定版本的版本将导致托管应用出现警告消息。 继承自 [managedAppProtection](../resources/intune_mam_managedappprotection.md)|
|isAssigned|Boolean|指示策略是否部署到任何包含组。 继承自 [targetedManagedAppProtection](../resources/intune_mam_targetedmanagedappprotection.md)|
|screenCaptureBlocked|Boolean|指示托管用户是否可以对托管应用进行屏幕截图|
|disableAppEncryptionIfDeviceEncryptionIsEnabled|Boolean|启用此设置后，如果启用设备级加密，则应用级加密将被禁用|
|encryptAppData|Boolean|指示是否应加密托管应用的应用程序数据|
|deployedAppCount|Int32|当前策略部署到的应用的数量。|
|minimumRequiredPatchVersion|String|定义用户可以拥有的最早的必需 Android 安全修补程序级别，用户可借此获得对应用的安全访问权限。
|
|minimumWarningPatchVersion|String|定义用户可以获得对应用的安全访问权限所需的最早推荐 Android 安全修补程序级别。|



## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [androidManagedAppProtection](../resources/intune_mam_androidmanagedappprotection.md) 对象。

## <a name="example"></a>示例
### <a name="request"></a>请求
下面是一个请求示例。
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

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
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



