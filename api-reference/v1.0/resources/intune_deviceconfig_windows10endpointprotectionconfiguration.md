# <a name="windows10endpointprotectionconfiguration-resource-type"></a>windows10EndpointProtectionConfiguration 资源类型

> **注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

本主题提供由 Windows10EndpointProtectionConfiguration 资源公开的已声明方法、属性和关系的说明。

继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[List windows10EndpointProtectionConfigurations](../api/intune_deviceconfig_windows10endpointprotectionconfiguration_list.md)|[windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md) 集合|列出 [windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md) 对象的属性和关系。|
|[Get windows10EndpointProtectionConfiguration](../api/intune_deviceconfig_windows10endpointprotectionconfiguration_get.md)|[windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md)|读取 [windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md) 对象的属性和关系。|
|[Create windows10EndpointProtectionConfiguration](../api/intune_deviceconfig_windows10endpointprotectionconfiguration_create.md)|[windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md)|创建新的 [windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md) 对象。|
|[Delete windows10EndpointProtectionConfiguration](../api/intune_deviceconfig_windows10endpointprotectionconfiguration_delete.md)|无|删除 [windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md)。|
|[Update windows10EndpointProtectionConfiguration](../api/intune_deviceconfig_windows10endpointprotectionconfiguration_update.md)|[windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md)|更新 [windows10EndpointProtectionConfiguration](../resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。 继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|创建对象的日期/时间。 继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|description|String|管理员提供的设备配置的说明。 继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|displayName|String|管理员提供的设备配置的名称。 继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|version|Int32|设备配置的版本。 继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|firewallBlockStatefulFTP|Boolean|阻止到设备的有状态 FTP 连接|
|firewallIdleTimeoutForSecurityAssociationInSeconds|Int32|配置安全关联的空闲超时（以秒为单位），值范围为从 300 到 3600（包括这两个值）。 这是一个时间段，在此之后安全关联将过期并被删除。 有效值为 300 至 3600。|
|firewallPreSharedKeyEncodingMethod|String|选择要使用的预共享密钥编码 可取值为：`deviceDefault`、`none`、`utF8`。|
|firewallIPSecExemptionsAllowNeighborDiscovery|Boolean|配置 IPSec 免除项以允许邻居发现 IPv6 ICMP 类型代码|
|firewallIPSecExemptionsAllowICMP|Boolean|配置 IPSec 免除项以允许 ICMP|
|firewallIPSecExemptionsAllowRouterDiscovery|Boolean|配置 IPSec 免除项以允许路由器发现 IPv6 ICMP 类型代码|
|firewallIPSecExemptionsAllowDHCP|Boolean|配置 IPSec 免除项以允许 IPv4 和 IPv6 DHCP 通信|
|firewallCertificateRevocationListCheckMethod|String|指定如何执行证书吊销列表 可取值为：`deviceDefault`、`none`、`attempt`、`require`。|
|firewallMergeKeyingModuleSettings|Boolean|如果键控模块不完全支持身份验证集，请指示模块仅忽略不受支持的身份验证套件而不是整个集|
|firewallPacketQueueingMethod|String|配置如何在隧道网关应用场景中应用数据包排队 可取值为：`deviceDefault`、`disabled`、`queueInbound`、`queueOutbound`、`queueBoth`。|
|firewallProfileDomain|[windowsFirewallNetworkProfile](../resources/intune_deviceconfig_windowsfirewallnetworkprofile.md)|配置域网络的防火墙配置文件设置|
|firewallProfilePublic|[windowsFirewallNetworkProfile](../resources/intune_deviceconfig_windowsfirewallnetworkprofile.md)|配置公用网络的防火墙配置文件设置|
|firewallProfilePrivate|[windowsFirewallNetworkProfile](../resources/intune_deviceconfig_windowsfirewallnetworkprofile.md)|配置专用网络的防火墙配置文件设置|
|defenderAttackSurfaceReductionExcludedPaths|String 集合|要从攻击面减少规则中排除的 exe 文件和文件夹的列表|
|defenderGuardedFoldersAllowedAppPaths|String 集合|允许访问受保护文件夹的 exe 路径列表|
|defenderAdditionalGuardedFolders|String 集合|要添加到受保护文件夹列表的文件夹路径列表|
|defenderExploitProtectionXml|Binary|包含有关 Exploit Protection 详细信息的 xml 内容。|
|defenderExploitProtectionXmlFileName|String|从中获取 DefenderExploitProtectionXml 的文件的名称。|
|defenderSecurityCenterBlockExploitProtectionOverride|Boolean|指示是否阻止用户覆盖 Exploit Protection 设置。|
|appLockerApplicationControl|String|使管理员能够选择在设备上允许哪些类型的应用。 可取值为：`notConfigured`、`enforceComponentsAndStoreApps`、`auditComponentsAndStoreApps`、`enforceComponentsStoreAppsAndSmartlocker`、`auditComponentsStoreAppsAndSmartlocker`。|
|smartScreenEnableInShell|Boolean|允许 IT 管理员配置适用于 Windows 的 SmartScreen。|
|smartScreenBlockOverrideForFiles|Boolean|允许 IT 管理员控制用户是否可以忽略 SmartScreen 警告并运行恶意文件。|
|applicationGuardEnabled|Boolean|启用 Windows Defender 应用程序防护|
|applicationGuardBlockFileTransfer|String|阻止剪贴板传输图像文件或文本文件或两者均不阻止 可取值为：`notConfigured`、`blockImageAndTextFile`、`blockImageFile`、`blockNone`、`blockTextFile`。|
|applicationGuardBlockNonEnterpriseContent|Boolean|阻止企业站点加载非企业内容，例如第三方插件|
|applicationGuardAllowPersistence|Boolean|允许 App Guard 容器（收藏夹、Cookie、Web 密码等）内的持久用户生成数据|
|applicationGuardForceAuditing|Boolean|强制审核将存留 Windows 日志和事件以满足安全/合规性条件（示例事件是用户登录注销、特权使用、软件安装、系统更改等）|
|applicationGuardBlockClipboardSharing|String|阻止剪贴板将数据从主机共享到容器或从容器共享到主机，或阻止两种方式，或两种方式均不阻止。 可取值为：`notConfigured`、`blockBoth`、`blockHostToContainer`、`blockContainerToHost`、`blockNone`。|
|applicationGuardAllowPrintToPDF|Boolean|允许从容器打印到 PDF|
|applicationGuardAllowPrintToXPS|Boolean|允许从容器打印到 XPS|
|applicationGuardAllowPrintToLocalPrinters|Boolean|允许从容器打印到本地打印机|
|applicationGuardAllowPrintToNetworkPrinters|Boolean|允许从容器打印到网络打印机|
|bitLockerDisableWarningForOtherDiskEncryption|Boolean|允许管理员禁用对用户计算机上其他磁盘加密的警告提示。|
|bitLockerEnableStorageCardEncryptionOnMobile|Boolean|允许管理员要求使用 BitLocker 开启加密功能。 此策略仅适用于移动 SKU。|
|bitLockerEncryptDevice|Boolean|允许管理员要求使用 BitLocker 开启加密功能。|
|bitLockerRemovableDrivePolicy|[bitLockerRemovableDrivePolicy](../resources/intune_deviceconfig_bitlockerremovabledrivepolicy.md)|BitLocker 可移动驱动器策略。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|assignments|[deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md) 集合|设备配置文件的分配列表。 继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md) 集合|按设备的设备配置安装状态。 继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|userStatuses|[deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md) 集合|按用户的设备配置安装状态。 继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md)|设备配置设备状态概述 继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md)|设备配置用户状态概述 继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md) 集合|设备配置设置状态设备摘要 继承自 [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windows10EndpointProtectionConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10EndpointProtectionConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "firewallBlockStatefulFTP": true,
  "firewallIdleTimeoutForSecurityAssociationInSeconds": 1024,
  "firewallPreSharedKeyEncodingMethod": "String",
  "firewallIPSecExemptionsAllowNeighborDiscovery": true,
  "firewallIPSecExemptionsAllowICMP": true,
  "firewallIPSecExemptionsAllowRouterDiscovery": true,
  "firewallIPSecExemptionsAllowDHCP": true,
  "firewallCertificateRevocationListCheckMethod": "String",
  "firewallMergeKeyingModuleSettings": true,
  "firewallPacketQueueingMethod": "String",
  "firewallProfileDomain": {
    "@odata.type": "microsoft.graph.windowsFirewallNetworkProfile",
    "firewallEnabled": "String",
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
    "firewallEnabled": "String",
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
    "firewallEnabled": "String",
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
    "String"
  ],
  "defenderGuardedFoldersAllowedAppPaths": [
    "String"
  ],
  "defenderAdditionalGuardedFolders": [
    "String"
  ],
  "defenderExploitProtectionXml": "binary",
  "defenderExploitProtectionXmlFileName": "String",
  "defenderSecurityCenterBlockExploitProtectionOverride": true,
  "appLockerApplicationControl": "String",
  "smartScreenEnableInShell": true,
  "smartScreenBlockOverrideForFiles": true,
  "applicationGuardEnabled": true,
  "applicationGuardBlockFileTransfer": "String",
  "applicationGuardBlockNonEnterpriseContent": true,
  "applicationGuardAllowPersistence": true,
  "applicationGuardForceAuditing": true,
  "applicationGuardBlockClipboardSharing": "String",
  "applicationGuardAllowPrintToPDF": true,
  "applicationGuardAllowPrintToXPS": true,
  "applicationGuardAllowPrintToLocalPrinters": true,
  "applicationGuardAllowPrintToNetworkPrinters": true,
  "bitLockerDisableWarningForOtherDiskEncryption": true,
  "bitLockerEnableStorageCardEncryptionOnMobile": true,
  "bitLockerEncryptDevice": true,
  "bitLockerRemovableDrivePolicy": {
    "@odata.type": "microsoft.graph.bitLockerRemovableDrivePolicy",
    "encryptionMethod": "String",
    "requireEncryptionForWriteAccess": true,
    "blockCrossOrganizationWriteAccess": true
  }
}
```



