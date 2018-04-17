# <a name="get-windowsinformationprotectionpolicy"></a><span data-ttu-id="5b17c-101">获取 windowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="5b17c-101">Get windowsInformationProtectionPolicy</span></span>

> <span data-ttu-id="5b17c-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="5b17c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5b17c-103">读取 [windowsInformationProtectionPolicy](../resources/intune_mam_windowsinformationprotectionpolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5b17c-103">Read properties and relationships of [plannerTaskDetails](../resources/intune_mam_windowsinformationprotectionpolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5b17c-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="5b17c-104">Prerequisites</span></span>
<span data-ttu-id="5b17c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="5b17c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5b17c-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="5b17c-107">Permission type</span></span>|<span data-ttu-id="5b17c-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="5b17c-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5b17c-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5b17c-109">Delegated (work or school account)</span></span>|<span data-ttu-id="5b17c-110">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="5b17c-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="5b17c-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5b17c-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5b17c-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="5b17c-112">Not supported.</span></span>|
|<span data-ttu-id="5b17c-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="5b17c-113">Application</span></span>|<span data-ttu-id="5b17c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="5b17c-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5b17c-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5b17c-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5b17c-116">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="5b17c-116">Optional query parameters</span></span>
<span data-ttu-id="5b17c-117">此方法支持 [OData 查询参数](https://developer.microsoft.com/zh-CN/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="5b17c-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/zh-CN/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="5b17c-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="5b17c-118">Request headers</span></span>
|<span data-ttu-id="5b17c-119">标头</span><span class="sxs-lookup"><span data-stu-id="5b17c-119">Header</span></span>|<span data-ttu-id="5b17c-120">值</span><span class="sxs-lookup"><span data-stu-id="5b17c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5b17c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5b17c-121">Authorization</span></span>|<span data-ttu-id="5b17c-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="5b17c-122">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="5b17c-123">Accept</span><span class="sxs-lookup"><span data-stu-id="5b17c-123">Accept</span></span>|<span data-ttu-id="5b17c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="5b17c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5b17c-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="5b17c-125">Request body</span></span>
<span data-ttu-id="5b17c-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5b17c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5b17c-127">响应</span><span class="sxs-lookup"><span data-stu-id="5b17c-127">Response</span></span>
<span data-ttu-id="5b17c-128">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [windowsInformationProtectionPolicy](../resources/intune_mam_windowsinformationprotectionpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5b17c-128">If successful, this method returns a `200 OK` response code and a [directoryObject](../resources/intune_mam_windowsinformationprotectionpolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5b17c-129">示例</span><span class="sxs-lookup"><span data-stu-id="5b17c-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="5b17c-130">请求</span><span class="sxs-lookup"><span data-stu-id="5b17c-130">Request</span></span>
<span data-ttu-id="5b17c-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5b17c-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}
```

### <a name="response"></a><span data-ttu-id="5b17c-132">响应</span><span class="sxs-lookup"><span data-stu-id="5b17c-132">Response</span></span>
<span data-ttu-id="5b17c-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5b17c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4867

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsInformationProtectionPolicy",
    "displayName": "Display Name value",
    "description": "Description value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "id": "6397be61-be61-6397-61be-976361be9763",
    "version": "Version value",
    "enforcementLevel": "encryptAndAuditOnly",
    "enterpriseDomain": "Enterprise Domain value",
    "enterpriseProtectedDomainNames": [
      {
        "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
        "displayName": "Display Name value",
        "resources": [
          "Resources value"
        ]
      }
    ],
    "protectionUnderLockConfigRequired": true,
    "dataRecoveryCertificate": {
      "@odata.type": "microsoft.graph.windowsInformationProtectionDataRecoveryCertificate",
      "subjectName": "Subject Name value",
      "description": "Description value",
      "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
      "certificate": "Y2VydGlmaWNhdGU="
    },
    "revokeOnUnenrollDisabled": true,
    "rightsManagementServicesTemplateId": "<Unknown Primitive Type Edm.Guid>",
    "azureRightsManagementServicesAllowed": true,
    "iconsVisible": true,
    "protectedApps": [
      {
        "@odata.type": "microsoft.graph.windowsInformationProtectionStoreApp",
        "displayName": "Display Name value",
        "description": "Description value",
        "publisherName": "Publisher Name value",
        "productName": "Product Name value",
        "denied": true
      }
    ],
    "exemptApps": [
      {
        "@odata.type": "microsoft.graph.windowsInformationProtectionStoreApp",
        "displayName": "Display Name value",
        "description": "Description value",
        "publisherName": "Publisher Name value",
        "productName": "Product Name value",
        "denied": true
      }
    ],
    "enterpriseNetworkDomainNames": [
      {
        "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
        "displayName": "Display Name value",
        "resources": [
          "Resources value"
        ]
      }
    ],
    "enterpriseProxiedDomains": [
      {
        "@odata.type": "microsoft.graph.windowsInformationProtectionProxiedDomainCollection",
        "displayName": "Display Name value",
        "proxiedDomains": [
          {
            "@odata.type": "microsoft.graph.proxiedDomain",
            "ipAddressOrFQDN": "Ip Address Or FQDN value",
            "proxy": "Proxy value"
          }
        ]
      }
    ],
    "enterpriseIPRanges": [
      {
        "@odata.type": "microsoft.graph.windowsInformationProtectionIPRangeCollection",
        "displayName": "Display Name value",
        "ranges": [
          {
            "@odata.type": "microsoft.graph.iPv6Range",
            "lowerAddress": "Lower Address value",
            "upperAddress": "Upper Address value"
          }
        ]
      }
    ],
    "enterpriseIPRangesAreAuthoritative": true,
    "enterpriseProxyServers": [
      {
        "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
        "displayName": "Display Name value",
        "resources": [
          "Resources value"
        ]
      }
    ],
    "enterpriseInternalProxyServers": [
      {
        "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
        "displayName": "Display Name value",
        "resources": [
          "Resources value"
        ]
      }
    ],
    "enterpriseProxyServersAreAuthoritative": true,
    "neutralDomainResources": [
      {
        "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
        "displayName": "Display Name value",
        "resources": [
          "Resources value"
        ]
      }
    ],
    "indexingEncryptedStoresOrItemsBlocked": true,
    "smbAutoEncryptedFileExtensions": [
      {
        "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection",
        "displayName": "Display Name value",
        "resources": [
          "Resources value"
        ]
      }
    ],
    "isAssigned": true,
    "revokeOnMdmHandoffDisabled": true,
    "mdmEnrollmentUrl": "https://example.com/mdmEnrollmentUrl/",
    "windowsHelloForBusinessBlocked": true,
    "pinMinimumLength": 0,
    "pinUppercaseLetters": "requireAtLeastOne",
    "pinLowercaseLetters": "requireAtLeastOne",
    "pinSpecialCharacters": "requireAtLeastOne",
    "pinExpirationDays": 1,
    "numberOfPastPinsRemembered": 10,
    "passwordMaximumAttemptCount": 11,
    "minutesOfInactivityBeforeDeviceLock": 3,
    "daysWithoutContactBeforeUnenroll": 0
  }
}
```


