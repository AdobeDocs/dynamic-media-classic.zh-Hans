---
title: 「快速入門：Adobe Dynamic Media Classic中的影片」
description: Adobe Dynamic Media Classic簡介和快速入門影片，可幫助您快速上手並執行。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: 1157400c-b33a-422e-848c-258660ddc748
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '1808'
ht-degree: 25%

---

# 快速入門： Adobe Dynamic Media Classic中的影片{#quick-start-video}

Adobe Dynamic Media Classic Video是端對端解決方案，可讓您輕鬆發佈高品質的最適化視訊，以便在多個熒幕(包括桌上型電腦、iOS、Android™、BlackBerry®和Windows®行動裝置)上串流。 自适应视频集可将同一视频以不同比特率和格式（如 400 kbps、800 kbps 和 1000 kbps）编码的不同版本分组在一起。台式计算机或移动设备可检测可用带宽。

例如，在 iOS 移动设备上，可检测 3G、4G 或 Wi-Fi 等带宽。然后，从自适应视频集内的不同视频比特率中自动选择正确的编码视频。视频将流式传输到台式机、移动设备或平板电脑。

另外，如果台式机或移动设备上的网络条件发生变化，则会自动动态切换视频质量。此外，如果客戶在桌上型電腦進入全熒幕模式，Adaptive Video Set會使用更好的解析度來回應，以改善客戶的觀看體驗。 對於在多個熒幕和裝置上播放Adobe Dynamic Media Classic視訊的客戶，使用「最適化視訊集」可提供最佳播放方式。

视频播放器用于确定要播放或选择的编码视频的逻辑取决于以下算法：

1. 視訊播放器會根據位元速率（最接近在播放器本身中為「初始位元速率」設定的值）載入初始視訊片段。
1. 視訊播放器會根據使用下列條件的頻寬速度變更進行切換：

   1. 播放器會挑選低於或等於預估頻寬的最高頻寬資料流。
   1. 播放器只考慮80%的可用頻寬。 不過，如果調高了，則比較保守的設定是70%，以避免高估且必須立即調回。

