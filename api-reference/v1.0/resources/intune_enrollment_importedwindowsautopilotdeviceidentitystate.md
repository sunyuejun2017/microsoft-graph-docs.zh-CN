# <a name="importedwindowsautopilotdeviceidentitystate-resource-type"></a>importedWindowsAutopilotDeviceIdentityState 资源类型

> **注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

尚未记录
## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|deviceImportStatus|字符串|设备目录服务 (DDS) 报告的设备状态。 可取值为：`unknown`、`pending`、`partial`、`complete`、`error`。|
|deviceRegistrationId|字符串|设备目录服务 (DDS) 报告的成功添加设备的设备注册 ID。|
|deviceErrorCode|Int32|设备目录服务 (DDS) 报告的设备错误代码。|
|deviceErrorName|字符串|设备目录服务 (DDS) 报告的设备错误名称。|

## <a name="relationships"></a>关系
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.importedWindowsAutopilotDeviceIdentityState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentityState",
  "deviceImportStatus": "String",
  "deviceRegistrationId": "String",
  "deviceErrorCode": 1024,
  "deviceErrorName": "String"
}
```



