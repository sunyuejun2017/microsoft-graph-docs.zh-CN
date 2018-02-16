# <a name="iosvppappassignmentsettings-resource-type"></a><span data-ttu-id="5d7bd-101">iosVppAppAssignmentSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="5d7bd-101">iosVppAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="5d7bd-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="5d7bd-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5d7bd-103">包含用于为组分配 iOS APP 移动应用的属性。</span><span class="sxs-lookup"><span data-stu-id="5d7bd-103">Contains properties used to assign an iOS VPP mobile app to a group.</span></span>

<span data-ttu-id="5d7bd-104">继承自 [mobileAppAssignmentSettings](../resources/intune_apps_mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="5d7bd-104">Inherits from [mobileAppAssignmentSettings](../resources/intune_apps_mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5d7bd-105">属性</span><span class="sxs-lookup"><span data-stu-id="5d7bd-105">Properties</span></span>
|<span data-ttu-id="5d7bd-106">属性</span><span class="sxs-lookup"><span data-stu-id="5d7bd-106">Property</span></span>|<span data-ttu-id="5d7bd-107">类型</span><span class="sxs-lookup"><span data-stu-id="5d7bd-107">Type</span></span>|<span data-ttu-id="5d7bd-108">说明</span><span class="sxs-lookup"><span data-stu-id="5d7bd-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5d7bd-109">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="5d7bd-109">useDeviceLicensing</span></span>|<span data-ttu-id="5d7bd-110">布尔值</span><span class="sxs-lookup"><span data-stu-id="5d7bd-110">Boolean</span></span>|<span data-ttu-id="5d7bd-111">是否使用设备许可。</span><span class="sxs-lookup"><span data-stu-id="5d7bd-111">Whether or not to use device licensing.</span></span>|
|<span data-ttu-id="5d7bd-112">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="5d7bd-112">vpnConfigurationId</span></span>|<span data-ttu-id="5d7bd-113">String</span><span class="sxs-lookup"><span data-stu-id="5d7bd-113">String</span></span>|<span data-ttu-id="5d7bd-114">要申请此应用的 VPN 配置 ID。</span><span class="sxs-lookup"><span data-stu-id="5d7bd-114">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5d7bd-115">关系</span><span class="sxs-lookup"><span data-stu-id="5d7bd-115">Relationships</span></span>
<span data-ttu-id="5d7bd-116">无</span><span class="sxs-lookup"><span data-stu-id="5d7bd-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5d7bd-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5d7bd-117">JSON Representation</span></span>
<span data-ttu-id="5d7bd-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5d7bd-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosVppAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosVppAppAssignmentSettings",
  "useDeviceLicensing": true,
  "vpnConfigurationId": "String"
}
```


