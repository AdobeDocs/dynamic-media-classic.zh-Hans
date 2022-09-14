---
title: 向视频添加章节标记
description: 了解如何在Adobe Dynamic Media Classic中向视频添加章节标记。
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

# 向视频添加章节标记 {#adding-chapter-markers-to-video}

可通过在单个视频或自适应视频集中添加章节标记，更轻松地观看和导航较长的视频。当用户播放视频时，他们可以选择视频时间轴上的章节标记（也称为视频清理器）。 这样，他们就可以轻松导航到自己的目标点，或立即跳转到新内容、演示、教程等。

>[!NOTE]
>
>使用的视频播放器必须支持使用章节标记。

请参阅 [添加或编辑视频查看器预设](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset) 如果要为 `Universal_HTML5_Video` 查看器(HTML5)。

另请参阅 [添加和编辑查看器预设](application-setup.md#adding_and_editing_viewer_presets).

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

在上面的示例中，`Chapter 1` 是可选的提示标识符。的提示时间 `00:00:000 --> 01:04:364` 指定章节的开始时间和结束时间（以00为单位）:00:000格式。 最后三个数字是毫秒；如果需要，可以将其保留为 000。的章节标题 `The bicycle store behind it all` 是章节内容的实际描述。 当指针悬停在视频时间轴中的可视提示点上时，提示标识符、开始提示时间和章节标题都会显示在视频播放器的弹出窗口中。

由于使用的是 HTML5 视频查看器，请确保创建的章节文件遵循 WebVTT（Web 视频文本跟踪）标准。章节文件扩展名为.VTT。 您可以了解有关 WebVTT 题注标准的详细信息。

请参阅 [WebVTT:Web视频文本跟踪格式](https://w3c.github.io/webvtt/).

**在视频中添加章节标记:**

1. 使用Adobe Dynamic Media Classic外的简单文本编辑器，创建视频章节文件。

   >[!NOTE]
   >
   >为全球支持英语以外语言的视频章节，WebVTT标准要求您为要支持的每种语言分别创建单独的.vtt文件和调用。

1. 以UTF8编码格式保存VTT文件，以避免章节标题文本中的字符呈现问题。

   通常，您希望使用视频文件名命名章节 VTT 文件，并在后面附加 `chapters`。这有助于使用现有的 Web 内容管理系统自动生成视频 URL。

1. 在Adobe Dynamic Media Classic中，上传您的WebVTT章节文件。

   请参阅 [上传文件](uploading-files.md#uploading_files).

1. 在左侧的“资源库”面板中，导航到包含要与上载的章节文件关联的视频文件的资源文件夹。
1. 在资产浏览面板中，选择一个视频资产，然后在资产的缩略图下方，选择 **[!UICONTROL 预览]** > **[!UICONTROL 查看器列表]**.
1. 在“查看器列表”表中，找到名为 **Univeral_HTML5_Video** 的 HTML5 查看器，然后执行以下操作之一：

   * 要获得弹出式视频查看器体验，请选择 **[!UICONTROL 复制URL]** 最右边。

      将复制的视频URL附加以下语法，以便将其与复制的URL关联到您的字幕文件：

      `&navigation=*<full Copy URL path to the chapter navigation file .vtt>*`

   * 对于嵌入式视频查看器体验，请选择 **[!UICONTROL 嵌入代码]** 最右边。

      在“嵌入代码”对话框中，选择 **[!UICONTROL 复制到剪贴板]**.

      对于HTML5 `Universal_HTML5_Video` 查看器中，将复制的嵌入代码附加到以下内容：

      `videoViewer.setParam("navigation","*<full Copy URL path to the chapter navigation file .vtt>*”`
