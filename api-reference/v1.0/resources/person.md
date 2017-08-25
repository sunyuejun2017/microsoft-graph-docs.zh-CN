# <a name="person-resource-type"></a><span data-ttu-id="656cd-101">person 资源类型</span><span class="sxs-lookup"><span data-stu-id="656cd-101">person resource type</span></span>

<span data-ttu-id="656cd-p101">邮件、联系人和社交网络中关于某个人员的信息聚合。人员可以是当地联系人、社交网络或你所在组织目录中的联系人以及来自最近通信（例如电子邮件和 Skype）的人员。</span><span class="sxs-lookup"><span data-stu-id="656cd-p101">An aggregation of information about a person from across mail, contacts, and social networks. People can be local contacts, contacts from social networking or your organization's directory, and people from recent communications (such as email and Skype).</span></span>

## <a name="methods"></a><span data-ttu-id="656cd-104">方法</span><span class="sxs-lookup"><span data-stu-id="656cd-104">Methods</span></span>

| <span data-ttu-id="656cd-105">方法</span><span class="sxs-lookup"><span data-stu-id="656cd-105">Method</span></span>           | <span data-ttu-id="656cd-106">返回类型</span><span class="sxs-lookup"><span data-stu-id="656cd-106">Return Type</span></span>    |<span data-ttu-id="656cd-107">说明</span><span class="sxs-lookup"><span data-stu-id="656cd-107">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="656cd-108">List people</span><span class="sxs-lookup"><span data-stu-id="656cd-108">List people</span></span>](../api/user_list_people.md) | <span data-ttu-id="656cd-109">**person**</span><span class="sxs-lookup"><span data-stu-id="656cd-109">**Person**</span></span> |<span data-ttu-id="656cd-110">获取按与[用户](../resources/user.md)的相关性排序的人员对象集合。</span><span class="sxs-lookup"><span data-stu-id="656cd-110">Get a collection of person objects ordered by their relevance to the [user](../resources/user.md).</span></span>|
|[<span data-ttu-id="656cd-111">Get person</span><span class="sxs-lookup"><span data-stu-id="656cd-111">Get person</span></span>](../api/person_get.md) | <span data-ttu-id="656cd-112">**person**</span><span class="sxs-lookup"><span data-stu-id="656cd-112">**Person**</span></span> |<span data-ttu-id="656cd-113">获取人员对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="656cd-113">Get the properties and relationships of a device object.</span></span>|


