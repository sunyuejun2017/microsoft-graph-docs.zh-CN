---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SharePointIds
ms.openlocfilehash: 36636ead90d8b913de4328aea9b6252e82f30c26
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/28/2017
---
# <a name="sharepointids-resource-type"></a>SharePointIds 资源类型

**SharePointIds** 资源将存储在 SharePoint 网站或 OneDrive for Business 中的项的各种标识符分组到一个单一结构。

**注意：**OneDrive 个人版返回的项将不包括 **SharePointIds** 方面。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "listId", "listItemId", "listItemUniqueId", "siteId", "siteUrl", "webId" ],
  "@odata.type": "microsoft.graph.sharepointIds"
}-->

```json
{
    "listId": "string",
    "listItemId": "string",
    "listItemUniqueId": "string",
    "siteId": "string",
    "siteUrl": "url",
    "webId": "string"
}
```

## <a name="properties"></a>属性

| 属性         | 类型         | 说明
|:-----------------|:-------------|:-------------------------------------------
| listId           | string       | SharePoint 中的项列表的唯一标识符 (guid)。
| listItemId       | string       | 包含列表中的项的整数标识符。
| listItemUniqueId | string       | OneDrive for Business 或 SharePoint 网站中的项的唯一标识符 (guid)。
| siteId           | string       | 项的网站集 (SPSite) 的唯一标识符 (guid)。
| siteUrl          | string (url) | 包含项的网站的 SharePoint URL。
| webId            | string       | 项的网站集 (SPWeb) 的唯一标识符 (guid)。

## <a name="remarks"></a>注解

有关 **driveItem** 上 facet 的详细信息，请参阅 [**driveItem**](driveitem.md)。



<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The SharepointIds facet provides Sharepoint ids associated with an item.",
  "keywords": "item, unique, id, csom, facet",
  "section": "documentation",
  "tocPath": "Facets/SharepointIds"
} -->
