# <a name="contact-resource-type"></a>联系人资源类型

联系人是 Outlook 中的一个项目，你可以在这里组织和保存有关你通信的人员和组织的信息。联系人包含在联系人文件夹中。

该资源支持：

- 使用[扩展](../../../concepts/extensibility_overview.md)将自己的数据添加到自定义属性。
- 通过提供 [delta](../api/contact_delta.md) 函数使用[增量查询](../../../concepts/delta_query_overview.md)跟踪增量添加、删除和更新。


## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[获取联系人](../api/contact_get.md) | [联系人](contact.md) |读取 contact 对象的属性和关系。|
|[创建](../api/user_post_contacts.md) | [联系人](contact.md) |将联系人添加到联系人根文件夹或其他联系人文件夹的联系人端点中。|
|[更新](../api/contact_update.md) | [联系人](contact.md) |更新 contact 对象。 |
|[删除](../api/contact_delete.md) | 无 |删除 contact 对象。 |
|[delta](../api/contact_delta.md)|[联系人](contact.md)集合| 获取指定文件夹中已添加、删除或更新的联系人集。|
|**开放扩展**| | |
|[创建开放扩展](../api/opentypeextension_post_opentypeextension.md) |[openTypeExtension](opentypeextension.md)| 创建开放扩展，并在新建或现有的资源实例中添加自定义属性。|
|[获取开放扩展](../api/opentypeextension_get.md) |[openTypeExtension](opentypeextension.md) 集合| 获取通过名称或完全限定的名称识别的一个或多个开放扩展对象。|
|**架构扩展**| | |
|[添加架构扩展值](../../../concepts/extensibility_schema_groups.md) || 创建架构扩展定义，然后使用它向资源添加自定义键入数据。|
|**扩展属性**| | |
|[创建单值扩展属性](../api/singlevaluelegacyextendedproperty_post_singlevalueextendedproperties.md) |[联系人](contact.md)  |在新建或现有的联系人中创建一个或多个单值扩展属性。   |
|[获取具有单值扩展属性的联系人](../api/singlevaluelegacyextendedproperty_get.md)  | [联系人](contact.md) | 通过使用 `$expand` 或 `$filter` 获取包含一个单值扩展属性的联系人。 |
|[创建多值扩展属性](../api/multivaluelegacyextendedproperty_post_multivalueextendedproperties.md) | [联系人](contact.md) | 在新建或现有的联系人中创建一个或多个多值扩展属性。  |
|[获取具有多值扩展属性的联系人](../api/multivaluelegacyextendedproperty_get.md)  | [联系人](contact.md) | 使用 `$expand` 获取包含一个多值扩展属性的联系人。 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|assistantName|String|联系人助理的姓名。|
|birthday|DateTimeOffset|联系人的生日。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`'2014-01-01T00:00:00Z'`|
|businessAddress|[PhysicalAddress](physicaladdress.md)|联系人的公司地址。|
|businessHomePage|String|联系人的公司主页。|
|businessPhones|String collection|联系人的公司电话号码。|
|categories|String collection|与联系人关联的类别。|
|changeKey|String|标识联系人的版本。每次联系人更改时，ChangeKey 也将更改。这样，Exchange 可以将更改应用于该对象的正确版本。|
|children|String collection|联系人子女的姓名。|
|companyName|String|联系人所在公司的名称。|
|createdDateTime|DateTimeOffset|创建联系人的时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`'2014-01-01T00:00:00Z'`|
|部门|String|联系人所在的部门。|
|displayName|String|联系人的显示名称。|
|emailAddresses|[EmailAddress](emailaddress.md) 集合|联系人的电子邮件地址。|
|flag|[followUpFlag](followupflag.md)|指示邮件的状态、开始日期、截止日期或完成日期的标记值。|
|fileAs|String|联系人备案的姓名。|
|generation|String|联系人所属的代。|
|givenName|String|联系人的名。|
|homeAddress|[PhysicalAddress](physicaladdress.md)|联系人的住宅地址。|
|homePhones|String collection|联系人的住宅电话号码。|
|id|String|联系人的唯一标识符。只读。|
|imAddresses|String collection|联系人的即时消息 (IM) 地址。|
|initials|String|联系人的姓名缩写。|
|jobTitle|String|联系人的职务。|
|lastModifiedDateTime|DateTimeOffset|修改联系人的时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`'2014-01-01T00:00:00Z'`|
|manager|String|联系人经理的姓名。
|middleName|String|联系人的中间名。|
|mobilePhone|String|联系人的移动电话号码。|
|nickName|String|联系人的昵称。|
|officeLocation|String|联系人的办公室位置。|
|otherAddress|[PhysicalAddress](physicaladdress.md)|联系人的其他地址。|
|parentFolderId|String|联系人的父文件夹 ID。|
|personalNotes|String|有关联系人的用户备注。|
|profession|String|联系人的职业。|
|spouseName|String|联系人配偶/伴侣的姓名。|
|surname|String|联系人的姓氏。|
|title|String|联系人的职位。|
|yomiCompanyName|String|联系人的注音日文公司名称。|
|yomiGivenName|String|联系人的注音日文名字。|
|yomiSurname|String|联系人的注音日文姓氏。|

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|extensions|[扩展](extension.md)集合|为联系人定义的开放扩展集合。只读。可为 Null。|
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) 集合| 为联系人定义的多值扩展属性的集合。只读。可为 Null。|
|照片|[profilePhoto](profilephoto.md)| 可选的联系人照片。可以获取或设置联系人的照片。|
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection| 为联系人定义的单值扩展属性的集合。只读。可为 Null。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "extensions",
    "multiValueExtendedProperties",
    "photo",
    "singleValueExtendedProperties"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.contact"
}-->

