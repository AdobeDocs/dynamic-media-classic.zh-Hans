---
title: 视频 SEO（搜索引擎优化）
description: 瞭解如何在Adobe Dynamic Media Classic中設定視訊SEO設定。
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

使用Adobe Dynamic Media Classic視訊SEO，您可以套用視訊中繼資料，以向搜尋引擎提供您視訊的說明。 Adobe Dynamic Media Classic可讓您建立視訊網站地圖和mRSS摘要。 這些標準XML檔案用於將視訊資訊提交至搜尋引擎：

* **視訊網站地圖**  — 通知Google視訊內容在網站上的確切位置與內容。 因此，您完全可以在Google上搜尋影片。 例如，视频站点地图可以指定视频的运行时间和类别。如需視訊網站地圖的相關資訊，請參閱 [視訊網站地圖和視訊網站地圖的替代方案](https://developers.google.com/search/docs/crawling-indexing/sitemaps/video-sitemaps?visit_id=637558394348624754-567115452&amp;rd=1).

* **mRSS (Media Really Simple Syndication)摘要**  — 內容發佈者用來將媒體檔案饋送至Yahoo！ 视频搜索。如需mRSS摘要的相關資訊，請參閱 [視訊網站地圖和視訊網站地圖的替代方案](https://developers.google.com/search/docs/crawling-indexing/sitemaps/video-sitemaps?visit_id=637558394348624754-567115452&amp;rd=1).

>[!NOTE]
>
>Google 支持使用视频站点地图和 mRSS 新闻频道协议将信息提交给搜索引擎。

Adobe Dynamic Media Classic可從儲存於每個視訊的中繼資料產生視訊網站地圖和mRSS摘要。 您创建视频站点地图和 mRSS 新闻频道时，要决定要包括视频文件的哪些元数据字段。这样，您会向搜索引擎描述您的视频，以便搜索引擎可以更准确地将流量引导到网站上的视频

>[!NOTE]
>
>在创建视频站点地图或 mRSS 新闻频道之前，要了解搜索引擎在 XML 文件中需要哪些字段，以及如何构建这些字段。要创建成功的视频站点地图或 mRSS 新闻频道，必须满足搜索引擎的要求。

Adobe Dynamic Media Classic會在您產生視訊網站地圖和mRSS摘要後，建立相關報表。 這些報告可在視訊SEO報告頁面上取得。

>[!NOTE]
>
>對於視訊網站地圖和mRSS摘要，Adobe Dynamic Media Classic只會從標示為發佈的視訊中擷取中繼資料。 请将视频标记为发布，以将其元数据加入视频站点地图和 mRSS 新闻频道中。

## 選擇視訊SEO設定 {#choosing-video-seo-settings}

在上選取視訊網站地圖和mRSS摘要的視訊SEO設定 **[!UICONTROL 視訊搜尋引擎最佳化設定]** 頁面。 若要開啟此頁面，請在全域導覽列上，前往 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 視訊SEO]** > **[!UICONTROL 設定]**.

在 **[!UICONTROL 一般設定]** 區域，選擇是否要產生視訊網站地圖、mRSS摘要，或兩者都產生。 在 **[!UICONTROL 產生設定]** 區域，將中繼資料欄位對應至輸入欄位。

選擇設定後，選取 **[!UICONTROL 儲存]** (或 **[!UICONTROL 儲存並產生]**)，以建立「視訊網站地圖」和/或「mRSS摘要」。

### 設定一般設定 {#choosing-general-settings}

於 **[!UICONTROL 產生模式]** 從下拉式清單中選擇報表模式：

* **視訊網站地圖**  — 建立視訊網站地圖。

* **mRSS摘要**  — 建立媒體RSS (mRSS)摘要。

* **兩者**  — 建立兩種型別的XML檔案。

* **關閉**  — 若要停止產生視訊網站地圖和媒體RSS (mRSS)摘要，請選擇此選項。

於 **[!UICONTROL 自動/手動模式]** 下拉式清單，選擇是否要自動或手動產生：

* **自動模式** - Adobe Dynamic Media Classic每天都會自動產生一個視訊網站地圖、媒體RSS (mRSS)摘要，或兩者皆產生。 選取 **[!UICONTROL 標籤為發佈]** 自動標示為發佈Adobe Dynamic Media Classic產生的XML檔案的選項。

   * **標籤為發佈** 標籤為發佈產生的XML檔案。

* **手動模式** - Adobe Dynamic Media Classic會在您選取時產生視訊網站地圖、媒體RSS (mRSS)摘要，或兩者皆產生 **[!UICONTROL 產生]** 或 **[!UICONTROL 儲存並產生]** 在「視訊搜尋最佳化設定」畫面中。 还要选择以下选项：

   * **沒有其他設定**  — 不會標籤為發佈產生的XML檔案。

   * **標籤為發佈**  — 標籤為發佈產生的XML檔案。

   * **允許部分產生**  — 如果XML檔案未包含所有影片的完整中繼資料資訊，搜尋引擎可以拒絕該檔案。 即使某些影片沒有中繼資料，此選項也會產生XML檔案。 在“报告”屏幕上会注册一个警告。如果您打算导出 XML 文件并手动处理缺失信息，请选择该选项。

### 选择生成设置 {#choosing-generation-settings}

「產生設定」區域會列出「視訊網站地圖」或mRSS摘要（或兩者）的輸入欄位，在「中繼資料」面板中則列出中繼資料欄位的名稱。 使用“常规设置”区域来将输入字段映射到元数据字段。如此一來，您就能告訴Adobe Dynamic Media Classic從何處取得視訊網站地圖和/或mRSS摘要的中繼資料。

1. 在“元数据视图”菜单上，选择一个元数据视图。您选择一个视图后，元数据字段的名称会显示在“元数据”面板中。请参阅[元数据视图](application-setup.md#metadata_views)。
1. 将元数据字段名称从“元数据”面板拖动到“登陆页面”、“标题”、“说明”、“标签”以及“类别”输入字段。“登陆页面”、“标题”、“说明”字段是必填的。

   >[!NOTE]
   >
   >您还可以在输入字段中手动输入数据。

1. 执行以下任一操作：

   * 若要儲存設定而不產生XML檔案，請選取 **[!UICONTROL 儲存]**.
   * 若要儲存並產生檔案，請選取 **[!UICONTROL 儲存並產生]**.

      生成 XML 文件并记录在“作业日志”中。视频站点地图 (video-sitemap) 和媒体 RSS (mRSS) 新闻频道 (mrss-feed) 文件存储在公司的根文件夹中。

>[!NOTE]
>
>先發佈視訊網站地圖或mRSS摘要，您才能將其提交至搜尋引擎。 视频站点地图和媒体 RSS (mRSS) 新闻频道文件存储在公司的根文件夹中。視需要標籤這些XML檔案以供發佈，然後選取 **[!UICONTROL 發佈]**.

## 將視訊網站地圖和mRSS摘要檔案提交至搜尋引擎 {#submitting-video-sitemap-and-mrss-feed-files-to-search-engines}

视频站点地图和媒体 RSS (mRSS) 新闻频道文件存储在公司的根文件夹中：

* `https://{publish-server}/is/content/{companyname}/mrss-feed.xml`
* `https://{publish-server}/is/content/{companyname}/video-sitemap.xml`

将上述 URL 之一复制到搜索引擎的网站站长工具，以将您的视频站点地图或媒体 RSS (mRSS) 新闻频道文件提交给搜索引擎。

## 檢視視訊SEO報表 {#viewing-video-seo-reports}

在視訊搜尋引擎最佳化報告頁面上檢視視訊SEO報告。 若要開啟此頁面，請在全域導覽列上，前往 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 視訊SEO]** > **[!UICONTROL 報表]**.

如果產生報表時發生錯誤，就會列在報表頁面上。
