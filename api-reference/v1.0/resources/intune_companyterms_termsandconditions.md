# <a name="termsandconditions-resource-type"></a>termsAndConditions 资源类型

> **注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

TermsAndConditions 实体表示给定条款和条件 (T&C) 策略的元数据和内容。 当用户第一次尝试注册到 Intune 时向用户显示 T&C 策略的内容，之后会在进行了管理员要求重新接受的编辑时显示。 这允许管理员与用户必须同意的预配进行通信，以便将设备注册到 Intune 中。
## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[List termsAndConditionses](../api/intune_companyterms_termsandconditions_list.md)|[termsAndConditions](../resources/intune_companyterms_termsandconditions.md) 集合|列出 [termsAndConditions](../resources/intune_companyterms_termsandconditions.md) 对象的属性和关系。|
|[Get termsAndConditions](../api/intune_companyterms_termsandconditions_get.md)|[termsAndConditions](../resources/intune_companyterms_termsandconditions.md)|读取 [termsAndConditions](../resources/intune_companyterms_termsandconditions.md) 对象的属性和关系。|
|[Create termsAndConditions](../api/intune_companyterms_termsandconditions_create.md)|[termsAndConditions](../resources/intune_companyterms_termsandconditions.md)|创建新的 [termsAndConditions](../resources/intune_companyterms_termsandconditions.md) 对象。|
|[Delete termsAndConditions](../api/intune_companyterms_termsandconditions_delete.md)|无|删除 [termsAndConditions](../resources/intune_companyterms_termsandconditions.md)。|
|[Update termsAndConditions](../api/intune_companyterms_termsandconditions_update.md)|[termsAndConditions](../resources/intune_companyterms_termsandconditions.md)|更新 [termsAndConditions](../resources/intune_companyterms_termsandconditions.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|T&C 策略的唯一标识符。|
|createdDateTime|DateTimeOffset|创建对象的日期/时间。|
|lastModifiedDateTime|DateTimeOffset|上次修改对象的日期/时间。|
|displayName|String|管理员提供的 T&C 策略名称。 |
|说明|String|管理员提供的 T&C 策略描述。|
|标题|String|管理员提供的条款和条件标题。 这会向用户显示，提示用户接受 T&C 策略。|
|bodyText|String|管理员提供的条款和条件正文文本，通常为条款本身。 这会向用户显示，提示用户接受 T&C 策略。|
|acceptanceStatement|String|管理员提供的条款和条件说明，通常会说明接受 T&C 策略中陈述的条款和条件意味着什么。 这会向用户显示，提示用户接受 T&C 策略。|
|版本|Int32|指示当前条款版本的整数。 当管理员对条款进行更改，并希望要求用户重新接受修改的 T&C 策略时会递增。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|assignments|[termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md) 集合|此 T&C 策略的分配列表。|
|acceptanceStatuses|[termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) 集合|此 T&C 策略的接受状态列表。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termsAndConditions"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termsAndConditions",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "description": "String",
  "title": "String",
  "bodyText": "String",
  "acceptanceStatement": "String",
  "version": 1024
}
```



