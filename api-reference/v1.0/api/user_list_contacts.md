# <a name="list-contacts"></a>列出联系人

从已登录用户的默认联系人文件夹中获取联系人集合。


### <a name="get-contacts-in-another-users-contact-folder"></a>获取其他用户的联系人文件夹中的联系人

如果你具有应用程序权限，或者具有某个用户的相应的委派[权限](#permissions)，则可以获取其他用户的联系人文件夹中的联系人。 本部分重点介绍涉及委派权限的应用场景。

例如，你的应用已从用户 John 获得委派权限。 假设另一位用户 Garth 与 John 共享了一个联系人文件夹。 可以通过在下面所示的查询示例中指定 Garth 的用户 ID（或者用户主体名称）获取该共享文件夹中的联系人。

<!-- { "blockType": "ignored" } -->
```http
GET /users/{Garth-id | Garth-userPrincipalName}/contacts
```

此功能适用于对单个用户执行的所有支持的 GET 联系人操作，如下面的 [HTTP 请求](#http-request)部分所示。 如果 Garth 将他的整个邮箱委派给 John，此功能同样适用。

如果 Garth 未与 John 共享他的联系人文件夹，也未将他的邮箱委派给 John，那么在这些 GET 操作中指定 Garth 的用户 ID 或用户主体名称将返回错误。 在这种情况下，指定用户 ID 或用户主体名称只适用于获取已登录用户自己的联系人文件夹中的联系人，而此查询等效于使用 /me 快捷方式：

<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts
```

此功能仅适用于以下资源的 GET 操作：

- 共享联系人文件夹、日历和邮件文件夹 
- 共享文件夹中的联系人、事件和邮件
- 委派邮箱中的上述资源

此功能不适用于针对联系人、事件、邮件及其文件夹的其他操作。


## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Contacts.Read、Contacts.ReadWrite    |
|委派（个人 Microsoft 帐户） | Contacts.Read、Contacts.ReadWrite    |
|应用程序 | Contacts.Read、Contacts.ReadWrite |

## <a name="http-request"></a>HTTP 请求

若要获取用户邮箱中的所有联系人，请执行以下操作：

<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts
GET /users/{id | userPrincipalName}/contacts
```

若要获取用户邮箱中特定文件夹中的联系人，请执行以下操作：

<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders/{Id}/contacts
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts

GET /me/contactFolder/{id}/childFolders/{id}/.../contacts
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts
```
## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持 [OData 查询参数](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) 来帮助自定义响应。

例如，你可以使用 `$filter` 查询参数根据联系人的电子邮件地址的域来过滤联系人：

`https://graph.microsoft.com/v1.0/me/contacts?$filter=emailAddresses/any(a:a/address eq '@domain.com')`



## <a name="request-headers"></a>请求标头
| 标头       | 值 |
|:---------------|:--------|
| Authorization  | Bearer {token}。必需。  |
| Content-Type   | application/json  |

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Contact](../resources/contact.md) 对象集合。
## <a name="example"></a>示例
##### <a name="request"></a>请求
下面是一个请求示例。
<!-- {
  "blockType": "request",
  "name": "get_contacts"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/contacts
```


##### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 263

{
  "value": [
    {
      "parentFolderId": "parentFolderId-value",
      "birthday": "datetime-value",
      "fileAs": "fileAs-value",
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "initials": "initials-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List contacts",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
