# <a name="windows10compliancepolicy-resource-type"></a>windows10CompliancePolicy 资源类型

> **注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

此类包含 Windows 10 的合规性设置。

继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[List windows10CompliancePolicies](../api/intune_deviceconfig_windows10compliancepolicy_list.md)|[windows10CompliancePolicy](../resources/intune_deviceconfig_windows10compliancepolicy.md) 集合|列出 [windows10CompliancePolicy](../resources/intune_deviceconfig_windows10compliancepolicy.md) 对象的属性和关系。|
|[Get windows10CompliancePolicy](../api/intune_deviceconfig_windows10compliancepolicy_get.md)|[windows10CompliancePolicy](../resources/intune_deviceconfig_windows10compliancepolicy.md)|读取 [windows10CompliancePolicy](../resources/intune_deviceconfig_windows10compliancepolicy.md) 对象的属性和关系。|
|[Create windows10CompliancePolicy](../api/intune_deviceconfig_windows10compliancepolicy_create.md)|[windows10CompliancePolicy](../resources/intune_deviceconfig_windows10compliancepolicy.md)|创建新的 [windows10CompliancePolicy](../resources/intune_deviceconfig_windows10compliancepolicy.md) 对象。|
|[Delete windows10CompliancePolicy](../api/intune_deviceconfig_windows10compliancepolicy_delete.md)|无|删除 [windows10CompliancePolicy](../resources/intune_deviceconfig_windows10compliancepolicy.md)。|
|[Update windows10CompliancePolicy](../api/intune_deviceconfig_windows10compliancepolicy_update.md)|[windows10CompliancePolicy](../resources/intune_deviceconfig_windows10compliancepolicy.md)|更新 [windows10CompliancePolicy](../resources/intune_deviceconfig_windows10compliancepolicy.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。 继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|
|createdDateTime|DateTimeOffset|创建对象的日期/时间。 继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|
|description|String|管理员提供的设备配置的说明。 继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改对象的日期/时间。 继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|
|displayName|String|管理员提供的设备配置的名称。 继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|
|version|Int32|设备配置的版本。 继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|
|passwordRequired|Boolean|需要密码才可解锁 Windows 设备。|
|passwordBlockSimple|Boolean|指示是否阻止简单密码。|
|passwordRequiredToUnlockFromIdle|Boolean|需要密码才可解锁闲置设备。|
|passwordMinutesOfInactivityBeforeLock|Int32|在需要密码之前不活动的分钟数。|
|passwordExpirationDays|Int32|密码过期天数。|
|passwordMinimumLength|Int32|密码最短长度。|
|passwordMinimumCharacterSetCount|Int32|密码中必需的字符集数。|
|passwordRequiredType|String|必需的密码类型。 可取值为：`deviceDefault`、`alphanumeric`、`numeric`。|
|passwordPreviousPasswordBlockCount|Int32|防止重复使用的先前密码的数量。|
|requireHealthyDeviceReport|Boolean|要求设备由 Windows 设备运行状况证明报告为正常。|
|osMinimumVersion|String|最低 Windows 10 版本。|
|osMaximumVersion|String|最高 Windows 10 版本。|
|mobileOsMinimumVersion|String|最低 Windows Phone 版本。|
|mobileOsMaximumVersion|String|最高 Windows Phone 版本。|
|earlyLaunchAntiMalwareDriverEnabled|Boolean|要求设备由 Windows 设备运行状况证明报告为正常 - 提前启动反恶意驱动程序已启用。|
|bitLockerEnabled|Boolean|要求设备由 Windows 设备运行状况证明报告为正常 - bit locker 已启用。|
|secureBootEnabled|Boolean|要求设备由 Windows 设备运行状况证明报告为正常 - 安全启动已启用。|
|codeIntegrityEnabled|Boolean|要求设备由 Windows 设备运行状况证明报告为正常。|
|storageRequireEncryption|Boolean|要求对 Windows 设备加密。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|scheduledActionsForRule|[deviceComplianceScheduledActionForRule](../resources/intune_deviceconfig_devicecompliancescheduledactionforrule.md) 集合|此规则的计划操作的列表 继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|
|deviceStatuses|[deviceComplianceDeviceStatus](../resources/intune_deviceconfig_devicecompliancedevicestatus.md) 集合|DeviceComplianceDeviceStatus 的列表。 继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|
|userStatuses|[deviceComplianceUserStatus](../resources/intune_deviceconfig_devicecomplianceuserstatus.md) 集合|DeviceComplianceUserStatus 的列表。 继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|
|deviceStatusOverview|[deviceComplianceDeviceOverview](../resources/intune_deviceconfig_devicecompliancedeviceoverview.md)|设备合规性设备状态概述 继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|
|userStatusOverview|[deviceComplianceUserOverview](../resources/intune_deviceconfig_devicecomplianceuseroverview.md)|设备合规性用户状态概述 继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md) 集合|合规性设置状态设备摘要 继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|
|assignments|[deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md) 集合|此合规性策略的分配集合。 继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windows10CompliancePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10CompliancePolicy",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "version": 1024,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordRequiredToUnlockFromIdle": true,
  "passwordMinutesOfInactivityBeforeLock": 1024,
  "passwordExpirationDays": 1024,
  "passwordMinimumLength": 1024,
  "passwordMinimumCharacterSetCount": 1024,
  "passwordRequiredType": "String",
  "passwordPreviousPasswordBlockCount": 1024,
  "requireHealthyDeviceReport": true,
  "osMinimumVersion": "String",
  "osMaximumVersion": "String",
  "mobileOsMinimumVersion": "String",
  "mobileOsMaximumVersion": "String",
  "earlyLaunchAntiMalwareDriverEnabled": true,
  "bitLockerEnabled": true,
  "secureBootEnabled": true,
  "codeIntegrityEnabled": true,
  "storageRequireEncryption": true
}
```



