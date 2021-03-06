---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: DateTimeColumn
ms.openlocfilehash: ce5f06b6e0d88324813372c2431b62e6b9105bcb
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/28/2017
---
# <a name="datetimecolumn-resource-type"></a>DateTimeColumn 资源类型

[columnDefinition](columnDefinition.md) 资源上的 **dateTimeColumn** 指示该列的值为日期或时间。

## <a name="json-representation"></a>JSON 表示形式

下面是 **dateTimeColumn** 资源的 JSON 表示形式。
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.dateTimeColumn" } -->

```json
{
  "displayAs": "default | friendly | standard",
  "format": "dateOnly | dateTime"
}
```

## <a name="properties"></a>属性

| 属性名称      | 类型               | 说明
|:-------------------|:-------------------|:----------------------------------------------
| **displayAs**      | string             | 值在用户体验中的显示方式。 必须是 `default`、`friendly` 或 `standard` 的其中一个。 有关更多详细信息，请参阅下文。 如果未指定，则视为 `default`。
| **format**         | string             | 指示值是否应该只显示为日期或日期和时间。 必须是 `dateOnly` 或 `dateTime` 的其中一个

## <a name="displayas-values"></a>DisplayAs 值

| 值        | 说明
|:-------------|:--------------------------------------------------------------
| **default**  | 使用用户体验中呈现的默认值。
| **friendly** | 使用友好相对表示形式（如 “今天下午 3:00”）
| **standard** | 使用标准绝对表示形式（如 “2017 年 5 月 10 日下午 3:20”）


<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/DateTimeColumn"
} -->
