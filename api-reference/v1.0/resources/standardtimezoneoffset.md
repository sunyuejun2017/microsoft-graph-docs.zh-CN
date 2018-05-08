# <a name="standardtimezoneoffset-resource-type"></a><span data-ttu-id="fde15-101">standardTimeZoneOffset 资源类型</span><span class="sxs-lookup"><span data-stu-id="fde15-101">standardTimeZoneOffset resource type</span></span>

<span data-ttu-id="fde15-102">指定时区何时从夏令时切换到标准时间。</span><span class="sxs-lookup"><span data-stu-id="fde15-102">Specifies when a time zone switches from daylight saving time to standard time.</span></span>

<span data-ttu-id="fde15-103">例如，如果为一个时区指定了以下属性：</span><span class="sxs-lookup"><span data-stu-id="fde15-103">For example, if a time zone is specified with the following properties:</span></span>

- <span data-ttu-id="fde15-104">**dayOccurrence** 为 3</span><span class="sxs-lookup"><span data-stu-id="fde15-104">**dayOccurrence** is 3</span></span>
- <span data-ttu-id="fde15-105">**dayOfWeek** 为“Sunday”</span><span class="sxs-lookup"><span data-stu-id="fde15-105">**dayOfWeek** is "Sunday"</span></span>
- <span data-ttu-id="fde15-106">**month** 为 10</span><span class="sxs-lookup"><span data-stu-id="fde15-106">**month** is 10</span></span>
- <span data-ttu-id="fde15-107">**time** 为 02:00:00 _ **year** 为 0，这意味着从夏令时切换到标准时间出现在每年十月第三个星期日的早上 2 点。</span><span class="sxs-lookup"><span data-stu-id="fde15-107">**time** is 02:00:00 _ **year** is 0 That means the transition from daylight saving time to standard occurs at 2 AM on the third Sunday of October, every year.</span></span>

## <a name="properties"></a><span data-ttu-id="fde15-108">属性</span><span class="sxs-lookup"><span data-stu-id="fde15-108">Properties</span></span>
| <span data-ttu-id="fde15-109">属性</span><span class="sxs-lookup"><span data-stu-id="fde15-109">Property</span></span>     | <span data-ttu-id="fde15-110">类型</span><span class="sxs-lookup"><span data-stu-id="fde15-110">Type</span></span>   |<span data-ttu-id="fde15-111">说明</span><span class="sxs-lookup"><span data-stu-id="fde15-111">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="fde15-112">dayOccurrence</span><span class="sxs-lookup"><span data-stu-id="fde15-112">dayOccurrence</span></span> | <span data-ttu-id="fde15-113">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="fde15-113">Edm.Int32</span></span> | <span data-ttu-id="fde15-114">表示从夏令时到标准时间的切换在一周的具体某天出现的次数。</span><span class="sxs-lookup"><span data-stu-id="fde15-114">Represents the nth occurrence of the day of week that the transition from daylight saving time to standard time occurs.</span></span> |
| <span data-ttu-id="fde15-115">dayOfWeek</span><span class="sxs-lookup"><span data-stu-id="fde15-115">DAYOFWEEK</span></span> | <span data-ttu-id="fde15-116">string</span><span class="sxs-lookup"><span data-stu-id="fde15-116">string</span></span> | <span data-ttu-id="fde15-117">表示从夏令时切换为标准时间时一周的具体某日。</span><span class="sxs-lookup"><span data-stu-id="fde15-117">Represents the day of the week when the transition from daylight saving time to standard time.</span></span> |
| <span data-ttu-id="fde15-118">month</span><span class="sxs-lookup"><span data-stu-id="fde15-118">month</span></span> | <span data-ttu-id="fde15-119">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="fde15-119">Edm.Int32</span></span> | <span data-ttu-id="fde15-120">表示从夏令时到标准时间的切换出现时一年的具体月份。</span><span class="sxs-lookup"><span data-stu-id="fde15-120">Represents the month of the year when the transition from daylight saving time to standard time occurs.</span></span> |
| <span data-ttu-id="fde15-121">time</span><span class="sxs-lookup"><span data-stu-id="fde15-121">time</span></span> | <span data-ttu-id="fde15-122">Edm.TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="fde15-122">Edm.TimeOfDay</span></span> | <span data-ttu-id="fde15-123">表示从夏令时到标准时间的切换出现时某日的具体时间。</span><span class="sxs-lookup"><span data-stu-id="fde15-123">Represents the date and time when the time changes from daylight saving time to standard time.</span></span> |
| <span data-ttu-id="fde15-124">year</span><span class="sxs-lookup"><span data-stu-id="fde15-124">year</span></span> | <span data-ttu-id="fde15-125">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="fde15-125">Edm.Int32</span></span> | <span data-ttu-id="fde15-126">表示从夏令时到标准时间的变更出现时的年度频率。</span><span class="sxs-lookup"><span data-stu-id="fde15-126">Represents how frequently in terms of years the change from daylight saving time to standard time occurs.</span></span> <span data-ttu-id="fde15-127">例如，值为 0 意味着每年。</span><span class="sxs-lookup"><span data-stu-id="fde15-127">For example, a value of 0 means every year.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="fde15-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fde15-128">JSON representation</span></span>

<span data-ttu-id="fde15-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fde15-129">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.standardTimeZoneOffset"
}-->

```json
{
  "dayOccurrence": "Int32",
  "dayOfWeek": "string",
  "month": "Int32",
  "time": "TimeOfDay",
  "year": "Int32"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "standardTimeZoneOffset resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->