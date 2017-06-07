# <a name="create-domain"></a>创建域

向租户添加域。

**重要说明**：必须完成所有权验证，才可以使用与 Azure AD 租户关联的域。有关详细信息，请参阅[列出 verificationDnsRecords](domain_list_verificationdnsrecords.md)。需要对根域进行验证。例如，需要对 contoso.com 进行验证。如果已验证根域，则将自动验证该根域的子域。例如，如果已验证 contoso.com，则将自动验证 subdomain.contoso.com。

### <a name="prerequisites"></a>先决条件

要执行此 API，需要以下**范围**之一：*Domain.ReadWrite.All* 或 *Directory.AccessAsUser.All*

### <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->
```http
POST /domains
```
### <a name="request-headers"></a>请求标头
| 名称       | 说明|
|:---------------|:----------|
| 授权  | *需要*持有者&lt;令牌&gt;|
| Content-Type  | application/json |

### <a name="request-body"></a>请求正文
在请求正文中，提供 [domain](../resources/domain.md) 对象的 JSON 表示形式。

> 请求正文包含新域的 id 属性。Id 是唯一可以指定，也是必须指定的属性。此 id 属性值是要创建的完全限定的域名。

### <a name="response"></a>响应
如果成功，此方法在响应正文中返回 `201, Created` 响应代码和 [domain](../resources/domain.md) 对象。

### <a name="example"></a>示例
##### <a name="request"></a>请求

在请求正文中，提供 [domain](../resources/domain.md) 对象的 JSON 表示形式。

<!-- {
  "blockType": "request",
  "id": "create_domain_from_domains"
}-->
```http
POST https://graph.microsoft.com/V1.0/domains
Content-type: application/json
Content-length: 192

{
  "id": "contoso.com"
}
```

##### <a name="response"></a>响应
注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domain"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 192

{
  "authenticationType": "authenticationType-value",
  "availabilityStatus": "availabilityStatus-value",
  "id": "contoso.com",
  "isAdminManaged": true,
  "isDefault": true,
  "isInitial": true,
  "isRoot": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create domain",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->