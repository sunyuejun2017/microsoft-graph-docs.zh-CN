<a id="domaindnsmxrecord-resource-type" class="xliff"></a>
# domainDnsMxRecord 资源类型

表示已添加到租户中特定域的 DNS 区域文件的 MX 记录。继承自 [DomainDnsRecord](domaindnsrecord.md) 实体。

<a id="methods" class="xliff"></a>
## 方法
不支持对该资源进行直接查询。请参阅[域](domain.md)主题了解有关如何查询域服务记录的信息。

<a id="properties" class="xliff"></a>
## 属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|id|字符串| 分配给此实体的唯一标识符。不可为 NULL，只读。|
|isOptional|Boolean| 如果为 false，则客户必须在 DNS 主机上配置 MX 记录才能使 Microsoft Online Services 在域中正常运行。 |
|label|String| 配置 DNS 主机上的 MX 记录的*别名/主机/名称*属性时使用的值。 |
|mailExchange|String| 配置 DNS 主机上的 MX 记录的*答复/目标/值*时使用的值。|
|preference|Int32| 配置 DNS 主机上的 MX 记录的*首选项/优先级*属性时使用的值。 |
|recordType|String| DNS 记录类型。此值始终是 *Mx*。Key |
|supportedService|String| Microsoft Online Service 或与该 Mx 记录存在依赖关系的功能。</br></br>可以为以下值之一：**null**、*Email*、*Sharepoint*、*EmailInternalRelayOnly*、*OfficeCommunicationsOnline*、*SharePointDefaultDomain*、*FullRedelegation*、*SharePointPublic*、*OrgIdAuthentication*、*Yammer*、*Intune* |
|ttl|Int32| 配置 DNS 主机上的 MX 记录的*生存时间 (ttl)* 属性时使用的值。不可为 null |

<a id="relationships" class="xliff"></a>
## 关系
无

<a id="json-representation" class="xliff"></a>
## JSON 表示形式
下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsMxRecord"
}-->

```json
{
  "canonicalName": "String",
  "id": "String (identifier)",
  "isOptional": true,
  "label": "String",
  "mailExchange": "String",
  "preference": 1024,
  "recordType": "String",
  "supportedService": "String",
  "ttl": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domainDnsMxRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->