# <a name="windows10secureassessmentconfiguration-resource-type"></a><span data-ttu-id="a8e99-101">windows10SecureAssessmentConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="a8e99-101">windows10SecureAssessmentConfiguration resource type</span></span>

> <span data-ttu-id="a8e99-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="a8e99-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a8e99-103">本主题提供由 secureAssessment 资源公开的已声明方法、属性和关系的说明。</span><span class="sxs-lookup"><span data-stu-id="a8e99-103">This topic provides descriptions of the declared methods, properties and relationships exposed by the secureAssessment resource.</span></span>

<span data-ttu-id="a8e99-104">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a8e99-104">Inherits from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="a8e99-105">方法</span><span class="sxs-lookup"><span data-stu-id="a8e99-105">Methods</span></span>
|<span data-ttu-id="a8e99-106">方法</span><span class="sxs-lookup"><span data-stu-id="a8e99-106">Method</span></span>|<span data-ttu-id="a8e99-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="a8e99-107">Return Type</span></span>|<span data-ttu-id="a8e99-108">说明</span><span class="sxs-lookup"><span data-stu-id="a8e99-108">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a8e99-109">List windows10SecureAssessmentConfigurations</span><span class="sxs-lookup"><span data-stu-id="a8e99-109">List windows10SecureAssessmentConfigurations</span></span>](../api/intune_deviceconfig_windows10secureassessmentconfiguration_list.md)|<span data-ttu-id="a8e99-110">[windows10SecureAssessmentConfiguration](../resources/intune_deviceconfig_windows10secureassessmentconfiguration.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a8e99-110">[windows10SecureAssessmentConfiguration](../resources/intune_deviceconfig_windows10secureassessmentconfiguration.md) collection</span></span>|<span data-ttu-id="a8e99-111">列出 [windows10SecureAssessmentConfiguration](../resources/intune_deviceconfig_windows10secureassessmentconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a8e99-111">List properties and relationships of the [windows10SecureAssessmentConfiguration](../resources/intune_deviceconfig_windows10secureassessmentconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="a8e99-112">Get windows10SecureAssessmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="a8e99-112">Get windows10SecureAssessmentConfiguration</span></span>](../api/intune_deviceconfig_windows10secureassessmentconfiguration_get.md)|[<span data-ttu-id="a8e99-113">windows10SecureAssessmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="a8e99-113">windows10SecureAssessmentConfiguration</span></span>](../resources/intune_deviceconfig_windows10secureassessmentconfiguration.md)|<span data-ttu-id="a8e99-114">读取 [windows10SecureAssessmentConfiguration](../resources/intune_deviceconfig_windows10secureassessmentconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a8e99-114">Read properties and relationships of [plannerTaskDetails](../resources/intune_deviceconfig_windows10secureassessmentconfiguration.md) object.</span></span>|
|[<span data-ttu-id="a8e99-115">Create windows10SecureAssessmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="a8e99-115">Create windows10SecureAssessmentConfiguration</span></span>](../api/intune_deviceconfig_windows10secureassessmentconfiguration_create.md)|[<span data-ttu-id="a8e99-116">windows10SecureAssessmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="a8e99-116">windows10SecureAssessmentConfiguration</span></span>](../resources/intune_deviceconfig_windows10secureassessmentconfiguration.md)|<span data-ttu-id="a8e99-117">创建新的 [windows10SecureAssessmentConfiguration](../resources/intune_deviceconfig_windows10secureassessmentconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a8e99-117">Create a new [plannerBucket](../resources/intune_deviceconfig_windows10secureassessmentconfiguration.md) object.</span></span>|
|[<span data-ttu-id="a8e99-118">Delete windows10SecureAssessmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="a8e99-118">Delete windows10SecureAssessmentConfiguration</span></span>](../api/intune_deviceconfig_windows10secureassessmentconfiguration_delete.md)|<span data-ttu-id="a8e99-119">无</span><span class="sxs-lookup"><span data-stu-id="a8e99-119">None</span></span>|<span data-ttu-id="a8e99-120">删除 [windows10SecureAssessmentConfiguration](../resources/intune_deviceconfig_windows10secureassessmentconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="a8e99-120">Deletes a [windows10SecureAssessmentConfiguration](../resources/intune_deviceconfig_windows10secureassessmentconfiguration.md).</span></span>|
|[<span data-ttu-id="a8e99-121">Update windows10SecureAssessmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="a8e99-121">Update windows10SecureAssessmentConfiguration</span></span>](../api/intune_deviceconfig_windows10secureassessmentconfiguration_update.md)|[<span data-ttu-id="a8e99-122">windows10SecureAssessmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="a8e99-122">windows10SecureAssessmentConfiguration</span></span>](../resources/intune_deviceconfig_windows10secureassessmentconfiguration.md)|<span data-ttu-id="a8e99-123">更新 [windows10SecureAssessmentConfiguration](../resources/intune_deviceconfig_windows10secureassessmentconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a8e99-123">Update the properties of a [calendar](../resources/intune_deviceconfig_windows10secureassessmentconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a8e99-124">属性</span><span class="sxs-lookup"><span data-stu-id="a8e99-124">Properties</span></span>
|<span data-ttu-id="a8e99-125">属性</span><span class="sxs-lookup"><span data-stu-id="a8e99-125">Property</span></span>|<span data-ttu-id="a8e99-126">类型</span><span class="sxs-lookup"><span data-stu-id="a8e99-126">Type</span></span>|<span data-ttu-id="a8e99-127">说明</span><span class="sxs-lookup"><span data-stu-id="a8e99-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8e99-128">id</span><span class="sxs-lookup"><span data-stu-id="a8e99-128">id</span></span>|<span data-ttu-id="a8e99-129">String</span><span class="sxs-lookup"><span data-stu-id="a8e99-129">String</span></span>|<span data-ttu-id="a8e99-130">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a8e99-130">Key of the setting.</span></span> <span data-ttu-id="a8e99-131">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a8e99-131">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a8e99-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a8e99-132">lastModifiedDateTime</span></span>|<span data-ttu-id="a8e99-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a8e99-133">DateTimeOffset</span></span>|<span data-ttu-id="a8e99-134">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="a8e99-134">Indicates the date the object was last modified.</span></span> <span data-ttu-id="a8e99-135">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a8e99-135">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a8e99-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a8e99-136">createdDateTime</span></span>|<span data-ttu-id="a8e99-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a8e99-137">DateTimeOffset</span></span>|<span data-ttu-id="a8e99-138">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="a8e99-138">DateTime the object was created.</span></span> <span data-ttu-id="a8e99-139">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a8e99-139">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a8e99-140">description</span><span class="sxs-lookup"><span data-stu-id="a8e99-140">description</span></span>|<span data-ttu-id="a8e99-141">String</span><span class="sxs-lookup"><span data-stu-id="a8e99-141">String</span></span>|<span data-ttu-id="a8e99-142">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="a8e99-142">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a8e99-143">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a8e99-143">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a8e99-144">displayName</span><span class="sxs-lookup"><span data-stu-id="a8e99-144">displayName</span></span>|<span data-ttu-id="a8e99-145">String</span><span class="sxs-lookup"><span data-stu-id="a8e99-145">String</span></span>|<span data-ttu-id="a8e99-146">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="a8e99-146">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a8e99-147">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a8e99-147">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a8e99-148">version</span><span class="sxs-lookup"><span data-stu-id="a8e99-148">version</span></span>|<span data-ttu-id="a8e99-149">Int32</span><span class="sxs-lookup"><span data-stu-id="a8e99-149">Int32</span></span>|<span data-ttu-id="a8e99-150">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="a8e99-150">Version of the device configuration.</span></span> <span data-ttu-id="a8e99-151">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a8e99-151">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a8e99-152">launchUri</span><span class="sxs-lookup"><span data-stu-id="a8e99-152">launchUri</span></span>|<span data-ttu-id="a8e99-153">String</span><span class="sxs-lookup"><span data-stu-id="a8e99-153">String</span></span>|<span data-ttu-id="a8e99-154">启动安全评估浏览器时指向自动加载的评估的 Url 链接。</span><span class="sxs-lookup"><span data-stu-id="a8e99-154">Url link to an assessment that's automatically loaded when the secure assessment browser is launched.</span></span> <span data-ttu-id="a8e99-155">它必须是有效的 Url (http\[s\]://msdn.microsoft.com/)。</span><span class="sxs-lookup"><span data-stu-id="a8e99-155">It has to be a valid Url (http\[s\]://msdn.microsoft.com/).</span></span>|
|<span data-ttu-id="a8e99-156">configurationAccount</span><span class="sxs-lookup"><span data-stu-id="a8e99-156">configurationAccount</span></span>|<span data-ttu-id="a8e99-157">String</span><span class="sxs-lookup"><span data-stu-id="a8e99-157">String</span></span>|<span data-ttu-id="a8e99-158">用于配置 Windows 设备进行测试的帐户。</span><span class="sxs-lookup"><span data-stu-id="a8e99-158">The account used to configure the Windows device for taking the test.</span></span> <span data-ttu-id="a8e99-159">用户可以是域帐户（域\用户）、AAD 帐户 (username@tenant.com) 或本地帐户（用户名）。</span><span class="sxs-lookup"><span data-stu-id="a8e99-159">The user can be a domain account (domain\user), an AAD account (username@tenant.com) or a local account (username).</span></span>|
|<span data-ttu-id="a8e99-160">allowPrinting</span><span class="sxs-lookup"><span data-stu-id="a8e99-160">allowPrinting</span></span>|<span data-ttu-id="a8e99-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="a8e99-161">Boolean</span></span>|<span data-ttu-id="a8e99-162">指示在测试期间是否允许应用打印。</span><span class="sxs-lookup"><span data-stu-id="a8e99-162">Indicates whether or not to allow the app from printing during the test.</span></span>|
|<span data-ttu-id="a8e99-163">allowScreenCapture</span><span class="sxs-lookup"><span data-stu-id="a8e99-163">allowScreenCapture</span></span>|<span data-ttu-id="a8e99-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="a8e99-164">Boolean</span></span>|<span data-ttu-id="a8e99-165">指示在测试期间是否允许屏幕捕获功能。</span><span class="sxs-lookup"><span data-stu-id="a8e99-165">Indicates whether or not to allow screen capture capability during a test.</span></span>|
|<span data-ttu-id="a8e99-166">allowTextSuggestion</span><span class="sxs-lookup"><span data-stu-id="a8e99-166">allowTextSuggestion</span></span>|<span data-ttu-id="a8e99-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="a8e99-167">Boolean</span></span>|<span data-ttu-id="a8e99-168">指示在测试期间是否允许文本建议。</span><span class="sxs-lookup"><span data-stu-id="a8e99-168">Indicates whether or not to allow text suggestions during the test.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a8e99-169">关系</span><span class="sxs-lookup"><span data-stu-id="a8e99-169">Relationships</span></span>
|<span data-ttu-id="a8e99-170">关系</span><span class="sxs-lookup"><span data-stu-id="a8e99-170">Relationship</span></span>|<span data-ttu-id="a8e99-171">类型</span><span class="sxs-lookup"><span data-stu-id="a8e99-171">Type</span></span>|<span data-ttu-id="a8e99-172">说明</span><span class="sxs-lookup"><span data-stu-id="a8e99-172">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8e99-173">assignments</span><span class="sxs-lookup"><span data-stu-id="a8e99-173">assignments</span></span>|<span data-ttu-id="a8e99-174">[deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a8e99-174">[deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="a8e99-175">设备配置文件的分配列表。</span><span class="sxs-lookup"><span data-stu-id="a8e99-175">The list of assignments for the device configuration profile.</span></span> <span data-ttu-id="a8e99-176">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a8e99-176">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a8e99-177">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="a8e99-177">deviceStatuses</span></span>|<span data-ttu-id="a8e99-178">[deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a8e99-178">[deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="a8e99-179">按设备的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="a8e99-179">Device configuration installation status by device.</span></span> <span data-ttu-id="a8e99-180">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a8e99-180">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a8e99-181">userStatuses</span><span class="sxs-lookup"><span data-stu-id="a8e99-181">userStatuses</span></span>|<span data-ttu-id="a8e99-182">[deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a8e99-182">[deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="a8e99-183">按用户的设备配置安装状态。</span><span class="sxs-lookup"><span data-stu-id="a8e99-183">Device configuration installation stauts by user.</span></span> <span data-ttu-id="a8e99-184">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a8e99-184">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a8e99-185">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="a8e99-185">deviceStatusOverview</span></span>|[<span data-ttu-id="a8e99-186">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="a8e99-186">deviceConfigurationDeviceOverview</span></span>](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md)|<span data-ttu-id="a8e99-187">设备配置设备状态概述 继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a8e99-187">Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a8e99-188">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="a8e99-188">userStatusOverview</span></span>|[<span data-ttu-id="a8e99-189">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="a8e99-189">deviceConfigurationUserOverview</span></span>](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md)|<span data-ttu-id="a8e99-190">设备配置用户状态概述 继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a8e99-190">Device Configuration users status overview Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a8e99-191">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="a8e99-191">deviceSettingStateSummaries</span></span>|<span data-ttu-id="a8e99-192">[settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a8e99-192">[settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="a8e99-193">设备配置设置状态设备摘要 继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a8e99-193">Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a8e99-194">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a8e99-194">JSON Representation</span></span>
<span data-ttu-id="a8e99-195">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a8e99-195">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windows10SecureAssessmentConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10SecureAssessmentConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "launchUri": "String",
  "configurationAccount": "String",
  "allowPrinting": true,
  "allowScreenCapture": true,
  "allowTextSuggestion": true
}
```


