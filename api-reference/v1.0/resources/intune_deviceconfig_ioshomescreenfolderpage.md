# <a name="ioshomescreenfolderpage-resource-type"></a><span data-ttu-id="59c8f-101">iosHomeScreenFolderPage 资源类型</span><span class="sxs-lookup"><span data-stu-id="59c8f-101">iosHomeScreenFolderPage resource type</span></span>

> <span data-ttu-id="59c8f-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="59c8f-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="59c8f-103">包含主屏幕上的应用的文件夹</span><span class="sxs-lookup"><span data-stu-id="59c8f-103">A folder containing apps on the Home Screen</span></span>
## <a name="properties"></a><span data-ttu-id="59c8f-104">属性</span><span class="sxs-lookup"><span data-stu-id="59c8f-104">Properties</span></span>
|<span data-ttu-id="59c8f-105">属性</span><span class="sxs-lookup"><span data-stu-id="59c8f-105">Property</span></span>|<span data-ttu-id="59c8f-106">类型</span><span class="sxs-lookup"><span data-stu-id="59c8f-106">Type</span></span>|<span data-ttu-id="59c8f-107">说明</span><span class="sxs-lookup"><span data-stu-id="59c8f-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="59c8f-108">displayName</span><span class="sxs-lookup"><span data-stu-id="59c8f-108">displayName</span></span>|<span data-ttu-id="59c8f-109">String</span><span class="sxs-lookup"><span data-stu-id="59c8f-109">String</span></span>|<span data-ttu-id="59c8f-110">文件夹页的名称</span><span class="sxs-lookup"><span data-stu-id="59c8f-110">Name of the page</span></span>|
|<span data-ttu-id="59c8f-111">应用</span><span class="sxs-lookup"><span data-stu-id="59c8f-111">apps</span></span>|<span data-ttu-id="59c8f-112">[iosHomeScreenApp](../resources/intune_deviceconfig_ioshomescreenapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="59c8f-112">[iosHomeScreenApp](../resources/intune_deviceconfig_ioshomescreenapp.md) collection</span></span>|<span data-ttu-id="59c8f-113">要在文件夹内的页面上显示的应用的集合。</span><span class="sxs-lookup"><span data-stu-id="59c8f-113">A list of apps to appear on a page within a folder.</span></span> <span data-ttu-id="59c8f-114">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="59c8f-114">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="59c8f-115">关系</span><span class="sxs-lookup"><span data-stu-id="59c8f-115">Relationships</span></span>
<span data-ttu-id="59c8f-116">无</span><span class="sxs-lookup"><span data-stu-id="59c8f-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="59c8f-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="59c8f-117">JSON Representation</span></span>
<span data-ttu-id="59c8f-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="59c8f-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosHomeScreenFolderPage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenFolderPage",
  "displayName": "String",
  "apps": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenApp",
      "displayName": "String",
      "bundleID": "String"
    }
  ]
}
```


