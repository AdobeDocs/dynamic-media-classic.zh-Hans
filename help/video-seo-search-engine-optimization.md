---
title: 视频 SEO（搜索引擎优化）
description: 了解如何在Adobe Dynamic Media Classic中配置视频SEO设置。
uuid: bac2c6a9-8466-4b8f-b835-6cb0b4168513
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/setup
discoiquuid: 34ecd868-775f-452b-b26e-d139f0e280ae
feature: Dynamic Media Classic
role: Admin
exl-id: f76b0e09-f148-46aa-b710-ec35bfebcb37
source-git-commit: cb55e09a997b9d36002c4ac429603576d52fb8bd
workflow-type: tm+mt
source-wordcount: '1037'
ht-degree: 37%

---

# 视频 SEO（搜索引擎优化）{#video-seo-search-engine-optimization}

SEO 是改进从搜索引擎到网站流量的过程。虽然搜索引擎擅长收集有关基于文本的内容，但却无法充分获取有关视频的信息，除非向它们提供此信息。

使用Adobe Dynamic Media Classic视频SEO，您可以应用视频元数据以为搜索引擎提供视频描述。 Adobe Dynamic Media Classic使您能够创建视频站点地图和mRSS源。 这些标准XML文件用于将视频信息提交到搜索引擎：

