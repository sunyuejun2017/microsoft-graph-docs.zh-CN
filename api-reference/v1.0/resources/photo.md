---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Photo
ms.openlocfilehash: a4284caa7c20e266d87e22e9b3d729e17bc88abf
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/28/2017
---
# <a name="photo-resource-type"></a>Photo 资源类型

**照片**资源提供 [driveItem](driveitem.md) 中的照片和相机属性，例如 EXIF 元数据。

## <a name="json-representation"></a>JSON 表示形式

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.photo"
}-->
```json
{
  "cameraMake": "string",
  "cameraModel": "string",
  "exposureDenominator": 1000.0,
  "exposureNumerator": 1.0,
  "fNumber": 1.8,
  "focalLength": 22.5,
  "iso": 100,
  "takenDateTime": "String (timestamp)"
}
```

## <a name="properties"></a>属性

| 属性                | 类型           | 说明
|:------------------------|:---------------|:----------------------------------
| **takenDateTime**       | DateTimeOffset | 表示照片拍摄的时间和日期。只读。
| **cameraMake**          | String         | 相机制造商。只读。
| **cameraModel**         | String         | 相机型号。只读。
| **fNumber**             | 双精度数         | 相机的 F-stop 值。只读。
| **exposureDenominator** | Double         | 相机的曝光时间分数的分母。只读。
| **exposureNumerator**   | Double         | 相机的曝光时间分数的分子。只读。
| **focalLength**         | 双精度数         | 相机的焦距。只读。
| **iso**                 | Int64          | 相机的 ISO 值。只读。

## <a name="remarks"></a>注解
OneDrive for Business 和 SharePoint 仅返回 **takenDateTime** 属性。

有关 DriveItem 方面的详细信息，请参阅 [DriveItem](driveitem.md)。
<!-- {
  "type": "#page.annotation",
  "description": "The photo facet provides details about the camera and settings on the camera for photos.",
  "keywords": "camera make,camera model, exposure, f-stop, iso",
  "section": "documentation",
  "tocPath": "Facets/Photo"
} -->
