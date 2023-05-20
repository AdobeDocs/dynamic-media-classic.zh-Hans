---
title: 新增註解至視訊
description: 瞭解如何在Adobe Dynamic Media Classic中為影片新增字幕。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: 66a1ab20-6036-4c3d-bb66-dd06d917c7f2
source-git-commit: cb55e09a997b9d36002c4ac429603576d52fb8bd
workflow-type: tm+mt
source-wordcount: '904'
ht-degree: 32%

---

# 新增註解至視訊 {#adding-captions-to-video}

您可以在单个视频或自适应视频集中添加题注，以便将视频范围扩大到全球市场。通过添加题注，可以避免为音频配音或针对每种不同的语言使用说母语的人来重新录制音频的操作。视频使用录制时的语言播放。同时显示外语字幕，以便使用不同语言的人也可以理解音频内容。

通过添加题注，还可以使耳聋或者有听力障碍的人也可以访问这部分内容。

>[!NOTE]
>
>所用的视频播放器必须支持题注的显示。

若要設定「註解效果」並編輯「註解選單」本身，包括下列任一檢視器的選單文字：

* `Universal_HTML5_Video` 查看者
* `Universal_HTML5_MixedMedia_dark` 查看者
* `Universal_HTML5_MixedMedia_light` 查看者

另請參閱 [新增或編輯視訊檢視器預設集](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset).

另請參閱 [新增和編輯檢視器預設集](application-setup.md#adding_and_editing_viewer_presets).

Adobe Dynamic Media Classic可以將註解檔案轉換為JSON （JavaScript物件標籤法）格式。 这种转换意味着，您可以将 JSON 文本作为视频的隐藏但完整的文本嵌入到网页中。搜尋引擎接著可以編目和索引內容，讓視訊更容易被發現，並為客戶提供更多有關視訊內容的詳細資訊。

另請參閱 [提供靜態（非影像）內容](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/c-serving-static-nonimage-contents.html?lang=en#image-serving-api) 在 *Adobe影像伺服API說明* 以取得在URL中使用JSON函式的詳細資訊。

**在视频中添加题注:**

1. 使用Adobe Dynamic Media Classic外部的第三方應用程式，根據您使用的檢視器型別建立您的視訊註解檔案。

   | 查看器类型 | 题注文件 |
   |--- |--- |
   | HTML5 | 如果您使用 HTML5 视频查看器，请确保您创建的题注文件遵循 WebVTT（Web 视频文本跟踪）标准。题注文件的扩展名为 .vtt。您可以了解有关 WebVTT 题注标准的详细信息。<br><br>[請參閱WebVTT](https://w3c.github.io/webvtt/)：網頁視訊文字追蹤格式。 <br><br>您可以在Adobe Dynamic Media Classic外部使用免費和付費的工具和服務來製作註解檔案。 例如，若要建立不含樣式的簡單視訊註解檔案，您可以使用下列免費線上註解製作與編輯工具： <br><br>[WebVTT註解製作器](https://testdrive-archive.azurewebsites.net/Graphics/CaptionMaker/Default.html) <br><br>為達到最佳效果，請在Internet Explorer 9或更新版本、Google Chrome或Safari中使用工具。 <br><br>在工具中，在 <b>輸入視訊檔案的URL</b> 欄位，貼上視訊檔案的URL，然後選取 <b>載入</b>. <br><br>例如，如果您正在使用Adobe Dynamic Media Classic URL作為視訊檔案，請按兩下個別視訊資產（非最適化視訊集或主要視訊）以在「詳細資料檢視」中開啟它。 在“详细信息视图”的右侧面板中，展开“URL 和嵌入代码”。然後在「行動」群組下方的「行動」 （漸進式）右側，選取 <b>複製URL</b>. 此程式會提供視訊檔案本身的URL，您隨後可將其貼到 <b>輸入視訊檔案的URL</b> 欄位。 随后，Internet Explorer、Chrome 或 Safari 就可以在本机播放视频。现在，按照屏幕上的站点说明创作并保存您的 WebVTT 文件。完成後，複製註解檔案內容並將其貼到純文字編輯器中，並以VTT副檔名儲存。 <br><br><b>注意：</b> 為了全球支援英文以外的其他語言的視訊註解，WebVTT標準要求您建立個別的.vtt檔案，並針對您想要支援的每種語言呼叫。 <br><br>通常，您需要以视频文件的名称来命名题注 VTT 文件，并在后面附加 captions。这有助于使用现有的 Web 内容管理系统自动生成视频 URL。 |

1. 在Adobe Dynamic Media Classic中，上傳您的WebVTT、DFXP或SMPTE XML註解檔案。

   另請參閱 [上傳檔案](uploading-files.md#uploading_files).

1. 在左侧的“资源库”面板中，导航至要与上载的题注文件相关联的视频文件所在的资源文件夹。
1. 在「資產瀏覽」面板中，選取單一視訊資產，然後在資產的縮圖影像下方選取「 」 **[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**.
1. 在「檢視器清單」表格中，找到名為的HTML5檢視器 **Univeral_HTML5_影片**， **Universal_HTML5_MixedMedia_dark**，或 **Universal_HTML5_MixedMedia_light**，然後執行下列任一項作業：

   * 若要取得快顯視訊檢視器體驗，請選取「 」 **[!UICONTROL 複製URL]** 名稱的最右側。

      將複製的影片URL附加至下列語法，這樣您就可以將它與複製的URL與註解檔案建立關聯：

      `&caption=<full Copy URL path to the caption file .vtt>,1`

      請注意 `,1` 在註解URL路徑結尾。 路徑中的VTT副檔名後面緊接著可以設定為，選擇性地啟用或停用視訊播放器列上的隱藏式字幕按鈕 `1` 或 `0`（分別）。

   * 若要內嵌視訊檢視器體驗，請選取「 」 **[!UICONTROL 內嵌程式碼]** 名稱的最右側。

      在內嵌程式碼對話方塊中，選取 **[!UICONTROL 複製到剪貼簿]**.

      針對HTML5 `Universal_HTML5_Video`， `Universal_HTML5_MixedMedia_dark`，或 `Universal_HTML5_MixedMedia_light` 檢視器，請在複製的內嵌程式碼後附加下列內容：

      `videoViewer.setParam("caption","<full Copy URL path to the caption file .vtt>,1”`

      請注意 `,1` 在URL路徑結尾。 在URL路徑中的VTT副檔名後面，您可以視需要選擇將設定為，啟用或停用視訊播放器列上的註解按鈕 `1` 或 `0`（分別）。
