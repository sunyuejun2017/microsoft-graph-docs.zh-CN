# <a name="list-managedappoperations"></a><span data-ttu-id="aeacc-101">列出 managedAppOperations</span><span class="sxs-lookup"><span data-stu-id="aeacc-101">List managedAppOperations</span></span>

> <span data-ttu-id="aeacc-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="aeacc-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="aeacc-103">列出 [managedAppOperation](../resources/intune_mam_managedappoperation.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="aeacc-103">List properties and relationships of the [managedAppOperation](../resources/intune_mam_managedappoperation.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="aeacc-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="aeacc-104">Prerequisites</span></span>
<span data-ttu-id="aeacc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="aeacc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="aeacc-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="aeacc-107">Permission type</span></span>|<span data-ttu-id="aeacc-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="aeacc-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aeacc-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="aeacc-109">Delegated (work or school account)</span></span>|<span data-ttu-id="aeacc-110">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="aeacc-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="aeacc-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="aeacc-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aeacc-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="aeacc-112">Not supported.</span></span>|
|<span data-ttu-id="aeacc-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="aeacc-113">Application</span></span>|<span data-ttu-id="aeacc-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="aeacc-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="aeacc-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="aeacc-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations
```

## <a name="request-headers"></a><span data-ttu-id="aeacc-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="aeacc-116">Request headers</span></span>
|<span data-ttu-id="aeacc-117">标头</span><span class="sxs-lookup"><span data-stu-id="aeacc-117">Header</span></span>|<span data-ttu-id="aeacc-118">值</span><span class="sxs-lookup"><span data-stu-id="aeacc-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aeacc-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="aeacc-119">Authorization</span></span>|<span data-ttu-id="aeacc-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="aeacc-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="aeacc-121">Accept</span><span class="sxs-lookup"><span data-stu-id="aeacc-121">Accept</span></span>|<span data-ttu-id="aeacc-122">application/json</span><span class="sxs-lookup"><span data-stu-id="aeacc-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aeacc-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="aeacc-123">Request body</span></span>
<span data-ttu-id="aeacc-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="aeacc-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aeacc-125">响应</span><span class="sxs-lookup"><span data-stu-id="aeacc-125">Response</span></span>
<span data-ttu-id="aeacc-126">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [managedAppOperation](../resources/intune_mam_managedappoperation.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="aeacc-126">If successful, this method returns a `200 OK` response code and collection of [groupSettingTemplate](../resources/intune_mam_managedappoperation.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aeacc-127">示例</span><span class="sxs-lookup"><span data-stu-id="aeacc-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="aeacc-128">请求</span><span class="sxs-lookup"><span data-stu-id="aeacc-128">Request</span></span>
<span data-ttu-id="aeacc-129">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="aeacc-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations
```

### <a name="response"></a><span data-ttu-id="aeacc-130">响应</span><span class="sxs-lookup"><span data-stu-id="aeacc-130">Response</span></span>
<span data-ttu-id="aeacc-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="aeacc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 329

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedAppOperation",
      "displayName": "Display Name value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "state": "State value",
      "id": "f2867b06-7b06-f286-067b-86f2067b86f2",
      "version": "Version value"
    }
  ]
}
```


