# <a name="configurationmanagerclientenabledfeatures-resource-type"></a>configurationManagerClientEnabledFeatures 资源类型

> **注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

Configuration Manager 客户端已启用的功能
## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|inventory|Boolean|目录是否由 Intune 管理|
|modernApps|Boolean|现代应用程序是否由 Intune 管理|
|resourceAccess|Boolean|资源访问权限是否由 Intune 管理|
|deviceConfiguration|Boolean|设备配置是否由 Intune 管理|
|compliancePolicy|Boolean|符合性策略是否由 Intune 管理|
|windowsUpdateForBusiness|Boolean|适用于企业的 Windows 更新是否由 Intune 管理|

## <a name="relationships"></a>关系
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.configurationManagerClientEnabledFeatures"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.configurationManagerClientEnabledFeatures",
  "inventory": true,
  "modernApps": true,
  "resourceAccess": true,
  "deviceConfiguration": true,
  "compliancePolicy": true,
  "windowsUpdateForBusiness": true
}
```



