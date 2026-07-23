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
autotag-review: '2026-05-13T17:37:15.687Z'
TQID: 'https://experienceleague.adobe.com/7o-hO9obr6JB8sIHWQ3KTC6dRzxIBYqlOJOAbanTig0'
product_v2: id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
source-git-commit: a41ad4865cfa5692ed38c030b45fbb579ce2b3f9
workflow-type: tm+mt
source-wordcount: 609
ht-degree: 12%

---

# 向视频添加章节标记 {#adding-chapter-markers-to-video}

您可以通过将章节标记添加到单个视频或自适应视频集，使长格式视频更易于观看和导航。 当用户播放视频时，可以选择视频时间轴上的章节标记（也称为视频洗刷）。 这样做可让他们轻松导航到兴趣点，或立即跳转到新内容、演示、教程等。

>[!NOTE]
>
>视频播放器必须支持使用章节标记。

如果要为`Universal_HTML5_Video`查看器(HTML5)配置章节导航提示点和章节标题弹出文本，请参阅[添加或编辑视频查看器预设](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset)。

另请参阅[添加和编辑查看器预设](application-setup.md#adding_and_editing_viewer_presets)。

可以按照与创建题注非常类似的方法为视频创建章节列表。 即，创建一个 WebVTT 文件。 但请注意，此文件必须与您使用的任何WebVTT字幕文件分开；请勿将字幕和章节合并到一个WebVTT文件中。

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

在上述示例中，`Chapter 1`是提示标识符，是可选的。 `00:00:000 --> 01:04:364`的提示时间以00:00:000格式指定章节的开始时间和结束时间。 最后三位数为毫秒，可保留为000（如果首选）。 `The bicycle store behind it all`的章节标题是章节内容的描述。 当指针悬停在视频时间轴上的可视提示点上时，提示标识符、开始提示时间和章节标题会显示在视频播放器弹出窗口中。

由于使用的是 HTML5 视频查看器，请确保创建的章节文件遵循 WebVTT（Web 视频文本跟踪）标准。 章节文件扩展名为`.VTT`。 您可以了解有关 WebVTT 题注标准的详细信息。

请参阅[WebVTT： Web视频字幕格式](https://w3c.github.io/webvtt/)。

**向视频添加章节标记：**

1. 使用Adobe Dynamic Media Classic外部的简单文本编辑器，创建视频章节文件。

   >[!NOTE]
   >
   >要获得英语以外的语言视频章节的全球支持，WebVTT标准要求您为要支持的每种语言创建单独的`.VTT`文件和调用。

1. 请将VTT文件保存为UTF-8编码，这样就可以避免在章节标题文本中出现字符演绎版问题。

   将章节VTT文件命名为与视频文件相同的名称，并将其附加到`_chapters`。 这样做可以帮助您使用现有Web内容管理系统自动生成视频URL。

1. 在Adobe Dynamic Media Classic中，上传WebVTT章节文件。

   查看[上载文件](uploading-files.md#uploading_files)。

1. 在左侧的“资产库”面板中，导航到资产文件夹，该文件夹包含要与您上传的章节文件关联的视频文件。
1. 在“资源浏览”面板中，选择单个视频资源，然后在资源的缩略图图像下方选择&#x200B;**[!UICONTROL 预览]** > **[!UICONTROL 查看器列表]**。
1. 在“查看器列表”表中，找到名为&#x200B;**Universal_HTML5_Video**&#x200B;的HTML5查看器，然后执行下列操作之一：

   * 若要获得弹出式视频查看器体验，请选择名称最右边的&#x200B;**[!UICONTROL 复制URL]**。

     将复制的视频的URL附加到以下语法，以便将其与复制的字幕文件关联：

     `&navigation=*<full Copy URL path to the chapter navigation file .vtt>*`

   * 对于嵌入的视频查看器体验，请选择名称最右侧的&#x200B;**[!UICONTROL 嵌入代码]**。

     在“嵌入代码”对话框中，选择&#x200B;**[!UICONTROL 复制到剪贴板]**。

     对于HTML5 `Universal_HTML5_Video`查看器，请将复制的嵌入代码附加到以下内容：

     `videoViewer.setParam("navigation","*<full Copy URL path to the chapter navigation file .vtt>*"`
