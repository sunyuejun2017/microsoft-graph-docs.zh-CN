# <a name="educationroot-resource-type"></a><span data-ttu-id="5fbb2-101">educationRoot 资源类型</span><span class="sxs-lookup"><span data-stu-id="5fbb2-101">educationRoot resource type</span></span>

<span data-ttu-id="5fbb2-102">`/education` 命名空间公开特定于教育部门的功能。</span><span class="sxs-lookup"><span data-stu-id="5fbb2-102">The `/education` namespace exposes functionality that is specific to the education sector.</span></span> <span data-ttu-id="5fbb2-103">`/education` 命名空间中的一些对象可在 Microsoft Graph 的其他部分中找到（例如，[users](user.md)）。</span><span class="sxs-lookup"><span data-stu-id="5fbb2-103">Some objects in the `/education` namespace can be found in other parts of Microsoft Graph (for example, [users](user.md)).</span></span> <span data-ttu-id="5fbb2-104">教育命名空间提供有关这些对象特定于教育的属性和功能。</span><span class="sxs-lookup"><span data-stu-id="5fbb2-104">The education namespace provides education-specific properties and features on these objects.</span></span>

## <a name="methods"></a><span data-ttu-id="5fbb2-105">方法</span><span class="sxs-lookup"><span data-stu-id="5fbb2-105">Methods</span></span>

| <span data-ttu-id="5fbb2-106">方法</span><span class="sxs-lookup"><span data-stu-id="5fbb2-106">Method</span></span>           | <span data-ttu-id="5fbb2-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="5fbb2-107">Return Type</span></span>    |<span data-ttu-id="5fbb2-108">说明</span><span class="sxs-lookup"><span data-stu-id="5fbb2-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5fbb2-109">Create educationClass</span><span class="sxs-lookup"><span data-stu-id="5fbb2-109">Create educationClass</span></span>](../api/educationroot_post_classes.md) |[<span data-ttu-id="5fbb2-110">educationClass</span><span class="sxs-lookup"><span data-stu-id="5fbb2-110">educationClass</span></span>](educationclass.md)| <span data-ttu-id="5fbb2-111">通过发布到 classes 集合创建新的 **educationClass**。</span><span class="sxs-lookup"><span data-stu-id="5fbb2-111">Create a new **plannerTask** by posting to the tasks collection.</span></span>|
|[<span data-ttu-id="5fbb2-112">List classes</span><span class="sxs-lookup"><span data-stu-id="5fbb2-112">List classes</span></span>](../api/educationroot_list_classes.md) |<span data-ttu-id="5fbb2-113">[educationClass](educationclass.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5fbb2-113">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="5fbb2-114">获取 **educationClass** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="5fbb2-114">Get an **educationClass** object collection.</span></span>|
|[<span data-ttu-id="5fbb2-115">Create educationSchool</span><span class="sxs-lookup"><span data-stu-id="5fbb2-115">Create educationSchool</span></span>](../api/educationroot_post_schools.md) |[<span data-ttu-id="5fbb2-116">educationSchool</span><span class="sxs-lookup"><span data-stu-id="5fbb2-116">educationSchool</span></span>](educationschool.md)| <span data-ttu-id="5fbb2-117">通过发布到 schools 集合创建新的 **educationSchool**。</span><span class="sxs-lookup"><span data-stu-id="5fbb2-117">Create a new **plannerTask** by posting to the tasks collection.</span></span>|
|[<span data-ttu-id="5fbb2-118">List schools</span><span class="sxs-lookup"><span data-stu-id="5fbb2-118">List schools</span></span>](../api/educationroot_list_schools.md) |<span data-ttu-id="5fbb2-119">[educationSchool](educationschool.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5fbb2-119">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="5fbb2-120">获取 **educationSchool** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="5fbb2-120">Get an **educationSchool** object collection.</span></span>|
|[<span data-ttu-id="5fbb2-121">Create educationUser</span><span class="sxs-lookup"><span data-stu-id="5fbb2-121">Create educationUser</span></span>](../api/educationroot_post_users.md) |[<span data-ttu-id="5fbb2-122">educationUser</span><span class="sxs-lookup"><span data-stu-id="5fbb2-122">educationUser</span></span>](educationuser.md)| <span data-ttu-id="5fbb2-123">通过发布到 users 集合创建新的 **educationUser**。</span><span class="sxs-lookup"><span data-stu-id="5fbb2-123">Create a new user by posting to the users collection.</span></span>|
|[<span data-ttu-id="5fbb2-124">List users</span><span class="sxs-lookup"><span data-stu-id="5fbb2-124">List users</span></span>](../api/educationroot_list_users.md) |<span data-ttu-id="5fbb2-125">[educationUser](educationuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5fbb2-125">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="5fbb2-126">获取 **educationUser** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="5fbb2-126">Get an **educationUser** object collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="5fbb2-127">属性</span><span class="sxs-lookup"><span data-stu-id="5fbb2-127">Properties</span></span>
<span data-ttu-id="5fbb2-128">无。</span><span class="sxs-lookup"><span data-stu-id="5fbb2-128">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="5fbb2-129">关系</span><span class="sxs-lookup"><span data-stu-id="5fbb2-129">Relationships</span></span>
| <span data-ttu-id="5fbb2-130">关系</span><span class="sxs-lookup"><span data-stu-id="5fbb2-130">Relationship</span></span> | <span data-ttu-id="5fbb2-131">类型</span><span class="sxs-lookup"><span data-stu-id="5fbb2-131">Type</span></span>   |<span data-ttu-id="5fbb2-132">说明</span><span class="sxs-lookup"><span data-stu-id="5fbb2-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5fbb2-133">classes</span><span class="sxs-lookup"><span data-stu-id="5fbb2-133">Classes</span></span>|<span data-ttu-id="5fbb2-134">[educationClass](educationclass.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5fbb2-134">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="5fbb2-p102">只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="5fbb2-p102">Read-only. Nullable.</span></span>|
|<span data-ttu-id="5fbb2-137">me</span><span class="sxs-lookup"><span data-stu-id="5fbb2-137">"@me"</span></span>|[<span data-ttu-id="5fbb2-138">educationUser</span><span class="sxs-lookup"><span data-stu-id="5fbb2-138">educationUser</span></span>](educationuser.md)| <span data-ttu-id="5fbb2-p103">只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="5fbb2-p103">Read-only. Nullable.</span></span>|
|<span data-ttu-id="5fbb2-141">schools</span><span class="sxs-lookup"><span data-stu-id="5fbb2-141">schools</span></span>|<span data-ttu-id="5fbb2-142">[educationSchool](educationschool.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5fbb2-142">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="5fbb2-p104">只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="5fbb2-p104">Read-only. Nullable.</span></span>|
|<span data-ttu-id="5fbb2-145">users</span><span class="sxs-lookup"><span data-stu-id="5fbb2-145">users</span></span>|<span data-ttu-id="5fbb2-146">[educationUser](educationuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5fbb2-146">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="5fbb2-p105">只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="5fbb2-p105">Read-only. Nullable.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationRoot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->