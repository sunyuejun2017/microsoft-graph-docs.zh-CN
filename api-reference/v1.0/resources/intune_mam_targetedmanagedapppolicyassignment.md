# <a name="targetedmanagedapppolicyassignment-resource-type"></a>targetedManagedAppPolicyAssignment 资源类型

> **注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

组或应用的部署类型。
## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 targetedManagedAppPolicyAssignments](../api/intune_mam_targetedmanagedapppolicyassignment_list.md)|[targetedManagedAppPolicyAssignment](../resources/intune_mam_targetedmanagedapppolicyassignment.md) 集合|列出 [targetedManagedAppPolicyAssignment](../resources/intune_mam_targetedmanagedapppolicyassignment.md) 对象的属性和关系。|
|[获取 targetedManagedAppPolicyAssignment](../api/intune_mam_targetedmanagedapppolicyassignment_get.md)|[targetedManagedAppPolicyAssignment](../resources/intune_mam_targetedmanagedapppolicyassignment.md)|读取 [targetedManagedAppPolicyAssignment](../resources/intune_mam_targetedmanagedapppolicyassignment.md) 对象的属性和关系。|
|[创建 targetedManagedAppPolicyAssignment](../api/intune_mam_targetedmanagedapppolicyassignment_create.md)|[targetedManagedAppPolicyAssignment](../resources/intune_mam_targetedmanagedapppolicyassignment.md)|创建新的 [targetedManagedAppPolicyAssignment](../resources/intune_mam_targetedmanagedapppolicyassignment.md) 对象。|
|[删除 targetedManagedAppPolicyAssignment](../api/intune_mam_targetedmanagedapppolicyassignment_delete.md)|无|删除 [targetedManagedAppPolicyAssignment](../resources/intune_mam_targetedmanagedapppolicyassignment.md)。|
|[更新 targetedManagedAppPolicyAssignment](../api/intune_mam_targetedmanagedapppolicyassignment_update.md)|[targetedManagedAppPolicyAssignment](../resources/intune_mam_targetedmanagedapppolicyassignment.md)|更新 [targetedManagedAppPolicyAssignment](../resources/intune_mam_targetedmanagedapppolicyassignment.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|Id|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune_mam_deviceandappmanagementassignmenttarget.md)|组或应用的部署标识符|

## <a name="relationships"></a>关系
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.targetedManagedAppPolicyAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.targetedManagedAppPolicyAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



