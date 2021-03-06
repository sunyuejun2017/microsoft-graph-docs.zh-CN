# <a name="devicecomplianceuserstatus-resource-type"></a>deviceComplianceUserStatus 资源类型

> **注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

尚未记录
## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 deviceComplianceUserStatuses](../api/intune_deviceconfig_devicecomplianceuserstatus_list.md)|[deviceComplianceUserStatus](../resources/intune_deviceconfig_devicecomplianceuserstatus.md) 集合|列出 [deviceComplianceUserStatus](../resources/intune_deviceconfig_devicecomplianceuserstatus.md) 对象的属性和关系。|
|[获取 deviceComplianceUserStatus](../api/intune_deviceconfig_devicecomplianceuserstatus_get.md)|[deviceComplianceUserStatus](../resources/intune_deviceconfig_devicecomplianceuserstatus.md)|读取 [deviceComplianceUserStatus](../resources/intune_deviceconfig_devicecomplianceuserstatus.md) 对象的属性和关系。|
|[创建 deviceComplianceUserStatus](../api/intune_deviceconfig_devicecomplianceuserstatus_create.md)|[deviceComplianceUserStatus](../resources/intune_deviceconfig_devicecomplianceuserstatus.md)|创建新的 [deviceComplianceUserStatus](../resources/intune_deviceconfig_devicecomplianceuserstatus.md) 对象。|
|[删除 deviceComplianceUserStatus](../api/intune_deviceconfig_devicecomplianceuserstatus_delete.md)|无|删除 [deviceComplianceUserStatus](../resources/intune_deviceconfig_devicecomplianceuserstatus.md)。|
|[更新 deviceComplianceUserStatus](../api/intune_deviceconfig_devicecomplianceuserstatus_update.md)|[deviceComplianceUserStatus](../resources/intune_deviceconfig_devicecomplianceuserstatus.md)|更新 [deviceComplianceUserStatus](../resources/intune_deviceconfig_devicecomplianceuserstatus.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。|
|userDisplayName|String|DevicePolicyStatus 的用户名。|
|devicesCount|Int32|该用户的设备计数。|
|状态|String|策略报告的合规性状态。 可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`。|
|lastReportedDateTime|DateTimeOffset|策略报告的上次修改日期时间。|
|userPrincipalName|String|UserPrincipalName。|

## <a name="relationships"></a>关系
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComplianceUserStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceUserStatus",
  "id": "String (identifier)",
  "userDisplayName": "String",
  "devicesCount": 1024,
  "status": "String",
  "lastReportedDateTime": "String (timestamp)",
  "userPrincipalName": "String"
}
```



