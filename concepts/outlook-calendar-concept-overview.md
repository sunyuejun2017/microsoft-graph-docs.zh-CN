# <a name="outlook-calendar-api-overview"></a>Outlook 日历 API 概述

Outlook 日历是 Office 365 中 Outlook 消息传递中心的一部分，它同样允许你管理电子邮件和联系人、在组织中查找有关用户的信息、启动在线对话、共享文件，以及实现小组协作。

## <a name="why-integrate-with-outlook-calendar"></a>为什么与 Outlook 日历集成？

### <a name="reach-hundreds-of-millions-of-customers-and-build-rich-scenarios"></a>覆盖数以亿计的客户并构建丰富的应用场景

数以百万计的客户使用 Outlook 日历作为集成中心的一部分，他们可以借此有效地沟通和完成任务。 他们可以设置会议、管理电子邮件、查找有关联系人和其他用户的信息，并可在一个位置启动对话或在线会议，比如 Web、移动或桌面设备。 Microsoft Graph 不仅可将应用连接到日历、邮件以及这些客户的联系人数据，还可使应用[与 Microsoft 365 的最佳功能进行集成](overview-major-services.md)，并支持各种各样的应用场景，以提高工作效率和协作。

### <a name="automate-appointment-organization-and-calendaring"></a>自动化约会组织和日历功能

客户希望 Outlook 帮助他们合理安排用于工作、家庭和个人活动的时间。 Microsoft Graph REST API 与客户体验保持密切对等，以便应用可以自然地创建、管理和响应事件：

- 在 Outlook 中，客户可以针对工作、家庭或其他目的创建单个日历，并在日历组中加以组织。 他们可以启用免费的**生日**和**节假日**日历，提醒他们联系人的生日和本地假日。 也可以添加匹配其兴趣的日历，如有关运动队和电视节目的日历。 客户可以选择和叠加日历，并在同一个视图中查看他们的事件。 在日历 API 中，应用可以按照类似的方式组织[日历组](../api-reference/v1.0/resources/calendargroup.md)中的[日历](../api-reference/v1.0/resources/calendar.md)，然后就像与用户邮箱中的任何其他**日历**一样与感兴趣的日历进行交互。 

- Outlook 客户可通过一致的方式将类别应用到事件、邮件、联系人、任务和组文章中来加强组织和发现。 使用日历 API，你可以访问和[定义用户的主类别列表](../api-reference/v1.0/api/outlookuser_post_mastercategories.md)，从而开发其他创造性的应用场景。 例如，体育俱乐部可以组织一场体育赛事，并提供一款应用，将每一项运动的电子邮件和事件按器自己的颜色类别区分开来。 对于诸如不可预见的时间表变化等最新新闻，这款应用还可以设置这些事件和电子邮件的**重要性**属性来提醒用户。

- 在日历文件夹中，可以[创建](../api-reference/v1.0/api/user_post_events.md)和[更新](../api-reference/v1.0/api/event_update.md)单个实例[事件](../api-reference/v1.0/resources/event.md)，或[安排和维护定期事件](outlook-schedule-recurring-events.md)。 你可以让客户使用关联的**事件**导航属性来响应[会议请求](../api-reference/v1.0/resources/eventmessage.md)，以及[推迟](../api-reference/v1.0/api/event_snoozereminder.md)或[直接关闭](../api-reference/v1.0/api/event_dismissreminder.md)[提醒](../api-reference/v1.0/resources/reminder.md)。


### <a name="help-customers-stay-synchronized-and-navigate-their-day"></a>帮助客户保持同步并浏览他们的日期

日历 API 可帮助客户浏览他们的日期并提高效率：

<!-- change link to notifications to the concept topic once it's created. In general, try staying in the conceptual level in these overview topics, if conceptual topics are available for the link destination. 
-->

- 可以通过订阅用户日历中的[更改通知](../api-reference/v1.0/resources/webhooks.md)和[跟踪事件更改](delta_query_events.md)使应用本地存储保持同步。
- 可以基于轻型[提醒视图](../api-reference/v1.0/api/user_reminderview.md)显示用户日程。 
- 可以方便地让用户[接受](../api-reference/v1.0/api/event_accept.md)并通过其 **webLink** 属性参与在线会议，这会在 Outlook 网页版中打开会议。
- 外出途中，用户还可以[暂时接受](../api-reference/v1.0/api/event_tentativelyaccept.md)或[拒绝](../api-reference/v1.0/api/event_decline.md)会议。

### <a name="enhance-collaboration"></a>增强协作

