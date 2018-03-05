# <a name="intunebrand-resource-type"></a><span data-ttu-id="05781-101">intuneBrand 资源类型</span><span class="sxs-lookup"><span data-stu-id="05781-101">intuneBrand resource type</span></span>

> <span data-ttu-id="05781-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="05781-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="05781-103">intuneBrand 包含在自定义公司门户应用程序以及最终用户网页版门户的外观时使用的数据。</span><span class="sxs-lookup"><span data-stu-id="05781-103">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>
## <a name="properties"></a><span data-ttu-id="05781-104">属性</span><span class="sxs-lookup"><span data-stu-id="05781-104">Properties</span></span>
|<span data-ttu-id="05781-105">属性</span><span class="sxs-lookup"><span data-stu-id="05781-105">Property</span></span>|<span data-ttu-id="05781-106">类型</span><span class="sxs-lookup"><span data-stu-id="05781-106">Type</span></span>|<span data-ttu-id="05781-107">说明</span><span class="sxs-lookup"><span data-stu-id="05781-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05781-108">displayName</span><span class="sxs-lookup"><span data-stu-id="05781-108">displayName</span></span>|<span data-ttu-id="05781-109">String</span><span class="sxs-lookup"><span data-stu-id="05781-109">String</span></span>|<span data-ttu-id="05781-110">向最终用户显示的公司/组织名称。</span><span class="sxs-lookup"><span data-stu-id="05781-110">Company/organization name that is displayed to end users.</span></span>|
|<span data-ttu-id="05781-111">contactITName</span><span class="sxs-lookup"><span data-stu-id="05781-111">contactITName</span></span>|<span data-ttu-id="05781-112">String</span><span class="sxs-lookup"><span data-stu-id="05781-112">String</span></span>|<span data-ttu-id="05781-113">负责 IT 支持的员工/组织名称。</span><span class="sxs-lookup"><span data-stu-id="05781-113">Name of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="05781-114">contactITPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="05781-114">contactITPhoneNumber</span></span>|<span data-ttu-id="05781-115">String</span><span class="sxs-lookup"><span data-stu-id="05781-115">String</span></span>|<span data-ttu-id="05781-116">负责 IT 支持的员工/组织的电话号码。</span><span class="sxs-lookup"><span data-stu-id="05781-116">Phone number of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="05781-117">contactITEmailAddress</span><span class="sxs-lookup"><span data-stu-id="05781-117">contactITEmailAddress</span></span>|<span data-ttu-id="05781-118">String</span><span class="sxs-lookup"><span data-stu-id="05781-118">String</span></span>|<span data-ttu-id="05781-119">负责 IT 支持的员工/组织的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="05781-119">Email address of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="05781-120">contactITNotes</span><span class="sxs-lookup"><span data-stu-id="05781-120">contactITNotes</span></span>|<span data-ttu-id="05781-121">String</span><span class="sxs-lookup"><span data-stu-id="05781-121">String</span></span>|<span data-ttu-id="05781-122">负责 IT 支持的员工/组织的文本注释。</span><span class="sxs-lookup"><span data-stu-id="05781-122">Text comments regarding the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="05781-123">privacyUrl</span><span class="sxs-lookup"><span data-stu-id="05781-123">privacyUrl</span></span>|<span data-ttu-id="05781-124">String</span><span class="sxs-lookup"><span data-stu-id="05781-124">String</span></span>|<span data-ttu-id="05781-125">指向公司/组织隐私策略的 URL。</span><span class="sxs-lookup"><span data-stu-id="05781-125">URL to the company/organization’s privacy policy.</span></span>|
|<span data-ttu-id="05781-126">onlineSupportSiteUrl</span><span class="sxs-lookup"><span data-stu-id="05781-126">onlineSupportSiteUrl</span></span>|<span data-ttu-id="05781-127">String</span><span class="sxs-lookup"><span data-stu-id="05781-127">String</span></span>|<span data-ttu-id="05781-128">指向公司/组织 IT 支持人员网站的 URL。</span><span class="sxs-lookup"><span data-stu-id="05781-128">URL to the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="05781-129">onlineSupportSiteName</span><span class="sxs-lookup"><span data-stu-id="05781-129">onlineSupportSiteName</span></span>|<span data-ttu-id="05781-130">String</span><span class="sxs-lookup"><span data-stu-id="05781-130">String</span></span>|<span data-ttu-id="05781-131">显示公司/组织 IT 支持人员网站的名称。</span><span class="sxs-lookup"><span data-stu-id="05781-131">Display name of the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="05781-132">themeColor</span><span class="sxs-lookup"><span data-stu-id="05781-132">themeColor</span></span>|[<span data-ttu-id="05781-133">rgbColor</span><span class="sxs-lookup"><span data-stu-id="05781-133">RGBColor</span></span>](../resources/intune_onboarding_rgbcolor.md)|<span data-ttu-id="05781-134">公司门户应用程序和 Web 门户中使用的主要主题颜色。</span><span class="sxs-lookup"><span data-stu-id="05781-134">Primary theme color used in the Company Portal applications and web portal.</span></span>|
|<span data-ttu-id="05781-135">showLogo</span><span class="sxs-lookup"><span data-stu-id="05781-135">showLogo</span></span>|<span data-ttu-id="05781-136">布尔值</span><span class="sxs-lookup"><span data-stu-id="05781-136">Boolean</span></span>|<span data-ttu-id="05781-137">表示是否显示管理员提供的徽标图像的布尔值。</span><span class="sxs-lookup"><span data-stu-id="05781-137">Boolean that represents whether the administrator-supplied logo images are shown or not shown.</span></span>|
|<span data-ttu-id="05781-138">lightBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="05781-138">lightBackgroundLogo</span></span>|[<span data-ttu-id="05781-139">mimeContent</span><span class="sxs-lookup"><span data-stu-id="05781-139">mimeContent</span></span>](../resources/intune_onboarding_mimecontent.md)|<span data-ttu-id="05781-140">在公司门户应用中显示的徽标图像，徽标后有浅色背景。</span><span class="sxs-lookup"><span data-stu-id="05781-140">Logo image displayed in Company Portal apps which have a light background behind the logo.</span></span>|
|<span data-ttu-id="05781-141">darkBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="05781-141">darkBackgroundLogo</span></span>|[<span data-ttu-id="05781-142">mimeContent</span><span class="sxs-lookup"><span data-stu-id="05781-142">mimeContent</span></span>](../resources/intune_onboarding_mimecontent.md)|<span data-ttu-id="05781-143">在公司门户应用中显示的徽标图像，徽标后有深色背景。</span><span class="sxs-lookup"><span data-stu-id="05781-143">Logo image displayed in Company Portal apps which have a dark background behind the logo.</span></span>|
|<span data-ttu-id="05781-144">showNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="05781-144">showNameNextToLogo</span></span>|<span data-ttu-id="05781-145">布尔值</span><span class="sxs-lookup"><span data-stu-id="05781-145">Boolean</span></span>|<span data-ttu-id="05781-146">表示是否要在徽标图像旁显示管理员提供的显示名称的布尔值。</span><span class="sxs-lookup"><span data-stu-id="05781-146">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image.</span></span>|
|<span data-ttu-id="05781-147">showDisplayNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="05781-147">showDisplayNameNextToLogo</span></span>|<span data-ttu-id="05781-148">布尔值</span><span class="sxs-lookup"><span data-stu-id="05781-148">Boolean</span></span>|<span data-ttu-id="05781-149">表示是否要在徽标图像旁显示管理员提供的显示名称的布尔值。</span><span class="sxs-lookup"><span data-stu-id="05781-149">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image.</span></span>|

## <a name="relationships"></a><span data-ttu-id="05781-150">关系</span><span class="sxs-lookup"><span data-stu-id="05781-150">Relationships</span></span>
<span data-ttu-id="05781-151">无</span><span class="sxs-lookup"><span data-stu-id="05781-151">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="05781-152">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="05781-152">JSON Representation</span></span>
<span data-ttu-id="05781-153">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="05781-153">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.intuneBrand"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.intuneBrand",
  "displayName": "String",
  "contactITName": "String",
  "contactITPhoneNumber": "String",
  "contactITEmailAddress": "String",
  "contactITNotes": "String",
  "privacyUrl": "String",
  "onlineSupportSiteUrl": "String",
  "onlineSupportSiteName": "String",
  "themeColor": {
    "@odata.type": "microsoft.graph.rgbColor",
    "r": 1024,
    "g": 1024,
    "b": 1024
  },
  "showLogo": true,
  "lightBackgroundLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "darkBackgroundLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "showNameNextToLogo": true,
  "showDisplayNameNextToLogo": true
}
```


