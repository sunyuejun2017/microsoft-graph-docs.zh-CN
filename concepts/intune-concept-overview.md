# <a name="intune-devices-and-apps-api-overview"></a>Intune 设备和应用 API 概述

Microsoft Intune 可帮助企业管理组织内的设备和应用。 你可以使用 Microsoft Graph 中的 Intune API 来管理设备和应用，甚至可以在使用首选工具时配置 Intune。 

如果你是 ISV，则还可以使用 Intune API 来管理客户端租户。

## <a name="why-integrate-with-intune"></a>为什么与 Intune 集成？

你可以使用 Microsoft Graph 中的 Intune API 访问 Intune 设备和应用程序信息，管理设备、管理应用和自动执行 Intune。

### <a name="manage-devices"></a>管理设备

可以使用 Intune API 执行以下操作：

- 定义并强制实施[设备合规性](../api-reference/v1.0/resources/intune_deviceconfig_devicecomplianceactionitem.md)策略，例如密码复杂性和持续时间、加密、威胁保护级别等。  （支持的策略会根据操作系统和版本的不同而异）。
- [保护公司数据](../api-reference/v1.0/resources/intune_mam_windowsinformationprotectionpolicy.md)，无论设备平台是 Windows、Android、Mac 还是 iOS。
- 创建和部署[设备配置](../api-reference/v1.0/resources/intune_deviceconfig_deviceconfiguration.md)策略，包括操作系统平台/版本控制、域成员身份和配置设置管理。
- 创建和部署设备[访问控制](../api-reference/v1.0/resources/intune_onboarding_onpremisesconditionalaccesssettings.md)策略，包括受限的下载、网络附件访问和文件传输。
- 执行[远程操作](../api-reference/v1.0/resources/intune_devices_manageddevice.md)，如定位设备、更改密码和擦除设备。

### <a name="manage-apps"></a>管理应用 

Intune API 可用于执行下列应用管理任务：

- [将应用部署到设备](../api-reference/v1.0/resources/intune_apps_mobileapp.md)或阻止部署应用。
- 管理对[电子书](../api-reference/v1.0/resources/intune_books_ebookinstallsummary.md)及相关服务的访问。
- 定义和部署应用配置设置、应用保护设置和应用使用策略。

### <a name="automate-intune"></a>自动执行 Intune

使用 Intune API 自动执行 Intune 可进行以下操作：

- 定义和分配[基于角色的](../api-reference/v1.0/resources/intune_rbac_conceptual.md)访问控件。
- 审核和报告合规性、使用情况和访问权限。
- 管理[电信费用](../api-reference/v1.0/resources/intune_tem_conceptual.md)。


## <a name="next-steps"></a>后续步骤

- [使用 Azure AD 访问 Intune API](https://docs.microsoft.com/intune/intune-graph-apis)。
- 了解如何使用 [PowerShell Intune 示例](https://github.com/microsoftgraph/powershell-intune-samples)执行常见任务。
- 了解如何[使用 Intune REST API](https://developer.microsoft.com/zh-CN/graph/docs/api-reference/v1.0/resources/intune_graph_overview)。
- 有关 Intune API 中新增功能的信息，请参阅[更改日志](changelog.md)。
- 浏览[示例](https://developer.microsoft.com/zh-CN/graph/graph/examples)，了解有关如何使用 Microsoft Graph 的更多信息。
