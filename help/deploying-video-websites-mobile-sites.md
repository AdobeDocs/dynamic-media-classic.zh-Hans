---
title: 将视频部署到网站和移动站点
description: 瞭解如何從Adobe Dynamic Media Classic將視訊部署至您的網站和行動網站。
uuid: 22bb4402-c0ab-4df0-89b9-99707d111927
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
discoiquuid: 0d006314-c4cc-4f6c-a51c-6075bb445e39
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: 3df22d48-edb5-4927-aefb-104b53f81f1a
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '1706'
ht-degree: 33%

---

# 将视频部署到网站和移动站点{#deploying-video-to-your-websites-and-mobile-sites}

網站、行動網站和案頭應用程式可使用URL字串或內嵌程式碼來存取Adobe Dynamic Media Classic伺服器內容，包括視訊。 Adobe Dynamic Media Classic會在發佈程式期間啟用這些URL字串。 若要將視訊的URL字串或內嵌程式碼放置在網頁、行動頁面和案頭應用程式中，請從Adobe Dynamic Media Classic複製。

>[!NOTE]
>
>在发布资源之前，URL 或嵌入代码处于非活动状态。

## 发布视频 {#publishing-video}

發佈影片可讓Adobe Dynamic Media Classic伺服器將影片傳送至您的網站、行動網站或應用程式。

您有兩種發佈視訊的不同方法：

* **上傳時自動立即發佈影片**  — 在視訊上傳程式中，Adobe Dynamic Media Classic可在上傳及編碼視訊時自動發佈視訊。 立即发布功能意味着，无需事后单独发布视频。

* **在上载后手动发布视频**  — 如果您不想立即發佈影片，可以隨時手動發佈影片。

在您發佈影片後，Adobe Dynamic Media Classic會啟用HTML頁面或應用程式程式碼的URL字串。

**发布视频:**

1. 执行以下任一操作：

   * 若要在上傳時自動立即發佈視訊，請在「上傳」頁面中選取「 」 **[!UICONTROL 上傳後發佈]**. 您已完成相应的操作，不需要执行其他步骤。
   * 若要在上傳後手動發佈視訊，請在「瀏覽」面板中選取視訊，然後在「全域導覽」列上選取 **發佈**.

## 將視訊URL連結至行動網站或網站 {#linking-a-video-url-to-a-mobile-site-or-a-website}

在发布视频后，您可以获取该视频的 URL 以在网站、移动站点或台式机应用程序中使用。如果要在网页顶部的弹出或模式窗口中显示视频，请使用视频 URL。

當客戶選取連結時，會自動偵測其裝置、頻寬和熒幕大小。 在桌面的预定义查看器中会显示适当的视频进行播放，智能手机和平板电脑在移动设备的本地视频播放器中播放。

