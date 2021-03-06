---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Drive
ms.openlocfilehash: 0b178967f7eb8da8bdf8584bb13a7d4f9950392b
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/28/2017
---
# <a name="drive-resource-type"></a>Drive 资源类型

驱动器资源是表示用户的 OneDrive 或 SharePoint 中文档库的顶级对象。

OneDrive 用户必须始终具有至少一个可用驱动器，即默认驱动器。没有 OneDrive 许可证的用户不能拥有可用的默认驱动器。

## <a name="json-representation"></a>JSON 表示形式

下面是 Drive 资源的 JSON 表示形式。

**drive** 资源派生自 [**baseItem**](baseitem.md) 并继承该资源的属性。

<!-- { "blockType": "resource", 
       "@odata.type": "microsoft.graph.drive",
       "keyProperty": "id", 
       "optionalProperties": [ "activities", "createdBy", "createdDateTime", "description", "lastModifiedBy", "lastModifiedDateTime", "name", "webUrl", "items", "root", "special", "system"] } -->

```json
{
  "id": "string",
  "createdBy": { "@odata.type": "microsoft.graph.identitySet" },
  "createdDateTime": "string (timestamp)",
  "description": "string",
  "driveType": "personal | business | documentLibrary",
  "items": [ { "@odata.type": "microsoft.graph.driveItem" } ],
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "string (timestamp)",
  "name": "string",
  "owner": { "@odata.type": "microsoft.graph.identitySet" },
  "quota": { "@odata.type": "microsoft.graph.quota" },
  "root": { "@odata.type": "microsoft.graph.driveItem" },
  "special": [ { "@odata.type": "microsoft.graph.driveItem" }],
  "system": { "@odata.type": "microsoft.graph.systemFacet" },
  "webUrl": "url"
}
```

## <a name="properties"></a>属性

| 属性             | 类型                          | 说明                                                                                                                                                                                                                      |
| :------------------- | :---------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| createdBy            | [identitySet][]               | 识别创建项目的用户、设备或应用程序。只读。                                                                                                                                                  |
| createdDateTime      | dateTimeOffset                | 创建项的日期和时间。只读。                                                                                                                                                                                       |
| 说明          | String                        | 提供驱动器的用户可见说明。 读写。
| driveType            | String                        | 说明了由该资源表示的驱动器的类型。OneDrive 个人版驱动器将返回 `personal`。OneDrive for Business 将返回 `business`。SharePoint 文档库将返回 `documentLibrary`。只读。 |
| id                   | String                        | 驱动器唯一标识符。只读。                                                                                                                                                                                   |
| lastModifiedBy       | [identitySet][]               | 上次修改项目的用户、设备和应用程序的标识。只读。                                                                                                                                           |
| lastModifiedDateTime | dateTimeOffset                | 上次修改项目的日期和时间。只读。                                                                                                                                                                             |
| name                 | string                        | 项目名称。读写。                                                                                                                                                                                                |
| 所有者                | [identitySet](identityset.md) | 可选。拥有此驱动器的用户帐户。只读。                                                                                                                                                                       |
| 配额                | [配额](quota.md)             | 可选。有关驱动器的存储空间配额的信息。只读。                                                                                                                                                          |
| sharepointIds        | [sharepointIds][]             | 返回对 SharePoint REST 兼容性有用的标识符。只读。                                                                                                                                                         |
| system               | [systemFacet][]               | 如果存在，则表示这是系统管理的驱动器。 只读。
| WebUrl               | string (url)                  | 在浏览器中显示此资源的 URL。只读。                                                                                                                                                                        |

[identitySet]: identityset.md
[sharepointIds]: sharepointids.md
[systemFacet]: systemfacet.md

## <a name="relationships"></a>关系

| 关系 | 类型                                 | 说明
|:-------------|:-------------------------------------|:-----------------------
| 项目        | [driveitem](driveitem.md) 集合 | 驱动器中包含的所有项。只读。可为 NULL。
| root         | [driveitem](driveitem.md)            | 驱动器的根文件夹。只读。
| special      | [driveitem](driveitem.md) 集合 | OneDrive 中可用的公用文件夹的集合。只读。可为 NULL。

## <a name="methods"></a>方法

|                        常见任务                         |         HTTP 方法         |
| :--------------------------------------------------------- | :-------------------------- |
| [获取其他驱动器的驱动器元数据][drive-get]           | `GET /drives/{drive-id}`    |
| [获取用户默认驱动器的根文件夹][item-get]       | `GET /drive/root`           |
| [列出驱动器下的子项][item-children]             | `GET /drive/root/children`  |
| [列出驱动器中所有项的变更][item-changes]    | `GET /drive/root/delta`     |
| [搜索驱动器中的项][item-search]               | `GET /drive/root/search`    |
| [访问特殊文件夹](../api/drive_get_specialfolder.md) | `GET /drive/special/{name}` |

在上表中，各示例使用的是 `/drive`，但其他路径也同样有效。

[item-resource]: driveitem.md
[identity-set]: identityset.md
[quota-facet]: quota.md
[drive-resource]: drive.md
[drive-get]: ../api/drive_get.md
[item-get]: ../api/driveitem_get.md
[item-changes]: ../api/driveitem_delta.md
[item-search]: ../api/driveitem_search.md
[item-children]: ../api/driveitem_list_children.md


<!-- {
  "type": "#page.annotation",
  "description": "Drive is a top level object for OneDrive API that provides access to the contents of a drive. ",
  "keywords": "drive,objects,resources",
  "section": "documentation",
  "tocPath": "Drives",
  "tocBookmarks": { "Resources/Drive": "#" }
} -->
