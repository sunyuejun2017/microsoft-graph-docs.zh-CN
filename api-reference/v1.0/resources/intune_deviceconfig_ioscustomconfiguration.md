# <a name="ioscustomconfiguration-resource-type"></a><span data-ttu-id="d2224-101">iosCustomConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="d2224-101">iosCustomConfiguration resource type</span></span>

> <span data-ttu-id="d2224-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="d2224-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d2224-103">本主题提供由 iosCustomConfiguration 资源公开的已声明方法、属性和关系的说明。</span><span class="sxs-lookup"><span data-stu-id="d2224-103">This topic provides descriptions of the declared methods, properties and relationships exposed by the iosCustomConfiguration resource.</span></span>

<span data-ttu-id="d2224-104">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d2224-104">Inherits from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="d2224-105">方法</span><span class="sxs-lookup"><span data-stu-id="d2224-105">Methods</span></span>
|<span data-ttu-id="d2224-106">方法</span><span class="sxs-lookup"><span data-stu-id="d2224-106">Method</span></span>|<span data-ttu-id="d2224-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="d2224-107">Return Type</span></span>|<span data-ttu-id="d2224-108">说明</span><span class="sxs-lookup"><span data-stu-id="d2224-108">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d2224-109">List iosCustomConfigurations</span><span class="sxs-lookup"><span data-stu-id="d2224-109">List iosCustomConfigurations</span></span>](../api/intune_deviceconfig_ioscustomconfiguration_list.md)|<span data-ttu-id="d2224-110">[iosCustomConfiguration](../resources/intune_deviceconfig_ioscustomconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d2224-110">[iosCustomConfiguration](../resources/intune_deviceconfig_ioscustomconfiguration.md) collection</span></span>|<span data-ttu-id="d2224-111">列出 [iosCustomConfiguration](../resources/intune_deviceconfig_ioscustomconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d2224-111">List properties and relationships of the [iosCustomConfiguration](../resources/intune_deviceconfig_ioscustomconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="d2224-112">Get iosCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="d2224-112">Get iosCustomConfiguration</span></span>](../api/intune_deviceconfig_ioscustomconfiguration_get.md)|[<span data-ttu-id="d2224-113">iosCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="d2224-113">iosCustomConfiguration</span></span>](../resources/intune_deviceconfig_ioscustomconfiguration.md)|<span data-ttu-id="d2224-114">读取 [iosCustomConfiguration](../resources/intune_deviceconfig_ioscustomconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d2224-114">Read properties and relationships of [plannerTaskDetails](../resources/intune_deviceconfig_ioscustomconfiguration.md) object.</span></span>|
|[<span data-ttu-id="d2224-115">Create iosCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="d2224-115">Create iosCustomConfiguration</span></span>](../api/intune_deviceconfig_ioscustomconfiguration_create.md)|[<span data-ttu-id="d2224-116">iosCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="d2224-116">iosCustomConfiguration</span></span>](../resources/intune_deviceconfig_ioscustomconfiguration.md)|<span data-ttu-id="d2224-117">创建新的 [iosCustomConfiguration](../resources/intune_deviceconfig_ioscustomconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d2224-117">Create a new [plannerBucket](../resources/intune_deviceconfig_ioscustomconfiguration.md) object.</span></span>|
|[<span data-ttu-id="d2224-118">Delete iosCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="d2224-118">Delete iosCustomConfiguration</span></span>](../api/intune_deviceconfig_ioscustomconfiguration_delete.md)|<span data-ttu-id="d2224-119">无</span><span class="sxs-lookup"><span data-stu-id="d2224-119">None</span></span>|<span data-ttu-id="d2224-120">删除 [iosCustomConfiguration](../resources/intune_deviceconfig_ioscustomconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="d2224-120">Deletes a [iosCustomConfiguration](../resources/intune_deviceconfig_ioscustomconfiguration.md).</span></span>|
|[<span data-ttu-id="d2224-121">Update iosCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="d2224-121">Update iosCustomConfiguration</span></span>](../api/intune_deviceconfig_ioscustomconfiguration_update.md)|[<span data-ttu-id="d2224-122">iosCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="d2224-122">iosCustomConfiguration</span></span>](../resources/intune_deviceconfig_ioscustomconfiguration.md)|<span data-ttu-id="d2224-123">更新 [iosCustomConfiguration](../resources/intune_deviceconfig_ioscustomconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d2224-123">Update the properties of a [calendar](../resources/intune_deviceconfig_ioscustomconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d2224-124">属性</span><span class="sxs-lookup"><span data-stu-id="d2224-124">Properties</span></span>
|<span data-ttu-id="d2224-125">属性</span><span class="sxs-lookup"><span data-stu-id="d2224-125">Property</span></span>|<span data-ttu-id="d2224-126">类型</span><span class="sxs-lookup"><span data-stu-id="d2224-126">Type</span></span>|<span data-ttu-id="d2224-127">说明</span><span class="sxs-lookup"><span data-stu-id="d2224-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2224-128">id</span><span class="sxs-lookup"><span data-stu-id="d2224-128">id</span></span>|<span data-ttu-id="d2224-129">String</span><span class="sxs-lookup"><span data-stu-id="d2224-129">String</span></span>|<span data-ttu-id="d2224-130">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d2224-130">Key of the setting.</span></span> <span data-ttu-id="d2224-131">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d2224-131">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d2224-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d2224-132">lastModifiedDateTime</span></span>|<span data-ttu-id="d2224-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d2224-133">DateTimeOffset</span></span>|<span data-ttu-id="d2224-134">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="d2224-134">Indicates the date the object was last modified.</span></span> <span data-ttu-id="d2224-135">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d2224-135">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d2224-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d2224-136">createdDateTime</span></span>|<span data-ttu-id="d2224-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d2224-137">DateTimeOffset</span></span>|<span data-ttu-id="d2224-138">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="d2224-138">DateTime the object was created.</span></span> <span data-ttu-id="d2224-139">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d2224-139">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d2224-140">description</span><span class="sxs-lookup"><span data-stu-id="d2224-140">description</span></span>|<span data-ttu-id="d2224-141">String</span><span class="sxs-lookup"><span data-stu-id="d2224-141">String</span></span>|<span data-ttu-id="d2224-142">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="d2224-142">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d2224-143">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d2224-143">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d2224-144">displayName</span><span class="sxs-lookup"><span data-stu-id="d2224-144">displayName</span></span>|<span data-ttu-id="d2224-145">String</span><span class="sxs-lookup"><span data-stu-id="d2224-145">String</span></span>|<span data-ttu-id="d2224-146">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="d2224-146">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d2224-147">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d2224-147">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d2224-148">version</span><span class="sxs-lookup"><span data-stu-id="d2224-148">version</span></span>|<span data-ttu-id="d2224-149">Int32</span><span class="sxs-lookup"><span data-stu-id="d2224-149">Int32</span></span>|<span data-ttu-id="d2224-150">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="d2224-150">Version of the device configuration.</span></span> <span data-ttu-id="d2224-151">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d2224-151">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d2224-152">payloadName</span><span class="sxs-lookup"><span data-stu-id="d2224-152">payloadName</span></span>|<span data-ttu-id="d2224-153">String</span><span class="sxs-lookup"><span data-stu-id="d2224-153">String</span></span>|<span data-ttu-id="d2224-154">向用户显示的名称。</span><span class="sxs-lookup"><span data-stu-id="d2224-154">Name that is displayed to the user.</span></span>|
|<span data-ttu-id="d2224-155">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="d2224-155">payloadFileName</span></span>|<span data-ttu-id="d2224-156">String</span><span class="sxs-lookup"><span data-stu-id="d2224-156">String</span></span>|<span data-ttu-id="d2224-157">有效负载文件名 (\*.mobileconfig</span><span class="sxs-lookup"><span data-stu-id="d2224-157">Payload file name (\*.mobileconfig</span></span> | <span data-ttu-id="d2224-158">\*.xml)。</span><span class="sxs-lookup"><span data-stu-id="d2224-158">\*.xml</span></span>|
|<span data-ttu-id="d2224-159">payload</span><span class="sxs-lookup"><span data-stu-id="d2224-159">Notification payload</span></span>|<span data-ttu-id="d2224-160">Binary</span><span class="sxs-lookup"><span data-stu-id="d2224-160">Binary</span></span>|<span data-ttu-id="d2224-161">有效负载。</span><span class="sxs-lookup"><span data-stu-id="d2224-161">Payload.</span></span> <span data-ttu-id="d2224-162">（UTF8 编码的字节数组）</span><span class="sxs-lookup"><span data-stu-id="d2224-162">(UTF8 encoded byte array)</span></span>|

## <a name="relationships"></a><span data-ttu-id="d2224-163">关系</span><span class="sxs-lookup"><span data-stu-id="d2224-163">Relationships</span></span>
|<span data-ttu-id="d2224-164">关系</span><span class="sxs-lookup"><span data-stu-id="d2224-164">Relationship</span></span>|<span data-ttu-id="d2224-165">类型</span><span class="sxs-lookup"><span data-stu-id="d2224-165">Type</span></span>|<span data-ttu-id="d2224-166">说明</span><span class="sxs-lookup"><span data-stu-id="d2224-166">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2224-167">assignments</span><span class="sxs-lookup"><span data-stu-id="d2224-167">assignments</span></span>|<span data-ttu-id="d2224-168">[deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d2224-168">[deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="d2224-169">设备配置文件的分配列表。</span><span class="sxs-lookup"><span data-stu-id="d2224-169">The list of assignments for the device configuration profile.</span></span> <span data-ttu-id="d2224-170">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d2224-170">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d2224-171">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="d2224-171">deviceStatuses</span></span>|<span data-ttu-id="d2224-172">[deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d2224-172">[deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="d2224-173">按设备的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="d2224-173">Device configuration installation status by device.</span></span> <span data-ttu-id="d2224-174">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d2224-174">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d2224-175">userStatuses</span><span class="sxs-lookup"><span data-stu-id="d2224-175">userStatuses</span></span>|<span data-ttu-id="d2224-176">[deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d2224-176">[deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="d2224-177">按用户的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="d2224-177">Device configuration installation stauts by user.</span></span> <span data-ttu-id="d2224-178">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d2224-178">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d2224-179">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="d2224-179">deviceStatusOverview</span></span>|[<span data-ttu-id="d2224-180">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="d2224-180">deviceConfigurationDeviceOverview</span></span>](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md)|<span data-ttu-id="d2224-181">设备配置设备状态概述 继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d2224-181">Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d2224-182">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="d2224-182">userStatusOverview</span></span>|[<span data-ttu-id="d2224-183">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="d2224-183">deviceConfigurationUserOverview</span></span>](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md)|<span data-ttu-id="d2224-184">设备配置用户状态概述 继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d2224-184">Device Configuration users status overview Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d2224-185">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="d2224-185">deviceSettingStateSummaries</span></span>|<span data-ttu-id="d2224-186">[settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d2224-186">[settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="d2224-187">设备配置设置状态设备摘要 继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d2224-187">Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d2224-188">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d2224-188">JSON Representation</span></span>
<span data-ttu-id="d2224-189">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d2224-189">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosCustomConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosCustomConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "payloadName": "String",
  "payloadFileName": "String",
  "payload": "binary"
}
```


