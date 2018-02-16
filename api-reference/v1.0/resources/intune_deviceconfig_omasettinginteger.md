# <a name="omasettinginteger-resource-type"></a><span data-ttu-id="892d5-101">omaSettingInteger 资源类型</span><span class="sxs-lookup"><span data-stu-id="892d5-101">omaSettingInteger resource type</span></span>

> <span data-ttu-id="892d5-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="892d5-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="892d5-103">OMA 设置整数定义。</span><span class="sxs-lookup"><span data-stu-id="892d5-103">OMA Settings Integer definition.</span></span>

<span data-ttu-id="892d5-104">继承自 [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="892d5-104">Inherits from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="892d5-105">属性</span><span class="sxs-lookup"><span data-stu-id="892d5-105">Properties</span></span>
|<span data-ttu-id="892d5-106">属性</span><span class="sxs-lookup"><span data-stu-id="892d5-106">Property</span></span>|<span data-ttu-id="892d5-107">类型</span><span class="sxs-lookup"><span data-stu-id="892d5-107">Type</span></span>|<span data-ttu-id="892d5-108">说明</span><span class="sxs-lookup"><span data-stu-id="892d5-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="892d5-109">displayName</span><span class="sxs-lookup"><span data-stu-id="892d5-109">displayName</span></span>|<span data-ttu-id="892d5-110">String</span><span class="sxs-lookup"><span data-stu-id="892d5-110">String</span></span>|<span data-ttu-id="892d5-111">显示名称。</span><span class="sxs-lookup"><span data-stu-id="892d5-111">Display Name</span></span> <span data-ttu-id="892d5-112">继承自 [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="892d5-112">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="892d5-113">description</span><span class="sxs-lookup"><span data-stu-id="892d5-113">description</span></span>|<span data-ttu-id="892d5-114">String</span><span class="sxs-lookup"><span data-stu-id="892d5-114">String</span></span>|<span data-ttu-id="892d5-115">说明。</span><span class="sxs-lookup"><span data-stu-id="892d5-115">Description.</span></span> <span data-ttu-id="892d5-116">继承自 [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="892d5-116">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="892d5-117">omaUri</span><span class="sxs-lookup"><span data-stu-id="892d5-117">omaUri</span></span>|<span data-ttu-id="892d5-118">String</span><span class="sxs-lookup"><span data-stu-id="892d5-118">String</span></span>|<span data-ttu-id="892d5-119">OMA。</span><span class="sxs-lookup"><span data-stu-id="892d5-119">OMA.</span></span> <span data-ttu-id="892d5-120">继承自 [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span><span class="sxs-lookup"><span data-stu-id="892d5-120">Inherited from [omaSetting](../resources/intune_deviceconfig_omasetting.md)</span></span>|
|<span data-ttu-id="892d5-121">值</span><span class="sxs-lookup"><span data-stu-id="892d5-121">value</span></span>|<span data-ttu-id="892d5-122">Int32</span><span class="sxs-lookup"><span data-stu-id="892d5-122">Int32</span></span>|<span data-ttu-id="892d5-123">值。</span><span class="sxs-lookup"><span data-stu-id="892d5-123">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="892d5-124">关系</span><span class="sxs-lookup"><span data-stu-id="892d5-124">Relationships</span></span>
<span data-ttu-id="892d5-125">无</span><span class="sxs-lookup"><span data-stu-id="892d5-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="892d5-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="892d5-126">JSON Representation</span></span>
<span data-ttu-id="892d5-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="892d5-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.omaSettingInteger"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingInteger",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": 1024
}
```


