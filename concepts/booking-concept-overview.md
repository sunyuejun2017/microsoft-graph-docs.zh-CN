# <a name="microsoft-bookings-api-overview"></a>Microsoft Bookings API 概述

Microsoft Bookings 提供了联机的移动应用，可使小型企业及其客户简单高效地制定预约计划。 任何提供预约服务的小型企业（如汽车维修店、发廊和律师事务所）都可以从管理他们的预订中受益，从而有时间来做一些有助于业务增长的更重要的任务。 拥有 Office 365 商业高级版订阅的企业都可以使用 Microsoft Bookings。

## <a name="why-integrate-with-microsoft-bookings-using-microsoft-graph"></a>为什么使用 Microsoft Graph 与 Microsoft Bookings 集成？

### <a name="streamline-appointment-booking"></a>简化预约流程
当不在电话旁边或下班时间，企业经营者也不会错过客户预订。 客户可以[看到提供的服务](../api-reference/beta/api/bookingbusiness_list_services.md)并随时在日程安排页、企业网站或 Facebook 上直接[预约](../api-reference/beta/api/bookingbusiness_post_appointments.md)。 

企业经营者可以在任何地方（Web 上或移动应用上）亲自或通过电话办理预订。 他们可以[重新安排](../api-reference/beta//api/bookingappointment_update.md)、[取消](../api-reference/beta/api/bookingappointment_cancel.md)现有预订或将其[重新分配](../api-reference/beta/api/bookingappointment_update.md)给其他可用的员工成员。 

### <a name="reduce-no-shows-and-increase-productivity-of-the-staff"></a>减少失约的情况并提高员工的工作效率
企业经营者可以指定[日程安排策略](../api-reference/beta/resources/bookingschedulingpolicy.md)，其中包含最低限度的预订和取消通知，客户可自行计划或重新计划预约。 自动的预约确认和提醒会减少失约情况，并让员工更好地利用他们的生产时间。 

### <a name="manage-customer-information-and-relationships-from-anywhere"></a>从任何位置管理客户信息和关系
完成预约时将自动验证客户是否已在[客户列表](../api-reference/beta/api/bookingbusiness_list_customers.md)上，并根据情况将客户的姓名和电子邮件地址[添加](../api-reference/beta/api/bookingbusiness_post_customers.md)到该列表。 这可使企业经营者方便地与客户保持联系，并定期发送新闻稿或其他宣传材料。

### <a name="integrate-with-productivity-and-team-collaboration-services-in-microsoft-graph"></a>在 Microsoft Graph 中集成工作效率和团队协作服务
使用相同的统一 Microsoft Graph REST 端点，可以访问 Bookings API，并[与 Microsoft 365 的最佳功能进行集成](overview-major-services.md)以支持更丰富的应用场景。 例如，可以使用 [Excel](excel-concept-overview.md#generate-reports-and-analyze-results) 跟踪和分析企业财务数据并生成专业的报表，或者使用 [SharePoint](sharepoint-concept-overview.md) 或 [Microsoft Teams](teams-concept-overview.md) 来增强团队协作。

## <a name="next-steps"></a>后续步骤

详细了解以下信息：

- 
  [Microsoft Bookings](https://support.office.com/zh-CN/article/Publish-your-business-calendar-online-with-Microsoft-Bookings-47403d64-a067-4754-9ae9-00157244c27d) 和其他 [Office 365 商业版应用](https://support.office.com/en-us/article/manage-your-business-apps-in-the-business-center-47eca808-cf96-42ba-83e8-55daf18e49dc?ui=en-US&rs=en-US&ad=US)。
- 在 Microsoft Graph 中[使用 Bookings API](../api-reference/beta/resources/booking-api-overview.md)。

