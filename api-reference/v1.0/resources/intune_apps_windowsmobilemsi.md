# <a name="windowsmobilemsi-resource-type"></a>windowsMobileMSI 资源类型

> **注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

包含 Windows Mobile MSI 业务线应用的属性和继承的属性。

继承自 [mobileLobApp](../resources/intune_apps_mobilelobapp.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[List windowsMobileMSIs](../api/intune_apps_windowsmobilemsi_list.md)|[windowsMobileMSI](../resources/intune_apps_windowsmobilemsi.md) 集合|列出 [windowsMobileMSI](../resources/intune_apps_windowsmobilemsi.md) 对象的属性和关系。|
|[Get windowsMobileMSI](../api/intune_apps_windowsmobilemsi_get.md)|[windowsMobileMSI](../resources/intune_apps_windowsmobilemsi.md)|读取 [windowsMobileMSI](../resources/intune_apps_windowsmobilemsi.md) 对象的属性和关系。|
|[Create windowsMobileMSI](../api/intune_apps_windowsmobilemsi_create.md)|[windowsMobileMSI](../resources/intune_apps_windowsmobilemsi.md)|创建新的 [windowsMobileMSI](../resources/intune_apps_windowsmobilemsi.md) 对象。|
|[Delete windowsMobileMSI](../api/intune_apps_windowsmobilemsi_delete.md)|无|删除 [windowsMobileMSI](../resources/intune_apps_windowsmobilemsi.md)。|
|[Update windowsMobileMSI](../api/intune_apps_windowsmobilemsi_update.md)|[windowsMobileMSI](../resources/intune_apps_windowsmobilemsi.md)|更新 [windowsMobileMSI](../resources/intune_apps_windowsmobilemsi.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|displayName|String|管理员提供或导入的应用标题。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|description|String|应用的说明。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|publisher|String|应用的发布者。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|largeIcon|[mimeContent](../resources/intune_apps_mimecontent.md)|要显示在应用详细信息中或用于图标上传的大图标。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|createdDateTime|DateTimeOffset|创建应用的日期和时间。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改应用的日期和时间。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|isFeatured|Boolean|指示应用是否被管理员标记为特色的值 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|privacyInformationUrl|String|隐私声明 Url。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|informationUrl|String|详细信息 Url。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|owner|String|应用的所有者。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|developer|String|应用的开发者。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|notes|String|应用的备注。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|publishingState|String|应用的发布状态。 除非应用已发布，否则无法分配应用。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md) 可取值为：`notPublished`、`processing`、`published`。|
|committedContentVersion|String|内部提交的内容版本。 继承自 [mobileLobApp](../resources/intune_apps_mobilelobapp.md)|
|fileName|String|主 Lob 应用程序文件的名称。 继承自 [mobileLobApp](../resources/intune_apps_mobilelobapp.md)|
|size|Int64|总大小，包括所有已上传文件。 继承自 [mobileLobApp](../resources/intune_apps_mobilelobapp.md)|
|commandLine|String|命令行。|
|productCode|String|产品代码。|
|productVersion|String|Windows Mobile MSI 业务线 (LoB) 应用的产品版本。|
|ignoreVersionDetection|Boolean|控制应用的版本是否将用于检测安装在设备上的应用的布尔值。 对于使用自更新功能的 Windows Mobile MSI 业务线 (LoB) 应用，将此值设置为 true。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|categories|[mobileAppCategory](../resources/intune_apps_mobileappcategory.md) 集合|此应用的类别列表。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|assignments|[mobileAppAssignment](../resources/intune_apps_mobileappassignment.md) 集合|此移动应用的组分配的列表。 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)|
|contentVersions|[mobileAppContent](../resources/intune_apps_mobileappcontent.md) 集合|此应用的内容版本列表。 继承自 [mobileLobApp](../resources/intune_apps_mobilelobapp.md)|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsMobileMSI"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsMobileMSI",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "publisher": "String",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "isFeatured": true,
  "privacyInformationUrl": "String",
  "informationUrl": "String",
  "owner": "String",
  "developer": "String",
  "notes": "String",
  "publishingState": "String",
  "committedContentVersion": "String",
  "fileName": "String",
  "size": 1024,
  "commandLine": "String",
  "productCode": "String",
  "productVersion": "String",
  "ignoreVersionDetection": true
}
```



