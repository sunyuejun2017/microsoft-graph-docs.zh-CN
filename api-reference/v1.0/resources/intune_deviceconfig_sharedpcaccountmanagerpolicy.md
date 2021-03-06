# <a name="sharedpcaccountmanagerpolicy-resource-type"></a>sharedPCAccountManagerPolicy 资源类型

> **注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

共享电脑帐户管理器策略 仅在启用了帐户管理器时适用。
## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|accountDeletionPolicy|String|配置何时删除帐户。 可取值为：`immediate`、`diskSpaceThreshold`、`diskSpaceThresholdOrInactiveThreshold`。|
|cacheAccountsAboveDiskFreePercentage|Int32|设置在电脑停止删除缓存的共享电脑帐户之前，电脑应有的可用磁盘空间百分比。 仅当 AccountDeletionPolicy 为 DiskSpaceThreshold 或 DiskSpaceThresholdOrInactiveThreshold 时适用。 有效值为 0 至 100|
|inactiveThresholdDays|Int32|指定当帐户在指定时间段内（以天数形式提供）未登录时，将何时开始删除帐户。 仅当 AccountDeletionPolicy 为 DiskSpaceThreshold 或 DiskSpaceThresholdOrInactiveThreshold 时适用。|
|removeAccountsBelowDiskFreePercentage|Int32|设置在删除缓存的帐户以释放磁盘空间之前，电脑上剩余的磁盘空间百分比。 将首先删除处于非活动状态时间最长的帐户。 仅当 AccountDeletionPolicy 为 DiskSpaceThresholdOrInactiveThreshold 时适用。 有效值为 0 至 100|

## <a name="relationships"></a>关系
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.sharedPCAccountManagerPolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.sharedPCAccountManagerPolicy",
  "accountDeletionPolicy": "String",
  "cacheAccountsAboveDiskFreePercentage": 1024,
  "inactiveThresholdDays": 1024,
  "removeAccountsBelowDiskFreePercentage": 1024
}
```



