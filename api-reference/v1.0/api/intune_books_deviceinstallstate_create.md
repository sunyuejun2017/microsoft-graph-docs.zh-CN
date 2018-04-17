# <a name="create-deviceinstallstate"></a><span data-ttu-id="379b1-101">创建 deviceInstallState</span><span class="sxs-lookup"><span data-stu-id="379b1-101">Create deviceInstallState</span></span>

> <span data-ttu-id="379b1-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="379b1-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="379b1-103">创建新的 [deviceInstallState](../resources/intune_books_deviceinstallstate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="379b1-103">Create a new [plannerBucket](../resources/intune_books_deviceinstallstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="379b1-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="379b1-104">Prerequisites</span></span>
<span data-ttu-id="379b1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="379b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="379b1-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="379b1-107">Permission type</span></span>|<span data-ttu-id="379b1-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="379b1-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="379b1-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="379b1-109">Delegated (work or school account)</span></span>|<span data-ttu-id="379b1-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="379b1-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="379b1-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="379b1-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="379b1-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="379b1-112">Not supported.</span></span>|
|<span data-ttu-id="379b1-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="379b1-113">Application</span></span>|<span data-ttu-id="379b1-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="379b1-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="379b1-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="379b1-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates
POST /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}/deviceStates
```

## <a name="request-headers"></a><span data-ttu-id="379b1-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="379b1-116">Request headers</span></span>
|<span data-ttu-id="379b1-117">标头</span><span class="sxs-lookup"><span data-stu-id="379b1-117">Header</span></span>|<span data-ttu-id="379b1-118">值</span><span class="sxs-lookup"><span data-stu-id="379b1-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="379b1-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="379b1-119">Authorization</span></span>|<span data-ttu-id="379b1-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="379b1-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="379b1-121">Accept</span><span class="sxs-lookup"><span data-stu-id="379b1-121">Accept</span></span>|<span data-ttu-id="379b1-122">application/json</span><span class="sxs-lookup"><span data-stu-id="379b1-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="379b1-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="379b1-123">Request body</span></span>
<span data-ttu-id="379b1-124">在请求正文中，提供 deviceInstallState 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="379b1-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="379b1-125">下表显示创建 deviceInstallState 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="379b1-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="379b1-126">属性</span><span class="sxs-lookup"><span data-stu-id="379b1-126">Property</span></span>|<span data-ttu-id="379b1-127">类型</span><span class="sxs-lookup"><span data-stu-id="379b1-127">Type</span></span>|<span data-ttu-id="379b1-128">说明</span><span class="sxs-lookup"><span data-stu-id="379b1-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="379b1-129">id</span><span class="sxs-lookup"><span data-stu-id="379b1-129">id</span></span>|<span data-ttu-id="379b1-130">String</span><span class="sxs-lookup"><span data-stu-id="379b1-130">String</span></span>|<span data-ttu-id="379b1-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="379b1-131">Key of the setting.</span></span>|
|<span data-ttu-id="379b1-132">deviceName</span><span class="sxs-lookup"><span data-stu-id="379b1-132">deviceName</span></span>|<span data-ttu-id="379b1-133">String</span><span class="sxs-lookup"><span data-stu-id="379b1-133">String</span></span>|<span data-ttu-id="379b1-134">设备名称。</span><span class="sxs-lookup"><span data-stu-id="379b1-134">Device name.</span></span>|
|<span data-ttu-id="379b1-135">deviceId</span><span class="sxs-lookup"><span data-stu-id="379b1-135">deviceId</span></span>|<span data-ttu-id="379b1-136">String</span><span class="sxs-lookup"><span data-stu-id="379b1-136">String</span></span>|<span data-ttu-id="379b1-137">设备 ID。</span><span class="sxs-lookup"><span data-stu-id="379b1-137">Device Id.</span></span>|
|<span data-ttu-id="379b1-138">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="379b1-138">lastSyncDateTime</span></span>|<span data-ttu-id="379b1-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="379b1-139">DateTimeOffset</span></span>|<span data-ttu-id="379b1-140">上次同步日期和时间。</span><span class="sxs-lookup"><span data-stu-id="379b1-140">Last sync date and time.</span></span>|
|<span data-ttu-id="379b1-141">installState</span><span class="sxs-lookup"><span data-stu-id="379b1-141">installState</span></span>|<span data-ttu-id="379b1-142">String</span><span class="sxs-lookup"><span data-stu-id="379b1-142">String</span></span>|<span data-ttu-id="379b1-143">电子图书的安装状态。</span><span class="sxs-lookup"><span data-stu-id="379b1-143">The install state of the eBook.</span></span> <span data-ttu-id="379b1-144">可取值为：`notApplicable`、`installed`、`failed`、`notInstalled`、`uninstallFailed`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="379b1-144">Possible values are: `notApplicable`, `installed`, `failed`, `notInstalled`, `uninstallFailed`, `unknown`.</span></span>|
|<span data-ttu-id="379b1-145">errorCode</span><span class="sxs-lookup"><span data-stu-id="379b1-145">errorCode</span></span>|<span data-ttu-id="379b1-146">String</span><span class="sxs-lookup"><span data-stu-id="379b1-146">String</span></span>|<span data-ttu-id="379b1-147">安装失败的错误代码。</span><span class="sxs-lookup"><span data-stu-id="379b1-147">The error code for install failures.</span></span>|
|<span data-ttu-id="379b1-148">osVersion</span><span class="sxs-lookup"><span data-stu-id="379b1-148">osVersion</span></span>|<span data-ttu-id="379b1-149">String</span><span class="sxs-lookup"><span data-stu-id="379b1-149">String</span></span>|<span data-ttu-id="379b1-150">操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="379b1-150">OS Version.</span></span>|
|<span data-ttu-id="379b1-151">osDescription</span><span class="sxs-lookup"><span data-stu-id="379b1-151">osDescription</span></span>|<span data-ttu-id="379b1-152">String</span><span class="sxs-lookup"><span data-stu-id="379b1-152">String</span></span>|<span data-ttu-id="379b1-153">操作系统说明。</span><span class="sxs-lookup"><span data-stu-id="379b1-153">OS Description.</span></span>|
|<span data-ttu-id="379b1-154">userName</span><span class="sxs-lookup"><span data-stu-id="379b1-154">UserName</span></span>|<span data-ttu-id="379b1-155">String</span><span class="sxs-lookup"><span data-stu-id="379b1-155">String</span></span>|<span data-ttu-id="379b1-156">设备用户名。</span><span class="sxs-lookup"><span data-stu-id="379b1-156">Device User Name.</span></span>|



## <a name="response"></a><span data-ttu-id="379b1-157">响应</span><span class="sxs-lookup"><span data-stu-id="379b1-157">Response</span></span>
<span data-ttu-id="379b1-158">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [deviceInstallState](../resources/intune_books_deviceinstallstate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="379b1-158">If successful, this method returns a `201 Created` response code and a [ListItemVersion](../resources/intune_books_deviceinstallstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="379b1-159">示例</span><span class="sxs-lookup"><span data-stu-id="379b1-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="379b1-160">请求</span><span class="sxs-lookup"><span data-stu-id="379b1-160">Request</span></span>
<span data-ttu-id="379b1-161">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="379b1-161">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates
Content-type: application/json
Content-length: 374

{
  "@odata.type": "#microsoft.graph.deviceInstallState",
  "deviceName": "Device Name value",
  "deviceId": "Device Id value",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "installState": "installed",
  "errorCode": "Error Code value",
  "osVersion": "Os Version value",
  "osDescription": "Os Description value",
  "userName": "User Name value"
}
```

### <a name="response"></a><span data-ttu-id="379b1-162">响应</span><span class="sxs-lookup"><span data-stu-id="379b1-162">Response</span></span>
<span data-ttu-id="379b1-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="379b1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 423

{
  "@odata.type": "#microsoft.graph.deviceInstallState",
  "id": "b9feb68f-b68f-b9fe-8fb6-feb98fb6feb9",
  "deviceName": "Device Name value",
  "deviceId": "Device Id value",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "installState": "installed",
  "errorCode": "Error Code value",
  "osVersion": "Os Version value",
  "osDescription": "Os Description value",
  "userName": "User Name value"
}
```


