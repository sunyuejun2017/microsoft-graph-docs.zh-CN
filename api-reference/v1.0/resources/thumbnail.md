---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: "缩略图"
ms.openlocfilehash: 065c6ae7bbd4f6aca3172afd4399f0a1b5ff3d25
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/28/2017
---
# <a name="thumbnail-resource-type"></a>缩略图资源类型

**缩略图**资源类型表示具有位图表示的图像、视频、文档 或任何项目的缩略图。

## <a name="json-representation"></a>JSON 表示形式

下面是**缩略图**资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": ["content", "height", "width", "sourceItemId"],
  "@odata.type": "microsoft.graph.thumbnail"
}-->

```json
{
  "height": 1024,
  "sourceItemId": "string",
  "url": "string",
  "width": 1024,

  /* relationships */
  "content": "stream"
}
```

## <a name="properties"></a>属性

| 属性     | 类型   | 说明                                                                                                                 |
| :----------- | :----- | :-------------------------------------------------------------------------------------------------------------------------- |
| height       | Int32  | 缩略图高度，以像素为单位。                                                                                     |
| sourceItemId | 字符串 | 提供缩略图的项的唯一标识符。仅当请求某个文件夹缩略图时可用。 |
| url          | String | 用于提取缩略图内容的 URL。                                                                                |
| width        | Int32  | 缩略图宽度，以像素为单位。                                                                                      |

## <a name="relationships"></a>关系

| 名称    | 类型   | 说明                           |
| :------ | :----- | :------------------------------------ |
| 内容 | 流 | 缩略图的内容流。 |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Thumbnail resource represents a single thumbnail for an item.",
  "section": "documentation",
  "tocPath": "Resources/Thumbnail"
} -->
