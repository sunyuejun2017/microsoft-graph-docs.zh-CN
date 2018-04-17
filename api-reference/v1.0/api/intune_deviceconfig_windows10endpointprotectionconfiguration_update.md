# <a name="update-windows10endpointprotectionconfiguration"></a><span data-ttu-id="c413e-101">更新 windows10EndpointProtectionConfiguration</span><span class="sxs-lookup"><span data-stu-id="c413e-101">Update windows10EndpointProtectionConfiguration</span></span>

> <span data-ttu-id="c413e-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="c413e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c413e-103">更新 [windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c413e-103">Update the properties of a [calendar](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c413e-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="c413e-104">Prerequisites</span></span>
<span data-ttu-id="c413e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="c413e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c413e-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="c413e-107">Permission type</span></span>|<span data-ttu-id="c413e-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c413e-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c413e-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c413e-109">Delegated (work or school account)</span></span>|<span data-ttu-id="c413e-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c413e-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c413e-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c413e-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c413e-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="c413e-112">Not supported.</span></span>|
|<span data-ttu-id="c413e-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="c413e-113">Application</span></span>|<span data-ttu-id="c413e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="c413e-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c413e-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c413e-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="c413e-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="c413e-116">Request headers</span></span>
|<span data-ttu-id="c413e-117">标头</span><span class="sxs-lookup"><span data-stu-id="c413e-117">Header</span></span>|<span data-ttu-id="c413e-118">值</span><span class="sxs-lookup"><span data-stu-id="c413e-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c413e-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="c413e-119">Authorization</span></span>|<span data-ttu-id="c413e-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c413e-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="c413e-121">Accept</span><span class="sxs-lookup"><span data-stu-id="c413e-121">Accept</span></span>|<span data-ttu-id="c413e-122">application/json</span><span class="sxs-lookup"><span data-stu-id="c413e-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c413e-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="c413e-123">Request body</span></span>
<span data-ttu-id="c413e-124">在请求正文中，提供 [windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c413e-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md) object.</span></span>

<span data-ttu-id="c413e-125">下表显示了创建 [windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c413e-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="c413e-126">属性</span><span class="sxs-lookup"><span data-stu-id="c413e-126">Property</span></span>|<span data-ttu-id="c413e-127">类型</span><span class="sxs-lookup"><span data-stu-id="c413e-127">Type</span></span>|<span data-ttu-id="c413e-128">说明</span><span class="sxs-lookup"><span data-stu-id="c413e-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c413e-129">id</span><span class="sxs-lookup"><span data-stu-id="c413e-129">id</span></span>|<span data-ttu-id="c413e-130">String</span><span class="sxs-lookup"><span data-stu-id="c413e-130">String</span></span>|<span data-ttu-id="c413e-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c413e-131">Key of the setting.</span></span> <span data-ttu-id="c413e-132">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c413e-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c413e-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c413e-133">lastModifiedDateTime</span></span>|<span data-ttu-id="c413e-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c413e-134">DateTimeOffset</span></span>|<span data-ttu-id="c413e-135">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c413e-135">Indicates the date the object was last modified.</span></span> <span data-ttu-id="c413e-136">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c413e-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c413e-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c413e-137">createdDateTime</span></span>|<span data-ttu-id="c413e-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c413e-138">DateTimeOffset</span></span>|<span data-ttu-id="c413e-139">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c413e-139">DateTime the object was created.</span></span> <span data-ttu-id="c413e-140">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c413e-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c413e-141">description</span><span class="sxs-lookup"><span data-stu-id="c413e-141">description</span></span>|<span data-ttu-id="c413e-142">String</span><span class="sxs-lookup"><span data-stu-id="c413e-142">String</span></span>|<span data-ttu-id="c413e-143">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="c413e-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c413e-144">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c413e-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c413e-145">displayName</span><span class="sxs-lookup"><span data-stu-id="c413e-145">displayName</span></span>|<span data-ttu-id="c413e-146">String</span><span class="sxs-lookup"><span data-stu-id="c413e-146">String</span></span>|<span data-ttu-id="c413e-147">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="c413e-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c413e-148">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c413e-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c413e-149">version</span><span class="sxs-lookup"><span data-stu-id="c413e-149">version</span></span>|<span data-ttu-id="c413e-150">Int32</span><span class="sxs-lookup"><span data-stu-id="c413e-150">Int32</span></span>|<span data-ttu-id="c413e-151">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="c413e-151">Version of the device configuration.</span></span> <span data-ttu-id="c413e-152">继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c413e-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c413e-153">firewallBlockStatefulFTP</span><span class="sxs-lookup"><span data-stu-id="c413e-153">firewallBlockStatefulFTP</span></span>|<span data-ttu-id="c413e-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="c413e-154">Boolean</span></span>|<span data-ttu-id="c413e-155">阻止到设备的有状态 FTP 连接</span><span class="sxs-lookup"><span data-stu-id="c413e-155">Blocks stateful FTP connections to the device</span></span>|
|<span data-ttu-id="c413e-156">firewallIdleTimeoutForSecurityAssociationInSeconds</span><span class="sxs-lookup"><span data-stu-id="c413e-156">firewallIdleTimeoutForSecurityAssociationInSeconds</span></span>|<span data-ttu-id="c413e-157">Int32</span><span class="sxs-lookup"><span data-stu-id="c413e-157">Int32</span></span>|<span data-ttu-id="c413e-158">配置安全关联的空闲超时（以秒为单位），值范围为 300 到 3600（包括这两个值）。</span><span class="sxs-lookup"><span data-stu-id="c413e-158">Configures the idle timeout for security associations, in seconds, from 300 to 3600 inclusive.</span></span> <span data-ttu-id="c413e-159">这是一个时间段，在此之后安全关联将过期并被删除。</span><span class="sxs-lookup"><span data-stu-id="c413e-159">This is the period after which security associations will expire and be deleted.</span></span> <span data-ttu-id="c413e-160">有效值为 300 至 3600</span><span class="sxs-lookup"><span data-stu-id="c413e-160">Valid values 300 to 3600</span></span>|
|<span data-ttu-id="c413e-161">firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="c413e-161">firewallPreSharedKeyEncodingMethod</span></span>|<span data-ttu-id="c413e-162">String</span><span class="sxs-lookup"><span data-stu-id="c413e-162">String</span></span>|<span data-ttu-id="c413e-163">选择要使用的预共享密钥编码。可取值为：`deviceDefault`、`none`、`utF8`。</span><span class="sxs-lookup"><span data-stu-id="c413e-163">Select the preshared key encoding to be used Possible values are: `deviceDefault`, `none`, `utF8`.</span></span>|
|<span data-ttu-id="c413e-164">firewallIPSecExemptionsAllowNeighborDiscovery</span><span class="sxs-lookup"><span data-stu-id="c413e-164">firewallIPSecExemptionsAllowNeighborDiscovery</span></span>|<span data-ttu-id="c413e-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="c413e-165">Boolean</span></span>|<span data-ttu-id="c413e-166">配置 IPSec 免除项以允许邻居发现 IPv6 ICMP 类型代码</span><span class="sxs-lookup"><span data-stu-id="c413e-166">Configures IPSec exemptions to allow neighbor discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="c413e-167">firewallIPSecExemptionsAllowICMP</span><span class="sxs-lookup"><span data-stu-id="c413e-167">firewallIPSecExemptionsAllowICMP</span></span>|<span data-ttu-id="c413e-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="c413e-168">Boolean</span></span>|<span data-ttu-id="c413e-169">配置 IPSec 免除项以允许 ICMP</span><span class="sxs-lookup"><span data-stu-id="c413e-169">Configures IPSec exemptions to allow ICMP</span></span>|
|<span data-ttu-id="c413e-170">firewallIPSecExemptionsAllowRouterDiscovery</span><span class="sxs-lookup"><span data-stu-id="c413e-170">firewallIPSecExemptionsAllowRouterDiscovery</span></span>|<span data-ttu-id="c413e-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="c413e-171">Boolean</span></span>|<span data-ttu-id="c413e-172">配置 IPSec 免除项以允许路由器发现 IPv6 ICMP 类型代码</span><span class="sxs-lookup"><span data-stu-id="c413e-172">Configures IPSec exemptions to allow router discovery IPv6 ICMP type-codes</span></span>|
|<span data-ttu-id="c413e-173">firewallIPSecExemptionsAllowDHCP</span><span class="sxs-lookup"><span data-stu-id="c413e-173">firewallIPSecExemptionsAllowDHCP</span></span>|<span data-ttu-id="c413e-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="c413e-174">Boolean</span></span>|<span data-ttu-id="c413e-175">配置 IPSec 免除项以允许 IPv4 和 IPv6 DHCP 通信</span><span class="sxs-lookup"><span data-stu-id="c413e-175">Configures IPSec exemptions to allow both IPv4 and IPv6 DHCP traffic</span></span>|
|<span data-ttu-id="c413e-176">firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="c413e-176">firewallCertificateRevocationListCheckMethod</span></span>|<span data-ttu-id="c413e-177">String</span><span class="sxs-lookup"><span data-stu-id="c413e-177">String</span></span>|<span data-ttu-id="c413e-178">指定如何强制执行证书吊销列表。可取值为：`deviceDefault`、`none`、`attempt`、`require`。</span><span class="sxs-lookup"><span data-stu-id="c413e-178">Specify how the certificate revocation list is to be enforced Possible values are: `deviceDefault`, `none`, `attempt`, `require`.</span></span>|
|<span data-ttu-id="c413e-179">firewallMergeKeyingModuleSettings</span><span class="sxs-lookup"><span data-stu-id="c413e-179">firewallMergeKeyingModuleSettings</span></span>|<span data-ttu-id="c413e-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="c413e-180">Boolean</span></span>|<span data-ttu-id="c413e-181">如果键控模块不完全支持身份验证集，请指示模块仅忽略不受支持的身份验证套件而不是整个集</span><span class="sxs-lookup"><span data-stu-id="c413e-181">If an authentication set is not fully supported by a keying module, direct the module to ignore only unsupported authentication suites rather than the entire set</span></span>|
|<span data-ttu-id="c413e-182">firewallPacketQueueingMethod</span><span class="sxs-lookup"><span data-stu-id="c413e-182">firewallPacketQueueingMethod</span></span>|<span data-ttu-id="c413e-183">String</span><span class="sxs-lookup"><span data-stu-id="c413e-183">String</span></span>|<span data-ttu-id="c413e-184">配置如何在隧道网关应用场景中应用数据包排队。可取值为：`deviceDefault`、`disabled`、`queueInbound`、`queueOutbound`、`queueBoth`。</span><span class="sxs-lookup"><span data-stu-id="c413e-184">Configures how packet queueing should be applied in the tunnel gateway scenario Possible values are: `deviceDefault`, `disabled`, `queueInbound`, `queueOutbound`, `queueBoth`.</span></span>|
|<span data-ttu-id="c413e-185">firewallProfileDomain</span><span class="sxs-lookup"><span data-stu-id="c413e-185">firewallProfileDomain</span></span>|[<span data-ttu-id="c413e-186">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="c413e-186">windowsFirewallNetworkProfile</span></span>](../resources/intune_deviceconfig_windowsfirewallnetworkprofile.md)|<span data-ttu-id="c413e-187">配置域网络的防火墙配置文件设置</span><span class="sxs-lookup"><span data-stu-id="c413e-187">Configures the firewall profile settings for domain networks</span></span>|
|<span data-ttu-id="c413e-188">firewallProfilePublic</span><span class="sxs-lookup"><span data-stu-id="c413e-188">firewallProfilePublic</span></span>|[<span data-ttu-id="c413e-189">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="c413e-189">windowsFirewallNetworkProfile</span></span>](../resources/intune_deviceconfig_windowsfirewallnetworkprofile.md)|<span data-ttu-id="c413e-190">配置公用网络的防火墙配置文件设置</span><span class="sxs-lookup"><span data-stu-id="c413e-190">Configures the firewall profile settings for public networks</span></span>|
|<span data-ttu-id="c413e-191">firewallProfilePrivate</span><span class="sxs-lookup"><span data-stu-id="c413e-191">firewallProfilePrivate</span></span>|[<span data-ttu-id="c413e-192">windowsFirewallNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="c413e-192">windowsFirewallNetworkProfile</span></span>](../resources/intune_deviceconfig_windowsfirewallnetworkprofile.md)|<span data-ttu-id="c413e-193">配置专用网络的防火墙配置文件设置</span><span class="sxs-lookup"><span data-stu-id="c413e-193">Configures the firewall profile settings for private networks</span></span>|
|<span data-ttu-id="c413e-194">defenderAttackSurfaceReductionExcludedPaths</span><span class="sxs-lookup"><span data-stu-id="c413e-194">defenderAttackSurfaceReductionExcludedPaths</span></span>|<span data-ttu-id="c413e-195">String 集合</span><span class="sxs-lookup"><span data-stu-id="c413e-195">String collection</span></span>|<span data-ttu-id="c413e-196">要从攻击面减少规则中排除的 exe 文件和文件夹的列表</span><span class="sxs-lookup"><span data-stu-id="c413e-196">List of exe files and folders to be excluded from attack surface reduction rules</span></span>|
|<span data-ttu-id="c413e-197">defenderGuardedFoldersAllowedAppPaths</span><span class="sxs-lookup"><span data-stu-id="c413e-197">defenderGuardedFoldersAllowedAppPaths</span></span>|<span data-ttu-id="c413e-198">String 集合</span><span class="sxs-lookup"><span data-stu-id="c413e-198">String collection</span></span>|<span data-ttu-id="c413e-199">允许访问受保护文件夹的 exe 路径列表</span><span class="sxs-lookup"><span data-stu-id="c413e-199">List of paths to exe that are allowed to access protected folders</span></span>|
|<span data-ttu-id="c413e-200">defenderAdditionalGuardedFolders</span><span class="sxs-lookup"><span data-stu-id="c413e-200">defenderAdditionalGuardedFolders</span></span>|<span data-ttu-id="c413e-201">String 集合</span><span class="sxs-lookup"><span data-stu-id="c413e-201">String collection</span></span>|<span data-ttu-id="c413e-202">要添加到受保护文件夹列表的文件夹路径列表</span><span class="sxs-lookup"><span data-stu-id="c413e-202">List of folder paths to be added to the list of protected folders</span></span>|
|<span data-ttu-id="c413e-203">defenderExploitProtectionXml</span><span class="sxs-lookup"><span data-stu-id="c413e-203">defenderExploitProtectionXml</span></span>|<span data-ttu-id="c413e-204">Binary</span><span class="sxs-lookup"><span data-stu-id="c413e-204">Binary</span></span>|<span data-ttu-id="c413e-205">包含有关 Exploit Protection 详细信息的 xml 内容。</span><span class="sxs-lookup"><span data-stu-id="c413e-205">Xml content containing information regarding exploit protection details.</span></span>|
|<span data-ttu-id="c413e-206">defenderExploitProtectionXmlFileName</span><span class="sxs-lookup"><span data-stu-id="c413e-206">defenderExploitProtectionXmlFileName</span></span>|<span data-ttu-id="c413e-207">String</span><span class="sxs-lookup"><span data-stu-id="c413e-207">String</span></span>|<span data-ttu-id="c413e-208">从中获取 DefenderExploitProtectionXml 的文件的名称。</span><span class="sxs-lookup"><span data-stu-id="c413e-208">Name of the file from which DefenderExploitProtectionXml was obtained.</span></span>|
|<span data-ttu-id="c413e-209">defenderSecurityCenterBlockExploitProtectionOverride</span><span class="sxs-lookup"><span data-stu-id="c413e-209">defenderSecurityCenterBlockExploitProtectionOverride</span></span>|<span data-ttu-id="c413e-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="c413e-210">Boolean</span></span>|<span data-ttu-id="c413e-211">指示是否阻止用户覆盖 Exploit Protection 设置。</span><span class="sxs-lookup"><span data-stu-id="c413e-211">Indicates whether or not to block user from overriding Exploit Protection settings.</span></span>|
|<span data-ttu-id="c413e-212">appLockerApplicationControl</span><span class="sxs-lookup"><span data-stu-id="c413e-212">appLockerApplicationControl</span></span>|<span data-ttu-id="c413e-213">String</span><span class="sxs-lookup"><span data-stu-id="c413e-213">String</span></span>|<span data-ttu-id="c413e-214">使管理员能够选择在设备上允许哪些类型的应用。</span><span class="sxs-lookup"><span data-stu-id="c413e-214">Enables the Admin to choose what types of app to allow on devices.</span></span> <span data-ttu-id="c413e-215">可取值为：`notConfigured`、`enforceComponentsAndStoreApps`、`auditComponentsAndStoreApps`、`enforceComponentsStoreAppsAndSmartlocker`、`auditComponentsStoreAppsAndSmartlocker`。</span><span class="sxs-lookup"><span data-stu-id="c413e-215">Possible values are: `notConfigured`, `enforceComponentsAndStoreApps`, `auditComponentsAndStoreApps`, `enforceComponentsStoreAppsAndSmartlocker`, `auditComponentsStoreAppsAndSmartlocker`.</span></span>|
|<span data-ttu-id="c413e-216">smartScreenEnableInShell</span><span class="sxs-lookup"><span data-stu-id="c413e-216">smartScreenEnableInShell</span></span>|<span data-ttu-id="c413e-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="c413e-217">Boolean</span></span>|<span data-ttu-id="c413e-218">允许 IT 管理员配置适用于 Windows 的 SmartScreen。</span><span class="sxs-lookup"><span data-stu-id="c413e-218">Allows IT Admins to configure SmartScreen for Windows.</span></span>|
|<span data-ttu-id="c413e-219">smartScreenBlockOverrideForFiles</span><span class="sxs-lookup"><span data-stu-id="c413e-219">smartScreenBlockOverrideForFiles</span></span>|<span data-ttu-id="c413e-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="c413e-220">Boolean</span></span>|<span data-ttu-id="c413e-221">允许 IT 管理员控制用户是否可以忽略 SmartScreen 警告并运行恶意文件。</span><span class="sxs-lookup"><span data-stu-id="c413e-221">Allows IT Admins to control whether users can can ignore SmartScreen warnings and run malicious files.</span></span>|
|<span data-ttu-id="c413e-222">applicationGuardEnabled</span><span class="sxs-lookup"><span data-stu-id="c413e-222">applicationGuardEnabled</span></span>|<span data-ttu-id="c413e-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="c413e-223">Boolean</span></span>|<span data-ttu-id="c413e-224">启用 Windows Defender 应用程序防护</span><span class="sxs-lookup"><span data-stu-id="c413e-224">Enable Windows Defender Application Guard</span></span>|
|<span data-ttu-id="c413e-225">applicationGuardBlockFileTransfer</span><span class="sxs-lookup"><span data-stu-id="c413e-225">applicationGuardBlockFileTransfer</span></span>|<span data-ttu-id="c413e-226">String</span><span class="sxs-lookup"><span data-stu-id="c413e-226">String</span></span>|<span data-ttu-id="c413e-227">阻止剪贴板传输图像文件或文本文件或两者均不阻止。可取值为：`notConfigured`、`blockImageAndTextFile`、`blockImageFile`、`blockNone`、`blockTextFile`。</span><span class="sxs-lookup"><span data-stu-id="c413e-227">Block clipboard to transfer image file, text file or neither of them Possible values are: `notConfigured`, `blockImageAndTextFile`, `blockImageFile`, `blockNone`, `blockTextFile`.</span></span>|
|<span data-ttu-id="c413e-228">applicationGuardBlockNonEnterpriseContent</span><span class="sxs-lookup"><span data-stu-id="c413e-228">applicationGuardBlockNonEnterpriseContent</span></span>|<span data-ttu-id="c413e-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="c413e-229">Boolean</span></span>|<span data-ttu-id="c413e-230">阻止企业站点加载非企业内容，例如第三方插件</span><span class="sxs-lookup"><span data-stu-id="c413e-230">Block enterprise sites to load non-enterprise content, such as third party plug-ins</span></span>|
|<span data-ttu-id="c413e-231">applicationGuardAllowPersistence</span><span class="sxs-lookup"><span data-stu-id="c413e-231">applicationGuardAllowPersistence</span></span>|<span data-ttu-id="c413e-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="c413e-232">Boolean</span></span>|<span data-ttu-id="c413e-233">允许 App Guard 容器（收藏夹、Cookie、Web 密码等）内的持久用户生成数据</span><span class="sxs-lookup"><span data-stu-id="c413e-233">Allow persisting user generated data inside the App Guard Containter (favorites, cookies, web passwords, etc.)</span></span>|
|<span data-ttu-id="c413e-234">applicationGuardForceAuditing</span><span class="sxs-lookup"><span data-stu-id="c413e-234">applicationGuardForceAuditing</span></span>|<span data-ttu-id="c413e-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="c413e-235">Boolean</span></span>|<span data-ttu-id="c413e-236">强制审核将存留 Windows 日志和事件以满足安全/符合性条件（示例事件是用户登录注销、特权使用、软件安装、系统更改等）</span><span class="sxs-lookup"><span data-stu-id="c413e-236">Force auditing will persist Windows logs and events to meet security/compliance criteria (sample events are user login-logoff, use of privilege rights, software installation, system changes, etc.)</span></span>|
|<span data-ttu-id="c413e-237">applicationGuardBlockClipboardSharing</span><span class="sxs-lookup"><span data-stu-id="c413e-237">applicationGuardBlockClipboardSharing</span></span>|<span data-ttu-id="c413e-238">String</span><span class="sxs-lookup"><span data-stu-id="c413e-238">String</span></span>|<span data-ttu-id="c413e-239">阻止剪贴板将数据从主机共享到容器或从容器共享到主机，或阻止两种方式，或两种方式均不阻止。</span><span class="sxs-lookup"><span data-stu-id="c413e-239">Block clipboard to share data from Host to Container, or from Container to Host, or both ways, or neither ways.</span></span> <span data-ttu-id="c413e-240">可取值为：`notConfigured`、`blockBoth`、`blockHostToContainer`、`blockContainerToHost`、`blockNone`。</span><span class="sxs-lookup"><span data-stu-id="c413e-240">Possible values are: `notConfigured`, `blockBoth`, `blockHostToContainer`, `blockContainerToHost`, `blockNone`.</span></span>|
|<span data-ttu-id="c413e-241">applicationGuardAllowPrintToPDF</span><span class="sxs-lookup"><span data-stu-id="c413e-241">applicationGuardAllowPrintToPDF</span></span>|<span data-ttu-id="c413e-242">Boolean</span><span class="sxs-lookup"><span data-stu-id="c413e-242">Boolean</span></span>|<span data-ttu-id="c413e-243">允许从容器打印为 PDF 格式</span><span class="sxs-lookup"><span data-stu-id="c413e-243">Allow printing to PDF from Container</span></span>|
|<span data-ttu-id="c413e-244">applicationGuardAllowPrintToXPS</span><span class="sxs-lookup"><span data-stu-id="c413e-244">applicationGuardAllowPrintToXPS</span></span>|<span data-ttu-id="c413e-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="c413e-245">Boolean</span></span>|<span data-ttu-id="c413e-246">允许从容器打印为 XPS 格式</span><span class="sxs-lookup"><span data-stu-id="c413e-246">Allow printing to XPS from Container</span></span>|
|<span data-ttu-id="c413e-247">applicationGuardAllowPrintToLocalPrinters</span><span class="sxs-lookup"><span data-stu-id="c413e-247">applicationGuardAllowPrintToLocalPrinters</span></span>|<span data-ttu-id="c413e-248">Boolean</span><span class="sxs-lookup"><span data-stu-id="c413e-248">Boolean</span></span>|<span data-ttu-id="c413e-249">允许从容器打印到本地打印机</span><span class="sxs-lookup"><span data-stu-id="c413e-249">Allow printing to Local Printers from Container</span></span>|
|<span data-ttu-id="c413e-250">applicationGuardAllowPrintToNetworkPrinters</span><span class="sxs-lookup"><span data-stu-id="c413e-250">applicationGuardAllowPrintToNetworkPrinters</span></span>|<span data-ttu-id="c413e-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="c413e-251">Boolean</span></span>|<span data-ttu-id="c413e-252">允许从容器打印到网络打印机</span><span class="sxs-lookup"><span data-stu-id="c413e-252">Allow printing to Network Printers from Container</span></span>|
|<span data-ttu-id="c413e-253">bitLockerDisableWarningForOtherDiskEncryption</span><span class="sxs-lookup"><span data-stu-id="c413e-253">bitLockerDisableWarningForOtherDiskEncryption</span></span>|<span data-ttu-id="c413e-254">Boolean</span><span class="sxs-lookup"><span data-stu-id="c413e-254">Boolean</span></span>|<span data-ttu-id="c413e-255">允许管理员禁用对用户计算机上其他磁盘加密的警告提示。</span><span class="sxs-lookup"><span data-stu-id="c413e-255">Allows the Admin to disable the warning prompt for other disk encryption on the user machines.</span></span>|
|<span data-ttu-id="c413e-256">bitLockerEnableStorageCardEncryptionOnMobile</span><span class="sxs-lookup"><span data-stu-id="c413e-256">bitLockerEnableStorageCardEncryptionOnMobile</span></span>|<span data-ttu-id="c413e-257">Boolean</span><span class="sxs-lookup"><span data-stu-id="c413e-257">Boolean</span></span>|<span data-ttu-id="c413e-258">允许管理员要求使用 BitLocker 开启加密功能。</span><span class="sxs-lookup"><span data-stu-id="c413e-258">Allows the admin to require encryption to be turned on using BitLocker.</span></span> <span data-ttu-id="c413e-259">此策略仅适用于移动 SKU。</span><span class="sxs-lookup"><span data-stu-id="c413e-259">This policy is valid only for a mobile SKU.</span></span>|
|<span data-ttu-id="c413e-260">bitLockerEncryptDevice</span><span class="sxs-lookup"><span data-stu-id="c413e-260">bitLockerEncryptDevice</span></span>|<span data-ttu-id="c413e-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="c413e-261">Boolean</span></span>|<span data-ttu-id="c413e-262">允许管理员要求使用 BitLocker 开启加密功能。</span><span class="sxs-lookup"><span data-stu-id="c413e-262">Allows the admin to require encryption to be turned on using BitLocker.</span></span>|
|<span data-ttu-id="c413e-263">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="c413e-263">bitLockerRemovableDrivePolicy</span></span>|[<span data-ttu-id="c413e-264">bitLockerRemovableDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="c413e-264">bitLockerRemovableDrivePolicy</span></span>](../resources/intune_deviceconfig_bitlockerremovabledrivepolicy.md)|<span data-ttu-id="c413e-265">BitLocker 可移动驱动器策略。</span><span class="sxs-lookup"><span data-stu-id="c413e-265">BitLocker Removable Drive Policy.</span></span>|



## <a name="response"></a><span data-ttu-id="c413e-266">响应</span><span class="sxs-lookup"><span data-stu-id="c413e-266">Response</span></span>
<span data-ttu-id="c413e-267">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c413e-267">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c413e-268">示例</span><span class="sxs-lookup"><span data-stu-id="c413e-268">Example</span></span>
### <a name="request"></a><span data-ttu-id="c413e-269">请求</span><span class="sxs-lookup"><span data-stu-id="c413e-269">Request</span></span>
<span data-ttu-id="c413e-270">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c413e-270">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 4230

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "firewallBlockStatefulFTP": true,
  "firewallIdleTimeoutForSecurityAssociationInSeconds": 2,
  "firewallPreSharedKeyEncodingMethod": "none",
  "firewallIPSecExemptionsAllowNeighborDiscovery": true,
  "firewallIPSecExemptionsAllowICMP": true,
  "firewallIPSecExemptionsAllowRouterDiscovery": true,
  "firewallIPSecExemptionsAllowDHCP": true,
  "firewallCertificateRevocationListCheckMethod": "none",
  "firewallMergeKeyingModuleSettings": true,
  "firewallPacketQueueingMethod": "disabled",
  "firewallProfileDomain": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "blocked",
    "stealthModeBlocked": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "policyRulesFromGroupPolicyMerged": true
  },
  "firewallProfilePublic": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "blocked",
    "stealthModeBlocked": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "policyRulesFromGroupPolicyMerged": true
  },
  "firewallProfilePrivate": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "blocked",
    "stealthModeBlocked": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "policyRulesFromGroupPolicyMerged": true
  },
  "defenderAttackSurfaceReductionExcludedPaths": [
    "Defender Attack Surface Reduction Excluded Paths value"
  ],
  "defenderGuardedFoldersAllowedAppPaths": [
    "Defender Guarded Folders Allowed App Paths value"
  ],
  "defenderAdditionalGuardedFolders": [
    "Defender Additional Guarded Folders value"
  ],
  "defenderExploitProtectionXml": "ZGVmZW5kZXJFeHBsb2l0UHJvdGVjdGlvblhtbA==",
  "defenderExploitProtectionXmlFileName": "Defender Exploit Protection Xml File Name value",
  "defenderSecurityCenterBlockExploitProtectionOverride": true,
  "appLockerApplicationControl": "enforceComponentsAndStoreApps",
  "smartScreenEnableInShell": true,
  "smartScreenBlockOverrideForFiles": true,
  "applicationGuardEnabled": true,
  "applicationGuardBlockFileTransfer": "blockImageAndTextFile",
  "applicationGuardBlockNonEnterpriseContent": true,
  "applicationGuardAllowPersistence": true,
  "applicationGuardForceAuditing": true,
  "applicationGuardBlockClipboardSharing": "blockBoth",
  "applicationGuardAllowPrintToPDF": true,
  "applicationGuardAllowPrintToXPS": true,
  "applicationGuardAllowPrintToLocalPrinters": true,
  "applicationGuardAllowPrintToNetworkPrinters": true,
  "bitLockerDisableWarningForOtherDiskEncryption": true,
  "bitLockerEnableStorageCardEncryptionOnMobile": true,
  "bitLockerEncryptDevice": true,
  "bitLockerRemovableDrivePolicy": {
    "@odata.type": "microsoft.graph.bitLockerRemovableDrivePolicy",
    "encryptionMethod": "aesCbc256",
    "requireEncryptionForWriteAccess": true,
    "blockCrossOrganizationWriteAccess": true
  }
}
```

### <a name="response"></a><span data-ttu-id="c413e-271">响应</span><span class="sxs-lookup"><span data-stu-id="c413e-271">Response</span></span>
<span data-ttu-id="c413e-p112">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c413e-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4417

{
  "@odata.type": "#microsoft.graph.windows10EndpointProtectionConfiguration",
  "id": "09709403-9403-0970-0394-700903947009",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "firewallBlockStatefulFTP": true,
  "firewallIdleTimeoutForSecurityAssociationInSeconds": 2,
  "firewallPreSharedKeyEncodingMethod": "none",
  "firewallIPSecExemptionsAllowNeighborDiscovery": true,
  "firewallIPSecExemptionsAllowICMP": true,
  "firewallIPSecExemptionsAllowRouterDiscovery": true,
  "firewallIPSecExemptionsAllowDHCP": true,
  "firewallCertificateRevocationListCheckMethod": "none",
  "firewallMergeKeyingModuleSettings": true,
  "firewallPacketQueueingMethod": "disabled",
  "firewallProfileDomain": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "blocked",
    "stealthModeBlocked": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "policyRulesFromGroupPolicyMerged": true
  },
  "firewallProfilePublic": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "blocked",
    "stealthModeBlocked": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "policyRulesFromGroupPolicyMerged": true
  },
  "firewallProfilePrivate": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "blocked",
    "stealthModeBlocked": true,
    "incomingTrafficBlocked": true,
    "unicastResponsesToMulticastBroadcastsBlocked": true,
    "inboundNotificationsBlocked": true,
    "authorizedApplicationRulesFromGroupPolicyMerged": true,
    "globalPortRulesFromGroupPolicyMerged": true,
    "connectionSecurityRulesFromGroupPolicyMerged": true,
    "outboundConnectionsBlocked": true,
    "inboundConnectionsBlocked": true,
    "securedPacketExemptionAllowed": true,
    "policyRulesFromGroupPolicyMerged": true
  },
  "defenderAttackSurfaceReductionExcludedPaths": [
    "Defender Attack Surface Reduction Excluded Paths value"
  ],
  "defenderGuardedFoldersAllowedAppPaths": [
    "Defender Guarded Folders Allowed App Paths value"
  ],
  "defenderAdditionalGuardedFolders": [
    "Defender Additional Guarded Folders value"
  ],
  "defenderExploitProtectionXml": "ZGVmZW5kZXJFeHBsb2l0UHJvdGVjdGlvblhtbA==",
  "defenderExploitProtectionXmlFileName": "Defender Exploit Protection Xml File Name value",
  "defenderSecurityCenterBlockExploitProtectionOverride": true,
  "appLockerApplicationControl": "enforceComponentsAndStoreApps",
  "smartScreenEnableInShell": true,
  "smartScreenBlockOverrideForFiles": true,
  "applicationGuardEnabled": true,
  "applicationGuardBlockFileTransfer": "blockImageAndTextFile",
  "applicationGuardBlockNonEnterpriseContent": true,
  "applicationGuardAllowPersistence": true,
  "applicationGuardForceAuditing": true,
  "applicationGuardBlockClipboardSharing": "blockBoth",
  "applicationGuardAllowPrintToPDF": true,
  "applicationGuardAllowPrintToXPS": true,
  "applicationGuardAllowPrintToLocalPrinters": true,
  "applicationGuardAllowPrintToNetworkPrinters": true,
  "bitLockerDisableWarningForOtherDiskEncryption": true,
  "bitLockerEnableStorageCardEncryptionOnMobile": true,
  "bitLockerEncryptDevice": true,
  "bitLockerRemovableDrivePolicy": {
    "@odata.type": "microsoft.graph.bitLockerRemovableDrivePolicy",
    "encryptionMethod": "aesCbc256",
    "requireEncryptionForWriteAccess": true,
    "blockCrossOrganizationWriteAccess": true
  }
}
```


