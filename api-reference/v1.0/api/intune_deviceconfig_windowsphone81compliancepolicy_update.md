# <a name="update-windowsphone81compliancepolicy"></a>更新 windowsPhone81CompliancePolicy

> **注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

更新 [windowsPhone81CompliancePolicy](../resources/intune_deviceconfig_windowsphone81compliancepolicy.md) 对象的属性。
## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。

|权限类型|权限（从最高特权到最低特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementConfiguration.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|不支持。|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|Accept|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [windowsPhone81CompliancePolicy](../resources/intune_deviceconfig_windowsphone81compliancepolicy.md) 对象的 JSON 表示形式。

下表显示创建 [windowsPhone81CompliancePolicy](../resources/intune_deviceconfig_windowsphone81compliancepolicy.md) 时所需的属性。

|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。 继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|
|createdDateTime|DateTimeOffset|创建对象的日期/时间。 继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|
|description|String|管理员提供的设备配置的说明。 继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改对象的日期/时间。 继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|
|displayName|String|管理员提供的设备配置的名称。 继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|
|version|Int32|设备配置的版本。 继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|
|passwordBlockSimple|Boolean|是否阻止同步日历。|
|passwordExpirationDays|Int32|密码过期前的天数。|
|passwordMinimumLength|Int32|密码的最小长度。|
|passwordMinutesOfInactivityBeforeLock|Int32|在需要密码之前不活动的分钟数。|
|passwordMinimumCharacterSetCount|Int32|密码中必需的字符集数。|
|passwordRequiredType|String|必需的密码类型。 可取值为：`deviceDefault`、`alphanumeric`、`numeric`。|
|passwordPreviousPasswordBlockCount|Int32|要阻止的以前密码的数量。 有效值为 0 至 24|
|passwordRequired|Boolean|是否需要密码。|
|osMinimumVersion|String|最低 Windows Phone 版本。|
|osMaximumVersion|String|最高 Windows Phone 版本。|
|storageRequireEncryption|Boolean|要求对 Windows Phone 设备加密。|



## <a name="response"></a>响应
如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [windowsPhone81CompliancePolicy](../resources/intune_deviceconfig_windowsphone81compliancepolicy.md) 对象。

## <a name="example"></a>示例
### <a name="request"></a>请求
下面是一个请求示例。
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 602

{
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequired": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "storageRequireEncryption": true
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 779

{
  "@odata.type": "#microsoft.graph.windowsPhone81CompliancePolicy",
  "id": "e6021ad4-1ad4-e602-d41a-02e6d41a02e6",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequired": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "storageRequireEncryption": true
}
```



