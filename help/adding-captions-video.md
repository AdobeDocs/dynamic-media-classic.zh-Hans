---
title: '在视频中添加字幕 '
description: 了解如何在AdobeDynamic Media Classic中向视频添加字幕。
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: 66a1ab20-6036-4c3d-bb66-dd06d917c7f2
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '904'
ht-degree: 32%

---

# 在视频中添加字幕 {#adding-captions-to-video}

您可以在单个视频或自适应视频集中添加题注，以便将视频范围扩大到全球市场。通过添加题注，可以避免为音频配音或针对每种不同的语言使用说母语的人来重新录制音频的操作。视频使用录制时的语言播放。同时显示外语字幕，以便使用不同语言的人也可以理解音频内容。

通过添加题注，还可以使耳聋或者有听力障碍的人也可以访问这部分内容。

>[!NOTE]
>
>所用的视频播放器必须支持题注的显示。

要配置题注效果并编辑题注菜单本身，包括以下任意查看器的菜单文本：

* `Universal_HTML5_Video` 查看者
* `Universal_HTML5_MixedMedia_dark` 查看者
* `Universal_HTML5_MixedMedia_light` 查看者

请参阅[添加或编辑视频查看器预设](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset)。

另请参阅[添加和编辑查看器预设](application-setup.md#adding_and_editing_viewer_presets)。

AdobeDynamic Media Classic可以将题注文件转换为JSON（JavaScript对象表示法）格式。 这种转换意味着，您可以将 JSON 文本作为视频的隐藏但完整的文本嵌入到网页中。然后，搜索引擎可以爬网并索引内容，以使视频更容易被发现，并为客户提供有关视频内容的更多详细信息。

请参阅&#x200B;*Adobe图像服务API帮助*&#x200B;中的[服务静态（非图像）内容](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/c-serving-static-nonimage-contents.html?lang=en#image-serving-api) ，以了解有关在URL中使用JSON函数的更多信息。

**在视频中添加题注:**

1. 使用AdobeDynamic Media Classic之外的第三方应用程序，根据您使用的查看器类型创建视频字幕文件。

   | 查看器类型 | 题注文件 |
   |--- |--- |
   | HTML5 | 如果您使用 HTML5 视频查看器，请确保您创建的题注文件遵循 WebVTT（Web 视频文本跟踪）标准。题注文件的扩展名为 .vtt。您可以了解有关 WebVTT 题注标准的详细信息。<br><br>[请参阅WebVTT](https://w3c.github.io/webvtt/):Web视频文本跟踪格式。<br><br>工具和服务的免费和付费均可用于在Dynamic Media Classic之外创作题注文件Adobe。例如，要创建不带样式的简单视频字幕文件，您可以使用以下免费的在线字幕创作和编辑工具：<br><br>[WebVTT字幕生成器](https://testdrive-archive.azurewebsites.net/Graphics/CaptionMaker/Default.html) <br><br>为获得最佳结果，请使用Internet Explorer 9或更高版本、Google Chrome或Safari中的工具。 <br><br>在工具的输入视 <b>频文件的URL字</b> 段中，粘贴视频文件的URL，然后选择 <b>加载</b>。<br><br>例如，如果您的视频文件使用AdobeDynamic Media Classic URL，请双击单个视频资产(不是自适应视频集或主控视频)以在详细信息视图中将其打开。在“详细信息视图”的右侧面板中，展开“URL 和嵌入代码”。然后，在移动设备组右侧（渐进式）下，选择<b>复制URL</b>。 此过程会为您提供视频文件本身的URL，然后您可以将该URL粘贴到<b>输入视频文件</b>的URL字段中。 随后，Internet Explorer、Chrome 或 Safari 可以本机播放视频。现在，按照屏幕上的站点说明创作并保存您的 WebVTT 文件。完成后，复制题注文件内容并将其粘贴到纯文本编辑器中，并以VTT文件扩展名进行保存。 <br><br><b>注意：</b> 要全局支持英语以外的语言的视频字幕，WebVTT标准要求您为要支持的每种语言分别创建单独的.vtt文件和调用。<br><br>通常，您需要以视频文件的名称来命名题注 VTT 文件，并在后面附加 captions。这有助于使用现有的 Web 内容管理系统自动生成视频 URL。 |

1. 在AdobeDynamic Media Classic中，上载WebVTT、DFXP或SMPTE XML字幕文件。

   请参阅[上传文件](uploading-files.md#uploading_files)。

1. 在左侧的“资源库”面板中，导航至要与上载的题注文件相关联的视频文件所在的资源文件夹。
1. 在“资产浏览”面板中，选择一个视频资产，然后在资产的缩略图图像下方，选择&#x200B;**[!UICONTROL 预览]** > **[!UICONTROL 查看器列表]**。
1. 在“查看器列表”表中，找到名为&#x200B;**Univeral_HTML5_Video**、**Universal_HTML5_MixedMedia_dark**&#x200B;或&#x200B;**Universal_HTML5_MixedMedia_light**&#x200B;的HTML5查看器，然后执行下列操作之一：

   * 对于弹出式视频查看器体验，请选择名称最右侧的&#x200B;**[!UICONTROL 复制URL]**。

      将复制的视频URL附加以下语法，以便将其与复制的URL关联到您的字幕文件：

      `&caption=<full Copy URL path to the caption file .vtt>,1`

      请注意标题URL路径末尾的`,1`。 在路径中的VTT文件扩展名后，您可以选择启用或禁用视频播放器栏上的隐藏式字幕按钮，方法是分别将设置为`1`或`0`。

   * 对于嵌入式视频查看器体验，请选择名称最右侧的&#x200B;**[!UICONTROL 嵌入代码]**。

      在“嵌入代码”对话框中，选择&#x200B;**[!UICONTROL 复制到剪贴板]**。

      对于HTML5 `Universal_HTML5_Video`、`Universal_HTML5_MixedMedia_dark`或`Universal_HTML5_MixedMedia_light`查看器，将复制的嵌入代码附加到以下内容：

      `videoViewer.setParam("caption","<full Copy URL path to the caption file .vtt>,1”`

      请注意URL路径末尾的`,1`。 在URL路径中紧靠VTT文件扩展名后，您可以选择启用或禁用视频播放器栏上的题注按钮，方法是分别将设置为`1`或`0`。
