# <a name="microsoft-graph-rest-api-v10-reference"></a>Microsoft Graph REST API 1.0 版参考

欢迎使用 1.0 版终结点的 Microsoft Graph REST API 参考。

1.0 版终结点 (`https://graph.microsoft.com/v1.0`) 上的 API 集处于一般可用 (GA) 状态，并经过与客户进行严格的审查和反馈流程，以满足实际的生产需求。 此终结点上的 API 更新本质上可以累加，并且不会破坏现有应用场景。

## <a name="common-use-cases"></a>常见用例

Microsoft Graph 的强大之处在于可以在单个 Microsoft Graph REST 终结点公开的不同服务之间轻松导航实体和关系。

很多服务旨在围绕[用户](../api-reference/v1.0/resources/user.md)和[组](../api-reference/v1.0/resources/group.md)实现丰富的应用场景。

### <a name="user-centric-use-cases-in-v10"></a>1.0 版中以用户为中心的用例

1. 获取用户 Lisa 的[个人资料](../api-reference/v1.0/api/user_get.md)和[照片](../api-reference/v1.0/resources/profilephoto.md)。
2. [获取 Lisa 的经理的个人资料信息](../api-reference/v1.0/api/user_list_manager.md)和[她的直接下属的 ID](../api-reference/v1.0/api/user_list_directreports.md)，全都存储在 Azure Active Directory 中。
3. [访问 Lisa 在 OneDrive for Business 上的文件](../api-reference/v1.0/api/driveitem_list_children.md)，查找最后修改[文件](../api-reference/v1.0/resources/driveitem.md)的人员的[身份](../api-reference/v1.0/resources/identityset.md)，并导航到此人的个人资料。
4. 在 Exchange Online 中[访问 Lisa 的日历](../api-reference/v1.0/api/calendar_get.md)，并[确定 Lisa 与团队成员在接下来的两周内会面的最佳时间](../api-reference/v1.0/api/user_findmeetingtimes.md)。
5. 在 Lisa 的日历中[订阅](../api-reference/v1.0/api/subscription_post_subscriptions.md)并[跟踪更改](../api-reference/v1.0/api/event_delta.md)，当她花费在会议上的时间超过 80% 时通知她。
6. 设置当 Lisa 不在办公室时的[自动答复](../api-reference/v1.0/api/user_update_mailboxsettings.md#example)。
7. 根据通信、协作和业务关系，[获取与 Lisa 最相关的人员](../api-reference/v1.0/api/user_list_people.md)。
8. 在 Lisa 的 OneDrive for Business 的 Excel 文件中，从一个[图表](../api-reference/v1.0/resources/chart.md)获取最新销售预测。
9. [在 Planner 中查找分配给 Lisa 的任务](../api-reference/v1.0/api/planneruser_list_tasks.md)。

### <a name="office-365-group-use-cases-in-v10"></a>1.0 版中的 Office 365 组用例

1. 针对组织中的 Office 365 组运行报表，并确定[组成员之间通信](../api-reference/v1.0/api/reportroot_getoffice365groupsactivitycounts.md)最多的组。
2. [查找此 Office 365 组的计划](../api-reference/v1.0/api/plannergroup_list_plans.md)，和该计划中的[任务分配](../api-reference/v1.0/resources/plannerassignments.md)。
3. 在 Office 365 组中[启动新对话](../api-reference/v1.0/api/group_post_conversations.md)以确定成员是否需要[创建另一个组](../api-reference/v1.0/api/group_post_groups.md)来分担工作负荷。
4. 为组[获取默认笔记本](../api-reference/v1.0/api/notebook_get.md)并[创建一个页面](../api-reference/v1.0/api/section_post_pages.md)注明调查结果。

## <a name="other-api-versions"></a>其他 API 版本

目前有两个版本的 Microsoft Graph REST API：1.0 版 和 beta 版。
如需了解仍处于预览状态的新 API 或增强 API，请参阅 [Microsoft Graph beta 终结点参考](../api-reference/beta/beta-overview.md)。 请注意，预览状态的 API 可能会发生更改，并可能在无通知的情况下破坏现有应用场景。 不要对 beta 终结点的 API 产生依赖。

请参阅[版本控制和支持](versioning_and_support.md)了解更多信息。

## <a name="connect-with-us"></a>与我们联系

是否希望在 Microsoft Graph 中增加其他 API 或功能？ 在 [UserVoice](https://officespdev.uservoice.com/forums/224641-general/filters/new?category_id=101632) 上发布新功能请求。

对现有 Microsoft Graph API 有反馈意见？ 在 [Github](https://github.com/microsoftgraph/microsoft-graph-docs/issues) 上与我们联系。

如有关于使用 Microsoft Graph 的代码的问题或帮助，请在 [Stack Overflow](https://stackoverflow.com/questions/tagged/microsoftgraph) 上加入我们。
