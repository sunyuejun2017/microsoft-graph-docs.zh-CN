---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: GeoCoordinates
ms.openlocfilehash: 61fc7c117d2da961b1b6d581e21db27d7afe3f31
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/28/2017
---
# <a name="geocoordinates-resource-type"></a>GeoCoordinates 资源类型

**GeoCoordinates** 资源基于文件中包含的元数据提供位置的地理坐标和海拔。如果 [**DriveItem**](driveitem.md) 具有一个非 null **位置**方面，则该项表示一个已知位置和与其相关的文件。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.geoCoordinates"
}-->

```json
{
  "altitude": 1024.13,
  "latitude": 26.13246,
  "longitude": 24.34616
}
```

## <a name="properties"></a>属性

| 属性  | 类型   | 说明
|:----------|:-------|:--------------------------------------------------------
| 海拔  | 双精度数 | 可选。此项高于海平面的高度（以英尺为单位）。只读。
| 纬度  | 双精度数 | 可选。此项的纬度（以十进制表示）。只读。
| 经度 | 双精度数 | 可选。此项的经度（以十进制表示）。只读。

## <a name="remarks"></a>注解

有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem](driveitem.md)。

<!-- {
  "type": "#page.annotation",
  "description": "The location facet provides geographic location related properties for an item",
  "keywords": "location,geographic,item,onedrive",
  "section": "documentation",
  "tocPath": "Facets/Location"
} -->
