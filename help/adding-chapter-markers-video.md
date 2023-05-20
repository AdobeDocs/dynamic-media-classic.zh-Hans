---
title: 將章節標籤新增至視訊
description: 瞭解如何在Adobe Dynamic Media Classic中新增章節標籤至影片。
uuid: 4e1e6daf-afc6-49d9-ac90-183fe2a903b2
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
discoiquuid: 8bc5e552-2abb-41f0-89d2-bdf3ae5d96c2
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: a9250841-2dba-4fdc-8a6e-91b2fecef72f
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '629'
ht-degree: 42%

---

# 將章節標籤新增至視訊 {#adding-chapter-markers-to-video}

可通过在单个视频或自适应视频集中添加章节标记，更轻松地观看和导航较长的视频。使用者播放視訊時，可以在視訊時間軸上選取章節標籤（也稱為視訊筆畫壓感器）。 如此可讓他們輕鬆導覽至興趣點，或立即跳至新內容、示範、教學課程等。

>[!NOTE]
>
>使用的视频播放器必须支持使用章节标记。

另請參閱 [新增或編輯視訊檢視器預設集](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset) 如果您想要為以下專案設定章節導覽提示點和章節標題彈出式文字： `Universal_HTML5_Video` 檢視器(HTML5)。

另請參閱 [新增和編輯檢視器預設集](application-setup.md#adding_and_editing_viewer_presets).

可以按照与创建题注非常类似的方法为视频创建章节列表。即，创建一个 WebVTT 文件。但要注意，该文件不能与可能还会使用的任何 WebVTT 题注文件相同；无法将题注和章节合并到一个 WebVTT 文件中。

您可以将以下示例作为用于创建具有章节导航的 WebVTT 文件的格式示例：

```as3
WEBVTT 
Chapter 1 
00:00.000 --> 01:04.364 
The bicycle store behind it all. 
Chapter 2 
01:04.364 --> 02:00.944 
Creative Cloud. 
Chapter 3 
02:00.944 --> 03:02.937 
Ease of management for a working solution. 
Chapter 4 
03:02.937 --> 03:35.000 
Cost-efficient access to rapidly evolving technology.
```

在上面的示例中，`Chapter 1` 是可选的提示标识符。的提示時間 `00:00:000 --> 01:04:364` 指定章節的開始時間和結束時間（以00為單位）:00:000格式。 最后三个数字是毫秒；如果需要，可以将其保留为 000。的章節標題 `The bicycle store behind it all` 是章節內容的實際說明。 當指標暫留在視訊時間軸中的視覺提示點上時，提示識別碼、開始提示時間和章節標題都會顯示在視訊播放器的快顯視窗中。

由于使用的是 HTML5 视频查看器，请确保创建的章节文件遵循 WebVTT（Web 视频文本跟踪）标准。章節副檔名為.VTT。 您可以了解有关 WebVTT 题注标准的详细信息。

另請參閱 [WebVTT：網頁視訊文字追蹤格式](https://w3c.github.io/webvtt/).

**在视频中添加章节标记:**

1. 使用Adobe Dynamic Media Classic外部的簡單文字編輯器，建立您的視訊章節檔案。

   >[!NOTE]
   >
   >為了全球支援英文以外的其他語言的視訊章節，WebVTT標準要求您為要支援的每種語言建立個別的.vtt檔案和呼叫。

1. 將VTT檔案儲存為UTF8編碼，這樣就能避免在章節標題文字中出現字元轉譯問題。

   通常，您希望使用视频文件名命名章节 VTT 文件，并在后面附加 `chapters`。这有助于使用现有的 Web 内容管理系统自动生成视频 URL。

1. 在Adobe Dynamic Media Classic中，上傳您的WebVTT章節檔案。

   另請參閱 [上傳檔案](uploading-files.md#uploading_files).

1. 在左侧的“资源库”面板中，导航到包含要与上载的章节文件关联的视频文件的资源文件夹。
1. 在「資產瀏覽」面板中，選取單一視訊資產，然後在資產的縮圖影像下方選取「 」 **[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**.
1. 在“查看器列表”表中，找到名为 **Univeral_HTML5_Video** 的 HTML5 查看器，然后执行以下操作之一：

   * 若要取得快顯視訊檢視器體驗，請選取「 」 **[!UICONTROL 複製URL]** 名稱的最右側。

      將複製的影片URL附加至下列語法，這樣您就可以將它與複製的URL與註解檔案建立關聯：

      `&navigation=*<full Copy URL path to the chapter navigation file .vtt>*`

   * 若要內嵌視訊檢視器體驗，請選取「 」 **[!UICONTROL 內嵌程式碼]** 名稱的最右側。

      在內嵌程式碼對話方塊中，選取 **[!UICONTROL 複製到剪貼簿]**.

      針對HTML5 `Universal_HTML5_Video` 檢視器，請在複製的內嵌程式碼後附加下列內容：

      `videoViewer.setParam("navigation","*<full Copy URL path to the chapter navigation file .vtt>*”`
