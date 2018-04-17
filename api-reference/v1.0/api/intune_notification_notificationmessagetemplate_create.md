# <a name="create-notificationmessagetemplate"></a><span data-ttu-id="30f71-101">创建 notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="30f71-101">Create notificationMessageTemplate</span></span>

> <span data-ttu-id="30f71-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="30f71-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="30f71-103">创建新的 [notificationMessageTemplate](../resources/intune_notification_notificationmessagetemplate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="30f71-103">Create a new [plannerBucket](../resources/intune_notification_notificationmessagetemplate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="30f71-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="30f71-104">Prerequisites</span></span>
<span data-ttu-id="30f71-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="30f71-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="30f71-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="30f71-107">Permission type</span></span>|<span data-ttu-id="30f71-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="30f71-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="30f71-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="30f71-109">Delegated (work or school account)</span></span>|<span data-ttu-id="30f71-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30f71-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="30f71-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="30f71-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="30f71-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="30f71-112">Not supported.</span></span>|
|<span data-ttu-id="30f71-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="30f71-113">Application</span></span>|<span data-ttu-id="30f71-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="30f71-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="30f71-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="30f71-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/notificationMessageTemplates
```

## <a name="request-headers"></a><span data-ttu-id="30f71-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="30f71-116">Request headers</span></span>
|<span data-ttu-id="30f71-117">标头</span><span class="sxs-lookup"><span data-stu-id="30f71-117">Header</span></span>|<span data-ttu-id="30f71-118">值</span><span class="sxs-lookup"><span data-stu-id="30f71-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="30f71-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="30f71-119">Authorization</span></span>|<span data-ttu-id="30f71-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="30f71-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="30f71-121">Accept</span><span class="sxs-lookup"><span data-stu-id="30f71-121">Accept</span></span>|<span data-ttu-id="30f71-122">application/json</span><span class="sxs-lookup"><span data-stu-id="30f71-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="30f71-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="30f71-123">Request body</span></span>
<span data-ttu-id="30f71-124">在请求正文中，提供 notificationMessageTemplate 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="30f71-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="30f71-125">下表显示创建 notificationMessageTemplate 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="30f71-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="30f71-126">属性</span><span class="sxs-lookup"><span data-stu-id="30f71-126">Property</span></span>|<span data-ttu-id="30f71-127">类型</span><span class="sxs-lookup"><span data-stu-id="30f71-127">Type</span></span>|<span data-ttu-id="30f71-128">说明</span><span class="sxs-lookup"><span data-stu-id="30f71-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="30f71-129">id</span><span class="sxs-lookup"><span data-stu-id="30f71-129">id</span></span>|<span data-ttu-id="30f71-130">String</span><span class="sxs-lookup"><span data-stu-id="30f71-130">String</span></span>|<span data-ttu-id="30f71-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="30f71-131">Key of the setting.</span></span>|
|<span data-ttu-id="30f71-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="30f71-132">lastModifiedDateTime</span></span>|<span data-ttu-id="30f71-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="30f71-133">DateTimeOffset</span></span>|<span data-ttu-id="30f71-134">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="30f71-134">Indicates the date the object was last modified.</span></span>|
|<span data-ttu-id="30f71-135">displayName</span><span class="sxs-lookup"><span data-stu-id="30f71-135">displayName</span></span>|<span data-ttu-id="30f71-136">String</span><span class="sxs-lookup"><span data-stu-id="30f71-136">String</span></span>|<span data-ttu-id="30f71-137">通知消息模板的显示名称。</span><span class="sxs-lookup"><span data-stu-id="30f71-137">Display name for the Notification Message Template.</span></span>|
|<span data-ttu-id="30f71-138">defaultLocale</span><span class="sxs-lookup"><span data-stu-id="30f71-138">DefaultLocale</span></span>|<span data-ttu-id="30f71-139">String</span><span class="sxs-lookup"><span data-stu-id="30f71-139">String</span></span>|<span data-ttu-id="30f71-140">请求的区域设置不可用时要回退到的默认区域设置。</span><span class="sxs-lookup"><span data-stu-id="30f71-140">The default locale to fallback onto when the requested locale is not available.</span></span>|
|<span data-ttu-id="30f71-141">brandingOptions</span><span class="sxs-lookup"><span data-stu-id="30f71-141">brandingOptions</span></span>|<span data-ttu-id="30f71-142">String</span><span class="sxs-lookup"><span data-stu-id="30f71-142">String</span></span>|<span data-ttu-id="30f71-143">消息模板品牌选项。</span><span class="sxs-lookup"><span data-stu-id="30f71-143">The Message Template Branding Options.</span></span> <span data-ttu-id="30f71-144">已在 Intune 管理员控制台中定义品牌。</span><span class="sxs-lookup"><span data-stu-id="30f71-144">Branding is defined in the Intune Admin Console.</span></span> <span data-ttu-id="30f71-145">可取值为：`none`、`includeCompanyLogo`、`includeCompanyName`、`includeContactInformation`。</span><span class="sxs-lookup"><span data-stu-id="30f71-145">Possible values are: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.</span></span>|



## <a name="response"></a><span data-ttu-id="30f71-146">响应</span><span class="sxs-lookup"><span data-stu-id="30f71-146">Response</span></span>
<span data-ttu-id="30f71-147">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [notificationMessageTemplate](../resources/intune_notification_notificationmessagetemplate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="30f71-147">If successful, this method returns a `201 Created` response code and a [directoryObject](../resources/intune_notification_notificationmessagetemplate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="30f71-148">示例</span><span class="sxs-lookup"><span data-stu-id="30f71-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="30f71-149">请求</span><span class="sxs-lookup"><span data-stu-id="30f71-149">Request</span></span>
<span data-ttu-id="30f71-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="30f71-150">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/notificationMessageTemplates
Content-type: application/json
Content-length: 261

{
  "@odata.type": "#microsoft.graph.notificationMessageTemplate",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "defaultLocale": "Default Locale value",
  "brandingOptions": "includeCompanyLogo"
}
```

### <a name="response"></a><span data-ttu-id="30f71-151">响应</span><span class="sxs-lookup"><span data-stu-id="30f71-151">Response</span></span>
<span data-ttu-id="30f71-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="30f71-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 310

{
  "@odata.type": "#microsoft.graph.notificationMessageTemplate",
  "id": "e1db399b-399b-e1db-9b39-dbe19b39dbe1",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "defaultLocale": "Default Locale value",
  "brandingOptions": "includeCompanyLogo"
}
```


