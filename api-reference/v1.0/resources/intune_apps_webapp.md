# <a name="webapp-resource-type"></a><span data-ttu-id="733e0-101">webApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="733e0-101">webApp resource type</span></span>

> <span data-ttu-id="733e0-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="733e0-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="733e0-103">包含 Web 应用的属性和继承的属性。</span><span class="sxs-lookup"><span data-stu-id="733e0-103">Contains properties and inherited properties for web apps.</span></span>

<span data-ttu-id="733e0-104">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="733e0-104">Inherits from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>

## <a name="methods"></a><span data-ttu-id="733e0-105">方法</span><span class="sxs-lookup"><span data-stu-id="733e0-105">Methods</span></span>
|<span data-ttu-id="733e0-106">方法</span><span class="sxs-lookup"><span data-stu-id="733e0-106">Method</span></span>|<span data-ttu-id="733e0-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="733e0-107">Return Type</span></span>|<span data-ttu-id="733e0-108">说明</span><span class="sxs-lookup"><span data-stu-id="733e0-108">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="733e0-109">List webApps</span><span class="sxs-lookup"><span data-stu-id="733e0-109">List webApps</span></span>](../api/intune_apps_webapp_list.md)|<span data-ttu-id="733e0-110">[webApp](../resources/intune_apps_webapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="733e0-110">[webApp](../resources/intune_apps_webapp.md) collection</span></span>|<span data-ttu-id="733e0-111">列出 [webApp](../resources/intune_apps_webapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="733e0-111">List properties and relationships of the [webApp](../resources/intune_apps_webapp.md) objects.</span></span>|
|[<span data-ttu-id="733e0-112">Get webApp</span><span class="sxs-lookup"><span data-stu-id="733e0-112">Get webApp</span></span>](../api/intune_apps_webapp_get.md)|[<span data-ttu-id="733e0-113">webApp</span><span class="sxs-lookup"><span data-stu-id="733e0-113">webApp</span></span>](../resources/intune_apps_webapp.md)|<span data-ttu-id="733e0-114">读取 [webApp](../resources/intune_apps_webapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="733e0-114">Read properties and relationships of [plannerBucketTaskBoardTaskFormat](../resources/intune_apps_webapp.md) object.</span></span>|
|[<span data-ttu-id="733e0-115">Create webApp</span><span class="sxs-lookup"><span data-stu-id="733e0-115">Create webApp</span></span>](../api/intune_apps_webapp_create.md)|[<span data-ttu-id="733e0-116">webApp</span><span class="sxs-lookup"><span data-stu-id="733e0-116">webApp</span></span>](../resources/intune_apps_webapp.md)|<span data-ttu-id="733e0-117">创建新的 [webApp](../resources/intune_apps_webapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="733e0-117">Create a new [plannerBucket](../resources/intune_apps_webapp.md) object.</span></span>|
|[<span data-ttu-id="733e0-118">Delete webApp</span><span class="sxs-lookup"><span data-stu-id="733e0-118">Delete webApp</span></span>](../api/intune_apps_webapp_delete.md)|<span data-ttu-id="733e0-119">无</span><span class="sxs-lookup"><span data-stu-id="733e0-119">None</span></span>|<span data-ttu-id="733e0-120">删除 [webApp](../resources/intune_apps_webapp.md)。</span><span class="sxs-lookup"><span data-stu-id="733e0-120">Deletes a [webApp](../resources/intune_apps_webapp.md).</span></span>|
|[<span data-ttu-id="733e0-121">Update webApp</span><span class="sxs-lookup"><span data-stu-id="733e0-121">Update webApp</span></span>](../api/intune_apps_webapp_update.md)|[<span data-ttu-id="733e0-122">webApp</span><span class="sxs-lookup"><span data-stu-id="733e0-122">webApp</span></span>](../resources/intune_apps_webapp.md)|<span data-ttu-id="733e0-123">更新 [webApp](../resources/intune_apps_webapp.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="733e0-123">Update the properties of a [calendar](../resources/intune_apps_webapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="733e0-124">属性</span><span class="sxs-lookup"><span data-stu-id="733e0-124">Properties</span></span>
|<span data-ttu-id="733e0-125">属性</span><span class="sxs-lookup"><span data-stu-id="733e0-125">Property</span></span>|<span data-ttu-id="733e0-126">类型</span><span class="sxs-lookup"><span data-stu-id="733e0-126">Type</span></span>|<span data-ttu-id="733e0-127">说明</span><span class="sxs-lookup"><span data-stu-id="733e0-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="733e0-128">id</span><span class="sxs-lookup"><span data-stu-id="733e0-128">id</span></span>|<span data-ttu-id="733e0-129">String</span><span class="sxs-lookup"><span data-stu-id="733e0-129">String</span></span>|<span data-ttu-id="733e0-130">实体的键。</span><span class="sxs-lookup"><span data-stu-id="733e0-130">Key of the setting.</span></span> <span data-ttu-id="733e0-131">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="733e0-131">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="733e0-132">displayName</span><span class="sxs-lookup"><span data-stu-id="733e0-132">displayName</span></span>|<span data-ttu-id="733e0-133">String</span><span class="sxs-lookup"><span data-stu-id="733e0-133">String</span></span>|<span data-ttu-id="733e0-134">管理员提供或导入的应用标题。</span><span class="sxs-lookup"><span data-stu-id="733e0-134">The admin provided or imported title of the app.</span></span> <span data-ttu-id="733e0-135">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="733e0-135">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="733e0-136">description</span><span class="sxs-lookup"><span data-stu-id="733e0-136">description</span></span>|<span data-ttu-id="733e0-137">String</span><span class="sxs-lookup"><span data-stu-id="733e0-137">String</span></span>|<span data-ttu-id="733e0-138">应用的说明。</span><span class="sxs-lookup"><span data-stu-id="733e0-138">The description of the app.</span></span> <span data-ttu-id="733e0-139">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="733e0-139">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="733e0-140">publisher</span><span class="sxs-lookup"><span data-stu-id="733e0-140">Publisher</span></span>|<span data-ttu-id="733e0-141">String</span><span class="sxs-lookup"><span data-stu-id="733e0-141">String</span></span>|<span data-ttu-id="733e0-142">应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="733e0-142">The name of the app.</span></span> <span data-ttu-id="733e0-143">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="733e0-143">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="733e0-144">largeIcon</span><span class="sxs-lookup"><span data-stu-id="733e0-144">largeIcon</span></span>|[<span data-ttu-id="733e0-145">mimeContent</span><span class="sxs-lookup"><span data-stu-id="733e0-145">mimeContent</span></span>](../resources/intune_apps_mimecontent.md)|<span data-ttu-id="733e0-146">要显示在应用详细信息中或用于图标上传的大图标。</span><span class="sxs-lookup"><span data-stu-id="733e0-146">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="733e0-147">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="733e0-147">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="733e0-148">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="733e0-148">createdDateTime</span></span>|<span data-ttu-id="733e0-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="733e0-149">DateTimeOffset</span></span>|<span data-ttu-id="733e0-150">创建应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="733e0-150">The date and time when the page was created.</span></span> <span data-ttu-id="733e0-151">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="733e0-151">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="733e0-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="733e0-152">lastModifiedDateTime</span></span>|<span data-ttu-id="733e0-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="733e0-153">DateTimeOffset</span></span>|<span data-ttu-id="733e0-154">上次修改应用的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="733e0-154">The date and time when the attachment was last modified.</span></span> <span data-ttu-id="733e0-155">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="733e0-155">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="733e0-156">isFeatured</span><span class="sxs-lookup"><span data-stu-id="733e0-156">isFeatured</span></span>|<span data-ttu-id="733e0-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="733e0-157">Boolean</span></span>|<span data-ttu-id="733e0-158">指示应用是否被管理员标记为特色的值 继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="733e0-158">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="733e0-159">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="733e0-159">privacyInformationUrl</span></span>|<span data-ttu-id="733e0-160">String</span><span class="sxs-lookup"><span data-stu-id="733e0-160">String</span></span>|<span data-ttu-id="733e0-161">隐私声明 Url。</span><span class="sxs-lookup"><span data-stu-id="733e0-161">The privacy statement Url.</span></span> <span data-ttu-id="733e0-162">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="733e0-162">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="733e0-163">informationUrl</span><span class="sxs-lookup"><span data-stu-id="733e0-163">informationUrl</span></span>|<span data-ttu-id="733e0-164">String</span><span class="sxs-lookup"><span data-stu-id="733e0-164">String</span></span>|<span data-ttu-id="733e0-165">详细信息 Url。</span><span class="sxs-lookup"><span data-stu-id="733e0-165">The more information Url.</span></span> <span data-ttu-id="733e0-166">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="733e0-166">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="733e0-167">owner</span><span class="sxs-lookup"><span data-stu-id="733e0-167">owner</span></span>|<span data-ttu-id="733e0-168">String</span><span class="sxs-lookup"><span data-stu-id="733e0-168">String</span></span>|<span data-ttu-id="733e0-169">应用的所有者。</span><span class="sxs-lookup"><span data-stu-id="733e0-169">The owner of the timesheet.</span></span> <span data-ttu-id="733e0-170">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="733e0-170">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="733e0-171">developer</span><span class="sxs-lookup"><span data-stu-id="733e0-171">developer</span></span>|<span data-ttu-id="733e0-172">String</span><span class="sxs-lookup"><span data-stu-id="733e0-172">String</span></span>|<span data-ttu-id="733e0-173">应用的开发者。</span><span class="sxs-lookup"><span data-stu-id="733e0-173">The name of the app.</span></span> <span data-ttu-id="733e0-174">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="733e0-174">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="733e0-175">notes</span><span class="sxs-lookup"><span data-stu-id="733e0-175">notes</span></span>|<span data-ttu-id="733e0-176">String</span><span class="sxs-lookup"><span data-stu-id="733e0-176">String</span></span>|<span data-ttu-id="733e0-177">应用的备注。</span><span class="sxs-lookup"><span data-stu-id="733e0-177">Notes for the app.</span></span> <span data-ttu-id="733e0-178">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="733e0-178">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="733e0-179">publishingState</span><span class="sxs-lookup"><span data-stu-id="733e0-179">publishingState</span></span>|<span data-ttu-id="733e0-180">String</span><span class="sxs-lookup"><span data-stu-id="733e0-180">String</span></span>|<span data-ttu-id="733e0-181">应用的发布状态。</span><span class="sxs-lookup"><span data-stu-id="733e0-181">The publishing state for the app.</span></span> <span data-ttu-id="733e0-182">除非应用已发布，否则无法分配应用。</span><span class="sxs-lookup"><span data-stu-id="733e0-182">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="733e0-183">继承自 [mobileApp](../resources/intune_apps_mobileapp.md) 可取值为：`notPublished`、`processing`、`published`。</span><span class="sxs-lookup"><span data-stu-id="733e0-183">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md) Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="733e0-184">appUrl</span><span class="sxs-lookup"><span data-stu-id="733e0-184">appUrl</span></span>|<span data-ttu-id="733e0-185">String</span><span class="sxs-lookup"><span data-stu-id="733e0-185">String</span></span>|<span data-ttu-id="733e0-186">Web 应用 URL。</span><span class="sxs-lookup"><span data-stu-id="733e0-186">The web app URL.</span></span>|
|<span data-ttu-id="733e0-187">useManagedBrowser</span><span class="sxs-lookup"><span data-stu-id="733e0-187">useManagedBrowser</span></span>|<span data-ttu-id="733e0-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="733e0-188">Boolean</span></span>|<span data-ttu-id="733e0-189">是否使用托管浏览器。</span><span class="sxs-lookup"><span data-stu-id="733e0-189">Whether or not to use managed browser.</span></span> <span data-ttu-id="733e0-190">此属性仅适用于 Android 和 iOS。</span><span class="sxs-lookup"><span data-stu-id="733e0-190">This property is only applicable for Android and IOS.</span></span>|

## <a name="relationships"></a><span data-ttu-id="733e0-191">关系</span><span class="sxs-lookup"><span data-stu-id="733e0-191">Relationships</span></span>
|<span data-ttu-id="733e0-192">关系</span><span class="sxs-lookup"><span data-stu-id="733e0-192">Relationship</span></span>|<span data-ttu-id="733e0-193">类型</span><span class="sxs-lookup"><span data-stu-id="733e0-193">Type</span></span>|<span data-ttu-id="733e0-194">说明</span><span class="sxs-lookup"><span data-stu-id="733e0-194">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="733e0-195">categories</span><span class="sxs-lookup"><span data-stu-id="733e0-195">categories</span></span>|<span data-ttu-id="733e0-196">[mobileAppCategory](../resources/intune_apps_mobileappcategory.md) 集合</span><span class="sxs-lookup"><span data-stu-id="733e0-196">[mobileAppCategory](../resources/intune_apps_mobileappcategory.md) collection</span></span>|<span data-ttu-id="733e0-197">此应用的类别列表。</span><span class="sxs-lookup"><span data-stu-id="733e0-197">The list of categories for this app.</span></span> <span data-ttu-id="733e0-198">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="733e0-198">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|
|<span data-ttu-id="733e0-199">assignments</span><span class="sxs-lookup"><span data-stu-id="733e0-199">assignments</span></span>|<span data-ttu-id="733e0-200">[mobileAppAssignment](../resources/intune_apps_mobileappassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="733e0-200">[mobileAppAssignment](../resources/intune_apps_mobileappassignment.md) collection</span></span>|<span data-ttu-id="733e0-201">此移动应用的组分配的列表。</span><span class="sxs-lookup"><span data-stu-id="733e0-201">The list of group assignments for this mobile app.</span></span> <span data-ttu-id="733e0-202">继承自 [mobileApp](../resources/intune_apps_mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="733e0-202">Inherited from [mobileApp](../resources/intune_apps_mobileapp.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="733e0-203">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="733e0-203">JSON Representation</span></span>
<span data-ttu-id="733e0-204">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="733e0-204">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.webApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.webApp",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "publisher": "String",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "isFeatured": true,
  "privacyInformationUrl": "String",
  "informationUrl": "String",
  "owner": "String",
  "developer": "String",
  "notes": "String",
  "publishingState": "String",
  "appUrl": "String",
  "useManagedBrowser": true
}
```


