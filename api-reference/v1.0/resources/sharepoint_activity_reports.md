# <a name="sharepoint-activity-reports"></a>SharePoint 活动报表

SharePoint 活动报表可用于获取每个有权使用 SharePoint 的用户的活动，具体是以用户与文件的交互为依据。 也可以查看以共享文件数为依据的协作级别。

> **注意：**若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - SharePoint 活动](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f)。

## <a name="reports"></a>报表

| 函数                                 | 返回类型 | 说明                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [获取用户详细信息](../api/reportroot_getsharepointactivityuserdetail.md) | Stream      | 获取用户执行的 SharePoint 活动的详细信息。 |
| [获取文件数](../api/reportroot_getsharepointactivityfilecounts.md) | Stream      | 获取与 SharePoint 网站中存储的文件进行交互的唯一许可用户数。 |
| [获取用户数](../api/reportroot_getsharepointactivityusercounts.md) | Stream      | 获取活跃用户数趋势。 如果用户执行了文件活动（保存、同步、修改或共享）或在指定时间内访问了页面，则视为活跃用户。 |
| [获取页面数](../api/reportroot_getsharepointactivitypages.md) | Stream      | 获取用户访问的唯一页面数。 |