* **视频站点地图**  — 告知Google视频内容在网站上的确切位置和内容。 因此，可以在Google上完全搜索视频。 例如，视频站点地图可以指定视频的运行时间和类别。有关视频站点地图的信息，请参阅 [视频站点地图和视频站点地图替代项](https://developers.google.com/search/docs/crawling-indexing/sitemaps/video-sitemaps?visit_id=637558394348624754-567115452&amp;rd=1).

* **mRSS（媒体真正简单的联合）信息源**  — 内容发布者使用它将媒体文件馈送到Yahoo！ 视频搜索。有关mRSS馈送的信息，请参阅 [视频站点地图和视频站点地图替代项](https://developers.google.com/search/docs/crawling-indexing/sitemaps/video-sitemaps?visit_id=637558394348624754-567115452&amp;rd=1).

>[!NOTE]
>
>Google 支持使用视频站点地图和 mRSS 新闻频道协议将信息提交给搜索引擎。

Adobe Dynamic Media Classic可以根据与每个视频一起存储的元数据生成视频站点地图和mRSS馈送。 您创建视频站点地图和 mRSS 新闻频道时，要决定要包括视频文件的哪些元数据字段。这样，您会向搜索引擎描述您的视频，以便搜索引擎可以更准确地将流量引导到网站上的视频

>[!NOTE]
>
>在创建视频站点地图或 mRSS 新闻频道之前，要了解搜索引擎在 XML 文件中需要哪些字段，以及如何构建这些字段。要创建成功的视频站点地图或 mRSS 新闻频道，必须满足搜索引擎的要求。

Adobe Dynamic Media Classic会在生成视频站点地图和mRSS源之后创建相关报表。 这些报告位于视频SEO报告页面上。

>[!NOTE]
>
>对于视频站点地图和mRSS馈送，Adobe Dynamic Media Classic仅从标记为发布的视频中捕获元数据。 请将视频标记为发布，以将其元数据加入视频站点地图和 mRSS 新闻频道中。

## 选择视频SEO设置 {#choosing-video-seo-settings}

在上为视频站点地图和mRSS馈送选择视频SEO设置 **[!UICONTROL 视频搜索引擎优化设置]** 页面。 要打开此页面，请在全局导航栏上，转到 **[!UICONTROL 设置]** > **[!UICONTROL 应用程序设置]** > **[!UICONTROL 视频SEO]** > **[!UICONTROL 设置]**.

在 **[!UICONTROL 常规设置]** 区域，选择是生成视频站点地图、mRSS馈送，还是同时生成两者。 在 **[!UICONTROL 生成设置]** 区域，将元数据字段映射到输入字段。

选择设置后，选择 **[!UICONTROL 保存]** (或 **[!UICONTROL 保存并生成]**)，以创建视频站点地图、mRSS馈送，或同时创建两者。

### 设置常规设置 {#choosing-general-settings}

在 **[!UICONTROL 生成模式]** 从下拉列表中，选择报表模式：

* **视频站点地图**  — 创建视频站点地图。

* **mRSS馈送**  — 创建媒体RSS (mRSS)源。

* **两者**  — 创建两种类型的XML文件。

* **关闭**  — 要停止生成视频站点地图和媒体RSS (mRSS)源，请选择此选项。

在 **[!UICONTROL 自动/手动模式]** 下拉列表，选择是自动生成还是手动生成：

* **自动模式** - Adobe Dynamic Media Classic每天自动生成一个视频站点地图、媒体RSS (mRSS)馈送，或同时生成这两者。 选择 **[!UICONTROL 标记为发布]** 用于自动标记为发布Adobe Dynamic Media Classic生成的XML文件的选项。

   * **标记为发布** 标记为发布生成的XML文件。

* **手动模式**  — 当您选择时，Adobe Dynamic Media Classic会生成视频站点地图和/或Media RSS (mRSS)馈送 **[!UICONTROL 生成]** 或 **[!UICONTROL 保存并生成]** 在“视频搜索优化设置”屏幕中。 还要选择以下选项：

   * **没有其他设置**  — 不标记为发布生成的XML文件。

   * **标记为发布**  — 标记为发布生成的XML文件。

   * **允许部分生成**  — 如果XML文件不包含所有视频的完整元数据信息，则搜索引擎可以拒绝该文件。 即使某些视频没有元数据，此选项也会生成XML文件。 在“报告”屏幕上会注册一个警告。如果您打算导出 XML 文件并手动处理缺失信息，请选择该选项。

### 选择生成设置 {#choosing-generation-settings}

“生成设置”区域列出了视频站点地图和/或mRSS馈送的输入字段，在“元数据”面板中列出了元数据字段的名称。 使用“常规设置”区域来将输入字段映射到元数据字段。这样，您就可以告知Adobe Dynamic Media Classic从何处获取视频站点地图和/或mRSS馈送的元数据。

1. 在“元数据视图”菜单上，选择一个元数据视图。您选择一个视图后，元数据字段的名称会显示在“元数据”面板中。请参阅[元数据视图](application-setup.md#metadata_views)。
1. 将元数据字段名称从“元数据”面板拖动到“登陆页面”、“标题”、“说明”、“标签”以及“类别”输入字段。“登陆页面”、“标题”、“说明”字段是必填的。

   >[!NOTE]
   >
   >您还可以在输入字段中手动输入数据。

1. 执行以下任一操作：

   * 要保存设置而不生成XML文件，请选择 **[!UICONTROL 保存]**.
   * 要保存并生成文件，请选择 **[!UICONTROL 保存并生成]**.

      生成 XML 文件并记录在“作业日志”中。视频站点地图 (video-sitemap) 和媒体 RSS (mRSS) 新闻频道 (mrss-feed) 文件存储在公司的根文件夹中。

>[!NOTE]
>
>在将视频站点地图或mRSS馈送提交到搜索引擎之前，请先发布该视频站点地图。 视频站点地图和媒体 RSS (mRSS) 新闻频道文件存储在公司的根文件夹中。如有必要，将这些XML文件标记为发布，然后选择 **[!UICONTROL Publish]**.

## 将视频站点地图和mRSS信息源文件提交到搜索引擎 {#submitting-video-sitemap-and-mrss-feed-files-to-search-engines}

视频站点地图和媒体 RSS (mRSS) 新闻频道文件存储在公司的根文件夹中：

* `https://{publish-server}/is/content/{companyname}/mrss-feed.xml`
* `https://{publish-server}/is/content/{companyname}/video-sitemap.xml`

将上述 URL 之一复制到搜索引擎的网站站长工具，以将您的视频站点地图或媒体 RSS (mRSS) 新闻频道文件提交给搜索引擎。

## 查看视频SEO报告 {#viewing-video-seo-reports}

在“视频搜索引擎优化报告”页面上查看视频SEO报告。 要打开此页面，请在全局导航栏上，转到 **[!UICONTROL 设置]** > **[!UICONTROL 应用程序设置]** > **[!UICONTROL 视频SEO]** > **[!UICONTROL 报告]**.

如果在生成报告时发生错误，则会列在报告页面上。
