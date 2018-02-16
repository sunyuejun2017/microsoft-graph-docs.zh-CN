# <a name="ioshomescreenpage-resource-type"></a><span data-ttu-id="dd251-101">iosHomeScreenPage 资源类型</span><span class="sxs-lookup"><span data-stu-id="dd251-101">iosHomeScreenPage resource type</span></span>

> <span data-ttu-id="dd251-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="dd251-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dd251-103">包含主屏幕上的应用和文件夹的页面</span><span class="sxs-lookup"><span data-stu-id="dd251-103">A page containing apps and folders on the Home Screen</span></span>
## <a name="properties"></a><span data-ttu-id="dd251-104">属性</span><span class="sxs-lookup"><span data-stu-id="dd251-104">Properties</span></span>
|<span data-ttu-id="dd251-105">属性</span><span class="sxs-lookup"><span data-stu-id="dd251-105">Property</span></span>|<span data-ttu-id="dd251-106">类型</span><span class="sxs-lookup"><span data-stu-id="dd251-106">Type</span></span>|<span data-ttu-id="dd251-107">说明</span><span class="sxs-lookup"><span data-stu-id="dd251-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dd251-108">displayName</span><span class="sxs-lookup"><span data-stu-id="dd251-108">displayName</span></span>|<span data-ttu-id="dd251-109">String</span><span class="sxs-lookup"><span data-stu-id="dd251-109">String</span></span>|<span data-ttu-id="dd251-110">页面的名称</span><span class="sxs-lookup"><span data-stu-id="dd251-110">Name of the page</span></span>|
|<span data-ttu-id="dd251-111">图标</span><span class="sxs-lookup"><span data-stu-id="dd251-111">Icons</span></span>|<span data-ttu-id="dd251-112">[iosHomeScreenItem](../resources/intune_deviceconfig_ioshomescreenitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="dd251-112">[iosHomeScreenItem](../resources/intune_deviceconfig_ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="dd251-113">要在页面上显示的应用和文件夹的列表。</span><span class="sxs-lookup"><span data-stu-id="dd251-113">A list of apps and folders to appear on a page.</span></span> <span data-ttu-id="dd251-114">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="dd251-114">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dd251-115">关系</span><span class="sxs-lookup"><span data-stu-id="dd251-115">Relationships</span></span>
<span data-ttu-id="dd251-116">无</span><span class="sxs-lookup"><span data-stu-id="dd251-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="dd251-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dd251-117">JSON Representation</span></span>
<span data-ttu-id="dd251-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dd251-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosHomeScreenPage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenPage",
  "displayName": "String",
  "icons": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenFolder",
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
  ]
}
```


