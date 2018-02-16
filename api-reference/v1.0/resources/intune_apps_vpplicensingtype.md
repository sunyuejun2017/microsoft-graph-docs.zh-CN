# <a name="vpplicensingtype-resource-type"></a><span data-ttu-id="57855-101">vppLicensingType 资源类型</span><span class="sxs-lookup"><span data-stu-id="57855-101">vppLicensingType resource type</span></span>

> <span data-ttu-id="57855-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="57855-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="57855-103">包含 iOS 批量采购程序 (Vpp) 许可类型的属性。</span><span class="sxs-lookup"><span data-stu-id="57855-103">Contains properties for iOS Volume-Purchased Program (Vpp) Licensing Type.</span></span>
## <a name="properties"></a><span data-ttu-id="57855-104">属性</span><span class="sxs-lookup"><span data-stu-id="57855-104">Properties</span></span>
|<span data-ttu-id="57855-105">属性</span><span class="sxs-lookup"><span data-stu-id="57855-105">Property</span></span>|<span data-ttu-id="57855-106">类型</span><span class="sxs-lookup"><span data-stu-id="57855-106">Type</span></span>|<span data-ttu-id="57855-107">说明</span><span class="sxs-lookup"><span data-stu-id="57855-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="57855-108">supportsUserLicensing</span><span class="sxs-lookup"><span data-stu-id="57855-108">supportsUserLicensing</span></span>|<span data-ttu-id="57855-109">布尔值</span><span class="sxs-lookup"><span data-stu-id="57855-109">Boolean</span></span>|<span data-ttu-id="57855-110">程序是否支持用户许可类型。</span><span class="sxs-lookup"><span data-stu-id="57855-110">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="57855-111">supportsDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="57855-111">supportsDeviceLicensing</span></span>|<span data-ttu-id="57855-112">布尔值</span><span class="sxs-lookup"><span data-stu-id="57855-112">Boolean</span></span>|<span data-ttu-id="57855-113">程序是否支持设备许可类型。</span><span class="sxs-lookup"><span data-stu-id="57855-113">Whether the program supports the device licensing type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="57855-114">关系</span><span class="sxs-lookup"><span data-stu-id="57855-114">Relationships</span></span>
<span data-ttu-id="57855-115">无</span><span class="sxs-lookup"><span data-stu-id="57855-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="57855-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="57855-116">JSON Representation</span></span>
<span data-ttu-id="57855-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="57855-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.vppLicensingType"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vppLicensingType",
  "supportsUserLicensing": true,
  "supportsDeviceLicensing": true
}
```


