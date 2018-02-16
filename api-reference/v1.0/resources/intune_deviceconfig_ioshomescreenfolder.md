# <a name="ioshomescreenfolder-resource-type"></a><span data-ttu-id="c4d64-101">iosHomeScreenFolder 资源类型</span><span class="sxs-lookup"><span data-stu-id="c4d64-101">iosHomeScreenFolder resource type</span></span>

> <span data-ttu-id="c4d64-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="c4d64-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c4d64-103">包含主屏幕上的应用页面的文件夹</span><span class="sxs-lookup"><span data-stu-id="c4d64-103">A folder containing pages of apps on the Home Screen</span></span>

<span data-ttu-id="c4d64-104">继承自 [iosHomeScreenItem](../resources/intune_deviceconfig_ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="c4d64-104">Inherits from [iosHomeScreenItem](../resources/intune_deviceconfig_ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c4d64-105">属性</span><span class="sxs-lookup"><span data-stu-id="c4d64-105">Properties</span></span>
|<span data-ttu-id="c4d64-106">属性</span><span class="sxs-lookup"><span data-stu-id="c4d64-106">Property</span></span>|<span data-ttu-id="c4d64-107">类型</span><span class="sxs-lookup"><span data-stu-id="c4d64-107">Type</span></span>|<span data-ttu-id="c4d64-108">说明</span><span class="sxs-lookup"><span data-stu-id="c4d64-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c4d64-109">displayName</span><span class="sxs-lookup"><span data-stu-id="c4d64-109">displayName</span></span>|<span data-ttu-id="c4d64-110">String</span><span class="sxs-lookup"><span data-stu-id="c4d64-110">String</span></span>|<span data-ttu-id="c4d64-111">继承自 [iosHomeScreenItem](../resources/intune_deviceconfig_ioshomescreenitem.md) 的应用的名称</span><span class="sxs-lookup"><span data-stu-id="c4d64-111">Name of the app Inherited from [iosHomeScreenItem](../resources/intune_deviceconfig_ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="c4d64-112">页面</span><span class="sxs-lookup"><span data-stu-id="c4d64-112">pages</span></span>|<span data-ttu-id="c4d64-113">[iosHomeScreenFolderPage](../resources/intune_deviceconfig_ioshomescreenfolderpage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c4d64-113">[iosHomeScreenFolderPage](../resources/intune_deviceconfig_ioshomescreenfolderpage.md) collection</span></span>|<span data-ttu-id="c4d64-114">主屏幕布局图标页面，必须为应用程序类型。</span><span class="sxs-lookup"><span data-stu-id="c4d64-114">Pages of Home Screen Layout Icons which must be Application Type.</span></span> <span data-ttu-id="c4d64-115">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="c4d64-115">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c4d64-116">关系</span><span class="sxs-lookup"><span data-stu-id="c4d64-116">Relationships</span></span>
<span data-ttu-id="c4d64-117">无</span><span class="sxs-lookup"><span data-stu-id="c4d64-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c4d64-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c4d64-118">JSON Representation</span></span>
<span data-ttu-id="c4d64-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c4d64-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosHomeScreenFolder"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenFolder",
  "displayName": "String",
  "pages": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
      "displayName": "String",
      "apps": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenApp",
          "displayName": "String",
          "bundleID": "String"
        }
      ]
    }
  ]
}
```


