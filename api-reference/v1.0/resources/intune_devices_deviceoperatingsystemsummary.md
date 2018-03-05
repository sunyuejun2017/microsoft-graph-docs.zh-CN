# <a name="deviceoperatingsystemsummary-resource-type"></a><span data-ttu-id="d3542-101">deviceOperatingSystemSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="d3542-101">deviceOperatingSystemSummary resource type</span></span>

> <span data-ttu-id="d3542-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="d3542-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d3542-103">设备操作系统摘要。</span><span class="sxs-lookup"><span data-stu-id="d3542-103">Device operating system summary.</span></span>
## <a name="properties"></a><span data-ttu-id="d3542-104">属性</span><span class="sxs-lookup"><span data-stu-id="d3542-104">Properties</span></span>
|<span data-ttu-id="d3542-105">属性</span><span class="sxs-lookup"><span data-stu-id="d3542-105">Property</span></span>|<span data-ttu-id="d3542-106">类型</span><span class="sxs-lookup"><span data-stu-id="d3542-106">Type</span></span>|<span data-ttu-id="d3542-107">说明</span><span class="sxs-lookup"><span data-stu-id="d3542-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3542-108">androidCount</span><span class="sxs-lookup"><span data-stu-id="d3542-108">androidCount</span></span>|<span data-ttu-id="d3542-109">Int32</span><span class="sxs-lookup"><span data-stu-id="d3542-109">Int32</span></span>|<span data-ttu-id="d3542-110">Android 设备计数。</span><span class="sxs-lookup"><span data-stu-id="d3542-110">Number of android device count.</span></span>|
|<span data-ttu-id="d3542-111">iosCount</span><span class="sxs-lookup"><span data-stu-id="d3542-111">iosCount</span></span>|<span data-ttu-id="d3542-112">Int32</span><span class="sxs-lookup"><span data-stu-id="d3542-112">Int32</span></span>|<span data-ttu-id="d3542-113">iOS 设备计数。</span><span class="sxs-lookup"><span data-stu-id="d3542-113">Number of iOS device count.</span></span>|
|<span data-ttu-id="d3542-114">macOSCount</span><span class="sxs-lookup"><span data-stu-id="d3542-114">macOSCount</span></span>|<span data-ttu-id="d3542-115">Int32</span><span class="sxs-lookup"><span data-stu-id="d3542-115">Int32</span></span>|<span data-ttu-id="d3542-116">Mac OS X 设备计数。</span><span class="sxs-lookup"><span data-stu-id="d3542-116">Number of Mac OS X device count.</span></span>|
|<span data-ttu-id="d3542-117">windowsMobileCount</span><span class="sxs-lookup"><span data-stu-id="d3542-117">windowsMobileCount</span></span>|<span data-ttu-id="d3542-118">Int32</span><span class="sxs-lookup"><span data-stu-id="d3542-118">Int32</span></span>|<span data-ttu-id="d3542-119">Windows 移动设备计数。</span><span class="sxs-lookup"><span data-stu-id="d3542-119">Number of Windows mobile device count.</span></span>|
|<span data-ttu-id="d3542-120">windowsCount</span><span class="sxs-lookup"><span data-stu-id="d3542-120">windowsCount</span></span>|<span data-ttu-id="d3542-121">Int32</span><span class="sxs-lookup"><span data-stu-id="d3542-121">Int32</span></span>|<span data-ttu-id="d3542-122">Windows 设备计数。</span><span class="sxs-lookup"><span data-stu-id="d3542-122">Number of Windows device count.</span></span>|
|<span data-ttu-id="d3542-123">unknownCount</span><span class="sxs-lookup"><span data-stu-id="d3542-123">unknownCount</span></span>|<span data-ttu-id="d3542-124">Int32</span><span class="sxs-lookup"><span data-stu-id="d3542-124">Int32</span></span>|<span data-ttu-id="d3542-125">未知设备计数。</span><span class="sxs-lookup"><span data-stu-id="d3542-125">Number of unknown device count.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d3542-126">关系</span><span class="sxs-lookup"><span data-stu-id="d3542-126">Relationships</span></span>
<span data-ttu-id="d3542-127">无</span><span class="sxs-lookup"><span data-stu-id="d3542-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d3542-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d3542-128">JSON Representation</span></span>
<span data-ttu-id="d3542-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d3542-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceOperatingSystemSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceOperatingSystemSummary",
  "androidCount": 1024,
  "iosCount": 1024,
  "macOSCount": 1024,
  "windowsMobileCount": 1024,
  "windowsCount": 1024,
  "unknownCount": 1024
}
```


