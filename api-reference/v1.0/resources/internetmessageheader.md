# <a name="internetmessageheader-resource-type"></a><span data-ttu-id="a5f35-101">internetMessageHeader 资源类型</span><span class="sxs-lookup"><span data-stu-id="a5f35-101">internetMessageHeader resource type</span></span>


<span data-ttu-id="a5f35-102">一个键值对，它表示 Internet 邮件头，正如 [RFC5322](https://www.ietf.org/rfc/rfc5322.txt) 所定义的那样，它提供邮件获取的从发件人到收件人的网络路径的详细信息。</span><span class="sxs-lookup"><span data-stu-id="a5f35-102">A key-value pair that represents an Internet message header, as defined by [RFC5322](https://www.ietf.org/rfc/rfc5322.txt), that provides details of the network path taken by a message from the sender to the recipient.</span></span> 

<span data-ttu-id="a5f35-103">有关 Internet 邮件头示例，请参阅[查看电子邮件头](https://support.office.com/zh-CN/article/View-e-mail-message-headers-CD039382-DC6E-4264-AC74-C048563D212C#bm4)。</span><span class="sxs-lookup"><span data-stu-id="a5f35-103">For examples of an Internet message header, see [View e-mail message headers](https://support.office.com/zh-CN/article/View-e-mail-message-headers-CD039382-DC6E-4264-AC74-C048563D212C#bm4).</span></span>


## <a name="properties"></a><span data-ttu-id="a5f35-104">属性</span><span class="sxs-lookup"><span data-stu-id="a5f35-104">Properties</span></span>
| <span data-ttu-id="a5f35-105">属性</span><span class="sxs-lookup"><span data-stu-id="a5f35-105">Property</span></span>     | <span data-ttu-id="a5f35-106">类型</span><span class="sxs-lookup"><span data-stu-id="a5f35-106">Type</span></span>   |<span data-ttu-id="a5f35-107">说明</span><span class="sxs-lookup"><span data-stu-id="a5f35-107">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a5f35-108">name</span><span class="sxs-lookup"><span data-stu-id="a5f35-108">name</span></span>|<span data-ttu-id="a5f35-109">string</span><span class="sxs-lookup"><span data-stu-id="a5f35-109">string</span></span>|<span data-ttu-id="a5f35-110">表示键值对中的键。</span><span class="sxs-lookup"><span data-stu-id="a5f35-110">Represents the key in a key-value pair.</span></span>|
|<span data-ttu-id="a5f35-111">value</span><span class="sxs-lookup"><span data-stu-id="a5f35-111">value</span></span>|<span data-ttu-id="a5f35-112">string</span><span class="sxs-lookup"><span data-stu-id="a5f35-112">string</span></span>|<span data-ttu-id="a5f35-113">键值对中的值。</span><span class="sxs-lookup"><span data-stu-id="a5f35-113">The value in a key-value pair.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a5f35-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a5f35-114">JSON representation</span></span>

<span data-ttu-id="a5f35-115">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a5f35-115">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.internetMessageHeader"
}-->

```json
{
  "name": "string",
  "value": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "internetMessageHeader resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->