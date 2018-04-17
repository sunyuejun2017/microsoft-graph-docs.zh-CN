# <a name="update-macoscustomconfiguration"></a><span data-ttu-id="0afcd-101">更新 macOSCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="0afcd-101">Update macOSCustomConfiguration</span></span>

> <span data-ttu-id="0afcd-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="0afcd-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0afcd-103">更新 [macOSCustomConfiguration](../resources/intune_deviceconfig_macoscustomconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="0afcd-103">Update the properties of a [calendar](../resources/intune_deviceconfig_macoscustomconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0afcd-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="0afcd-104">Prerequisites</span></span>
<span data-ttu-id="0afcd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="0afcd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0afcd-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="0afcd-107">Permission type</span></span>|<span data-ttu-id="0afcd-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0afcd-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0afcd-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0afcd-109">Delegated (work or school account)</span></span>|<span data-ttu-id="0afcd-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0afcd-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0afcd-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0afcd-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0afcd-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="0afcd-112">Not supported.</span></span>|
|<span data-ttu-id="0afcd-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="0afcd-113">Application</span></span>|<span data-ttu-id="0afcd-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="0afcd-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0afcd-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0afcd-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="0afcd-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="0afcd-116">Request headers</span></span>
|<span data-ttu-id="0afcd-117">标头</span><span class="sxs-lookup"><span data-stu-id="0afcd-117">Header</span></span>|<span data-ttu-id="0afcd-118">值</span><span class="sxs-lookup"><span data-stu-id="0afcd-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0afcd-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="0afcd-119">Authorization</span></span>|<span data-ttu-id="0afcd-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0afcd-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="0afcd-121">Accept</span><span class="sxs-lookup"><span data-stu-id="0afcd-121">Accept</span></span>|<span data-ttu-id="0afcd-122">application/json</span><span class="sxs-lookup"><span data-stu-id="0afcd-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0afcd-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="0afcd-123">Request body</span></span>
<span data-ttu-id="0afcd-124">在请求正文中，提供 [macOSCustomConfiguration](../resources/intune_deviceconfig_macoscustomconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0afcd-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_deviceconfig_macoscustomconfiguration.md) object.</span></span>

