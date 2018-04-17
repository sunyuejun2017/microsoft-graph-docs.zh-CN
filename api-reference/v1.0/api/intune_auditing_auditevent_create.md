# <a name="create-auditevent"></a><span data-ttu-id="5a2b8-101">创建 auditEvent</span><span class="sxs-lookup"><span data-stu-id="5a2b8-101">Create auditEvent</span></span>

> <span data-ttu-id="5a2b8-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="5a2b8-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5a2b8-103">创建新的 [auditEvent](../resources/intune_auditing_auditevent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5a2b8-103">Create a new [plannerBucket](../resources/intune_auditing_auditevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5a2b8-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="5a2b8-104">Prerequisites</span></span>
<span data-ttu-id="5a2b8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="5a2b8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5a2b8-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="5a2b8-107">Permission type</span></span>|<span data-ttu-id="5a2b8-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="5a2b8-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5a2b8-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5a2b8-109">Delegated (work or school account)</span></span>|<span data-ttu-id="5a2b8-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a2b8-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5a2b8-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5a2b8-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5a2b8-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="5a2b8-112">Not supported.</span></span>|
|<span data-ttu-id="5a2b8-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="5a2b8-113">Application</span></span>|<span data-ttu-id="5a2b8-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="5a2b8-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5a2b8-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5a2b8-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/auditEvents
```

## <a name="request-headers"></a><span data-ttu-id="5a2b8-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="5a2b8-116">Request headers</span></span>
|<span data-ttu-id="5a2b8-117">标头</span><span class="sxs-lookup"><span data-stu-id="5a2b8-117">Header</span></span>|<span data-ttu-id="5a2b8-118">值</span><span class="sxs-lookup"><span data-stu-id="5a2b8-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5a2b8-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="5a2b8-119">Authorization</span></span>|<span data-ttu-id="5a2b8-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="5a2b8-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="5a2b8-121">Accept</span><span class="sxs-lookup"><span data-stu-id="5a2b8-121">Accept</span></span>|<span data-ttu-id="5a2b8-122">application/json</span><span class="sxs-lookup"><span data-stu-id="5a2b8-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5a2b8-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="5a2b8-123">Request body</span></span>
<span data-ttu-id="5a2b8-124">在请求正文中，提供 auditEvent 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5a2b8-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="5a2b8-125">下表显示了创建 auditEvent 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="5a2b8-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="5a2b8-126">属性</span><span class="sxs-lookup"><span data-stu-id="5a2b8-126">Property</span></span>|<span data-ttu-id="5a2b8-127">类型</span><span class="sxs-lookup"><span data-stu-id="5a2b8-127">Type</span></span>|<span data-ttu-id="5a2b8-128">说明</span><span class="sxs-lookup"><span data-stu-id="5a2b8-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5a2b8-129">id</span><span class="sxs-lookup"><span data-stu-id="5a2b8-129">id</span></span>|<span data-ttu-id="5a2b8-130">String</span><span class="sxs-lookup"><span data-stu-id="5a2b8-130">String</span></span>|<span data-ttu-id="5a2b8-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="5a2b8-131">Key of the setting.</span></span>|
|<span data-ttu-id="5a2b8-132">displayName</span><span class="sxs-lookup"><span data-stu-id="5a2b8-132">displayName</span></span>|<span data-ttu-id="5a2b8-133">String</span><span class="sxs-lookup"><span data-stu-id="5a2b8-133">String</span></span>|<span data-ttu-id="5a2b8-134">事件显示名称。</span><span class="sxs-lookup"><span data-stu-id="5a2b8-134">Event display name.</span></span>|
|<span data-ttu-id="5a2b8-135">componentName</span><span class="sxs-lookup"><span data-stu-id="5a2b8-135">--componentName</span></span>|<span data-ttu-id="5a2b8-136">String</span><span class="sxs-lookup"><span data-stu-id="5a2b8-136">String</span></span>|<span data-ttu-id="5a2b8-137">组件名称。</span><span class="sxs-lookup"><span data-stu-id="5a2b8-137">Component name.</span></span>|
|<span data-ttu-id="5a2b8-138">actor</span><span class="sxs-lookup"><span data-stu-id="5a2b8-138">actor</span></span>|[<span data-ttu-id="5a2b8-139">auditActor</span><span class="sxs-lookup"><span data-stu-id="5a2b8-139">auditActor</span></span>](../resources/intune_auditing_auditactor.md)|<span data-ttu-id="5a2b8-140">与审核事件关联的 AAD 用户和应用程序。</span><span class="sxs-lookup"><span data-stu-id="5a2b8-140">AAD user and application that are associated with the audit event.</span></span>|
|<span data-ttu-id="5a2b8-141">activity</span><span class="sxs-lookup"><span data-stu-id="5a2b8-141">activity</span></span>|<span data-ttu-id="5a2b8-142">String</span><span class="sxs-lookup"><span data-stu-id="5a2b8-142">String</span></span>|<span data-ttu-id="5a2b8-143">活动的友好名称。</span><span class="sxs-lookup"><span data-stu-id="5a2b8-143">Friendly name of the activity.</span></span>|
|<span data-ttu-id="5a2b8-144">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="5a2b8-144">activityDateTime</span></span>|<span data-ttu-id="5a2b8-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5a2b8-145">DateTimeOffset</span></span>|<span data-ttu-id="5a2b8-146">执行活动时的日期时间（UTC 时间）。</span><span class="sxs-lookup"><span data-stu-id="5a2b8-146">The date time in UTC when the activity was performed.</span></span>|
|<span data-ttu-id="5a2b8-147">activityType</span><span class="sxs-lookup"><span data-stu-id="5a2b8-147">activityType</span></span>|<span data-ttu-id="5a2b8-148">String</span><span class="sxs-lookup"><span data-stu-id="5a2b8-148">String</span></span>|<span data-ttu-id="5a2b8-149">执行的活动类型。</span><span class="sxs-lookup"><span data-stu-id="5a2b8-149">The type of activity that was being performed.</span></span>|
|<span data-ttu-id="5a2b8-150">activityOperationType</span><span class="sxs-lookup"><span data-stu-id="5a2b8-150">activityOperationType</span></span>|<span data-ttu-id="5a2b8-151">String</span><span class="sxs-lookup"><span data-stu-id="5a2b8-151">String</span></span>|<span data-ttu-id="5a2b8-152">活动的 HTTP 操作类型。</span><span class="sxs-lookup"><span data-stu-id="5a2b8-152">The HTTP operation type of the activity.</span></span>|
|<span data-ttu-id="5a2b8-153">activityResult</span><span class="sxs-lookup"><span data-stu-id="5a2b8-153">activityResult</span></span>|<span data-ttu-id="5a2b8-154">String</span><span class="sxs-lookup"><span data-stu-id="5a2b8-154">String</span></span>|<span data-ttu-id="5a2b8-155">活动结果。</span><span class="sxs-lookup"><span data-stu-id="5a2b8-155">The result of the submission.</span></span>|
|<span data-ttu-id="5a2b8-156">correlationId</span><span class="sxs-lookup"><span data-stu-id="5a2b8-156">correlationId</span></span>|<span data-ttu-id="5a2b8-157">Guid</span><span class="sxs-lookup"><span data-stu-id="5a2b8-157">Guid</span></span>|<span data-ttu-id="5a2b8-158">用于关联系统内的活动的客户端请求 ID。</span><span class="sxs-lookup"><span data-stu-id="5a2b8-158">The client request Id that is used to correlate activity within the system.</span></span>|
|<span data-ttu-id="5a2b8-159">resources</span><span class="sxs-lookup"><span data-stu-id="5a2b8-159">resources</span></span>|<span data-ttu-id="5a2b8-160">[auditResource](../resources/intune_auditing_auditresource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5a2b8-160">[auditResource](../resources/intune_auditing_auditresource.md) collection</span></span>|<span data-ttu-id="5a2b8-161">正在修改的资源。</span><span class="sxs-lookup"><span data-stu-id="5a2b8-161">Resources being modified.</span></span>|
|<span data-ttu-id="5a2b8-162">category</span><span class="sxs-lookup"><span data-stu-id="5a2b8-162">category</span></span>|<span data-ttu-id="5a2b8-163">String</span><span class="sxs-lookup"><span data-stu-id="5a2b8-163">String</span></span>|<span data-ttu-id="5a2b8-164">审核类别。</span><span class="sxs-lookup"><span data-stu-id="5a2b8-164">Audit category.</span></span>|



## <a name="response"></a><span data-ttu-id="5a2b8-165">响应</span><span class="sxs-lookup"><span data-stu-id="5a2b8-165">Response</span></span>
<span data-ttu-id="5a2b8-166">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [auditEvent](../resources/intune_auditing_auditevent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5a2b8-166">If successful, this method returns a `201 Created` response code and a [DriveItemVersion](../resources/intune_auditing_auditevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5a2b8-167">示例</span><span class="sxs-lookup"><span data-stu-id="5a2b8-167">Example</span></span>
### <a name="request"></a><span data-ttu-id="5a2b8-168">请求</span><span class="sxs-lookup"><span data-stu-id="5a2b8-168">Request</span></span>
<span data-ttu-id="5a2b8-169">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5a2b8-169">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/auditEvents
Content-type: application/json
Content-length: 1444

{
  "@odata.type": "#microsoft.graph.auditEvent",
  "displayName": "Display Name value",
  "componentName": "Component Name value",
  "actor": {
    "@odata.type": "microsoft.graph.auditActor",
    "type": "Type value",
    "permissions": [
      "Permissions value"
    ],
    "userPermissions": [
      "User Permissions value"
    ],
    "applicationId": "Application Id value",
    "applicationDisplayName": "Application Display Name value",
    "userPrincipalName": "User Principal Name value",
    "servicePrincipalName": "Service Principal Name value",
    "ipAddress": "Ip Address value",
    "userId": "User Id value"
  },
  "activity": "Activity value",
  "activityDateTime": "2016-12-31T23:59:51.6363086-08:00",
  "activityType": "Activity Type value",
  "activityOperationType": "Activity Operation Type value",
  "activityResult": "Activity Result value",
  "correlationId": "<Unknown Primitive Type Edm.Guid>",
  "resources": [
    {
      "@odata.type": "microsoft.graph.auditResource",
      "displayName": "Display Name value",
      "modifiedProperties": [
        {
          "@odata.type": "microsoft.graph.auditProperty",
          "displayName": "Display Name value",
          "oldValue": "Old Value value",
          "newValue": "New Value value"
        }
      ],
      "type": "Type value",
      "resourceId": "Resource Id value"
    }
  ],
  "category": "Category value"
}
```

### <a name="response"></a><span data-ttu-id="5a2b8-170">响应</span><span class="sxs-lookup"><span data-stu-id="5a2b8-170">Response</span></span>
<span data-ttu-id="5a2b8-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5a2b8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1493

{
  "@odata.type": "#microsoft.graph.auditEvent",
  "id": "59653ce8-3ce8-5965-e83c-6559e83c6559",
  "displayName": "Display Name value",
  "componentName": "Component Name value",
  "actor": {
    "@odata.type": "microsoft.graph.auditActor",
    "type": "Type value",
    "permissions": [
      "Permissions value"
    ],
    "userPermissions": [
      "User Permissions value"
    ],
    "applicationId": "Application Id value",
    "applicationDisplayName": "Application Display Name value",
    "userPrincipalName": "User Principal Name value",
    "servicePrincipalName": "Service Principal Name value",
    "ipAddress": "Ip Address value",
    "userId": "User Id value"
  },
  "activity": "Activity value",
  "activityDateTime": "2016-12-31T23:59:51.6363086-08:00",
  "activityType": "Activity Type value",
  "activityOperationType": "Activity Operation Type value",
  "activityResult": "Activity Result value",
  "correlationId": "<Unknown Primitive Type Edm.Guid>",
  "resources": [
    {
      "@odata.type": "microsoft.graph.auditResource",
      "displayName": "Display Name value",
      "modifiedProperties": [
        {
          "@odata.type": "microsoft.graph.auditProperty",
          "displayName": "Display Name value",
          "oldValue": "Old Value value",
          "newValue": "New Value value"
        }
      ],
      "type": "Type value",
      "resourceId": "Resource Id value"
    }
  ],
  "category": "Category value"
}
```


