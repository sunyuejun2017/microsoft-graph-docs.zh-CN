# <a name="remoteassistancepartner-resource-type"></a>remoteAssistancePartner 资源类型

> **注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

remoteAssistPartner 资源表示给定远程协助合作伙伴服务的元数据和状态。
## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 remoteAssistancePartners](../api/intune_remoteassistance_remoteassistancepartner_list.md)|[remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md) 集合|列出 [remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md) 对象的属性和关系。|
|[获取 remoteAssistancePartner](../api/intune_remoteassistance_remoteassistancepartner_get.md)|[remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md)|读取 [remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md) 对象的属性和关系。|
|[创建 remoteAssistancePartner](../api/intune_remoteassistance_remoteassistancepartner_create.md)|[remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md)|创建新的 [remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md) 对象。|
|[删除 remoteAssistancePartner](../api/intune_remoteassistance_remoteassistancepartner_delete.md)|无|删除 [remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md)。|
|[更新 remoteAssistancePartner](../api/intune_remoteassistance_remoteassistancepartner_update.md)|[remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md)|更新 [remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md) 对象的属性。|
|[beginOnboarding 操作](../api/intune_remoteassistance_remoteassistancepartner_beginonboarding.md)|无|尚未记录|
|[断开连接操作](../api/intune_remoteassistance_remoteassistancepartner_disconnect.md)|无|尚未记录|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|合作伙伴的唯一标识符。|
|displayName|String|合作伙伴的显示名称。|
|onboardingUrl|String|合作伙伴的载入门户的 URL，其中管理员可以配置其远程协助服务。|
|onboardingStatus|String|TBD 可取值为：`notOnboarded`、`onboarding`、`onboarded`。|
|lastConnectionDateTime|DateTimeOffset|由 TEM 合作伙伴发送到 Intune 的上一个请求的时间戳。|

## <a name="relationships"></a>关系
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.remoteAssistancePartner"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.remoteAssistancePartner",
  "id": "String (identifier)",
  "displayName": "String",
  "onboardingUrl": "String",
  "onboardingStatus": "String",
  "lastConnectionDateTime": "String (timestamp)"
}
```



