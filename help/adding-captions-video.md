---
title: 在视频中添加题注
description: 了解如何向视频中添加字幕
uuid: 4cc64469-4369-44a9-83db-63bad51aba8a
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic，查看器，视频
role: 业务从业者
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '912'
ht-degree: 63%

---


# 在视频中添加题注{#adding-captions-to-video}

您可以在单个视频或自适应视频集中添加题注，以便将视频范围扩大到全球市场。通过添加题注，可以避免为音频配音或针对每种不同的语言使用说母语的人来重新录制音频的操作。视频使用录制时的语言播放。同时显示外语字幕，以便使用不同语言的人也可以理解音频内容。

通过添加题注，还可以使耳聋或者有听力障碍的人也可以访问这部分内容。

>[!NOTE]
>
>所用的视频播放器必须支持题注的显示。

请参阅[添加或编辑视频查看器预设](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset)以配置题注效果和编辑题注菜单本身，包括任何以下查看器的菜单文本：

* `Universal_HTML5_Video` 查看者.
* `Universal_HTML5_MixedMedia_dark` 查看者.
* `Universal_HTML5_MixedMedia_light` 查看者.

请参阅[添加和编辑查看器预设](application-setup.md#adding_and_editing_viewer_presets)。

Dynamic Media Classic能够将题注文件转换为JSON（JavaScript对象表示法）格式。 这种转换意味着，您可以将 JSON 文本作为视频的隐藏但完整的文本嵌入到网页中。然后，搜索引擎可以对内容进行爬网和索引，以便更轻松地找到视频，并为客户提供有关视频内容的附加详细信息。

有关在URL中使用JSON函数的详细信息，请参阅&#x200B;*Adobe图像服务API帮助*&#x200B;中的[服务静态（非图像）内容](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/c-serving-static-nonimage-contents.html?lang=en#image-serving-api)。

**在视频中添加题注**

1. 在Dynamic Media Classic外部使用第三方应用程序，根据您使用的查看器类型创建视频题注文件。

   | 查看器类型 | 题注文件 |
   |--- |--- |
   | HTML5 | 如果您使用 HTML5 视频查看器，请确保您创建的题注文件遵循 WebVTT（Web 视频文本跟踪）标准。题注文件的扩展名为 .vtt。您可以了解有关 WebVTT 题注标准的详细信息。<br><br>[请参阅WebVTT](https://dev.w3.org/html5/webvtt/):Web视频文本轨道格式。<br><br>在Dynamic Media Classic之外，您可以使用免费和付费的工具和服务创作题注文件。例如，要创建没有样式的简单视频题注文件，可以使用以下免费的在线题注创作和编辑工具：<br><br>[WebVTT题注生成器](https://testdrive-archive.azurewebsites.net/Graphics/CaptionMaker/Default.html) <br><br>为获得最佳效果，请使用Internet Explorer 9或更高版本、Google Chrome或Safari中的工具。 <br><br>在工具的“<b>输入视频文件的 URL</b>”字段中粘贴您的视频文件的 URL，然后单击“<b>载入</b>”。<br><br>例如，如果您正在为视频文件使用Dynamic Media Classic URL，则在DMC中，按住多次单击单个视频资产(而非自适应视频集或主控视频)，以在详细信息视图中打开它。在“详细信息视图”的右侧面板中，展开“URL 和嵌入代码”。然后在“移动设备”组下“移动设备（渐进式）”的右侧，单击“复制 URL”。此过程会为您提供视频文件本身的URL，然后您可以将该URL粘贴到视频文件</b>的<b>输入URL字段中。 随后，Internet Explorer、Chrome 或 Safari 可以本机播放视频。现在，按照屏幕上的站点说明创作并保存您的 WebVTT 文件。在完成后，将题注文件内容复制并粘贴到纯文本编辑器中，然后将其保存为扩展名为 .vtt 的文件。<br><br><b>注意：</b> 要全局支持英语以外的语言的视频字幕，请注意，WebVTT标准要求您为要支持的每种语言分别创建单独的.vtt文件和调用。<br><br>通常，您需要以视频文件的名称来命名题注 VTT 文件，并在后面附加 captions。这有助于使用现有的 Web 内容管理系统自动生成视频 URL。 |

1. 在Dynamic Media Classic中，上传WebVTT、DFXP或SMPTE XML题注文件。

   请参阅[上载文件](uploading-files.md#uploading_files)。

1. 在左侧的“资源库”面板中，导航至要与上载的题注文件相关联的视频文件所在的资源文件夹。
1. 在“资源浏览”面板中，选择单个视频资源，然后在资源的缩览图图像下方单击“**[!UICONTROL 预览]**”>“**[!UICONTROL 查看器列表]**”。
1. 在“查看器”列表表中，找到名为&#x200B;**Univeral_HTML5_Video**、**Universal_HTML5_MixedMedia_dark**&#x200B;或&#x200B;**Universal_HTML5_MixedMedia_light**&#x200B;的HT，然后执行以下操作之一：

   * 针对弹出式视频查看器，请在名称的最右侧单击“**[!UICONTROL 复制 URL]**”。

      使用下列语法附加该视频的已复制 URL，以便将其与您的题注文件的已复制 URL 相关联：

      `&caption=<full Copy URL path to the caption file .vtt>,1`

      请注意题注URL路径末尾的`,1`。 在路径中紧靠 .vtt 文件扩展名后面，您可以选择在视频播放器栏上启用或禁用隐藏式题注按钮，方法是设置为 `1` 以进行启用，或者设置为 `0` 以进行禁用。

   * 为了针对嵌入视频查看器，请在名称的最右侧单击“**[!UICONTROL 嵌入代码]**”。

      在“嵌入代码”对话框中，单击“**[!UICONTROL 复制到剪贴板]**”。

      对于HTML5 `Universal_HTML5_Video`、`Universal_HTML5_MixedMedia_dark`或`Universal_HTML5_MixedMedia_light`查看器，在复制的嵌入代码后面附加以下代码：

      `videoViewer.setParam("caption","<full Copy URL path to the caption file .vtt>,1”`

      请注意URL路径末尾的`,1`。 在 URL 路径中紧靠 .vtt 文件扩展名后面，您可以选择在视频播放器栏上启用或禁用题注按钮，方法是设置为 `1` 以进行启用，或者设置为 `0` 以进行禁用。

