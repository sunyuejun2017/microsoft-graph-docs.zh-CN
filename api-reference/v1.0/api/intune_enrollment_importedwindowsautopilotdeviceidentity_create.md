# <a name="create-importedwindowsautopilotdeviceidentity"></a><span data-ttu-id="7f588-101">创建 importedWindowsAutopilotDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="7f588-101">Create importedWindowsAutopilotDeviceIdentity</span></span>

> <span data-ttu-id="7f588-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="7f588-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7f588-103">创建新的 [importedWindowsAutopilotDeviceIdentity](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7f588-103">Create a new [managedMobileApp](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7f588-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="7f588-104">Prerequisites</span></span>
<span data-ttu-id="7f588-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="7f588-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="7f588-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="7f588-107">Permission type</span></span>|<span data-ttu-id="7f588-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="7f588-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7f588-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7f588-109">Delegated (work or school account)</span></span>|<span data-ttu-id="7f588-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f588-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="7f588-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7f588-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7f588-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="7f588-112">Not supported.</span></span>|
|<span data-ttu-id="7f588-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="7f588-113">Application</span></span>|<span data-ttu-id="7f588-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="7f588-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7f588-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7f588-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedWindowsAutopilotDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="7f588-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="7f588-116">Request headers</span></span>
|<span data-ttu-id="7f588-117">标头</span><span class="sxs-lookup"><span data-stu-id="7f588-117">Header</span></span>|<span data-ttu-id="7f588-118">值</span><span class="sxs-lookup"><span data-stu-id="7f588-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7f588-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="7f588-119">Authorization</span></span>|<span data-ttu-id="7f588-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7f588-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7f588-121">Accept</span><span class="sxs-lookup"><span data-stu-id="7f588-121">Accept</span></span>|<span data-ttu-id="7f588-122">application/json</span><span class="sxs-lookup"><span data-stu-id="7f588-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7f588-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="7f588-123">Request body</span></span>
<span data-ttu-id="7f588-124">在请求正文中，提供 importedWindowsAutopilotDeviceIdentity 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7f588-124">In the request body, supply a JSON representation for the windows10GeneralConfiguration object.</span></span>

<span data-ttu-id="7f588-125">下表显示创建 importedWindowsAutopilotDeviceIdentity 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="7f588-125">The following table shows the properties that are required when you create the iosUpdateDeviceStatus.</span></span>

|<span data-ttu-id="7f588-126">属性</span><span class="sxs-lookup"><span data-stu-id="7f588-126">Property</span></span>|<span data-ttu-id="7f588-127">类型</span><span class="sxs-lookup"><span data-stu-id="7f588-127">Type</span></span>|<span data-ttu-id="7f588-128">说明</span><span class="sxs-lookup"><span data-stu-id="7f588-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f588-129">id</span><span class="sxs-lookup"><span data-stu-id="7f588-129">id</span></span>|<span data-ttu-id="7f588-130">String</span><span class="sxs-lookup"><span data-stu-id="7f588-130">String</span></span>|<span data-ttu-id="7f588-131">对象的 GUID</span><span class="sxs-lookup"><span data-stu-id="7f588-131">The GUID for the object.</span></span>|
|<span data-ttu-id="7f588-132">orderIdentifier</span><span class="sxs-lookup"><span data-stu-id="7f588-132">orderIdentifier</span></span>|<span data-ttu-id="7f588-133">String</span><span class="sxs-lookup"><span data-stu-id="7f588-133">String</span></span>|<span data-ttu-id="7f588-134">Windows AutoPilot 设备的订单编码。</span><span class="sxs-lookup"><span data-stu-id="7f588-134">Order Id of the Windows autopilot device.</span></span>|
|<span data-ttu-id="7f588-135">serialNumber</span><span class="sxs-lookup"><span data-stu-id="7f588-135">serialNumber</span></span>|<span data-ttu-id="7f588-136">String</span><span class="sxs-lookup"><span data-stu-id="7f588-136">String</span></span>|<span data-ttu-id="7f588-137">Windows AutoPilot 设备的序列号。</span><span class="sxs-lookup"><span data-stu-id="7f588-137">Serial number of the Windows autopilot device.</span></span>|
|<span data-ttu-id="7f588-138">productKey</span><span class="sxs-lookup"><span data-stu-id="7f588-138">productKey</span></span>|<span data-ttu-id="7f588-139">String</span><span class="sxs-lookup"><span data-stu-id="7f588-139">String</span></span>|<span data-ttu-id="7f588-140">Windows AutoPilot 设备的产品密钥。</span><span class="sxs-lookup"><span data-stu-id="7f588-140">Product Key of the Windows autopilot device.</span></span>|
|<span data-ttu-id="7f588-141">hardwareIdentifier</span><span class="sxs-lookup"><span data-stu-id="7f588-141">hardwareIdentifier</span></span>|<span data-ttu-id="7f588-142">Binary</span><span class="sxs-lookup"><span data-stu-id="7f588-142">Binary</span></span>|<span data-ttu-id="7f588-143">Windows AutoPilot 设备的硬件 Blob。</span><span class="sxs-lookup"><span data-stu-id="7f588-143">Hardware Blob of the Windows autopilot device.</span></span>|
|<span data-ttu-id="7f588-144">state</span><span class="sxs-lookup"><span data-stu-id="7f588-144">state</span></span>|[<span data-ttu-id="7f588-145">importedWindowsAutopilotDeviceIdentityState</span><span class="sxs-lookup"><span data-stu-id="7f588-145">importedWindowsAutopilotDeviceIdentityState</span></span>](../resources/intune_enrollment_importedwindowsautopilotdeviceidentitystate.md)|<span data-ttu-id="7f588-146">导入设备的当前状态。</span><span class="sxs-lookup"><span data-stu-id="7f588-146">Current state of the imported device.</span></span>|



## <a name="response"></a><span data-ttu-id="7f588-147">响应</span><span class="sxs-lookup"><span data-stu-id="7f588-147">Response</span></span>
<span data-ttu-id="7f588-148">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [importedWindowsAutopilotDeviceIdentity](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7f588-148">If successful, this method returns a `201 Created` response code and a [windowsPhone81CompliancePolicy](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7f588-149">示例</span><span class="sxs-lookup"><span data-stu-id="7f588-149">Example</span></span>
### <a name="request"></a><span data-ttu-id="7f588-150">请求</span><span class="sxs-lookup"><span data-stu-id="7f588-150">Request</span></span>
<span data-ttu-id="7f588-151">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7f588-151">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/importedWindowsAutopilotDeviceIdentities
Content-type: application/json
Content-length: 541

{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentity",
  "orderIdentifier": "Order Identifier value",
  "serialNumber": "Serial Number value",
  "productKey": "Product Key value",
  "hardwareIdentifier": "aGFyZHdhcmVJZGVudGlmaWVy",
  "state": {
    "@odata.type": "microsoft.graph.importedWindowsAutopilotDeviceIdentityState",
    "deviceImportStatus": "pending",
    "deviceRegistrationId": "Device Registration Id value",
    "deviceErrorCode": 15,
    "deviceErrorName": "Device Error Name value"
  }
}
```

### <a name="response"></a><span data-ttu-id="7f588-152">响应</span><span class="sxs-lookup"><span data-stu-id="7f588-152">Response</span></span>
<span data-ttu-id="7f588-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7f588-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 590

{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentity",
  "id": "985b4f49-4f49-985b-494f-5b98494f5b98",
  "orderIdentifier": "Order Identifier value",
  "serialNumber": "Serial Number value",
  "productKey": "Product Key value",
  "hardwareIdentifier": "aGFyZHdhcmVJZGVudGlmaWVy",
  "state": {
    "@odata.type": "microsoft.graph.importedWindowsAutopilotDeviceIdentityState",
    "deviceImportStatus": "pending",
    "deviceRegistrationId": "Device Registration Id value",
    "deviceErrorCode": 15,
    "deviceErrorName": "Device Error Name value"
  }
}
```


