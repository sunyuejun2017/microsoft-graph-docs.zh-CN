# <a name="update-localizednotificationmessage"></a><span data-ttu-id="8ac00-101">更新 localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="8ac00-101">Update localizedNotificationMessage</span></span>

> <span data-ttu-id="8ac00-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="8ac00-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8ac00-103">更新 [localizedNotificationMessage](../resources/intune_notification_localizednotificationmessage.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="8ac00-103">Update the properties of a [calendar](../resources/intune_notification_localizednotificationmessage.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8ac00-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="8ac00-104">Prerequisites</span></span>
<span data-ttu-id="8ac00-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="8ac00-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8ac00-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="8ac00-107">Permission type</span></span>|<span data-ttu-id="8ac00-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="8ac00-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8ac00-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8ac00-109">Delegated (work or school account)</span></span>|<span data-ttu-id="8ac00-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ac00-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="8ac00-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8ac00-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8ac00-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="8ac00-112">Not supported.</span></span>|
|<span data-ttu-id="8ac00-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="8ac00-113">Application</span></span>|<span data-ttu-id="8ac00-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="8ac00-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8ac00-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8ac00-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages/{localizedNotificationMessageId}
```

## <a name="request-headers"></a><span data-ttu-id="8ac00-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="8ac00-116">Request headers</span></span>
|<span data-ttu-id="8ac00-117">标头</span><span class="sxs-lookup"><span data-stu-id="8ac00-117">Header</span></span>|<span data-ttu-id="8ac00-118">值</span><span class="sxs-lookup"><span data-stu-id="8ac00-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8ac00-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="8ac00-119">Authorization</span></span>|<span data-ttu-id="8ac00-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8ac00-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="8ac00-121">Accept</span><span class="sxs-lookup"><span data-stu-id="8ac00-121">Accept</span></span>|<span data-ttu-id="8ac00-122">application/json</span><span class="sxs-lookup"><span data-stu-id="8ac00-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8ac00-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="8ac00-123">Request body</span></span>
<span data-ttu-id="8ac00-124">在请求正文中，提供 [localizedNotificationMessage](../resources/intune_notification_localizednotificationmessage.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8ac00-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_notification_localizednotificationmessage.md) object.</span></span>

<span data-ttu-id="8ac00-125">下表显示创建 [localizedNotificationMessage](../resources/intune_notification_localizednotificationmessage.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="8ac00-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="8ac00-126">属性</span><span class="sxs-lookup"><span data-stu-id="8ac00-126">Property</span></span>|<span data-ttu-id="8ac00-127">类型</span><span class="sxs-lookup"><span data-stu-id="8ac00-127">Type</span></span>|<span data-ttu-id="8ac00-128">说明</span><span class="sxs-lookup"><span data-stu-id="8ac00-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ac00-129">id</span><span class="sxs-lookup"><span data-stu-id="8ac00-129">id</span></span>|<span data-ttu-id="8ac00-130">String</span><span class="sxs-lookup"><span data-stu-id="8ac00-130">String</span></span>|<span data-ttu-id="8ac00-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="8ac00-131">Key of the setting.</span></span>|
|<span data-ttu-id="8ac00-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8ac00-132">lastModifiedDateTime</span></span>|<span data-ttu-id="8ac00-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8ac00-133">DateTimeOffset</span></span>|<span data-ttu-id="8ac00-134">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="8ac00-134">Indicates the date the object was last modified.</span></span>|
|<span data-ttu-id="8ac00-135">locale</span><span class="sxs-lookup"><span data-stu-id="8ac00-135">locale</span></span>|<span data-ttu-id="8ac00-136">String</span><span class="sxs-lookup"><span data-stu-id="8ac00-136">String</span></span>|<span data-ttu-id="8ac00-137">此消息的目标区域设置。</span><span class="sxs-lookup"><span data-stu-id="8ac00-137">The Locale for which this message is destined.</span></span>|
|<span data-ttu-id="8ac00-138">subject</span><span class="sxs-lookup"><span data-stu-id="8ac00-138">subject</span></span>|<span data-ttu-id="8ac00-139">String</span><span class="sxs-lookup"><span data-stu-id="8ac00-139">String</span></span>|<span data-ttu-id="8ac00-140">消息模板主题。</span><span class="sxs-lookup"><span data-stu-id="8ac00-140">The Message Template Subject.</span></span>|
|<span data-ttu-id="8ac00-141">messageTemplate</span><span class="sxs-lookup"><span data-stu-id="8ac00-141">messageTemplate</span></span>|<span data-ttu-id="8ac00-142">String</span><span class="sxs-lookup"><span data-stu-id="8ac00-142">String</span></span>|<span data-ttu-id="8ac00-143">消息模板内容。</span><span class="sxs-lookup"><span data-stu-id="8ac00-143">The Message Template content.</span></span>|
|<span data-ttu-id="8ac00-144">isDefault</span><span class="sxs-lookup"><span data-stu-id="8ac00-144">isDefault</span></span>|<span data-ttu-id="8ac00-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="8ac00-145">Boolean</span></span>|<span data-ttu-id="8ac00-146">用于指示这是否是语言回退的默认区域设置的标记。</span><span class="sxs-lookup"><span data-stu-id="8ac00-146">Flag to indicate whether or not this is the default locale for language fallback.</span></span> <span data-ttu-id="8ac00-147">此标志只能设置。</span><span class="sxs-lookup"><span data-stu-id="8ac00-147">This flag can only be set.</span></span> <span data-ttu-id="8ac00-148">若要取消设置，请在其他本地化通知消息中将该属性设置为 true。</span><span class="sxs-lookup"><span data-stu-id="8ac00-148">To unset, set this property to true on another Localized Notification Message.</span></span>|



## <a name="response"></a><span data-ttu-id="8ac00-149">响应</span><span class="sxs-lookup"><span data-stu-id="8ac00-149">Response</span></span>
<span data-ttu-id="8ac00-150">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [localizedNotificationMessage](../resources/intune_notification_localizednotificationmessage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8ac00-150">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_notification_localizednotificationmessage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8ac00-151">示例</span><span class="sxs-lookup"><span data-stu-id="8ac00-151">Example</span></span>
### <a name="request"></a><span data-ttu-id="8ac00-152">请求</span><span class="sxs-lookup"><span data-stu-id="8ac00-152">Request</span></span>
<span data-ttu-id="8ac00-153">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8ac00-153">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages/{localizedNotificationMessageId}
Content-type: application/json
Content-length: 197

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "locale": "Locale value",
  "subject": "Subject value",
  "messageTemplate": "Message Template value",
  "isDefault": true
}
```

### <a name="response"></a><span data-ttu-id="8ac00-154">响应</span><span class="sxs-lookup"><span data-stu-id="8ac00-154">Response</span></span>
<span data-ttu-id="8ac00-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8ac00-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 313

{
  "@odata.type": "#microsoft.graph.localizedNotificationMessage",
  "id": "7a777708-7708-7a77-0877-777a0877777a",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "locale": "Locale value",
  "subject": "Subject value",
  "messageTemplate": "Message Template value",
  "isDefault": true
}
```