若要檢視演演算法的邏輯，請前往 [https://android.googlesource.com/platform/frameworks/av/+/master/media/libstagefright/httplive/LiveSession.cpp](https://android.googlesource.com/platform/frameworks/av/+/master/media/libstagefright/httplive/LiveSession.cpp) 以取得相關的技術資訊。

為管理單一視訊和自我調整視訊集，Adobe Dynamic Media Classic支援下列專案：

* 以多種支援的視訊格式和音訊格式上傳視訊，並將視訊編碼為MP4 H.264格式，以便跨多個熒幕播放。 您可以使用預先定義的Adobe Dynamic Media Classic最適化視訊預設集、單一視訊編碼預設集，或自訂您自己的編碼來控制視訊的品質和大小。

另請參閱 [啟用或停用自我調整視訊預設集](/help/application-setup.md#activating-or-deactivating-adaptive-video-presets)

另請參閱 [視訊預設集](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/549_video-presets_converted%20renamed_Done-AVS) 訓練影片。

產生最適化視訊集時，其中會包含MP4視訊。

>[!NOTE]
>
>主要/來源視訊和任何其他來源格式視訊為 *not* 新增至最適化視訊集。

* HTML HTML HTML Univeral_Media5_Video、Universal_Media5_MixedMedia_dark和Universal_Media5_Viewers和Universal_Media_Light檢視器中的視訊字幕，以及Universal_Media5_Viewers、Universal_HTMLHTML 5_MixedMedia_dark和Universal_HTML5_MixedMedia_light檢視器中的視訊章節導覽。

   另請參閱 [新增註解至視訊](adding-captions-video.md).

   另請參閱 [將章節標籤新增至視訊](adding-chapter-markers-video.md).

* 利用对元数据的全面支持来组织、浏览和搜索视频，从而高效地管理视频资源。
* 將最適化視訊集傳送至網路、桌上型電腦和行動裝置，包括iPhone、iPad、Android™、BlackBerry®和Windows® phone。

   各種iOS平台均支援最適化視訊串流。

   請參閱以下連結的最新支援： [Adobe檢視器參考指南](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources.html).

   Adobe Dynamic Media Classic支援MP4 H.264視訊的行動視訊播放。 您可以在下列網站找到支援此視訊格式的BlackBerry®裝置：

   另請參閱 [BlackBerry®支援的視訊格式](https://support.blackberry.com/kb/articleDetail?ArticleNumber=000005482).

   您可以在下列位置找到支援此視訊格式的Windows®裝置：

   另請參閱 [Windows® Phone支援的視訊格式](https://docs.microsoft.com/en-us/).

* 使用Adobe Dynamic Media Classic檢視器預設集播放視訊，包括下列專案：

   * 单视频查看器。
   * 兼有视频和图像内容的混合媒体查看器。

* 配置视频播放器来满足您的品牌需求。
* 通过简单的 URL 或嵌入代码将视频集成到您的网站、移动站点或移动应用程序中。

請參閱下列訓練影片：
* [MP4影片概觀](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/563_MP4%20Video%20Overview_converted%20renamed_eVideos-AVS)

* [MP4視訊預覽](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/564_MP4%20Video%20Preview_converted%20renamed_eVideos-AVS)

* [MP4視訊上傳](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/565_MP4%20Video%20Upload_converted%20renamed_eVideos-AVS)

* [串流概述](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/567_Streaming%20Overview_master_eVideos_converted%20renamed_eVideos-AVS)

**快速入門**

下列逐步工作流程說明可協助您快速上手並執行Adobe Dynamic Media Classic中的最適化視訊集。 每個步驟之後，都會有主題標題的互動參照，讓您在其中找到更多資訊。

## 1.上傳視訊並進行編碼

可以使用以下两种方案之一上载并生成自适应视频集：

* **上傳預先編碼的視訊**  — 如果您的視訊已在Adobe Dynamic Media Classic外部編碼，請在全域導覽列上，選取 **[!UICONTROL 上傳]** 瀏覽並直接將MP4視訊檔案上傳至Adobe Dynamic Media Classic。 接著，前往 **[!UICONTROL 建置]** > **[!UICONTROL 最適化視訊集]**. 浏览至您的视频文件。將您想要的視訊檔案拖放到「最適化視訊集」表格中，然後儲存該集合。
* **上傳主要來源影片**  — 如果您的視訊未編碼，請在全域導覽列上選取 **[!UICONTROL 上傳]** 上傳主要視訊來源檔案（非MP4）。 Adobe Dynamic Media Classic會為您將它們編碼為MP4檔案。 在 **[!UICONTROL 上載工作選項]** 對話方塊，下 **[!UICONTROL EVideo選項]**，選取 **[!UICONTROL 自我調整視訊]**.

   通过使用此首选的选项，可以创建一个自适应视频集以自动将正确编码预设应用于视频（不论是 16:9 还是 4:3），以便与您上载的视频尺寸相匹配。當您送出上載工作時，系統會自動為您建立最適化視訊集，其中包含三個以正確外觀比例編碼的視訊設定。

   或者，在同一個 **[!UICONTROL 工作選項]** 對話方塊，下 **[!UICONTROL EVideo選項]**，展開 **[!UICONTROL 單一編碼預設集]**.選取您想要的個別視訊編碼預設集 **案頭**， **行動(iPhone、iPad、Android™)**、和 **平板電腦(iPad、Android™)** 以便建立MP4檔案。

* 或者，您也可以使用重新處理主要視訊 **[!UICONTROL 重新處理]** 功能。 已将最新编码的视频添加到现有的自适应视频集。

另請參閱 [上傳並編碼視訊](uploading-encoding-videos.md#uploading_and_encoding_videos).

**可选**

Adobe Dynamic Media Classic提供許多預先定義的視訊編碼預設集。 這些預先定義的預設集反映了目前最常用的視訊編碼設定，並已針對目標頁面上的播放進行最佳化。

不过，如果需要进一步自定义，管理员可以创建视频预设，以便为最终用户自定义视频大小和播放体验。管理員可以從「 」下方的「 」視訊預設集頁面新增和管理視訊預設集 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 視訊預設集]** > **[!UICONTROL 單一編碼預設集]**. “视频预设”页提供用于添加、编辑、删除和激活视频预设的选项。

另請參閱 [使用視訊編碼預設集](uploading-encoding-videos.md#working_with_video_encoding_presets).

## 2.在視訊檢視器中預覽視訊

若要檢視視訊在案頭、您的網站或行動裝置上播放給使用者的效果，請在「瀏覽」面板中選取視訊，然後選取「 」 **[!UICONTROL 預覽]**.

另請參閱 [在視訊檢視器中預覽視訊](previewing-videos-video-viewer.md#previewing_videos_in_a_video_viewer).

您可以在「預覽」頁面上播放視訊。 您也可以選擇不同的視訊檢視器，瞭解您的視訊在不同播放器中的顯示方式。 作为最佳做法，请使用 HTML5 视频播放器在台式机、平板电脑和移动设备上进行多屏幕播放。

**可选**

檢視器預設集自訂 — Adobe Dynamic Media Classic提供預先定義的檢視器預設集，用於傳送視訊。 这些预设决定了查看器的外观及其播放控件的工作方式。要自定义视频查看器，管理员可以从“视频预设”页中添加和管理视频预设。若要開啟此頁面，請前往Adobe Dynamic Media Classic右上角的 **[!UICONTROL 設定]** > **[!UICONTROL 檢視器預設集]**. “查看器预设”页提供用于添加、编辑、删除和激活查看器预设的命令。

另請參閱 [使用視訊檢視器預設集](previewing-videos-video-viewer.md#working_with_video_viewer_presets).

另請參閱 [視訊預設集](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/549_video-presets_converted%20renamed_Done-AVS) 訓練影片。

## 3.將視訊部署至您的網站和行動網站

要将视频集成到您的网站，您可以执行以下操作之一：

* 在視訊本身的快顯視窗或強制回應視窗中顯示視訊，在此情況下，請使用 **[!UICONTROL 複製URL]** 功能。

   要获取视频的 URL，请在网格视图或列表视图的浏览面板中选择该视频。選取 **[!UICONTROL 預覽]**，然後選取 **[!UICONTROL 複製URL]** 右側 `Universal_HTML5_Viewer`.

   當您選取 **[!UICONTROL 複製URL]**，則會將URL複製到剪貼簿。 将此代码放置在网站、移动站点或应用程序的 HTML 中。

   >[!NOTE]
   >
   >只有在发布视频或自适应视频集后，才会激活 URL。

* 顯示內嵌在網頁上的影片，在此情況下，請使用 **[!UICONTROL 內嵌程式碼]** 功能。

   要获取视频的嵌入代码，请在网格视图或列表视图的浏览面板中选择该视频。前往 **[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**. 在表格的「動作」欄下，選取 **[!UICONTROL 內嵌程式碼]** 右側 `Universal_HTML5_Video`. 不允许编辑代码。

   選取 **[!UICONTROL 關閉]** 並將內嵌程式碼貼到您的網頁中。

   >[!NOTE]
   >
   >只有在发布视频或自适应视频集后，才会激活嵌入代码。

另請參閱 [將視訊部署至您的網站和行動網站](deploying-video-websites-mobile-sites.md#deploying_video_to_your_websites_and_mobile_sites).

>[!MORELIKETHIS]
>
>* [视频编码最佳做法](uploading-encoding-videos.md#best_practices_for_video_encoding)

