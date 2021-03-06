# <a name="invitation-manager"></a>邀请管理器

使用邀请管理器来创建一个邀请，以将外部用户添加到组织。 

邀请进程使用以下流程：

* 创建邀请
* 将邀请发送至邀请的用户（包含邀请链接）
* 邀请的用户单击邀请链接、登录并兑现邀请和创建用户实体表示邀请的用户完成操作
* 兑现完成后，将用户重定向至指定页面

创建邀请会在响应中返回兑现 URL (*inviteRedeemUrl*)。通过将 *sendInvitationMessage* 设置为 true，创建邀请 API 可以自动向邀请的用户发送包含兑现 URL 的电子邮件。还可以自定义要发送至邀请的用户的邮件。反之，如果想要通过一些其他的方法发送兑现 URL，则可以将 *sendInvitationMessage* 设置为 false，然后使用响应中的兑现 URL 创建自己的通信。目前没有可以执行兑现进程的 API。邀请的用户必须单击在上述步骤中的通信中发送的 *inviteRedeemUrl* 链接，并在浏览器中进行交互式兑现流程。完成后，邀请的用户即成为组织中的外部用户。


### <a name="methods"></a>方法
| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[创建邀请](../api/invitation_post.md) | 邀请 | 写入 invitation 对象的属性和关系。|

### <a name="properties"></a>属性
| 属性       | 类型    |说明|
|:---------------|:--------|:----------|
|invitedUserDisplayName|String|被邀请的用户的显示名称。|
|invitedUserEmailAddress|字符串|被邀请的用户的电子邮件地址。必填。|
|invitedUserMessageInfo|[invitedUserMessageInfo](invitedusermessageinfo.md)|要发送至邀请用户的邮件的其他配置，其中包括自定义邮件文本、语言和抄送收件人列表。|
|sendInvitationMessage|Boolean|指示电子邮件是否应发送至邀请的用户。默认值为 false。|
|inviteRedirectUrl|字符串|兑现邀请后，用户应被重定向至的 URL。必填。|
|inviteRedeemUrl|String|用户可用于兑现邀请的 URL。只读|
|invitedUserType|字符串|被邀请的用户的 userType。默认情况下，此值为“来宾”。如果你是公司管理员，则可以以“成员”身份进行邀请。 |
|status|String|邀请的状态。可能的值：Completed、InProgress 和 Error|

### <a name="relationships"></a>关系
| 关系 | 类型    |说明|
|:---------------|:--------|:----------|
|invitedUser|[用户](user.md)|创建为邀请创建进程组成部分的用户。只读|

### <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.invitations" } -->
```json
{
  "invitedUserDisplayName": "string",
  "invitedUserEmailAddress": "string",
  "invitedUserMessageInfo": {"@odata.type": "microsoft.graph.invitedUserMessageInfo"},
  "sendInvitationMessage": false,
  "inviteRedirectUrl": "string",
  "inviteRedeemUrl": "string",
  "status": "string",

  "invitedUser": [{"@odata.type": "microsoft.graph.user"}]
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2016-22-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "invitation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
