<a id="licensedetails-resource-type" class="xliff"></a>

# licenseDetails 资源类型

包含已分配给用户的许可证的相关信息。

<a id="methods" class="xliff"></a>

## 方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[List licenseDetails](../api/user_list_licensedetails.md) | licenseDetails collection |检索用户的 licenseDetails 对象列表。|

<!--|[Get licenseDetails](../api/licensedetails_get.md) | licenseDetails |Read properties and relationships of a licenseDetails object.|-->

<a id="properties" class="xliff"></a>

## 属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|id|String| 许可证详细信息对象的唯一标识符。只读，密钥，不可为 NULL |
|servicePlans|[servicePlanInfo](serviceplaninfo.md) collection| 许可证分配的服务计划的相关信息。只读，不可为 Null |
|skuId|Guid| 服务 SKU 的唯一标识符 (GUID)。等同于相关的 [SubscribedSku](subscribedsku.md) 对象上的 skuId 属性。只读 |
|skuPartNumber|String| 唯一的 SKU 显示名称。等同于相关的 [SubscribedSku](subscribedsku.md) 对象上的 skuPartNumber；例如：“AAD_Premium”。只读 |

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
  "@odata.type": "microsoft.graph.licenseDetails"
}-->

```json
{
  "id": "String (identifier)",
  "servicePlans": [{"@odata.type": "microsoft.graph.servicePlanInfo"}],
  "skuId": "Guid",
  "skuPartNumber": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "licenseDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->