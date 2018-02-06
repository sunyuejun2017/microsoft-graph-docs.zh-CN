# <a name="delete-conversation"></a><span data-ttu-id="ba7e7-101">删除对话</span><span class="sxs-lookup"><span data-stu-id="ba7e7-101">Delete conversation</span></span>
<span data-ttu-id="ba7e7-102">删除 [conversation](../resources/conversation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ba7e7-102">Delete conversation object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ba7e7-103">权限</span><span class="sxs-lookup"><span data-stu-id="ba7e7-103">Permissions</span></span>
<span data-ttu-id="ba7e7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="ba7e7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ba7e7-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="ba7e7-106">Permission type</span></span>      | <span data-ttu-id="ba7e7-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ba7e7-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ba7e7-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ba7e7-108">Delegated (work or school account)</span></span> | <span data-ttu-id="ba7e7-109">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba7e7-109">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="ba7e7-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ba7e7-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ba7e7-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="ba7e7-111">Not supported.</span></span>    |
|<span data-ttu-id="ba7e7-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="ba7e7-112">Application</span></span> | <span data-ttu-id="ba7e7-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="ba7e7-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ba7e7-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ba7e7-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/conversations/{id}
```

## <a name="request-headers"></a><span data-ttu-id="ba7e7-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="ba7e7-115">Request headers</span></span>
| <span data-ttu-id="ba7e7-116">名称</span><span class="sxs-lookup"><span data-stu-id="ba7e7-116">Name</span></span>       | <span data-ttu-id="ba7e7-117">类型</span><span class="sxs-lookup"><span data-stu-id="ba7e7-117">Type</span></span> | <span data-ttu-id="ba7e7-118">说明</span><span class="sxs-lookup"><span data-stu-id="ba7e7-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ba7e7-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="ba7e7-119">Authorization</span></span>  | <span data-ttu-id="ba7e7-120">string</span><span class="sxs-lookup"><span data-stu-id="ba7e7-120">string</span></span>  | <span data-ttu-id="ba7e7-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ba7e7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ba7e7-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="ba7e7-123">Request body</span></span>
<span data-ttu-id="ba7e7-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ba7e7-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ba7e7-125">响应</span><span class="sxs-lookup"><span data-stu-id="ba7e7-125">Response</span></span>
<span data-ttu-id="ba7e7-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="ba7e7-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ba7e7-128">示例</span><span class="sxs-lookup"><span data-stu-id="ba7e7-128">Example</span></span>
#### <a name="request"></a><span data-ttu-id="ba7e7-129">请求</span><span class="sxs-lookup"><span data-stu-id="ba7e7-129">Request</span></span>
<span data-ttu-id="ba7e7-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ba7e7-130">The following is an example of the request body.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_group_conversation"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/conversations/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgAQABuXO3guDWBMpyKF7LsVwfU=
```

#### <a name="response"></a><span data-ttu-id="ba7e7-131">响应</span><span class="sxs-lookup"><span data-stu-id="ba7e7-131">Response</span></span>
<span data-ttu-id="ba7e7-132">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ba7e7-132">Here is an example of the response.</span></span> 
><span data-ttu-id="ba7e7-133">**注意：**为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="ba7e7-133">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="ba7e7-134">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="ba7e7-134">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete conversation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->