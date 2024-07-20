---
title: 视频 SEO（搜索引擎优化）
description: 了解如何在Adobe Dynamic Media Classic中配置视频SEO设置。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/setup
feature: Dynamic Media Classic
role: Admin
exl-id: f76b0e09-f148-46aa-b710-ec35bfebcb37
topic: Content Management
level: Intermediate
source-git-commit: 61665faba1e6bb711aae5becf0150d1ebe3105c0
workflow-type: tm+mt
source-wordcount: '1022'
ht-degree: 27%

---

# 视频 SEO（搜索引擎优化）{#video-seo-search-engine-optimization}

SEO 是改进从搜索引擎到网站流量的过程。尽管搜索引擎在收集有关文本内容的信息方面表现出色，但它们无法充分获取有关视频的信息。 必须向他们提供这种资料。

使用Adobe Dynamic Media Classic视频SEO，您可以应用视频元数据以为搜索引擎提供视频描述。 Adobe Dynamic Media Classic使您能够创建视频站点地图和mRSS源。 这些标准XML文件用于将视频信息提交到搜索引擎：

* **视频站点地图**：准确告知Google视频内容在网站上的位置和内容。 因此，可以在Google上完全搜索视频。 例如，视频站点地图可以指定视频的运行时间和类别。有关视频站点地图的信息，请参阅[视频站点地图和视频站点地图替代项](https://developers.google.com/search/docs/crawling-indexing/sitemaps/video-sitemaps?visit_id=637558394348624754-567115452&amp;rd=1)。

* **mRSS (Media Really Simple Syndication)源**：内容发布者使用它将媒体文件馈送到Yahoo！ 视频搜索。有关mRSS源的信息，请参阅[视频站点地图和视频站点地图替代项](https://developers.google.com/search/docs/crawling-indexing/sitemaps/video-sitemaps?visit_id=637558394348624754-567115452&amp;rd=1)。

>[!NOTE]
>
>Google 支持使用视频站点地图和 mRSS 新闻频道协议将信息提交给搜索引擎。

Adobe Dynamic Media Classic可以根据与每个视频一起存储的元数据生成视频站点地图和mRSS馈送。 您创建视频站点地图和 mRSS 新闻频道时，要决定要包括视频文件的哪些元数据字段。这样，您就可以将视频描述给搜索引擎，以便搜索引擎可以更准确地将流量引导至您网站上的视频。

>[!NOTE]
>
>在创建视频站点地图或 mRSS 新闻频道之前，要了解搜索引擎在 XML 文件中需要哪些字段，以及如何构建这些字段。要创建成功的视频站点地图或 mRSS 新闻频道，必须满足搜索引擎的要求。

Adobe Dynamic Media Classic会在生成视频站点地图和mRSS源之后创建这些报表。 这些报告位于视频SEO报告页面上。

>[!NOTE]
>
>对于视频站点地图和mRSS馈送，Adobe Dynamic Media Classic仅从标记为发布的视频中捕获元数据。 标记要发布的视频，以将其元数据包含在视频站点地图和mRSS馈送中。

## 选择视频SEO设置

在&#x200B;**[!UICONTROL 视频搜索引擎优化设置]**&#x200B;页面上为视频站点地图和mRSS源选择视频SEO设置。 若要打开此页面，请在全局导航栏上，转到&#x200B;**[!UICONTROL 设置]** > **[!UICONTROL 应用程序设置]** > **[!UICONTROL 视频SEO]** > **[!UICONTROL 设置]**。

在&#x200B;**[!UICONTROL 常规设置]**&#x200B;区域，选择是生成视频站点地图、mRSS源，还是同时生成两者。 在&#x200B;**[!UICONTROL 生成设置]**&#x200B;区域中，将元数据字段映射到输入字段。

选择设置后，选择&#x200B;**[!UICONTROL 保存]**（或&#x200B;**[!UICONTROL 保存并生成]**）以创建视频站点地图、mRSS源，或同时创建两者。

### 设置常规设置 {#choosing-general-settings}

在&#x200B;**[!UICONTROL 生成模式]**&#x200B;下拉列表中，选择报表模式：

* **视频站点地图**：创建视频站点地图。

* **mRSS源**：创建媒体RSS (mRSS)源。

* **Both**：创建两种类型的XML文件。

* **关**：要停止生成视频站点地图和媒体RSS (mRSS)源，请选择此选项。

在&#x200B;**[!UICONTROL 自动/手动模式]**&#x200B;下拉列表中，选择是自动生成还是手动生成：

* **自动模式**： Adobe Dynamic Media Classic每天自动生成一个视频站点地图、媒体RSS (mRSS)源，或同时生成这两者。 选择&#x200B;**[!UICONTROL 标记为Publish]**&#x200B;选项，以便您可以自动标记为发布Adobe Dynamic Media Classic生成的XML文件。

   * **标记为Publish**&#x200B;标记为发布生成的XML文件。

* **手动模式**：当您在“视频搜索优化设置”屏幕中选择&#x200B;**[!UICONTROL 生成]**&#x200B;或&#x200B;**[!UICONTROL 保存并生成]**&#x200B;时，Adobe Dynamic Media Classic会生成视频站点地图和/或Media RSS (mRSS)源。 还要选择以下选项：

   * **没有其他设置**：不标记为发布生成的XML文件。

   * **标记为Publish**：标记为发布生成的XML文件。

   * **允许部分生成**：如果XML文件不包含所有视频的完整元数据信息，则搜索引擎可以拒绝该文件。 即使某些视频没有元数据，此选项也会生成XML文件。 在“报告”屏幕上会注册一个警告。如果您打算导出 XML 文件并手动处理缺失信息，请选择该选项。

### 选择生成设置 {#choosing-generation-settings}

“生成设置”区域列出视频站点地图或mRSS馈送（或同时列出两者）的输入字段。 在元数据面板中，列出了元数据字段的名称。 使用“常规设置”区域来将输入字段映射到元数据字段。这样，您就可以告知Adobe Dynamic Media Classic从何处获取视频站点地图和/或mRSS馈送的元数据。

1. 在“元数据视图”菜单上，选择一个元数据视图。选择视图后，元数据字段的名称将显示在元数据面板中。
请参阅[元数据视图](application-setup.md#metadata_views)。
1. 将元数据字段名称从“元数据”面板拖动到“登陆页面”、“标题”、“说明”、“标签”以及“类别”输入字段。“登陆页面”、“标题”、“说明”字段是必填的。

   >[!NOTE]
   >
   >您还可以在输入字段中手动输入数据。

1. 执行以下任一操作：

   * 要保存设置而不生成XML文件，请选择&#x200B;**[!UICONTROL 保存]**。
   * 要保存并生成文件，请选择&#x200B;**[!UICONTROL 保存并生成]**。

     生成 XML 文件并记录在“作业日志”中。视频站点地图 (video-sitemap) 和媒体 RSS (mRSS) 新闻频道 (mrss-feed) 文件存储在公司的根文件夹中。

>[!NOTE]
>
>在将视频站点地图或mRSS源提交到搜索引擎之前，请先Publish该源。 视频站点地图和媒体 RSS (mRSS) 新闻频道文件存储在公司的根文件夹中。如有必要，将这些XML文件标记为发布，然后选择&#x200B;**[!UICONTROL Publish]**。

## 将视频站点地图和mRSS信息源文件提交到搜索引擎 {#submitting-video-sitemap-and-mrss-feed-files-to-search-engines}

视频站点地图和媒体 RSS (mRSS) 新闻频道文件存储在公司的根文件夹中：

* `https://{publish-server}/is/content/{companyname}/mrss-feed.xml`
* `https://{publish-server}/is/content/{companyname}/video-sitemap.xml`

将这些URL之一复制到搜索引擎的网站管理员工具中，以将您的视频站点地图或媒体RSS (mRSS)信息源文件提交到搜索引擎。

## 查看视频SEO报表 {#viewing-video-seo-reports}

在视频搜索引擎优化报告页面上查看视频SEO报告。 若要打开此页面，请在全局导航栏上，转到&#x200B;**[!UICONTROL 设置]** > **[!UICONTROL 应用程序设置]** > **[!UICONTROL 视频SEO]** > **[!UICONTROL 报告]**。

如果在生成报告时发生错误，则会列在报告页面上。
