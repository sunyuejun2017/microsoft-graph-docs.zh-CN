# <a name="ioshomescreenitem-resource-type"></a><span data-ttu-id="f9f21-101">iosHomeScreenItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="f9f21-101">iosHomeScreenItem resource type</span></span>

> <span data-ttu-id="f9f21-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="f9f21-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f9f21-103">表示 iOS 主屏幕上的项</span><span class="sxs-lookup"><span data-stu-id="f9f21-103">Represents an item on the iOS Home Screen</span></span>
## <a name="properties"></a><span data-ttu-id="f9f21-104">属性</span><span class="sxs-lookup"><span data-stu-id="f9f21-104">Properties</span></span>
|<span data-ttu-id="f9f21-105">属性</span><span class="sxs-lookup"><span data-stu-id="f9f21-105">Property</span></span>|<span data-ttu-id="f9f21-106">类型</span><span class="sxs-lookup"><span data-stu-id="f9f21-106">Type</span></span>|<span data-ttu-id="f9f21-107">说明</span><span class="sxs-lookup"><span data-stu-id="f9f21-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9f21-108">displayName</span><span class="sxs-lookup"><span data-stu-id="f9f21-108">displayName</span></span>|<span data-ttu-id="f9f21-109">String</span><span class="sxs-lookup"><span data-stu-id="f9f21-109">String</span></span>|<span data-ttu-id="f9f21-110">应用的名称</span><span class="sxs-lookup"><span data-stu-id="f9f21-110">Name of the app</span></span>|

## <a name="relationships"></a><span data-ttu-id="f9f21-111">关系</span><span class="sxs-lookup"><span data-stu-id="f9f21-111">Relationships</span></span>
<span data-ttu-id="f9f21-112">无</span><span class="sxs-lookup"><span data-stu-id="f9f21-112">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f9f21-113">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f9f21-113">JSON Representation</span></span>
<span data-ttu-id="f9f21-114">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f9f21-114">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosHomeScreenItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenItem",
  "displayName": "String"
}
```