<span data-ttu-id="0afcd-125">下表显示了创建 [macOSCustomConfiguration](../resources/intune_deviceconfig_macoscustomconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="0afcd-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="0afcd-126">属性</span><span class="sxs-lookup"><span data-stu-id="0afcd-126">Property</span></span>|<span data-ttu-id="0afcd-127">类型</span><span class="sxs-lookup"><span data-stu-id="0afcd-127">Type</span></span>|<span data-ttu-id="0afcd-128">说明</span><span class="sxs-lookup"><span data-stu-id="0afcd-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0afcd-129">id</span><span class="sxs-lookup"><span data-stu-id="0afcd-129">id</span></span>|<span data-ttu-id="0afcd-130">String</span><span class="sxs-lookup"><span data-stu-id="0afcd-130">String</span></span>|<span data-ttu-id="0afcd-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="0afcd-131">Key of the setting.</span></span> <span data-ttu-id="0afcd-132">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0afcd-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0afcd-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0afcd-133">lastModifiedDateTime</span></span>|<span data-ttu-id="0afcd-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0afcd-134">DateTimeOffset</span></span>|<span data-ttu-id="0afcd-135">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="0afcd-135">Indicates the date the object was last modified.</span></span> <span data-ttu-id="0afcd-136">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0afcd-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0afcd-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0afcd-137">createdDateTime</span></span>|<span data-ttu-id="0afcd-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0afcd-138">DateTimeOffset</span></span>|<span data-ttu-id="0afcd-139">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="0afcd-139">DateTime the object was created.</span></span> <span data-ttu-id="0afcd-140">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0afcd-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0afcd-141">description</span><span class="sxs-lookup"><span data-stu-id="0afcd-141">description</span></span>|<span data-ttu-id="0afcd-142">String</span><span class="sxs-lookup"><span data-stu-id="0afcd-142">String</span></span>|<span data-ttu-id="0afcd-143">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="0afcd-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0afcd-144">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0afcd-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0afcd-145">displayName</span><span class="sxs-lookup"><span data-stu-id="0afcd-145">displayName</span></span>|<span data-ttu-id="0afcd-146">String</span><span class="sxs-lookup"><span data-stu-id="0afcd-146">String</span></span>|<span data-ttu-id="0afcd-147">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="0afcd-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0afcd-148">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0afcd-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0afcd-149">version</span><span class="sxs-lookup"><span data-stu-id="0afcd-149">version</span></span>|<span data-ttu-id="0afcd-150">Int32</span><span class="sxs-lookup"><span data-stu-id="0afcd-150">Int32</span></span>|<span data-ttu-id="0afcd-151">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="0afcd-151">Version of the device configuration.</span></span> <span data-ttu-id="0afcd-152">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0afcd-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0afcd-153">payloadName</span><span class="sxs-lookup"><span data-stu-id="0afcd-153">payloadName</span></span>|<span data-ttu-id="0afcd-154">String</span><span class="sxs-lookup"><span data-stu-id="0afcd-154">String</span></span>|<span data-ttu-id="0afcd-155">向用户显示的名称。</span><span class="sxs-lookup"><span data-stu-id="0afcd-155">Name that is displayed to the user.</span></span>|
|<span data-ttu-id="0afcd-156">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="0afcd-156">payloadFileName</span></span>|<span data-ttu-id="0afcd-157">String</span><span class="sxs-lookup"><span data-stu-id="0afcd-157">String</span></span>|<span data-ttu-id="0afcd-158">有效负载文件名 (\*.mobileconfig</span><span class="sxs-lookup"><span data-stu-id="0afcd-158">Payload file name (\*.mobileconfig</span></span> | <span data-ttu-id="0afcd-159">\*.xml)。</span><span class="sxs-lookup"><span data-stu-id="0afcd-159">\*.xml</span></span>|
|<span data-ttu-id="0afcd-160">payload</span><span class="sxs-lookup"><span data-stu-id="0afcd-160">Notification payload</span></span>|<span data-ttu-id="0afcd-161">Binary</span><span class="sxs-lookup"><span data-stu-id="0afcd-161">Binary</span></span>|<span data-ttu-id="0afcd-162">有效负载。</span><span class="sxs-lookup"><span data-stu-id="0afcd-162">Payload.</span></span> <span data-ttu-id="0afcd-163">（UTF8 编码的字节数组）</span><span class="sxs-lookup"><span data-stu-id="0afcd-163">(UTF8 encoded byte array)</span></span>|



## <a name="response"></a><span data-ttu-id="0afcd-164">响应</span><span class="sxs-lookup"><span data-stu-id="0afcd-164">Response</span></span>
<span data-ttu-id="0afcd-165">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [macOSCustomConfiguration](../resources/intune_deviceconfig_macoscustomconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0afcd-165">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_deviceconfig_macoscustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0afcd-166">示例</span><span class="sxs-lookup"><span data-stu-id="0afcd-166">Example</span></span>
### <a name="request"></a><span data-ttu-id="0afcd-167">请求</span><span class="sxs-lookup"><span data-stu-id="0afcd-167">Request</span></span>
<span data-ttu-id="0afcd-168">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0afcd-168">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 282

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "payloadName": "Payload Name value",
  "payloadFileName": "Payload File Name value",
  "payload": "cGF5bG9hZA=="
}
```

### <a name="response"></a><span data-ttu-id="0afcd-169">响应</span><span class="sxs-lookup"><span data-stu-id="0afcd-169">Response</span></span>
<span data-ttu-id="0afcd-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0afcd-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 453

{
  "@odata.type": "#microsoft.graph.macOSCustomConfiguration",
  "id": "a253835d-835d-a253-5d83-53a25d8353a2",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "payloadName": "Payload Name value",
  "payloadFileName": "Payload File Name value",
  "payload": "cGF5bG9hZA=="
}
```


