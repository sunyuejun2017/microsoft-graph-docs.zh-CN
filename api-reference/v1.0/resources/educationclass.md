# <a name="educationclass-resource-type"></a>educationClass 资源类型

表示学校的课程。 **educationClass** 资源对应于 Office 365 组并共享同一个 ID。 学生是课程的正式成员，教师为所有者，且具有相应权限。 若要使 Office 体验正常进行，教师必须同时为教师和成员集合的成员。  


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[Get educationClass](../api/educationclass_get.md) | [educationClass](educationclass.md) |读取 **educationClass** 对象的属性和关系。|
|[Add member](../api/educationclass_post_members.md) |[educationUser](educationuser.md)| 通过发布到 members 导航属性，为课程添加一个新的 **educationUser**。|
|[List members](../api/educationclass_list_members.md) |[educationUser](educationuser.md) 集合| 获取 **educationUser** 对象集合。|
|[Remove student](../api/educationclass_delete_members.md) |[educationUser](educationuser.md)| 通过成员导航属性从课程删除 **educationUser**。|
|[List schools](../api/educationclass_list_schools.md) |[educationSchool](educationschool.md) 集合| 获取 **educationSchool** 对象集合。|
|[Add teacher](../api/educationclass_post_teachers.md) |[educationUser](educationuser.md)| 通过发布到 teachers 导航属性，为课程添加一个新的 **educationUser**。|
|[List teachers](../api/educationclass_list_teachers.md) |[educationUser](educationuser.md) 集合| 获取课程的教师列表。|
|[Remove teacher](../api/educationclass_delete_teachers.md) |[educationUser](educationuser.md)| 通过教师导航属性从课程删除 **educationUser**。|
|[Get group](../api/educationclass_get_group.md) |[group](group.md)| 获得与此 **educationClass** 对应的 Office 365 **group**。|
|[Update](../api/educationclass_update.md) | [educationClass](educationclass.md)    |更新 **educationClass** 对象。 |
|[Delete](../api/educationclass_delete.md) | 无 |删除 **educationClass** 对象。 |

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|id| String| 课程的唯一标识符。|
|description|String| 课程说明。|
|displayName|String| 课程名称。|
|mailNickname|String| 向所有成员发送电子邮件的邮件名称（如果已启用）。 |
|createdBy|[identitySet](identityset.md)| 创建了课程的实体 |
|classCode|String| 学校用于标识课程的课程代码。|
|externalId|String| 来自同步系统的课程 ID。 |
|externalName|String|同步系统中的课程名称。|
|externalSource|string| 此课程的创建方式。 可取值为：`sis`、`manual`、`unknownFutureValue`。|
|term|[educationTerm](educationterm.md)|此课程的学期。|


## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|members|[educationUser](../resources/educationuser.md) 集合| 课程中的所有用户。 可为 NULL。|
|schools|[educationSchool](../resources/educationschool.md) 集合| 与此课程相关的所有学校。 可为 NULL。|
|teachers|[educationUser](../resources/educationuser.md) 集合|  课程中的所有教师。 可为 NULL。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationClass"
}-->

```json
{
  "id": "String",
  "description": "String",
  "classCode": "String",
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "displayName": "String",
  "externalId": "String",
  "externalName": "String",
  "externalSource": "string",
  "mailNickname": "String",
  "term": {"@odata.type": "microsoft.graph.education.term"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationClass resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
