# <a name="using-the-activity-feed-api-in-microsoft-graph-to-enable-cross-device-experiences"></a>使用 Microsoft Graph 中的活动源 API 启用跨设备体验

这些活动通过帮助用户跨设备快速继续应用中的重要任务来提高其效率。 Microsoft 通过诸如 Windows Timeline、Windows Sets、Cortana“从我离开的位置继续”和 Microsoft Launcher 的体验帮助提高用户应用的生产力，这些应用均由活动源驱动。 当使用活动时，这些 Microsoft 体验即可开始驱动应用。 此外，还可以在应用中显示这些活动，以帮助用户恢复他们之前在任何平台（包括 Windows、Android 和 iOS）、任何设备上所做的操作。

## <a name="why-integrate-with-activities"></a>为什么与这些活动集成？
### <a name="enable-experiences-that-flow-seamlessly-between-windows-android-linux-and-ios-devices"></a>能够实现在 Windows、Android、Linux 和 iOS 设备之间无缝转换的体验 
出色的应用程序可帮助用户执行非常棒的操作 - 产生许多创造力、生产力和娱乐方案。 返回到任务可能是一个挑战，尤其是当某人想要在其他设备或平台上继续执行该任务的时候。 通过将活动集成到应用程序，可以帮助用户使用任意方便的屏幕快速返回到最近的任务，可以使任务在 Web、移动和桌面之间相互移动。 借助历史记录项，用户可以轻松查看最近使用的活动、使用的具体时间以及持续时间。   

每个用户活动均表示应用内的单个目标：产品页、电视节目、文档或在游戏中的当前活动。 只需一个深层链接即可继续应用中的活动。 使用[获取最近的活动](https://developer.microsoft.com/zh-CN/graph/docs/api-reference/v1.0/api/projectrome_get_recent_activities)来为购物应用创建最近查看产品的列表，或当前阅读的书籍和新闻文章列表。 

### <a name="create-richer-activities-for-any-experience-with-adaptive-cards"></a>使用自适应卡片来为任何体验创建更丰富的活动
在 Windows Timeline 等 Microsoft 体验中呈现活动时，将使用[自适应卡片](http://adaptivecards.io/)显示它们，这允许用户创建精美、丰富的卡片来展示应用的活动。 另外，还可以使用自适应卡片 SDK 来在自己的应用中呈现丰富的卡片。 如果没有为每个活动提供一个自适应卡片，我们将基于你的应用程序名称和图标、必填的“标题”字段和可选“描述”字段来自动创建一个简单的活动卡片。 

### <a name="let-microsoft-help-drive-app-usage-with-features-that-reach-hundreds-of-millions-of-customers"></a>让 Microsoft 通过可服务于数亿客户的功能来帮助提升应用的使用率
与用户活动集成不仅能使用户无缝地继续应用中的活动，而且还意味着可以利用一组不断发展的适用于 Windows、iOS 和 Android 的 Microsoft 体验，这些体验旨在提高用户生产力并帮助用户在所有设备上与应用互动。 通过使用 Microsoft Graph，可仅与用户活动进行一次集成，即可服务于数亿消费者和组织中使用 Windows 以及适用于 iOS 和 Android 设备的 Microsoft 产品的数千万客户。

![Windows Timeline 的屏幕截图](https://winblogs.azureedge.net/win/2017/05/22-591a3ec9833f4.jpg)

## <a name="see-also"></a>另请参阅

- [Microsoft Graph 中的跨设备体验](cross-device-concept-overview.md)
- [使用活动源 API 继续用户跨设备的活动](../api-reference/v1.0/resources/activity-feed-api-overview.md)
- [通过一个请求使用深层插入发布活动和历史记录项](https://developer.microsoft.com/zh-CN/graph/docs/api-reference/v1.0/api/projectrome_put_activity#example-2---deep-insert)
- [详细了解 Project Rome](http://aka.ms/projectrome)