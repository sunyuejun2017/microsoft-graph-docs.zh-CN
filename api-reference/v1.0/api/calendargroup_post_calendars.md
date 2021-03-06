# <a name="create-calendar"></a>创建日历

此 API 可用于在[用户](../resources/user.md)的日历组中新建日历。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。

| 权限类型                        | 权限（从最低特权到最高特权） |
| :------------------------------------- | :------------------------------------------ |
| 委派（工作或学校帐户）     | Calendars.ReadWrite                         |
| 委派（个人 Microsoft 帐户） | Calendars.ReadWrite                         |
| 应用程序                            | Calendars.ReadWrite                         |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

用户的默认 [calendarGroup](../resources/calendargroup.md)。

```http
POST /me/calendarGroup/calendars
POST /users/{id | userPrincipalName}/calendarGroup/calendars
```

用户的任意 [calendarGroup](../resources/calendargroup.md)。

```http
POST /me/calendarGroups/{id}/calendars
POST /users/{id | userPrincipalName}/calendarGroups/{id}/calendars
```

## <a name="request-headers"></a>请求标头

| 标头        | 值                       |
| :------------ | :-------------------------- |
| Authorization | Bearer {token}。必需。   |
| Content-Type  | application/json. Required. |

## <a name="request-body"></a>请求正文

在请求正文中，提供 [calendar](../resources/calendar.md) 对象的 JSON 表示形式。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [calendar](../resources/calendar.md) 对象。

## <a name="example"></a>示例

##### <a name="request"></a>请求

下面是一个请求示例。

<!-- {
  "blockType": "request",
  "name": "create_calendar_from_calendargroup"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/calendarGroups/{id}/calendars
Content-type: application/json
Content-length: 78

{
  "name": "name-value",
  "color": {
  }
}
```

在请求正文中，提供 [calendar](../resources/calendar.md) 对象的 JSON 表示形式。

##### <a name="response"></a>响应

下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 98

{
  "name": "name-value",
  "color": {
  },
  "changeKey": "changeKey-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!-- {
  "type": "#page.annotation",
  "description": "Create Calendar",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
