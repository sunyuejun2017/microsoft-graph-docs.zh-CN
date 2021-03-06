# <a name="overview-of-social-intelligence-and-analytics-in-microsoft-graph"></a>Microsoft Graph 中的社交智能和分析概述

Microsoft 365 云服务的亿万用户组成了 Microsoft Graph 的核心部分。 用户的数据通过 Microsoft Graph 提供的服务得到精心的管理、保护和适当的授权，以提升企业生产力和创造力。 因为在 Microsoft Graph 中有大量的用户数据，所以派生自用户社交交互的数据将尤为受到关注。 它可以对回答类似以下问题提供智能见解：

- “此用户就此主题的信息应与谁联系？”
- “此人最感兴趣的文档有哪些？”

你可以在 Microsoft Graph 中使用人员 API 和见解 API 来构建更为智能的应用，分别访问与用户相关度高的人员和文档。

人员 API 基于用户的联系人、社交网络、组织目录以及电子邮件和 Skype 上的最近通信，返回按与该用户相关性排序的人员。 这对于选取人员的应用场景尤为有用。

见解 API 使用高级分析和机器学习为用户提供他们在工作中所需的相关度最高的文件。 API 提升了我们所熟悉的 Office 365 体验，其中包括 Office Delve、SharePoint Home、OneDrive for Business 中的发现视图以及 Outlook 网页版。

![人员和见解 API 为用户返回具有相关度的人员和文档](images/social-intel-concept-overview-data.png)

## <a name="why-integrate-with-people-data"></a>为什么与人员数据集成？

人员 API 可返回单个实体的数据[人员](../api-reference/v1.0/resources/person.md)，其中包括当今商界中的个人典型数据。 ****“人员”数据的优势在于它相对于 Microsoft Graph 用户的__“相关性”。 相关性是基于用户的通信和协作模式以及业务关系来计算的，并且以每个人的相关性分数进行记录。 有 3 种主要类型的“相关性”__ 数据的应用程序。

### <a name="browse-people-by-relevance"></a>按相关性浏览人员

你可以浏览与登录用户相关的人员或与登录用户组织中某一些用户相关的人员，前提是你已获取相应的[授权](people_example.md#authorization)。 获取按相关性排序的“人员”**** 对象的集合。 而且，通过指定查询参数 `top`、`skip`、`orderby`、`select` 和 `filter`，你还可以进一步[自定义](people_example.md#browse-people)响应中返回的****“人员”对象的集合。

### <a name="fuzzy-searches-based-on-people-criteria"></a>基于人员条件的模糊搜索

人员 API 允许你搜索与登录用户相关的人员，前提是你的应用已获取该用户授予的权限。 （详细了解[人员权限](permissions_reference.md#people-permissions)。）

模糊搜索根据完全匹配以及搜索意图推断返回结果。 为了说明这一点，请见以下示例：这将返回与登录用户相关的****、其名字或电子邮件地址__ 中包含以“j”开头的单词的人员对象。

<!-- { "blockType": "ignored" } -->
```http
GET /me/people/?$search=j
```

### <a name="fuzzy-searches-based-on-topic-criteria"></a>基于主题条件的模糊搜索

你也可以借助人员 API 搜索与登录用户相关并表示出有兴趣与该用户就某些“话题”进行交流的人员。 主题只是用户在电子邮件对话中使用最多的词。 Microsoft 从其上下文中随机提取这些词并为该数据创建索引，便于进行模糊搜索。

以下示例说明有关就主题“甲壳虫”为目的进行搜索所得出的推理。

<!-- { "blockType": "ignored" } -->
```http
GET /me/people/?$search="topic:beetle" 
```

在主题数据索引中进行的模糊搜索返回了表示甲壳虫昆虫、标志性大众甲壳虫汽车、披头士乐队和其他定义的实例。


## <a name="why-integrate-with-document-based-insights-preview"></a>为什么与基于文档的见解（预览版）集成？

### <a name="use-intelligence-to-improve-collaboration"></a>使用智能来提升协作

在平时的工作日中，用户通常会与存储在多个文档中的大量信息进行交互，并以多种不同的方式与其他用户协作。 当他们需要任何信息时，即可随时找到所需的信息，这一点很重要。

你可以使用见解 API（其中包含[热门](../api-reference/beta/resources/insights_trending.md)、[共享](../api-reference/beta/resources/insights_shared.md)和[使用](../api-reference/beta/resources/insights_used.md) API），根据用户的当前上下文和需求跨 Office 365 处理文件，使用户工作更为高效并提升组织中的协作。

在应用中呈现见解 API 中的结果很简单。 每个结果都附带了一组常用可视化属性，例如，预览图像 URL 或预览文本。

### <a name="make-relevant-content-visible"></a>使相关内容可见

在 Office 365 中，Delve 使用_热门_见解来帮助用户发现目前最令他们感兴趣的文档。 请参见图 1。

通过编程的方式，可以使用见解 API 中的[热门](../api-reference/beta/resources/insights_trending.md)实体为应用客户提供类似体验。 使用****“热门”实体可连接到最近热门或与用户相关的文档。 [列出热门文档](../api-reference/beta/api/insights_list_trending.md)将返回存储在 OneDrive 或 SharePoint 团队网站上的文件，并参照这些文件的重要程度来对其排序。 

**图 1. Office 365 中的 Delve 为用户显示热门文档**

![Office 365 中的 Delve 为用户显示热门文档的屏幕截图](images/delve_concept.png)

### <a name="allow-users-to-collaborate-and-get-back-to-work"></a>允许用户进行协作和恢复工作

新的 Office 365 人员卡片融入了“使用”__ 和__“共享”见解，以连接人员和知识单元之间的点。 人员卡片将标识和显示有关人员的相关文档。 用户可以在整个套件内查看人员卡片（例如，在 Outlook 网页版中）。 请参见图 2。

见解 API 提供与[使用](../api-reference/beta/resources/insights_used.md)和[共享](../api-reference/beta/resources/insights_shared.md)实体类似的功能。 它们返回用户最近最常查看或使用的内容，或同事最近在 Office 365 中与用户共享的内容。

**图 2. Outlook 网页版显示用户的人员卡片**

![Outlook 网页版中用户的人员卡片屏幕截图，显示最近使用的文件](images/peoplecard_concept.png)

## <a name="next-steps"></a>后续步骤

* 在 [Graph 浏览器](https://developer.microsoft.com/zh-CN/graph/graph-explorer)中使用你自己的文件尝试人员和见解 API。 登录，然后选择左侧列中的“显示更多示例”****。 使用菜单打开“人员”**** 和“见解(beta)”****。
* 了解有关[人员 API](people_example.md) 和[人员](../api-reference/v1.0/resources/person.md)实体的详细信息。
* 若要开始使用见解 API，请参阅[使用见解 API](../api-reference/beta/resources/insights.md)。
