# <a name="onpremisesconditionalaccesssettings-resource-type"></a>onPremisesConditionalAccessSettings 资源类型

> **注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

表示租户的 Exchange 本地条件访问设置的单例实体。
## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 onPremisesConditionalAccessSettings](../api/intune_onboarding_onpremisesconditionalaccesssettings_get.md)|[onPremisesConditionalAccessSettings](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md)|读取 [onPremisesConditionalAccessSettings](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md) 对象的属性和关系。|
|[更新 onPremisesConditionalAccessSettings](../api/intune_onboarding_onpremisesconditionalaccesssettings_update.md)|[onPremisesConditionalAccessSettings](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md)|更新 [onPremisesConditionalAccessSettings](../resources/intune_onboarding_onpremisesconditionalaccesssettings.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|尚未记录|
|已启用|Boolean|指示是否为该组织启用了本地条件访问|
|includedGroups|Guid 集合|本地条件访问将面向的用户组。 这些组中的所有用户都需要托管移动设备并符合邮件访问的要求。|
|excludedGroups|Guid 集合|将由本地条件访问豁免的用户组。 这些组中的所有用户都将从条件访问策略中豁免。|
|overrideDefaultRule|Boolean|允许设备时重写默认访问规则以确保授予访问。|

## <a name="relationships"></a>关系
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.onPremisesConditionalAccessSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.onPremisesConditionalAccessSettings",
  "id": "String (identifier)",
  "enabled": true,
  "includedGroups": [
    "<Unknown Primitive Type Edm.Guid>"
  ],
  "excludedGroups": [
    "<Unknown Primitive Type Edm.Guid>"
  ],
  "overrideDefaultRule": true
}
```



