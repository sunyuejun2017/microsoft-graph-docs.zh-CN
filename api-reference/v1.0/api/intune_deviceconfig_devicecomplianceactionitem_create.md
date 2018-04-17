# <a name="create-devicecomplianceactionitem"></a><span data-ttu-id="41ed4-101">创建 deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="41ed4-101">Create deviceComplianceActionItem</span></span>

> <span data-ttu-id="41ed4-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="41ed4-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="41ed4-103">创建新的 [deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="41ed4-103">Create a new [plannerBucket](../resources/intune_deviceconfig_devicecomplianceactionitem.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="41ed4-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="41ed4-104">Prerequisites</span></span>
<span data-ttu-id="41ed4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="41ed4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="41ed4-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="41ed4-107">Permission type</span></span>|<span data-ttu-id="41ed4-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="41ed4-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="41ed4-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="41ed4-109">Delegated (work or school account)</span></span>|<span data-ttu-id="41ed4-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41ed4-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="41ed4-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="41ed4-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="41ed4-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="41ed4-112">Not supported.</span></span>|
|<span data-ttu-id="41ed4-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="41ed4-113">Application</span></span>|<span data-ttu-id="41ed4-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="41ed4-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="41ed4-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="41ed4-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="41ed4-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="41ed4-116">Request headers</span></span>
|<span data-ttu-id="41ed4-117">标头</span><span class="sxs-lookup"><span data-stu-id="41ed4-117">Header</span></span>|<span data-ttu-id="41ed4-118">值</span><span class="sxs-lookup"><span data-stu-id="41ed4-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="41ed4-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="41ed4-119">Authorization</span></span>|<span data-ttu-id="41ed4-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="41ed4-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="41ed4-121">Accept</span><span class="sxs-lookup"><span data-stu-id="41ed4-121">Accept</span></span>|<span data-ttu-id="41ed4-122">application/json</span><span class="sxs-lookup"><span data-stu-id="41ed4-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="41ed4-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="41ed4-123">Request body</span></span>
<span data-ttu-id="41ed4-124">在请求正文中，提供 deviceComplianceActionItem 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="41ed4-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="41ed4-125">下表显示了创建 deviceComplianceActionItem 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="41ed4-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="41ed4-126">属性</span><span class="sxs-lookup"><span data-stu-id="41ed4-126">Property</span></span>|<span data-ttu-id="41ed4-127">类型</span><span class="sxs-lookup"><span data-stu-id="41ed4-127">Type</span></span>|<span data-ttu-id="41ed4-128">说明</span><span class="sxs-lookup"><span data-stu-id="41ed4-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="41ed4-129">id</span><span class="sxs-lookup"><span data-stu-id="41ed4-129">id</span></span>|<span data-ttu-id="41ed4-130">String</span><span class="sxs-lookup"><span data-stu-id="41ed4-130">String</span></span>|<span data-ttu-id="41ed4-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="41ed4-131">Key of the setting.</span></span>|
|<span data-ttu-id="41ed4-132">gracePeriodHours</span><span class="sxs-lookup"><span data-stu-id="41ed4-132">gracePeriodHours</span></span>|<span data-ttu-id="41ed4-133">Int32</span><span class="sxs-lookup"><span data-stu-id="41ed4-133">Int32</span></span>|<span data-ttu-id="41ed4-134">强制执行操作前要等待的小时数。</span><span class="sxs-lookup"><span data-stu-id="41ed4-134">Number of hours to wait till the action will be enforced.</span></span> <span data-ttu-id="41ed4-135">有效值为 0 至 8760</span><span class="sxs-lookup"><span data-stu-id="41ed4-135">Valid values 0 to 8760</span></span>|
|<span data-ttu-id="41ed4-136">actionType</span><span class="sxs-lookup"><span data-stu-id="41ed4-136">actionType</span></span>|<span data-ttu-id="41ed4-137">String</span><span class="sxs-lookup"><span data-stu-id="41ed4-137">String</span></span>|<span data-ttu-id="41ed4-138">要执行的操作。可取值为：`noAction`、`notification`、`block`、`retire`、`wipe`、`removeResourceAccessProfiles`。</span><span class="sxs-lookup"><span data-stu-id="41ed4-138">What action to take Possible values are: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`.</span></span>|
|<span data-ttu-id="41ed4-139">notificationTemplateId</span><span class="sxs-lookup"><span data-stu-id="41ed4-139">notificationTemplateId</span></span>|<span data-ttu-id="41ed4-140">String</span><span class="sxs-lookup"><span data-stu-id="41ed4-140">String</span></span>|<span data-ttu-id="41ed4-141">要使用的通知消息模板</span><span class="sxs-lookup"><span data-stu-id="41ed4-141">What notification Message template to use</span></span>|
|<span data-ttu-id="41ed4-142">notificationMessageCCList</span><span class="sxs-lookup"><span data-stu-id="41ed4-142">notificationMessageCCList</span></span>|<span data-ttu-id="41ed4-143">String 集合</span><span class="sxs-lookup"><span data-stu-id="41ed4-143">String collection</span></span>|<span data-ttu-id="41ed4-144">指定此通知邮件抄送对象的组 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="41ed4-144">A list of group IDs to speicify who to CC this notification message to.</span></span>|



## <a name="response"></a><span data-ttu-id="41ed4-145">响应</span><span class="sxs-lookup"><span data-stu-id="41ed4-145">Response</span></span>
<span data-ttu-id="41ed4-146">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="41ed4-146">If successful, this method returns a `201 Created` response code and a [directoryObject](../resources/intune_deviceconfig_devicecomplianceactionitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="41ed4-147">示例</span><span class="sxs-lookup"><span data-stu-id="41ed4-147">Example</span></span>
### <a name="request"></a><span data-ttu-id="41ed4-148">请求</span><span class="sxs-lookup"><span data-stu-id="41ed4-148">Request</span></span>
<span data-ttu-id="41ed4-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="41ed4-149">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations
Content-type: application/json
Content-length: 271

{
  "@odata.type": "#microsoft.graph.deviceComplianceActionItem",
  "gracePeriodHours": 0,
  "actionType": "notification",
  "notificationTemplateId": "Notification Template Id value",
  "notificationMessageCCList": [
    "Notification Message CCList value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="41ed4-150">响应</span><span class="sxs-lookup"><span data-stu-id="41ed4-150">Response</span></span>
<span data-ttu-id="41ed4-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="41ed4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 320

{
  "@odata.type": "#microsoft.graph.deviceComplianceActionItem",
  "id": "e01a1893-1893-e01a-9318-1ae093181ae0",
  "gracePeriodHours": 0,
  "actionType": "notification",
  "notificationTemplateId": "Notification Template Id value",
  "notificationMessageCCList": [
    "Notification Message CCList value"
  ]
}
```