```json
{
  "assistantName": "string",
  "birthday": "String (timestamp)",
  "businessAddress": {"@odata.type": "microsoft.graph.physicalAddress"},
  "businessHomePage": "string",
  "businessPhones": ["string"],
  "categories": ["string"],
  "changeKey": "string",
  "children": ["string"],
  "companyName": "string",
  "createdDateTime": "String (timestamp)",
  "department": "string",
  "displayName": "string",
  "emailAddresses": [{"@odata.type": "microsoft.graph.emailAddress"}],
  "flag": {"@odata.type": "microsoft.graph.followupFlag"},
  "fileAs": "string",
  "generation": "string",
  "givenName": "string",
  "homeAddress": {"@odata.type": "microsoft.graph.physicalAddress"},
  "homePhones": ["string"],
  "id": "string (identifier)",
  "imAddresses": ["string"],
  "initials": "string",
  "jobTitle": "string",
  "lastModifiedDateTime": "String (timestamp)",
  "manager": "string",
  "middleName": "string",
  "mobilePhone": "string",
  "nickName": "string",
  "officeLocation": "string",
  "otherAddress": {"@odata.type": "microsoft.graph.physicalAddress"},
  "parentFolderId": "string",
  "personalNotes": "string",
  "profession": "string",
  "spouseName": "string",
  "surname": "string",
  "title": "string",
  "yomiCompanyName": "string",
  "yomiGivenName": "string",
  "yomiSurname": "string",

  "photo": { "@odata.type": "microsoft.graph.profilePhoto" }
}

```

## <a name="see-also"></a>另请参阅

- [使用增量查询跟踪 Microsoft Graph 数据更改](../../../concepts/delta_query_overview.md)
- [获取文件夹中邮件的增量更改](../../../concepts/delta_query_messages.md)
- [使用扩展向资源添加自定义数据](../../../concepts/extensibility_overview.md)
- [使用开放扩展向用户添加自定义数据](../../../concepts/extensibility_open_users.md)
- [使用架构扩展向组添加自定义数据](../../../concepts/extensibility_schema_groups.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "contact resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
