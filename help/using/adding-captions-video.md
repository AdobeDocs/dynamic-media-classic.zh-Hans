---
title: 向视频添加字幕
description: 了解如何在Adobe Dynamic Media Classic中为视频添加字幕。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: 66a1ab20-6036-4c3d-bb66-dd06d917c7f2
topic: Content Management
level: Intermediate
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '705'
ht-degree: 17%

---

# 向视频添加字幕 {#add-captions-to-video}

将视频覆盖范围扩展到全球市场。 为此，您可以向单个视频或自适应视频集添加字幕。 通过添加题注，可以避免为音频配音或针对每种不同的语言使用说母语的人来重新录制音频的操作。视频使用录制时的语言播放。同时显示外语字幕，以便使用不同语言的人也可以理解音频内容。

通过添加题注，还可以使耳聋或者有听力障碍的人也可以访问这部分内容。

>[!NOTE]
>
>所用的视频播放器必须支持题注的显示。

要配置字幕效果并编辑“字幕菜单”本身，包括以下任何查看器的菜单文本：

* `Universal_HTML5_Video` 查看者
* `Universal_HTML5_MixedMedia_dark` 查看者
* `Universal_HTML5_MixedMedia_light` 查看者

请参阅 [添加或编辑视频查看器预设](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset).

另请参阅 [添加和编辑查看器预设](application-setup.md#adding_and_editing_viewer_presets).

Adobe Dynamic Media Classic可以将字幕文件转换为JSON（JavaScript对象表示法）格式。 这种转换意味着，您可以将JSON文本作为隐藏但完整的视频转录内容嵌入到网页中。 然后，搜索引擎可以对内容进行爬网和索引，使视频更容易被发现，并为客户提供有关视频内容的更多详细信息。

请参阅 [提供静态（非图像）内容](https://experienceleague.adobe.com/en/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/c-serving-static-nonimage-contents#image-serving-api) 有关在URL中使用JSON函数的更多信息，请参阅。

**要向视频添加字幕，请执行以下操作：**

1. 使用Adobe Dynamic Media Classic之外的第三方应用程序，根据您使用的查看器类型创建视频字幕文件。

   | 查看器类型 | 题注文件 |
   |--- |--- |
   | HTML5 | 如果您使用 HTML5 视频查看器，请确保您创建的题注文件遵循 WebVTT（Web 视频文本跟踪）标准。字幕文件扩展名为 `.VTT`. 您可以了解有关 WebVTT 题注标准的详细信息。<br><br>[请参阅WebVTT](https://w3c.github.io/webvtt/)：Web视频字幕格式。 <br><br>有许多网站同时提供免费和收费的工具和服务，可用于创作WebVTT字幕文件。 <br><br>按照站点中的屏幕说明创作和保存WebVTT文件。 完成后，复制字幕文件内容并将其粘贴到纯文本编辑器中，并以VTT文件扩展名保存。 <br><br><b>注意：</b> 为了在全球范围内支持英语以外的其他语言的视频字幕，WebVTT标准要求您创建单独的 `.VTT` 要支持的每种语言的文件和调用。 <br><br>通常，您希望将字幕VTT文件的名称与视频文件相同，并附加字幕。 这样，它可以帮助您使用现有Web内容管理系统自动生成视频URL。 |

1. 在Adobe Dynamic Media Classic中，上传WebVTT、DFXP或SMPTE XML描述文件。

   请参阅 [上载文件](uploading-files.md#uploading_files).

1. 在左侧的“资产库”面板中，导航到包含视频文件的资产文件夹，以与您上传的字幕文件相关联。
1. 在“资源浏览”面板中，选择单个视频资源，然后选择该资源的缩略图图像下方 **[!UICONTROL 预览]** > **[!UICONTROL 查看器列表]**.
1. 在“查看器列表”表格中，找到名为的HTML5查看器 **Univeral_HTML5_视频**， **Universal_Media5_MixedMedia_darkHTML**，或 **Universal_HTML5_MixedMedia_light**，然后执行以下操作之一：

   * 要获得弹出式视频查看器体验，请选择 **[!UICONTROL 复制URL]** 在名字的最右边。

     将复制的视频的URL附加到以下语法，以便将其与复制的字幕文件关联：

     `&caption=<full Copy URL path to the caption file .vtt>,1`

     请注意 `,1` 标题URL路径末尾。 紧跟路径中VTT文件扩展名之后，您可以选择通过将设置为来启用或禁用视频播放器栏上的隐藏式字幕按钮 `1` 或 `0`、ID名称和ID名称等。

   * 要获得嵌入式视频查看器体验，请选择 **[!UICONTROL 嵌入代码]** 在名字的最右边。

     在嵌入代码对话框中，选择 **[!UICONTROL 复制到剪贴板]**.

     对于HTML5 `Universal_HTML5_Video`， `Universal_HTML5_MixedMedia_dark`，或 `Universal_HTML5_MixedMedia_light` 查看器，将复制的嵌入代码附加到以下内容：

     `videoViewer.setParam("caption","<full Copy URL path to the caption file .vtt>,1"`

     请注意 `,1` URL路径末尾的。 在URL路径中的VTT文件扩展名之后，您可以选择通过将设置为来启用或禁用视频播放器栏上的字幕按钮 `1` 或 `0`、ID名称和ID名称等。