另請參閱 [將視訊檢視器內嵌在網頁上](deploying-video-websites-mobile-sites.md#embedding_the_video_viewer_on_a_web_page).

**将视频 URL 链接到移动站点或网站:**

1. 在「資產瀏覽」面板的 **[!UICONTROL 顯示]** 下拉式清單，選取 **[!UICONTROL 視訊]** 或 **[!UICONTROL 最適化視訊集]**.
1. 在左侧的“资源库”面板中，导航到包含要链接到的视频或自适应视频集的资源文件夹。
1. 在“资源浏览”面板上方的工具栏右侧，执行以下任一操作：

   * 選取 **[!UICONTROL 格點檢視]** 或 **[!UICONTROL 清單檢視]**. 在“资源浏览”面板中，双击单个资源的视频缩略图，以便在详细信息视图中将其打开。在右側的「URL和內嵌程式碼」面板中，在「HTTP串流」下方選取「 」 **[!UICONTROL 複製URL]** 位於您想要的檢視器右側。 依據最佳做法的要求，複製與 `Universal_HTML5_Video` 檢視器。
   * 選取 **[!UICONTROL 格點檢視]**. 在「資產瀏覽」面板中，選取單一資產，然後前往縮圖影像下方 **[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**.

      在「檢視器清單」頁面中，選取表格的「動作」欄下 **[!UICONTROL 複製URL]**. 依據最佳做法的要求，複製與 `Universal_HTML5_Video` 檢視器。

   * 選取 **[!UICONTROL 清單檢視]**. 在「資產瀏覽」面板中，選取單一資產，然後在縮圖影像右側，前往 **[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**.

      在「檢視器清單」頁面中，選取表格的「動作」欄下 **[!UICONTROL 複製URL]**. 依據最佳做法的要求，複製與 `Universal_HTML5_Video` 檢視器。

   * 選取 **[!UICONTROL 格點檢視]**， **[!UICONTROL 清單檢視]**，或 **[!UICONTROL 詳細資料檢視]**. 在相同工具列上，前往 **[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**.

      在「檢視器清單」頁面中，選取表格的「動作」欄下 **[!UICONTROL 複製URL]**. 依據最佳做法的要求，複製與 `Universal_HTML5_Video` 檢視器。

1. 将 HTML5 视频 URL 链接粘贴到您的网站和移动站点中。

## 將視訊檢視器內嵌在網頁上 {#embedding-the-video-viewer-on-a-web-page}

如果要播放网页中嵌入的视频，请使用嵌入代码功能。可以将嵌入代码复制到剪贴板中，以便将其粘贴到网页中。在“嵌入代码”对话框中不允许编辑代码。

另請參閱 [將視訊URL連結至行動網站或網站](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website).

**在网页中嵌入视频查看器:**

1. 在「資產瀏覽」面板的「顯示」下拉式清單中，選取 **[!UICONTROL 視訊]** 或 **[!UICONTROL 最適化視訊集]**.
1. 在左侧的“资源库”面板中，导航到包含要复制其嵌入代码的视频或自适应视频集的资源文件夹。
1. 在“资源浏览”面板上方的工具栏右侧，执行以下任一操作：

   * 選取 **[!UICONTROL 格點檢視]** 或 **[!UICONTROL 清單檢視]**. 在“资源浏览”面板中，双击单个资源的视频缩略图，以便在详细信息视图中将其打开。在右側的「URL和內嵌程式碼」面板中，在「HTTP串流」下方選取「 」 **[!UICONTROL 內嵌程式碼]** 位於您想要的檢視器右側。 最佳做法是選取 **[!UICONTROL 內嵌程式碼]** 與 `Universal_HTML5_Video` 檢視器。
   * 選取 **[!UICONTROL 格點檢視]**. 在「資產瀏覽」面板中，選取單一資產，然後在視訊縮圖影像下方選取 **[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**.

      在「檢視器清單」頁面中，選取表格的「動作」欄下 **[!UICONTROL 內嵌程式碼]**. 最佳做法是選取 **[!UICONTROL 內嵌程式碼]** 與 `Universal_HTML5_Video` 檢視器。

   * 選取 **[!UICONTROL 清單檢視]**. 在「資產瀏覽」面板中，選取單一資產，然後在縮圖影像右側，前往 **[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**.

      在「檢視器清單」頁面中，選取表格的「動作」欄下 **[!UICONTROL 內嵌程式碼]**. 最佳做法是選取 **[!UICONTROL 內嵌程式碼]** 與 `Universal_HTML5_Video` 檢視器。

   * 選取 **[!UICONTROL 格點檢視]**， **[!UICONTROL 清單檢視]**，或 **[!UICONTROL 詳細資料檢視]**. 在相同工具列上，前往 **[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**.

      在「檢視器清單」頁面中，選取表格的「動作」欄下 **[!UICONTROL 內嵌程式碼]**. 最佳做法是選取 **[!UICONTROL 內嵌程式碼]** 與 `Universal_HTML5_Video` 檢視器。

1. 在內嵌程式碼對話方塊中，選取 **[!UICONTROL 複製到剪貼簿]**.

   在“嵌入代码”对话框中不允许编辑代码。

1. 選取 **[!UICONTROL 關閉]**.
1. 在网页中粘贴嵌入代码。

### 實作內嵌程式碼，以搭配MP4視訊資產使用HTML5視訊 {#implementing-embed-code-for-using-html-video-with-mp-video-assets}

如果您未使用Adobe Dynamic Media Classic HTML5視訊播放器，而是想要使用原生HTML5 `<video>` 標籤後，您可使用下列內嵌程式碼範例：

```as3
<video poster="S7 video thumbnail URL" controls> 
        <source src="S7 OGG video asset URL (no player)" type='video/ogg; codecs="theora, vorbis"'/> 
        <source src="S7 MP4 mobile progressive video asset URL (no player)" type='video/mp4; codecs="avc1.4D401E, mp4a.40.2"'/> 
        <p>This is fallback content</p> 
</video>
```

* Replace `"S7 video thumbnail URL"` 搭配視訊的縮圖URL，也就是使用者在播放視訊前所看到的視訊縮圖影像。

   另請參閱 [取得視訊縮圖URL](deploying-video-websites-mobile-sites.md#obtaining_video_thumbnail_urls).

* Replace `"S7 OGG video asset URL (no player)"` 以OGG視訊的漸進式URL顯示。

   另請參閱 [將視訊URL連結至行動網站或網站](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website).

* Replace `"S7 MP4 mobile progressive video asset URL (no player)"` 搭配視訊的行動漸進式URL。

   另請參閱 [將視訊URL連結至行動網站或網站](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website).

## 使用協力廠商視訊播放器部署視訊 {#deploying-video-using-a-third-party-video-player}

如果您使用協力廠商視訊播放器或自訂的視訊播放器，而不是Dynamic Media Classic視訊檢視器，您會取得適用於HLS多位元速率視訊串流或漸進式下載的直接視訊URL。

**使用第三方视频播放器部署视频:**

1. 在Adobe Dynamic Media Classic中的全域導覽列上，前往 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 一般設定]**.
1. 根据要使用的 URL 类型，请执行以下任务之一：

* 產生直接HLS串流視訊URL （多位元速率）的方式

   於 **[!UICONTROL 應用程式一般設定]** 頁面，在 **[!UICONTROL 伺服器]** 群組，在 **[!UICONTROL 已發佈的伺服器名稱]** 文字欄位，建構直接URL。 使用下列語法： `server/is/content/company/folder/filename.m3u8`

   例如，假設已發佈的伺服器名稱為 `https://s7d9.scene7.com/.` 使用步驟2中的語法，直接URL可能如下所示：
   `https://s7d9.scene7.com/is/content/GeoRetail/AdobeRIA-AVS.m3u8`

* 產生直接HLS串流視訊URL （單位元速率）的方式

   於 **[!UICONTROL 應用程式一般設定]** 頁面，在 **[!UICONTROL 伺服器]** 群組，在 **[!UICONTROL HLS資料流伺服器名稱]** 文字欄位，使用下列語法建構直接URL：

   `server/company/folder/filename.ext.m3u8`

   例如，假設HLS串流伺服器名稱為 `https://s7mbrstream.scene7.com/hls-vod/`. 使用步驟2中的語法，直接URL可能如下所示：
   `https://s7mbrstream.scene7.com/hls-vod/GeoRetail/MBR/ToyStory3\_Teaser1\_High\_iPad\_768x432\_1296K.mp4.m3u8`

* 生成直接渐进式视频 URL

   在“**[!UICONTROL 应用程序常规设置]**”页面的“**[!UICONTROL 服务器]**”组的“**[!UICONTROL 渐进式视频服务器名称]**”文本框中，使用以下语法构建直接 eVideo URL：

   `server/company/folder/filename`

   例如，假設漸進式視訊伺服器名稱為 `https://s7d9.scene7.com/is/content/`. 使用步驟2中的語法，直接URL可能如下所示：
   `https://s7d9.scene7.com/e2/GeoRetail/SourceVideo/outdoors.mp4`

## 使用視訊縮圖 {#working-with-video-thumbnails}

Adobe Dynamic Media Classic會產生已編碼視訊和預先編碼視訊的縮圖。 您可以像使用任何图像资源一样使用视频缩略图。此外，您也可以取得Adobe Dynamic Media Classic產生之視訊縮圖的URL。 然後您可以在Adobe Dynamic Media Classic外部部署這些URL。 例如，您可以在搜索结果、相关视频列表和网站上的视频播放列表中部署缩略图。

基于视频的第一个异构帧（不是全黑帧或全白帧等）生成缩略图。

### 取得視訊縮圖URL {#obtaining-video-thumbnail-urls}

Adobe Dynamic Media Classic會在上傳程式期間自動產生視訊縮圖。 縮圖會出現在「清單檢視」和「格點檢視」的「瀏覽」面板中。

要生成视频缩略图的 URL，请执行发布操作。

另請參閱 [發佈視訊](deploying-video-websites-mobile-sites.md#publishing_video).

发布后，您可以在“URL 和嵌入代码”面板的“详细信息视图”中获取视频缩略图 URL。選取 **[!UICONTROL 複製URL]** 右側，方便您複製其URL。

### 修改視訊檢視器中的海報影格 {#modifying-poster-frames-in-video-viewers}

*海报帧*&#x200B;是在开始播放视频之前在视频查看器中显示的初始帧。Adobe Dynamic Media Classic使用視訊縮圖作為海報影格。

您可以将图像修饰符应用于海报帧。例如，您可以裁切海报帧或使其变得透明。要修改海报帧，请打开视频查看器配置屏幕，并在“海报图像修饰符”部分中输入修饰符。

另請參閱 [新增或編輯視訊檢視器預設集](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset).

另請參閱 [影像伺服指南](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/c-is-home.html?lang=en#image-serving-api).

还可以通过将修饰符附加到视频缩略图 URL 的后面来修改视频缩略图。

>[!MORELIKETHIS]
>
>* [發佈檔案](publishing-files.md#publishing_files)