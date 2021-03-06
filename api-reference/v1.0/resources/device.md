# <a name="device-resource-type"></a>设备资源类型

表示在组织中注册的设备。 可以在云中使用设备注册服务或 Intune 创建设备。 条件访问策略使用它们进行多重身份验证。 这些设备范围很广，从台式机、笔记本电脑到手机和平板电脑均包括在内。 继承自 [directoryObject](directoryobject.md)。

使用此资源，可以使用[扩展](../../../concepts/extensibility_overview.md)将自己的数据添加到自定义属性。


## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[获取设备](../api/device_get.md) | [设备](device.md) |读取 device 对象的属性和关系。|
|[列出设备](../api/device_list.md) | [设备](device.md) 集合| 检索目录中的注册设备列表。 |
|[更新设备](../api/device_update.md) | [设备](device.md) |更新 device 对象的属性。 |
|[删除设备](../api/device_delete.md) | 无 |删除 device 对象。 |
|[列出 registeredOwners](../api/device_list_registeredowners.md) |[directoryObject](directoryobject.md) 集合| 通过 registeredOwners 导航属性，获取身份为设备注册所有者的用户。|
|[列出 registeredUsers](../api/device_list_registeredusers.md) |[directoryObject](directoryobject.md) 集合| 从 registeredUsers 导航属性获取设备的注册用户。|
|**开放扩展**| | |
|[创建开放扩展](../api/opentypeextension_post_opentypeextension.md) |[openTypeExtension](opentypeextension.md)| 创建开放扩展，并将自定义属性添加到新资源或现有资源。|
|[获取开放扩展](../api/opentypeextension_get.md) |[openTypeExtension](opentypeextension.md) 集合| 获取扩展名称标识的开放扩展。|
|**架构扩展**| | |
|[添加架构扩展值](../../../concepts/extensibility_schema_groups.md) || 创建架构扩展定义，然后使用它向资源添加自定义键入数据。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|accountEnabled|Boolean| 启用帐户时为 **true**，否则为 **false**。必需。|
|alternativeSecurityIds|alternativeSecurityId 集合| 仅供内部使用。 不可为 null。 |
|approximateLastSignInDateTime|DateTimeOffset| 时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 (UTC) 如下所示：`'2014-01-01T00:00:00Z'`。只读。 |
|deviceId|Guid| 由 Azure 设备注册服务在设备注册时设置的唯一标识符。 |
|deviceMetadata|String| 仅供内部使用。 设置为 null。 |
|deviceVersion|Int32| 仅供内部使用。 |
|displayName|String|设备显示名称。必需。 |
|id|String|设备唯一标识符。继承自 [directoryObject](directoryobject.md)。密钥，不可为 NULL。只读。|
|isCompliant|Boolean|如果设备符合移动设备管理 (MDM) 策略，则为 **true**；否则；为 **false**。 只读。 |
|isManaged|Boolean|如果设备由移动设备管理 (MDM) 应用进行托管，则为 **true**；否则，为 **false**。|
|onPremisesLastSyncDateTime|DateTimeOffset|对象最后一次与本地目录同步的时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 (UTC) 如下所示：`'2014-01-01T00:00:00Z'`。只读。|
|onPremisesSyncEnabled|Boolean|如果此对象从本地目录同步，则为 **true**；如果此对象最初从本地目录同步，但以后不再同步，则为 **false**；如果此对象从未从本地目录同步，则为 **null**（默认值）。 只读。 |
|operatingSystem|String| 设备上操作系统的类型。必需。 |
|operatingSystemVersion|String|设备上操作系统的版本。必需。 |
|physicalIds|String 集合| 仅供内部使用。 不可为 null。 |
|trustType|String| 加入设备的信任类型。 只读。 可取值为： <br />**Workplace** - 表示*自带个人设备*<br />**AzureAd** - 仅云加入设备<br />**ServerAd** - 加入 Azure AD 的本地域加入设备。 如需了解更多详情，请参阅 [Azure Active Directory 中的设备管理简介](https://docs.microsoft.com/zh-CN/azure/active-directory/device-management-introduction) |

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|extensions|[扩展](extension.md)集合|为设备定义的开放扩展集合。只读。可为 NULL。|
|registeredOwners|[directoryObject](directoryobject.md) 集合|云加入设备或已注册个人设备的用户。 已注册的所有者是在注册时设置。 目前，只能有一个所有者。 只读。 可为 NULL。 |
|registeredUsers|[directoryObject](directoryobject.md) 集合|设备的已注册用户集合。 对于云加入设备和已注册的个人设备，已注册用户在设备注册时设置为与已注册所有者相同的值。 只读。 可为 Null。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "extensions",
    "registeredOwners",
    "registeredUsers"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.device"
}-->

```json
{
  "accountEnabled": true,
  "approximateLastSignInDateTime": "String (timestamp)",
  "deviceId": "string",
  "deviceMetadata": "string",
  "deviceVersion": 1024,
  "displayName": "string",
  "id": "string (identifier)",
  "isCompliant": true,
  "isManaged": true,
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesSyncEnabled": true,
  "operatingSystem": "string",
  "operatingSystemVersion": "string",
  "physicalIds": ["string"],
  "trustType": "string"
}

```

## <a name="see-also"></a>另请参阅

- [使用扩展向资源添加自定义数据](../../../concepts/extensibility_overview.md)
- [使用开放扩展向用户添加自定义数据](../../../concepts/extensibility_open_users.md)
- [使用架构扩展向组添加自定义数据](../../../concepts/extensibility_schema_groups.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "device resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
