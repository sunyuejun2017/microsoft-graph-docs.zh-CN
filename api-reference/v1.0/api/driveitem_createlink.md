---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: "使用链接共享文件"
ms.openlocfilehash: 342e6ce403225a5d4b8b555a79355a721055e465
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/28/2017
---
# <a name="create-a-sharing-link-for-a-driveitem"></a>为 DriveItem 创建共享链接

可以使用 **createLink** 操作通过共享链接共享 [DriveItem](../resources/driveitem.md)。

如果调用应用程序指定的链接类型尚不存在，**CreateLink** 操作将创建新的共享链接。如果应用程序指定的共享链接类型已存在，则返回现有的共享链接。

DriveItem 资源从其上级继承共享权限。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All    |
|委派（个人 Microsoft 帐户） | Files.ReadWrite、Files.ReadWrite.All    |
|应用程序 | Files.ReadWrite.All、Sites.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/createLink
POST /groups/{groupId}/drive/items/{itemId}/createLink
POST /me/drive/items/{itemId}/createLink
POST /sites/{siteId}/drive/items/{itemId}/createLink
POST /users/{userId}/drive/items/{itemId}/createLink
```

### <a name="request-body"></a>请求正文

请求正文定义应用程序正在请求的共享链接的属性。
请求应为具有以下属性的 JSON 对象。

|   名称    |  类型  |                                 说明                                  |
| :-------- | :----- | :--------------------------------------------------------------------------- |
| **类型**  | string | 要创建的共享链接的类型。`view`、`edit` 或 `embed`。       |
| **scope** | string | 可选。 要创建的链接的范围。 `anonymous` 或 `organization`。 |


### <a name="link-types"></a>链接类型

**type** 参数允许使用以下值：

| 类型值 | 说明                                                                                  |
|:-----------|:---------------------------------------------------------------------------------------------|
| `view`     | 创建到 DriveItem 的只读链接。                                                        |
| `edit`     | 创建到 DriveItem 的读写链接。                                                       |
| `embed`    | 创建到 DriveItem 的可嵌入链接。 此选项仅适用于 OneDrive 个人版中的文件。 |

### <a name="scope-types"></a>范围类型

**scope** 参数允许使用以下值。
如果未指定 **scope** 参数，则为组织创建默认的链接类型。

| 类型值     | 说明                                                                                                                   |
|:---------------|:------------------------------------------------------------------------------------------------------------------------------|
| `anonymous`    | 创建到任意用户都可使用链接访问的 DriveItem 的链接。 管理员可禁用匿名链接。                 |
| `organization` | 创建到用户组织内的任意用户都可访问的 DriveItem 的链接。 OneDrive 个人版不支持组织链接范围。 |

## <a name="response"></a>响应

如果成功，此方法将在响应正文中返回单个 [Permission](../resources/permission.md) 资源，此响应正文表示请求的共享权限。

如果已经为此项目创建新的共享链接，则响应为 `201 Created`；如果返回现有链接，则为 `200 OK`。

## <a name="example"></a>示例

下面的示例请求为在用户的 OneDrive 中按 {itemId} 指定的 DriveItem 创建共享链接。
共享链接配置为只读并且可由具有该链接的任何用户使用。

### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "item_createlink"
}-->

```http
POST /me/drive/items/{itemId}/createLink
Content-type: application/json

{
  "type": "view",
  "scope": "anonymous"
}
```

### <a name="response"></a>响应

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.permission" } -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "123ABC",
  "roles": ["write"],
  "link": {
    "type": "view",
    "scope": "anonymous",
    "webUrl": "https://1drv.ms/A6913278E564460AA616C71B28AD6EB6",
    "application": {
      "id": "1234",
      "displayName": "Sample Application"
    },
  }
}
```

## <a name="creating-company-sharable-links"></a>创建公司可共享的链接

OneDrive for Business 和 SharePoint 都支持公司可共享的链接。
此类链接与匿名链接类似，只不过仅适用于拥有组织的成员。
若要创建公司可共享的链接，请使用值为 `organization` 的 **scope** 参数。

### <a name="request"></a>请求

<!-- { "blockType": "request", "name": "create-link-scoped", "scopes": "files.readwrite service.sharepoint" } -->

```http
POST /me/drive/items/{item-id}/createLink
Content-Type: application/json

{
  "type": "edit",
  "scope": "organization"
}
```

### <a name="response"></a>响应

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.permission" } -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "123ABC",
  "roles": ["write"],
  "link": {
    "type": "edit",
    "scope": "organization",
    "webUrl": "https://contoso-my.sharepoint.com/personal/ellen_contoso_com/...",
    "application": {
      "id": "1234",
      "displayName": "Sample Application"
    },
  }
}
```

## <a name="creating-embeddable-links"></a>创建可嵌入的链接

使用 `embed` 链接类型时，可以在 `<iframe>` HTML 元素中嵌入返回的 webUrl。创建嵌入链接时，`webHtml` 属性包含 `<iframe>` 的 HTML 代码以托管内容。

**注意：**仅 OneDrive 个人版支持嵌入链接。

### <a name="request"></a>请求

<!-- { "blockType": "request", "name": "create-embedded-link", "scopes": "files.readwrite service.onedrive" } -->

```http
POST /me/drive/items/{item-id}/createLink
Content-Type: application/json

{
  "type": "embed"
}
```

### <a name="response"></a>响应

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.permission" } -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "123ABC",
  "roles": ["read"],
  "link": {
    "type": "embed",
    "webHtml": "<IFRAME src=\"https://onedrive.live.com/...\"></IFRAME>",
    "webUrl": "https://onedive.live.com/...",
    "application": {
      "id": "1234",
      "displayName": "Sample Application"
    },
  }
}
```

## <a name="remarks"></a>注解

* 使用此操作创建的链接不会过期，除非对组织强制执行了默认过期策略。
* 链接在项的共享权限中可见，可以由该项的所有者删除。
* 除非项已被签出，否则链接始终指向该项的最新版本（仅限 SharePoint）。

<!-- {
  "type": "#page.annotation",
  "description": "Create a new sharing link for an item.",
  "keywords": "create,sharing,sharing link",
  "section": "documentation",
  "tocPath": "Sharing/Create link"
} -->
