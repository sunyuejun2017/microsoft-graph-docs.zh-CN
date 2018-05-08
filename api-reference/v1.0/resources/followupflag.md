# <a name="followupflag-resource-type"></a><span data-ttu-id="873dd-101">followupFlag 资源类型</span><span class="sxs-lookup"><span data-stu-id="873dd-101">followupFlag resource type</span></span>


<span data-ttu-id="873dd-102">允许设置标记，以便用户在日后跟进项目。</span><span class="sxs-lookup"><span data-stu-id="873dd-102">Allows setting a flag for the user to follow up on an item later.</span></span> <span data-ttu-id="873dd-103">受支持的项包括[邮件](message.md)和[联系人](contact.md)。</span><span class="sxs-lookup"><span data-stu-id="873dd-103">Supported items include [message](message.md) and [contact](contact.md).</span></span>

## <a name="properties"></a><span data-ttu-id="873dd-104">属性</span><span class="sxs-lookup"><span data-stu-id="873dd-104">Properties</span></span>
| <span data-ttu-id="873dd-105">属性</span><span class="sxs-lookup"><span data-stu-id="873dd-105">Property</span></span>     | <span data-ttu-id="873dd-106">类型</span><span class="sxs-lookup"><span data-stu-id="873dd-106">Type</span></span>   |<span data-ttu-id="873dd-107">说明</span><span class="sxs-lookup"><span data-stu-id="873dd-107">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="873dd-108">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="873dd-108">completedDateTime</span></span>|[<span data-ttu-id="873dd-109">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="873dd-109">dateTimeTimeZone</span></span>](dateTimeTimeZone.md)|<span data-ttu-id="873dd-110">完成跟进的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="873dd-110">The date and time that the response was returned.</span></span>|
|<span data-ttu-id="873dd-111">dueDateTime</span><span class="sxs-lookup"><span data-stu-id="873dd-111">dueDateTime</span></span>|<span data-ttu-id="873dd-112">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="873dd-112">**dateTimeTimeZone**</span></span>|<span data-ttu-id="873dd-113">待完成的跟进的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="873dd-113">The date and time that the follow-up is to be finished.</span></span>|
|<span data-ttu-id="873dd-114">flagStatus</span><span class="sxs-lookup"><span data-stu-id="873dd-114">flagStatus</span></span>|<span data-ttu-id="873dd-115">String</span><span class="sxs-lookup"><span data-stu-id="873dd-115">String</span></span>|<span data-ttu-id="873dd-116">项目的跟进状态。</span><span class="sxs-lookup"><span data-stu-id="873dd-116">The status for follow-up for an item.</span></span> <span data-ttu-id="873dd-117">可取值为：`notFlagged`、`complete` 和 `flagged`。</span><span class="sxs-lookup"><span data-stu-id="873dd-117">Possible values are: `notFlagged`, `complete`, `flagged`.</span></span>|
|<span data-ttu-id="873dd-118">startDateTime</span><span class="sxs-lookup"><span data-stu-id="873dd-118">startDateTime</span></span>|<span data-ttu-id="873dd-119">**dateTimeTimeZone**</span><span class="sxs-lookup"><span data-stu-id="873dd-119">**dateTimeTimeZone**</span></span>|<span data-ttu-id="873dd-120">要开始的跟进的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="873dd-120">Gets the date and time that the meeting is to begin.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="873dd-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="873dd-121">JSON representation</span></span>

<span data-ttu-id="873dd-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="873dd-122">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.followupFlag"
}-->

```json
{
  "completedDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "dueDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "flagStatus": "String",
  "startDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "followupFlag resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->