# <a name="office-365-active-users-reports"></a>Office 365 活跃用户报表

Office 365 活跃用户报表可用于确定组织中个人使用的产品许可证数，并向下钻取哪些用户使用什么产品的相关信息。 此类报表有助于管理员发现未充分利用的产品或可能需要获取额外培训或信息的用户。

> **注意：**若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 活跃用户](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d)。

## <a name="reports"></a>报表
| 函数                                 | 返回类型 | 说明                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [获取用户详细信息](../api/reportroot_getoffice365activeuserdetail.md) | Stream      | 获取 Office 365 活跃用户的详细信息。 |
| [获取用户数](../api/reportroot_getoffice365activeusercounts.md) | Stream      | 按产品获取报表周期内的每日活跃用户数。 |
| [获取服务用户数](../api/reportroot_getoffice365servicesusercounts.md) | Stream      | 按活动类型和服务获取用户数。 |