## <a name="properties"></a><span data-ttu-id="656cd-114">属性</span><span class="sxs-lookup"><span data-stu-id="656cd-114">Properties</span></span>
| <span data-ttu-id="656cd-115">属性</span><span class="sxs-lookup"><span data-stu-id="656cd-115">Property</span></span>     | <span data-ttu-id="656cd-116">类型</span><span class="sxs-lookup"><span data-stu-id="656cd-116">Type</span></span>   |<span data-ttu-id="656cd-117">说明</span><span class="sxs-lookup"><span data-stu-id="656cd-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="656cd-118">birthday</span><span class="sxs-lookup"><span data-stu-id="656cd-118">birthday</span></span>|<span data-ttu-id="656cd-119">String</span><span class="sxs-lookup"><span data-stu-id="656cd-119">String</span></span>|<span data-ttu-id="656cd-120">人员的生日。</span><span class="sxs-lookup"><span data-stu-id="656cd-120">The person's birthday.</span></span>|
|<span data-ttu-id="656cd-121">companyName</span><span class="sxs-lookup"><span data-stu-id="656cd-121">companyName</span></span>|<span data-ttu-id="656cd-122">String</span><span class="sxs-lookup"><span data-stu-id="656cd-122">String</span></span>|<span data-ttu-id="656cd-123">人员的公司名称。</span><span class="sxs-lookup"><span data-stu-id="656cd-123">The name of the contact's company.</span></span>|
|<span data-ttu-id="656cd-124">department</span><span class="sxs-lookup"><span data-stu-id="656cd-124">department</span></span>|<span data-ttu-id="656cd-125">String</span><span class="sxs-lookup"><span data-stu-id="656cd-125">String</span></span>|<span data-ttu-id="656cd-126">人员的部门。</span><span class="sxs-lookup"><span data-stu-id="656cd-126">The person's department.</span></span>|
|<span data-ttu-id="656cd-127">displayName</span><span class="sxs-lookup"><span data-stu-id="656cd-127">displayName</span></span>|<span data-ttu-id="656cd-128">String</span><span class="sxs-lookup"><span data-stu-id="656cd-128">String</span></span>|<span data-ttu-id="656cd-129">人员的显示名称。</span><span class="sxs-lookup"><span data-stu-id="656cd-129">The person's display name.</span></span>|
|<span data-ttu-id="656cd-130">scoredEmailAddresses</span><span class="sxs-lookup"><span data-stu-id="656cd-130">scoredEmailAddresses</span></span>|<span data-ttu-id="656cd-131">[scoredEmailAddress](scoredemailaddress.md) collection</span><span class="sxs-lookup"><span data-stu-id="656cd-131">[scoredEmailAddress](scoredemailaddress.md) collection</span></span>|<span data-ttu-id="656cd-132">人员的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="656cd-132">The contact's email addresses.</span></span>|
|<span data-ttu-id="656cd-133">givenName</span><span class="sxs-lookup"><span data-stu-id="656cd-133">givenName</span></span>|<span data-ttu-id="656cd-134">String</span><span class="sxs-lookup"><span data-stu-id="656cd-134">String</span></span>|<span data-ttu-id="656cd-135">人员的名字。</span><span class="sxs-lookup"><span data-stu-id="656cd-135">The contact's given name.</span></span>|
|<span data-ttu-id="656cd-136">id</span><span class="sxs-lookup"><span data-stu-id="656cd-136">id</span></span>|<span data-ttu-id="656cd-137">String</span><span class="sxs-lookup"><span data-stu-id="656cd-137">String</span></span>|<span data-ttu-id="656cd-p102">人员的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="656cd-p102">The group's unique identifier. Read-only.</span></span>|
|<span data-ttu-id="656cd-140">imAddress</span><span class="sxs-lookup"><span data-stu-id="656cd-140">IMAddress</span></span>|<span data-ttu-id="656cd-141">String collection</span><span class="sxs-lookup"><span data-stu-id="656cd-141">String collection</span></span>|<span data-ttu-id="656cd-p103">用户的即时消息 IP 语音 (VOIP) 会话初始协议 (SIP) 地址。只读。</span><span class="sxs-lookup"><span data-stu-id="656cd-p103">The instant message voice over IP (VOIP) session initiation protocol (SIP) addresses for the user. Read-only.</span></span>|
|<span data-ttu-id="656cd-144">isFavorite</span><span class="sxs-lookup"><span data-stu-id="656cd-144">isFavorite</span></span>|<span data-ttu-id="656cd-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="656cd-145">Boolean</span></span>|<span data-ttu-id="656cd-146">如果用户已将此人员标记为常用联系人，则为 `true`。</span><span class="sxs-lookup"><span data-stu-id="656cd-146">`true` if the user has flagged this person as a favorite.</span></span>|
|<span data-ttu-id="656cd-147">jobTitle</span><span class="sxs-lookup"><span data-stu-id="656cd-147">jobTitle</span></span>|<span data-ttu-id="656cd-148">String</span><span class="sxs-lookup"><span data-stu-id="656cd-148">String</span></span>|<span data-ttu-id="656cd-149">人员的职务。</span><span class="sxs-lookup"><span data-stu-id="656cd-149">The contact’s job title.</span></span>|
|<span data-ttu-id="656cd-150">officeLocation</span><span class="sxs-lookup"><span data-stu-id="656cd-150">officeLocation</span></span>|<span data-ttu-id="656cd-151">String</span><span class="sxs-lookup"><span data-stu-id="656cd-151">String</span></span>|<span data-ttu-id="656cd-152">人员的办公室位置。</span><span class="sxs-lookup"><span data-stu-id="656cd-152">The location of the contact's office.</span></span>|
|<span data-ttu-id="656cd-153">personNotes</span><span class="sxs-lookup"><span data-stu-id="656cd-153">personNotes</span></span>|<span data-ttu-id="656cd-154">String</span><span class="sxs-lookup"><span data-stu-id="656cd-154">String</span></span>|<span data-ttu-id="656cd-155">用户对此人员所做的任意格式的备注。</span><span class="sxs-lookup"><span data-stu-id="656cd-155">Free-form notes that the the user has taken about this person.</span></span>|
|<span data-ttu-id="656cd-156">personType</span><span class="sxs-lookup"><span data-stu-id="656cd-156">personType</span></span>|<span data-ttu-id="656cd-157">[personType](persontype.md) collection</span><span class="sxs-lookup"><span data-stu-id="656cd-157">[personType](persontype.md) collection</span></span>|<span data-ttu-id="656cd-158">人员类型。</span><span class="sxs-lookup"><span data-stu-id="656cd-158">The type of person.</span></span>|
|<span data-ttu-id="656cd-159">phones</span><span class="sxs-lookup"><span data-stu-id="656cd-159">phones</span></span>|<span data-ttu-id="656cd-160">[phone](phone.md) collection</span><span class="sxs-lookup"><span data-stu-id="656cd-160">[phone](phone.md) collection</span></span>|<span data-ttu-id="656cd-161">人员的电话号码。</span><span class="sxs-lookup"><span data-stu-id="656cd-161">The user's phone numbers.</span></span>|
|<span data-ttu-id="656cd-162">postalAddresses</span><span class="sxs-lookup"><span data-stu-id="656cd-162">postalAddresses</span></span>|<span data-ttu-id="656cd-163">[location](location.md) collection</span><span class="sxs-lookup"><span data-stu-id="656cd-163">[location](location.md) collection</span></span>|<span data-ttu-id="656cd-164">人员的地址。</span><span class="sxs-lookup"><span data-stu-id="656cd-164">The person's addresses.</span></span>|
|<span data-ttu-id="656cd-165">profession</span><span class="sxs-lookup"><span data-stu-id="656cd-165">profession</span></span>|<span data-ttu-id="656cd-166">String</span><span class="sxs-lookup"><span data-stu-id="656cd-166">String</span></span>|<span data-ttu-id="656cd-167">人员的职业。</span><span class="sxs-lookup"><span data-stu-id="656cd-167">The person's profession.</span></span>|
|<span data-ttu-id="656cd-168">surname</span><span class="sxs-lookup"><span data-stu-id="656cd-168">surname</span></span>|<span data-ttu-id="656cd-169">String</span><span class="sxs-lookup"><span data-stu-id="656cd-169">String</span></span>|<span data-ttu-id="656cd-170">人员的姓氏。</span><span class="sxs-lookup"><span data-stu-id="656cd-170">The person's surname.</span></span>|
|<span data-ttu-id="656cd-171">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="656cd-171">userPrincipalName</span></span>|<span data-ttu-id="656cd-172">String</span><span class="sxs-lookup"><span data-stu-id="656cd-172">String</span></span>|<span data-ttu-id="656cd-p104">人员的用户主体名称 (UPN)。UPN 是人员基于 Internet 标准 [RFC 822](http://www.ietf.org/rfc/rfc0822.txt) 的 Internet 式登录名。按照惯例，此名称应映射到人员的电子邮件名称。常规格式为：别名@域。</span><span class="sxs-lookup"><span data-stu-id="656cd-p104">The user principal name (UPN) of the person. The UPN is an Internet-style login name for the person based on the Internet standard [RFC 822](http://www.ietf.org/rfc/rfc0822.txt). By convention, this should map to the person's email name. The general format is alias@domain.</span></span>|
|<span data-ttu-id="656cd-177">websites</span><span class="sxs-lookup"><span data-stu-id="656cd-177">Websites</span></span>|<span data-ttu-id="656cd-178">[website](website.md) collection</span><span class="sxs-lookup"><span data-stu-id="656cd-178">[website](website.md) collection</span></span>|<span data-ttu-id="656cd-179">人员的网站。</span><span class="sxs-lookup"><span data-stu-id="656cd-179">The person's websites.</span></span>|
|<span data-ttu-id="656cd-180">yomiCompany</span><span class="sxs-lookup"><span data-stu-id="656cd-180">yomiCompany</span></span>|<span data-ttu-id="656cd-181">String</span><span class="sxs-lookup"><span data-stu-id="656cd-181">String</span></span>|<span data-ttu-id="656cd-182">人员所在公司的注音日文名称。</span><span class="sxs-lookup"><span data-stu-id="656cd-182">The phonetic Japanese company name of the contact.</span></span>|

## <a name="relationships"></a><span data-ttu-id="656cd-183">Relationships</span><span class="sxs-lookup"><span data-stu-id="656cd-183">Relationships</span></span>
<span data-ttu-id="656cd-184">无。</span><span class="sxs-lookup"><span data-stu-id="656cd-184">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="656cd-185">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="656cd-185">JSON representation</span></span>

<span data-ttu-id="656cd-186">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="656cd-186">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.person"
}-->

```json
{
  "birthday": "string",
  "companyName": "string",
  "department": "string",
  "displayName": "string",
  "scoredEmailAddresses": [{"@odata.type": "microsoft.graph.scoredemailaddress"}],
  "givenName": "string",
  "id": "string (identifier)",
  "isFavorite": true,
  "jobTitle": "string",
  "officeLocation": "string",
  "personNotes": "string",
  "personType": [{"@odata.type": "microsoft.graph.persontype"}],
  "phones": [{"@odata.type": "microsoft.graph.phone"}],
  "postalAddresses": [{"@odata.type": "microsoft.graph.location"}],
  "profession": "string",
  "surname": "string",
  "userPrincipalName": "string",
  "websites": [{"@odata.type": "microsoft.graph.website"}],
  "yomiCompany": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "person resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->