# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="bdda2-101">keyValuePair 资源类型</span><span class="sxs-lookup"><span data-stu-id="bdda2-101">keyValuePair resource type</span></span>

> <span data-ttu-id="bdda2-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="bdda2-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bdda2-103">用于存储自定义设置的键值对</span><span class="sxs-lookup"><span data-stu-id="bdda2-103">Key value pair for storing custom settings</span></span>
## <a name="properties"></a><span data-ttu-id="bdda2-104">属性</span><span class="sxs-lookup"><span data-stu-id="bdda2-104">Properties</span></span>
|<span data-ttu-id="bdda2-105">属性</span><span class="sxs-lookup"><span data-stu-id="bdda2-105">Property</span></span>|<span data-ttu-id="bdda2-106">类型</span><span class="sxs-lookup"><span data-stu-id="bdda2-106">Type</span></span>|<span data-ttu-id="bdda2-107">说明</span><span class="sxs-lookup"><span data-stu-id="bdda2-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bdda2-108">名称</span><span class="sxs-lookup"><span data-stu-id="bdda2-108">name</span></span>|<span data-ttu-id="bdda2-109">String</span><span class="sxs-lookup"><span data-stu-id="bdda2-109">String</span></span>|<span data-ttu-id="bdda2-110">此键值对的名称</span><span class="sxs-lookup"><span data-stu-id="bdda2-110">Name for this key-value pair</span></span>|
|<span data-ttu-id="bdda2-111">value</span><span class="sxs-lookup"><span data-stu-id="bdda2-111">value</span></span>|<span data-ttu-id="bdda2-112">String</span><span class="sxs-lookup"><span data-stu-id="bdda2-112">String</span></span>|<span data-ttu-id="bdda2-113">此键值对的值</span><span class="sxs-lookup"><span data-stu-id="bdda2-113">Value for this key-value pair</span></span>|

## <a name="relationships"></a><span data-ttu-id="bdda2-114">关系</span><span class="sxs-lookup"><span data-stu-id="bdda2-114">Relationships</span></span>
<span data-ttu-id="bdda2-115">无</span><span class="sxs-lookup"><span data-stu-id="bdda2-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="bdda2-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bdda2-116">JSON Representation</span></span>
<span data-ttu-id="bdda2-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bdda2-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.keyValuePair"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.keyValuePair",
  "name": "String",
  "value": "String"
}
```


