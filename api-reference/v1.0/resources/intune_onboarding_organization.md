# <a name="organization-resource-type"></a>组织资源类型

> **注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

组织资源表示在租户级别操作和配置的全局设置和资源的实例。
## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 organizations](../api/intune_onboarding_organization_list.md)|[organization](../resources/intune_onboarding_organization.md) 集合|列出 [organization](../resources/intune_onboarding_organization.md) 对象的属性和关系。|
|[获取 organization](../api/intune_onboarding_organization_get.md)|[organization](../resources/intune_onboarding_organization.md)|读取 [organization](../resources/intune_onboarding_organization.md) 对象的属性和关系。|
|[更新 organization](../api/intune_onboarding_organization_update.md)|[organization](../resources/intune_onboarding_organization.md)|更新 [organization](../resources/intune_onboarding_organization.md) 对象的属性。|
|[setMobileDeviceManagementAuthority 操作](../api/intune_onboarding_organization_setmobiledevicemanagementauthority.md)|Int32|设置移动设备管理机构|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|对象的 GUID。|
|mobileDeviceManagementAuthority|String|移动设备管理机构。 可取值为：`unknown`、`intune`、`sccm`、`office365`。|

## <a name="relationships"></a>Relationships
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.organization"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.organization",
  "id": "String (identifier)",
  "mobileDeviceManagementAuthority": "String"
}
```



