# <a name="managedappoperation-resource-type"></a>managedAppOperation 资源类型

> **注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

表示对应用注册应用的操作。
## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 managedAppOperations](../api/intune_mam_managedappoperation_list.md)|[managedAppOperation](../resources/intune_mam_managedappoperation.md) 集合|列出 [managedAppOperation](../resources/intune_mam_managedappoperation.md) 对象的属性和关系。|
|[获取 managedAppOperation](../api/intune_mam_managedappoperation_get.md)|[managedAppOperation](../resources/intune_mam_managedappoperation.md)|读取 [managedAppOperation](../resources/intune_mam_managedappoperation.md) 对象的属性和关系。|
|[创建 managedAppOperation](../api/intune_mam_managedappoperation_create.md)|[managedAppOperation](../resources/intune_mam_managedappoperation.md)|创建新的 [managedAppOperation](../resources/intune_mam_managedappoperation.md) 对象。|
|[删除 managedAppOperation](../api/intune_mam_managedappoperation_delete.md)|无|删除 [managedAppOperation](../resources/intune_mam_managedappoperation.md)。|
|[更新 managedAppOperation](../api/intune_mam_managedappoperation_update.md)|[managedAppOperation](../resources/intune_mam_managedappoperation.md)|更新 [managedAppOperation](../resources/intune_mam_managedappoperation.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|String|操作名称。|
|lastModifiedDateTime|DateTimeOffset|上次修改应用操作的时间。|
|state|String|操作的当前状态|
|id|String|实体的键。|
|version|String|实体版本。|

## <a name="relationships"></a>关系
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppOperation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppOperation",
  "displayName": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "state": "String",
  "id": "String (identifier)",
  "version": "String"
}
```



