# <a name="update-rule"></a><span data-ttu-id="64f75-101">更新规则</span><span class="sxs-lookup"><span data-stu-id="64f75-101">Update rule</span></span>


<span data-ttu-id="64f75-102">为 [messageRule](../resources/messagerule.md) 对象更改可写属性并保存更改。</span><span class="sxs-lookup"><span data-stu-id="64f75-102">Change writable properties on a [messageRule](../resources/messagerule.md) object and save the changes.</span></span>

## <a name="permissions"></a><span data-ttu-id="64f75-103">权限</span><span class="sxs-lookup"><span data-stu-id="64f75-103">Permissions</span></span>
<span data-ttu-id="64f75-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="64f75-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="64f75-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="64f75-106">Permission type</span></span>      | <span data-ttu-id="64f75-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="64f75-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="64f75-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="64f75-108">Delegated (work or school account)</span></span> | <span data-ttu-id="64f75-109">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="64f75-109">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="64f75-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="64f75-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="64f75-111">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="64f75-111">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="64f75-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="64f75-112">Application</span></span> | <span data-ttu-id="64f75-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="64f75-113">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="64f75-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="64f75-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailFolders/inbox/messagerules/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/inbox/messagerules/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="64f75-115">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="64f75-115">Optional request headers</span></span>
| <span data-ttu-id="64f75-116">名称</span><span class="sxs-lookup"><span data-stu-id="64f75-116">Name</span></span>       | <span data-ttu-id="64f75-117">说明</span><span class="sxs-lookup"><span data-stu-id="64f75-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="64f75-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="64f75-118">Authorization</span></span>  | <span data-ttu-id="64f75-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="64f75-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="64f75-121">请求正文</span><span class="sxs-lookup"><span data-stu-id="64f75-121">Request body</span></span>
<span data-ttu-id="64f75-p103">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="64f75-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="64f75-125">属性</span><span class="sxs-lookup"><span data-stu-id="64f75-125">Property</span></span>     | <span data-ttu-id="64f75-126">类型</span><span class="sxs-lookup"><span data-stu-id="64f75-126">Type</span></span>   |<span data-ttu-id="64f75-127">说明</span><span class="sxs-lookup"><span data-stu-id="64f75-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="64f75-128">actions</span><span class="sxs-lookup"><span data-stu-id="64f75-128">Actions</span></span> | [<span data-ttu-id="64f75-129">messageRuleActions</span><span class="sxs-lookup"><span data-stu-id="64f75-129">messageRuleActions</span></span>](../resources/messageruleactions.md) | <span data-ttu-id="64f75-130">满足相应条件时对邮件执行的操作。</span><span class="sxs-lookup"><span data-stu-id="64f75-130">Actions to be taken on a message when the corresponding conditions are fulfilled.</span></span> |
| <span data-ttu-id="64f75-131">conditions</span><span class="sxs-lookup"><span data-stu-id="64f75-131">Conditions</span></span> | [<span data-ttu-id="64f75-132">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="64f75-132">messageRulePredicates</span></span>](../resources/messagerulepredicates.md) | <span data-ttu-id="64f75-133">满足条件时，将触发该规则的相应操作。</span><span class="sxs-lookup"><span data-stu-id="64f75-133">Conditions that when fulfilled, will trigger the corresponding actions for that rule.</span></span> |
| <span data-ttu-id="64f75-134">displayName</span><span class="sxs-lookup"><span data-stu-id="64f75-134">displayName</span></span> | <span data-ttu-id="64f75-135">String</span><span class="sxs-lookup"><span data-stu-id="64f75-135">String</span></span> | <span data-ttu-id="64f75-136">规则的显示名称。</span><span class="sxs-lookup"><span data-stu-id="64f75-136">The name of the new formatting rule.</span></span> |
| <span data-ttu-id="64f75-137">exceptions</span><span class="sxs-lookup"><span data-stu-id="64f75-137">exceptions</span></span> | [<span data-ttu-id="64f75-138">messageRulePredicates</span><span class="sxs-lookup"><span data-stu-id="64f75-138">messageRulePredicates</span></span>](../resources/messagerulepredicates.md) | <span data-ttu-id="64f75-139">规则的例外情况。</span><span class="sxs-lookup"><span data-stu-id="64f75-139">Exception conditions for the rule.</span></span> |
| <span data-ttu-id="64f75-140">isEnabled</span><span class="sxs-lookup"><span data-stu-id="64f75-140">isEnabled</span></span> | <span data-ttu-id="64f75-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="64f75-141">Boolean</span></span> | <span data-ttu-id="64f75-142">指示是否启用规则以应用到邮件。</span><span class="sxs-lookup"><span data-stu-id="64f75-142">Indicates whether the rule is enabled to be applied to messages.</span></span> |
| <span data-ttu-id="64f75-143">isReadOnly</span><span class="sxs-lookup"><span data-stu-id="64f75-143">IsReadOnly</span></span> | <span data-ttu-id="64f75-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="64f75-144">Boolean</span></span> | <span data-ttu-id="64f75-145">表示规则是否为只读且无法由规则 REST API 修改或删除。</span><span class="sxs-lookup"><span data-stu-id="64f75-145">Indicates if the rule is read-only and cannot be modified or deleted by the rules REST API.</span></span> |
| <span data-ttu-id="64f75-146">Sequence</span><span class="sxs-lookup"><span data-stu-id="64f75-146">Sequence</span></span> | <span data-ttu-id="64f75-147">Int32</span><span class="sxs-lookup"><span data-stu-id="64f75-147">Int32</span></span> | <span data-ttu-id="64f75-148">表示在其他规则中执行规则的顺序。</span><span class="sxs-lookup"><span data-stu-id="64f75-148">Indicates the order in which the rule is executed, among other rules.</span></span> |


