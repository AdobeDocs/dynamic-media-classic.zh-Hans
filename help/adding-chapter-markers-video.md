---
title: 在视频中添加章节标记
seo-title: 在视频中添加章节标记
description: 'null'
seo-description: 了解如何向视频添加章节标记。
uuid: 4e1e6daf-afc6-49d9-ac90-183fe2a903b2
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
discoiquuid: 8bc5e552-2abb-41f0-89d2-bdf3ae5d96c2
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '625'
ht-degree: 88%

---


# 在视频中添加章节标记{#adding-chapter-markers-to-video}

可通过在单个视频或自适应视频集中添加章节标记，更轻松地观看和导航较长的视频。在用户播放视频时，他们可以单击视频时间轴（也称为视频洗刷）上的章节标记以轻松导航到焦点，或者立即跳到新的内容、演示和教程，等等。

>[!NOTE]
>
>使用的视频播放器必须支持使用章节标记。

请参阅[添加或编辑视频查看器预设](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset)，以便为 `Universal_HTML5_Video` 查看器 (HTML5) 配置章节导航提示点和章节标题弹出文本。

请参阅[添加和编辑查看器预设](application-setup.md#adding_and_editing_viewer_presets)。

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

在上面的示例中，`Chapter 1` 是可选的提示标识符。`00:00:000 --> 01:04:364` 提示时间使用 00:00:000 格式指定章节的开始和结束时间。最后三个数字是毫秒；如果需要，可以将其保留为 000。The chapter title of `The bicycle store behind it all` is the actual description of the chapter’s contents. 在用户将鼠标指针悬停在视频时间轴中的可视提示点上时，将在视频播放器的弹出窗口中显示提示标识符、开始提示时间和章节标题。

由于使用的是 HTML5 视频查看器，请确保创建的章节文件遵循 WebVTT（Web 视频文本跟踪）标准。章节文件的扩展名为 .vtt。您可以了解有关 WebVTT 题注标准的详细信息。

See [WebVTT: The Web Video Text Tracks format](https://dev.w3.org/html5/webvtt/).

**在视频中添加章节标记**

1. 在Dynamic Media经典之外使用简单的文本编辑器创建视频章节文件。

   >[!NOTE]
   >
   >要让视频章节获得英语之外的其他语言的全球支持，请注意，WebVTT 标准要求为每种要支持的语言创建单独的 .vtt 文件和调用。

1. 使用 UTF8 编码保存 .vtt 文件，以避免章节标题文本出现字符再现问题。

   通常，您希望使用视频文件名命名章节 VTT 文件，并在后面附加 `chapters`。这有助于使用现有的 Web 内容管理系统自动生成视频 URL。

1. 在Dynamic Media经典中，上传WebVTT章文件。

   请参阅[上载文件](uploading-files.md#uploading_files)。

1. 在左侧的“资源库”面板中，导航到包含要与上载的章节文件关联的视频文件的资源文件夹。
1. 在“资源浏览”面板中，选择单个视频资源，然后单击资源缩览图下面的“**预览**”>“**查看器列表**”。
1. 在“查看器列表”表中，找到名为 **Univeral_HTML5_Video** 的 HTML5 查看器，然后执行以下操作之一：

   * 针对弹出式视频查看器，请在名称的最右侧单击“**复制 URL**”。

      使用下列语法附加该视频的已复制 URL，以便将其与您的题注文件的已复制 URL 相关联：

      `&navigation=*<full Copy URL path to the chapter navigation file .vtt>*`

   * 为了针对嵌入视频查看器，请在名称的最右侧单击“**嵌入代码**”。

      在“嵌入代码”对话框中，单击“**复制到剪贴板**”。

      For the HTML5 `Universal_HTML5_Video` viewer, append the copied embed code with the following:

      `videoViewer.setParam("navigation","*<full Copy URL path to the chapter navigation file .vtt>*”`

