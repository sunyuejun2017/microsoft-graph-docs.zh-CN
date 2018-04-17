# <a name="update-mobileappcontentfile"></a><span data-ttu-id="489f4-101">更新 mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="489f4-101">Update mobileAppContentFile</span></span>

> <span data-ttu-id="489f4-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="489f4-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="489f4-103">更新 [mobileAppContentFile](../resources/intune_apps_mobileappcontentfile.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="489f4-103">Update the properties of a [calendar](../resources/intune_apps_mobileappcontentfile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="489f4-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="489f4-104">Prerequisites</span></span>
<span data-ttu-id="489f4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="489f4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="489f4-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="489f4-107">Permission type</span></span>|<span data-ttu-id="489f4-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="489f4-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="489f4-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="489f4-109">Delegated (work or school account)</span></span>|<span data-ttu-id="489f4-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="489f4-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="489f4-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="489f4-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="489f4-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="489f4-112">Not supported.</span></span>|
|<span data-ttu-id="489f4-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="489f4-113">Application</span></span>|<span data-ttu-id="489f4-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="489f4-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="489f4-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="489f4-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}
```

## <a name="request-headers"></a><span data-ttu-id="489f4-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="489f4-116">Request headers</span></span>
|<span data-ttu-id="489f4-117">标头</span><span class="sxs-lookup"><span data-stu-id="489f4-117">Header</span></span>|<span data-ttu-id="489f4-118">值</span><span class="sxs-lookup"><span data-stu-id="489f4-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="489f4-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="489f4-119">Authorization</span></span>|<span data-ttu-id="489f4-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="489f4-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="489f4-121">Accept</span><span class="sxs-lookup"><span data-stu-id="489f4-121">Accept</span></span>|<span data-ttu-id="489f4-122">application/json</span><span class="sxs-lookup"><span data-stu-id="489f4-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="489f4-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="489f4-123">Request body</span></span>
<span data-ttu-id="489f4-124">在请求正文中，提供 [mobileAppContentFile](../resources/intune_apps_mobileappcontentfile.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="489f4-124">In the request body, supply a JSON representation of [ContactFolder](../resources/intune_apps_mobileappcontentfile.md) object.</span></span>

<span data-ttu-id="489f4-125">下表显示了创建 [mobileAppContentFile](../resources/intune_apps_mobileappcontentfile.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="489f4-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="489f4-126">属性</span><span class="sxs-lookup"><span data-stu-id="489f4-126">Property</span></span>|<span data-ttu-id="489f4-127">类型</span><span class="sxs-lookup"><span data-stu-id="489f4-127">Type</span></span>|<span data-ttu-id="489f4-128">说明</span><span class="sxs-lookup"><span data-stu-id="489f4-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="489f4-129">azureStorageUri</span><span class="sxs-lookup"><span data-stu-id="489f4-129">azureStorageUri</span></span>|<span data-ttu-id="489f4-130">String</span><span class="sxs-lookup"><span data-stu-id="489f4-130">String</span></span>|<span data-ttu-id="489f4-131">Azure 存储 URI。</span><span class="sxs-lookup"><span data-stu-id="489f4-131">The Azure Storage URI.</span></span>|
|<span data-ttu-id="489f4-132">isCommitted</span><span class="sxs-lookup"><span data-stu-id="489f4-132">isCommitted</span></span>|<span data-ttu-id="489f4-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="489f4-133">Boolean</span></span>|<span data-ttu-id="489f4-134">指示文件是否已提交的值。</span><span class="sxs-lookup"><span data-stu-id="489f4-134">A value indicating whether the file is committed.</span></span>|
|<span data-ttu-id="489f4-135">id</span><span class="sxs-lookup"><span data-stu-id="489f4-135">id</span></span>|<span data-ttu-id="489f4-136">String</span><span class="sxs-lookup"><span data-stu-id="489f4-136">String</span></span>|<span data-ttu-id="489f4-137">文件 ID。</span><span class="sxs-lookup"><span data-stu-id="489f4-137">The File Id.</span></span>|
|<span data-ttu-id="489f4-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="489f4-138">createdDateTime</span></span>|<span data-ttu-id="489f4-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="489f4-139">DateTimeOffset</span></span>|<span data-ttu-id="489f4-140">创建文件的时间。</span><span class="sxs-lookup"><span data-stu-id="489f4-140">The time the file was created.</span></span>|
|<span data-ttu-id="489f4-141">name</span><span class="sxs-lookup"><span data-stu-id="489f4-141">name</span></span>|<span data-ttu-id="489f4-142">String</span><span class="sxs-lookup"><span data-stu-id="489f4-142">String</span></span>|<span data-ttu-id="489f4-143">文件名称。</span><span class="sxs-lookup"><span data-stu-id="489f4-143">The file name</span></span>|
|<span data-ttu-id="489f4-144">size</span><span class="sxs-lookup"><span data-stu-id="489f4-144">size</span></span>|<span data-ttu-id="489f4-145">Int64</span><span class="sxs-lookup"><span data-stu-id="489f4-145">Int64</span></span>|<span data-ttu-id="489f4-146">加密前的文件大小。</span><span class="sxs-lookup"><span data-stu-id="489f4-146">The size of the file prior to encryption.</span></span>|
|<span data-ttu-id="489f4-147">sizeEncrypted</span><span class="sxs-lookup"><span data-stu-id="489f4-147">sizeEncrypted</span></span>|<span data-ttu-id="489f4-148">Int64</span><span class="sxs-lookup"><span data-stu-id="489f4-148">Int64</span></span>|<span data-ttu-id="489f4-149">加密后的文件大小。</span><span class="sxs-lookup"><span data-stu-id="489f4-149">The size of the file after encryption.</span></span>|
|<span data-ttu-id="489f4-150">azureStorageUriExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="489f4-150">azureStorageUriExpirationDateTime</span></span>|<span data-ttu-id="489f4-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="489f4-151">DateTimeOffset</span></span>|<span data-ttu-id="489f4-152">Azure 存储 URI 的到期时间。</span><span class="sxs-lookup"><span data-stu-id="489f4-152">The time the Azure storage Uri expires.</span></span>|
|<span data-ttu-id="489f4-153">manifest</span><span class="sxs-lookup"><span data-stu-id="489f4-153">manifest</span></span>|<span data-ttu-id="489f4-154">Binary</span><span class="sxs-lookup"><span data-stu-id="489f4-154">Binary</span></span>|<span data-ttu-id="489f4-155">清单信息。</span><span class="sxs-lookup"><span data-stu-id="489f4-155">The manifest information.</span></span>|
|<span data-ttu-id="489f4-156">uploadState</span><span class="sxs-lookup"><span data-stu-id="489f4-156">uploadState</span></span>|<span data-ttu-id="489f4-157">String</span><span class="sxs-lookup"><span data-stu-id="489f4-157">String</span></span>|<span data-ttu-id="489f4-158">当前上传请求的状态。</span><span class="sxs-lookup"><span data-stu-id="489f4-158">The state of the current upload request.</span></span> <span data-ttu-id="489f4-159">可取值为：`success`、`transientError`、`error`、`unknown`、`azureStorageUriRequestSuccess`、`azureStorageUriRequestPending`、`azureStorageUriRequestFailed`、`azureStorageUriRequestTimedOut`、`azureStorageUriRenewalSuccess`、`azureStorageUriRenewalPending`、`azureStorageUriRenewalFailed`、`azureStorageUriRenewalTimedOut`、`commitFileSuccess`、`commitFilePending`、`commitFileFailed`、`commitFileTimedOut`。</span><span class="sxs-lookup"><span data-stu-id="489f4-159">Possible values are: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span></span>|



## <a name="response"></a><span data-ttu-id="489f4-160">响应</span><span class="sxs-lookup"><span data-stu-id="489f4-160">Response</span></span>
<span data-ttu-id="489f4-161">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [mobileAppContentFile](../resources/intune_apps_mobileappcontentfile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="489f4-161">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_apps_mobileappcontentfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="489f4-162">示例</span><span class="sxs-lookup"><span data-stu-id="489f4-162">Example</span></span>
### <a name="request"></a><span data-ttu-id="489f4-163">请求</span><span class="sxs-lookup"><span data-stu-id="489f4-163">Request</span></span>
<span data-ttu-id="489f4-164">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="489f4-164">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}
Content-type: application/json
Content-length: 283

{
  "azureStorageUri": "Azure Storage Uri value",
  "isCommitted": true,
  "name": "Name value",
  "size": 4,
  "sizeEncrypted": 13,
  "azureStorageUriExpirationDateTime": "2017-01-01T00:00:08.4940464-08:00",
  "manifest": "bWFuaWZlc3Q=",
  "uploadState": "transientError"
}
```

### <a name="response"></a><span data-ttu-id="489f4-165">响应</span><span class="sxs-lookup"><span data-stu-id="489f4-165">Response</span></span>
<span data-ttu-id="489f4-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="489f4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 450

{
  "@odata.type": "#microsoft.graph.mobileAppContentFile",
  "azureStorageUri": "Azure Storage Uri value",
  "isCommitted": true,
  "id": "eab2e29b-e29b-eab2-9be2-b2ea9be2b2ea",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "name": "Name value",
  "size": 4,
  "sizeEncrypted": 13,
  "azureStorageUriExpirationDateTime": "2017-01-01T00:00:08.4940464-08:00",
  "manifest": "bWFuaWZlc3Q=",
  "uploadState": "transientError"
}
```