## <a name="response"></a><span data-ttu-id="64f75-149">响应</span><span class="sxs-lookup"><span data-stu-id="64f75-149">Response</span></span>
<span data-ttu-id="64f75-150">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [messageRule](../resources/messagerule.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="64f75-150">If successful, this method returns a `200 OK` response code and updated [ChartSeries](../resources/messagerule.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="64f75-151">示例</span><span class="sxs-lookup"><span data-stu-id="64f75-151">Example</span></span>
##### <a name="request"></a><span data-ttu-id="64f75-152">请求</span><span class="sxs-lookup"><span data-stu-id="64f75-152">Request</span></span>
<span data-ttu-id="64f75-153">下面的示例更改规则名称，并更改针对[获取规则](messagerule_get.md)[示例](messagerule_get.md#example)中的规则所采取的操作，从转发到一个地址到将其重要性标记为“高”。</span><span class="sxs-lookup"><span data-stu-id="64f75-153">The following example changes the name of the rule, and the actions to be taken for that rule in the [example](messagerule_get.md#example) in [Get rule](messagerule_get.md), from forwarding to an address to marking its importance as high.</span></span> 
<!-- {
  "blockType": "request",
  "name": "update_messagerule"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/mailfolders/inbox/messagerules('AQAAAJ5dZqA=')

Content-type: application/json

{
    "displayName": "Important from partner",
    "actions": {
        "markImportance": "high"
     }
} 
```
##### <a name="response"></a><span data-ttu-id="64f75-154">响应</span><span class="sxs-lookup"><span data-stu-id="64f75-154">Response</span></span>
<span data-ttu-id="64f75-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="64f75-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.messageRule"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#Me/mailFolders('inbox')/messageRules/$entity",
  "id":"AQAAAJ5dZqA=",
  "displayName":"Important from partner",
  "sequence":2,
  "isEnabled":true,
  "hasError":false,
  "isReadOnly":false,
  "conditions":{
    "senderContains":[
      "ADELE"
    ]
  },
  "actions":{
    "markImportance": "high"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update rule",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->