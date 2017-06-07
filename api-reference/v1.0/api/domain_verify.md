# <a name="domain-verify"></a>域：验证

验证域的所有权。

> **重要说明：**仅适用于未验证的域。对于未验证的域，[域](../resources/domain.md)的 isVerified 属性为 false。

### <a name="prerequisites"></a>先决条件

要执行此 API，需要以下**范围**之一：*Directory.Read.All* 或 *Domain.ReadWrite.All*

### <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->
```http
POST /domains/{id}/verify
```

> 对于 {id}，请使用其完全限定的域名指定该域。

### <a name="request-headers"></a>请求标头

| 名称       | 说明|
|:---------------|:----------|
| 授权  | *需要*持有者&lt;令牌&gt;|
| Content-Type  | application/json |

### <a name="request-body"></a>请求正文

### <a name="response"></a>响应
如果成功，此方法在响应正文中返回 `200, OK` 响应代码和 [domain](../resources/domain.md) 对象。

### <a name="example"></a>示例
##### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "domain_verify"
}-->
```http
POST https://graph.microsoft.com/V1.0/domains/contoso.com/verify
```

##### <a name="response"></a>响应
注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domain"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 192

{
  "authenticationType": "authenticationType-value",
  "availabilityStatus": "availabilityStatus-value",
  "isAdminManaged": true,
  "isDefault": true,
  "isInitial": true,
  "isRoot": true,
  "name": "contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domain: verify",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->