- 在 Outlook 中，客户可以与他人共享日历并授予读取、写入或删除日历内容的权限。 或者，他们可以委派一个日历，让另一个客户代表他们响应会议请求。 通过编程方式，虽然无法代表用户启动共享或委派操作，但可以使用一组属性来验证共享状态并启用有关共享或委派日历的应用场景：**canEdit**、**canShare**、**canViewPrivateItems**、**isShared** 和 **isSharedWithMe**。
- 日历 API 使你能够获得已登录用户或将其日历共享或委派给已登录用户的用户的日历项目。 例如，如果 Garth 与 John 共享日历，或者如果 Garth 向 John 委派了访问权限，则来自 John 的[委派权限](permissions_reference.md#delegated-permissions-application-permissions-and-effective-permissions)将授予你对 Garth 共享日历和内容的读取访问权限。
- ** Office 365 组可使组成员方便地直接在 Outlook 中进行协作、访问组对话和日历。 除了组日历和用户日历之间的一些细微差异外，通过日历 API 可像与用户日历那样与组日历进行交互。 请参阅[日历](../api-reference/v1.0/resources/calendar.md)资源了解详细信息。

** 表示在工作或学校帐户中专门适用于 Outlook 日历的功能。


### <a name="schedule-smart"></a>智能日程安排

Outlook 和日历 API 提供了很多智能便利的功能来安排事件：

- 在 Outlook 日历应用设置中，客户可以启用在电子邮件中自动添加事件，如航班、酒店或就餐预订，以及开具发票等。 添加后，即可像用户邮箱中的任何其他[事件](../api-reference/v1.0/resources/event.md)那样与这些事件交互，并借此 Outlook 功能生成创造性应用场景。
- ** 在 Outlook 中，预订会议室就像添加**事件**与会者那样简单。 日历 API 将会议室表示为 [emailAddress](../api-reference/v1.0/resources/emailaddress.md) 对象。 可以[获取租户中可用的会议室](../api-reference/beta/api/user_findrooms.md)并[获取会议室列表](../api-reference/beta/api/user_findroomlists.md)。 若要在特定房间内组织会议，请将其分配给**事件**的 **location** 属性。
- ** 你可以进一步[使用 findMeetingTimes 来标识开会的可能时间或地点](findmeetingtimes_example.md)。 [FindMeetingTimes](../api-reference/v1.0/api/user_findmeetingtimes.md) 函数会考虑与会者的闲/忙状态，以及你所提供的任何首选房间、时间和其他限制。 如果首次尝试未返回常见的会议时间，请检查原因，调整条件并再次调用 **findMeetingTimes**。


### <a name="teleconference-across-multiple-locations-and-time-zones"></a>跨多个地点和时区的电话会议

在全球化背景下，当今的商务会议通常涉及来自不同地点和时区的与会者。 下面介绍了如何使用日历 API 来管理此类会议：

- 如 Outlook 中的一个示例所示，客户可以组织一场会议，并包括从西雅图会议室、巴黎咖啡店和中国家庭办公室加入的与会者。 通过编程方式，事件 **locations** 属性（[location](../api-reference/v1.0/resources/location.md) 对象集合）可反映每个 **location** 的 **displayName** 和 **locationType** 中此级别的详细信息。 请参阅[示例](../api-reference/v1.0/api/event_get.md#request-2)。
- Outlook 为客户提供了组织事件和针对每个事件的开始和结束时间指定一个时区的灵活性。 为了支持这种灵活性，默认情况下，日历 API 会以 UTC 格式返回**事件**的**开始**和**结束**时间，并提供 **originalStartTimeZone** 和 **originalEndTimeZone** 属性，以记录创建事件时使用的时区。 
- 或者，可以指定 `Prefer: outlook.timezone="{time zone name}"` 标头，以便 GET 事件操作返回指定时区的**开始**和**结束**时间。 时区名称可以是 Windows 支持的任何名称，也可以是此[列表](../api-reference/v1.0/resources/datetimetimezone.md)上的这些名称。 请参阅使用中的 `Prefer` 标头[示例](../api-reference/v1.0/api/event_get.md#request-1)


### <a name="take-advantage-of-social-intelligence-and-other-developer-conveniences-in-microsoft-graph"></a>利用 Microsoft Graph 的社交智能以及其他开发者的便利性

使用 Microsoft Graph 中的[人员 API](people_example.md) 连接到[人员数据](../api-reference/v1.0/resources/person.md)，这基于用户的通信和协作模式以及业务关系。 你可以实现诸如人员选取器等控件，并在代表用户组织会议时建议与用户相关的人员。

节省在外部数据存储中存储和管理应用数据的开销。 使用 Microsoft Graph，可以在各个资源实例中将自定义应用数据存储为[开放扩展](extensibility_overview.md#open-extensions)。 如果需要键入数据，或者希望能够共享类型化架构，可以将自定义应用数据存储在[架构扩展](extensibility_overview.md#schema-extensions)中。


## <a name="next-steps"></a>后续步骤

- 在 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer/?request=me%2Fevents&version=v1.0)中选择和试用日历示例查询。
- 了解以下信息：
  - [在 Outlook 日历上找到可能的会议时间](findmeetingtimes_example.md)
  - [在 Outlook 中将重复约会安排为定期事件](outlook-schedule-recurring-events.md)
- 查看 Outlook [日历 API](../api-reference/v1.0/resources/calendar.md) 引用。

<!-- Replace the last item with the calendar API overview when it's published.
-->
