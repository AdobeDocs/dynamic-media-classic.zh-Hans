---
title: 向视频添加章节标记
description: 了解如何在Adobe Dynamic Media Classic中为视频添加章节标记。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: a9250841-2dba-4fdc-8a6e-91b2fecef72f
topic: Content Management
level: Intermediate
source-git-commit: ad7e20fdbe9028c6255865cce95d109f9e9eeab2
workflow-type: tm+mt
source-wordcount: '622'
ht-degree: 24%

---

# 向视频添加章节标记 {#adding-chapter-markers-to-video}

您可以通过将章节标记添加到单个视频或自适应视频集，使长格式视频更易于观看和导航。 当用户播放视频时，可以选择视频时间轴上的章节标记（也称为视频洗刷）。 这样做可让他们轻松导航到兴趣点，或立即跳转到新内容、演示、教程等。

>[!NOTE]
>
>使用的视频播放器必须支持使用章节标记。

如果要为`Universal_HTML5_Video`查看器配置章节导航提示点和章节标题弹出文本(HTML5)，请参阅[添加或编辑视频查看器预设](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset)。

另请参阅[添加和编辑查看器预设](application-setup.md#adding_and_editing_viewer_presets)。

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

在上述示例中，`Chapter 1`是提示标识符，是可选的。 `00:00:000 --> 01:04:364`的提示时间以00:00:000格式指定章节的开始时间和结束时间。 最后三个数字是毫秒；如果需要，可以将其保留为 000。`The bicycle store behind it all`的章节标题是章节内容的实际描述。 当指针悬停在视频时间轴中的可视提示点上时，提示标识符、开始提示时间和章节标题都会显示在视频播放器的弹出窗口中。

由于使用的是 HTML5 视频查看器，请确保创建的章节文件遵循 WebVTT（Web 视频文本跟踪）标准。章节文件扩展名为`.VTT`。 您可以了解有关 WebVTT 题注标准的详细信息。

请参阅[WebVTT： Web视频字幕格式](https://w3c.github.io/webvtt/)。

**向视频添加章节标记：**

1. 使用Adobe Dynamic Media Classic外部的简单文本编辑器，创建视频章节文件。

   >[!NOTE]
   >
   >要获得英语以外的语言视频章节的全球支持，WebVTT标准要求您为要支持的每种语言创建单独的`.VTT`文件和调用。

1. 将VTT文件保存为UTF8编码，这样可以避免章节标题文本中的字符呈现出现问题。

   通常，您希望将章节VTT文件命名为与视频文件相同的名称，并将其附加到`chapters`。 这样，它可以帮助您使用现有Web内容管理系统自动生成视频URL。

1. 在Adobe Dynamic Media Classic中，上传WebVTT章节文件。

   查看[上载文件](uploading-files.md#uploading_files)。

1. 在左侧的“资产库”面板中，导航到资产文件夹，该文件夹包含要与您上传的章节文件关联的视频文件。
1. 在“资源浏览”面板中，选择单个视频资源，然后在资源的缩略图图像下方选择&#x200B;**[!UICONTROL 预览]** > **[!UICONTROL 查看器列表]**。
1. 在“查看器列表”表中，找到名为 **Univeral_HTML5_Video** 的 HTML5 查看器，然后执行以下操作之一：

   * 若要获得弹出式视频查看器体验，请选择名称最右边的&#x200B;**[!UICONTROL 复制URL]**。

     将复制的视频的URL附加到以下语法，以便将其与复制的字幕文件关联：

     `&navigation=*<full Copy URL path to the chapter navigation file .vtt>*`

   * 对于嵌入的视频查看器体验，请选择名称最右侧的&#x200B;**[!UICONTROL 嵌入代码]**。

     在“嵌入代码”对话框中，选择&#x200B;**[!UICONTROL 复制到剪贴板]**。

     对于HTML5 `Universal_HTML5_Video`查看器，将复制的嵌入代码附加到以下内容：

     `videoViewer.setParam("navigation","*<full Copy URL path to the chapter navigation file .vtt>*"`
