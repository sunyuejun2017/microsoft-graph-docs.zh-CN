# <a name="configurationmanagerclientenabledfeatures-resource-type"></a><span data-ttu-id="e427c-101">configurationManagerClientEnabledFeatures 资源类型</span><span class="sxs-lookup"><span data-stu-id="e427c-101">configurationManagerClientEnabledFeatures resource type</span></span>

> <span data-ttu-id="e427c-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="e427c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e427c-103">Configuration Manager 客户端已启用的功能</span><span class="sxs-lookup"><span data-stu-id="e427c-103">configuration Manager client enabled features</span></span>
## <a name="properties"></a><span data-ttu-id="e427c-104">属性</span><span class="sxs-lookup"><span data-stu-id="e427c-104">Properties</span></span>
|<span data-ttu-id="e427c-105">属性</span><span class="sxs-lookup"><span data-stu-id="e427c-105">Property</span></span>|<span data-ttu-id="e427c-106">类型</span><span class="sxs-lookup"><span data-stu-id="e427c-106">Type</span></span>|<span data-ttu-id="e427c-107">说明</span><span class="sxs-lookup"><span data-stu-id="e427c-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e427c-108">inventory</span><span class="sxs-lookup"><span data-stu-id="e427c-108">inventory</span></span>|<span data-ttu-id="e427c-109">Boolean</span><span class="sxs-lookup"><span data-stu-id="e427c-109">Boolean</span></span>|<span data-ttu-id="e427c-110">目录是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="e427c-110">Whether inventory is managed by Intune</span></span>|
|<span data-ttu-id="e427c-111">modernApps</span><span class="sxs-lookup"><span data-stu-id="e427c-111">modernApps</span></span>|<span data-ttu-id="e427c-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="e427c-112">Boolean</span></span>|<span data-ttu-id="e427c-113">现代应用程序是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="e427c-113">Whether modern application is managed by Intune</span></span>|
|<span data-ttu-id="e427c-114">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="e427c-114">resourceAccess</span></span>|<span data-ttu-id="e427c-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="e427c-115">Boolean</span></span>|<span data-ttu-id="e427c-116">资源访问权限是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="e427c-116">Whether resource access is managed by Intune</span></span>|
|<span data-ttu-id="e427c-117">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="e427c-117">deviceConfiguration</span></span>|<span data-ttu-id="e427c-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="e427c-118">Boolean</span></span>|<span data-ttu-id="e427c-119">设备配置是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="e427c-119">Whether device configuration is managed by Intune</span></span>|
|<span data-ttu-id="e427c-120">compliancePolicy</span><span class="sxs-lookup"><span data-stu-id="e427c-120">compliancePolicy</span></span>|<span data-ttu-id="e427c-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="e427c-121">Boolean</span></span>|<span data-ttu-id="e427c-122">符合性策略是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="e427c-122">Whether compliance policy is managed by Intune</span></span>|
|<span data-ttu-id="e427c-123">windowsUpdateForBusiness</span><span class="sxs-lookup"><span data-stu-id="e427c-123">windowsUpdateForBusiness</span></span>|<span data-ttu-id="e427c-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="e427c-124">Boolean</span></span>|<span data-ttu-id="e427c-125">适用于企业的 Windows 更新是否由 Intune 管理</span><span class="sxs-lookup"><span data-stu-id="e427c-125">Whether Windows Update for Business is managed by Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="e427c-126">关系</span><span class="sxs-lookup"><span data-stu-id="e427c-126">Relationships</span></span>
<span data-ttu-id="e427c-127">无</span><span class="sxs-lookup"><span data-stu-id="e427c-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e427c-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e427c-128">JSON Representation</span></span>
<span data-ttu-id="e427c-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e427c-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.configurationManagerClientEnabledFeatures"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.configurationManagerClientEnabledFeatures",
  "inventory": true,
  "modernApps": true,
  "resourceAccess": true,
  "deviceConfiguration": true,
  "compliancePolicy": true,
  "windowsUpdateForBusiness": true
}
```


