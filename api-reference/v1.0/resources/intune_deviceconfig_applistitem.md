# <a name="applistitem-resource-type"></a><span data-ttu-id="74719-101">appListItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="74719-101">appListItem resource type</span></span>

> <span data-ttu-id="74719-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="74719-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="74719-103">表示托管应用程序列表中的应用</span><span class="sxs-lookup"><span data-stu-id="74719-103">Represents an app in the list of managed applications</span></span>
## <a name="properties"></a><span data-ttu-id="74719-104">属性</span><span class="sxs-lookup"><span data-stu-id="74719-104">Properties</span></span>
|<span data-ttu-id="74719-105">属性</span><span class="sxs-lookup"><span data-stu-id="74719-105">Property</span></span>|<span data-ttu-id="74719-106">类型</span><span class="sxs-lookup"><span data-stu-id="74719-106">Type</span></span>|<span data-ttu-id="74719-107">说明</span><span class="sxs-lookup"><span data-stu-id="74719-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="74719-108">名称</span><span class="sxs-lookup"><span data-stu-id="74719-108">name</span></span>|<span data-ttu-id="74719-109">String</span><span class="sxs-lookup"><span data-stu-id="74719-109">String</span></span>|<span data-ttu-id="74719-110">应用程序名称</span><span class="sxs-lookup"><span data-stu-id="74719-110">The application name.</span></span>|
|<span data-ttu-id="74719-111">publisher</span><span class="sxs-lookup"><span data-stu-id="74719-111">Publisher</span></span>|<span data-ttu-id="74719-112">String</span><span class="sxs-lookup"><span data-stu-id="74719-112">String</span></span>|<span data-ttu-id="74719-113">应用程序发布者</span><span class="sxs-lookup"><span data-stu-id="74719-113">The publisher of the application</span></span>|
|<span data-ttu-id="74719-114">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="74719-114">appStoreUrl</span></span>|<span data-ttu-id="74719-115">String</span><span class="sxs-lookup"><span data-stu-id="74719-115">String</span></span>|<span data-ttu-id="74719-116">应用程序的应用商店 URL</span><span class="sxs-lookup"><span data-stu-id="74719-116">The URL of the add-in's web application.</span></span>|
|<span data-ttu-id="74719-117">appId</span><span class="sxs-lookup"><span data-stu-id="74719-117">AppId</span></span>|<span data-ttu-id="74719-118">String</span><span class="sxs-lookup"><span data-stu-id="74719-118">String</span></span>|<span data-ttu-id="74719-119">应用程序或应用程序的捆绑标识符</span><span class="sxs-lookup"><span data-stu-id="74719-119">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="74719-120">关系</span><span class="sxs-lookup"><span data-stu-id="74719-120">Relationships</span></span>
<span data-ttu-id="74719-121">无</span><span class="sxs-lookup"><span data-stu-id="74719-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="74719-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="74719-122">JSON Representation</span></span>
<span data-ttu-id="74719-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="74719-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.appListItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appListItem",
  "name": "String",
  "publisher": "String",
  "appStoreUrl": "String",
  "appId": "String"
}
```


