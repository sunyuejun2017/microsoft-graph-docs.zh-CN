# <a name="mailbox-usage-reports"></a>邮箱使用情况报表

邮箱使用情况报表可用于获取使用邮箱的用户及其活动级别（主要是以发送和接收的电子邮件数为依据）。 此外，还可以了解每个邮箱占用的存储空间，以及即将达到存储配额的邮箱数。

> **注意：**若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 邮箱使用情况](https://support.office.com/client/Mailbox-usage-beffbe01-ce2d-4614-9ae5-7898868e2729)。

## <a name="reports"></a>报表

| 函数                                 | 返回类型 | 说明                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [获取邮箱详细信息](../api/reportroot_getmailboxusagedetail.md) | Stream      | 获取邮箱使用情况的详细信息。         |
| [获取邮箱数](../api/reportroot_getmailboxusagemailboxcounts.md) | Stream      | 获取组织中的用户邮箱总数和报表周期内的每日活跃邮箱数。 如果用户发送或阅读任何电子邮件，则将邮箱视为活跃邮箱。 |
| [获取配额状态邮箱数](../api/reportroot_getmailboxusagequotastatusmailboxcounts.md) | Stream      | 获取每个配额类别中的用户邮箱数。 |
| [获取存储](../api/reportroot_getmailboxusagestorage.md) | Stream      | 获取组织使用的存储空间。 |
