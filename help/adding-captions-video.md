---
title: 向视频添加字幕
description: 了解如何在Adobe Dynamic Media Classic中为视频添加字幕。
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

# 向视频添加字幕 {#adding-captions-to-video}

您可以在单个视频或自适应视频集中添加题注，以便将视频范围扩大到全球市场。通过添加题注，可以避免为音频配音或针对每种不同的语言使用说母语的人来重新录制音频的操作。视频使用录制时的语言播放。同时显示外语字幕，以便使用不同语言的人也可以理解音频内容。

通过添加题注，还可以使耳聋或者有听力障碍的人也可以访问这部分内容。

>[!NOTE]
>
>所用的视频播放器必须支持题注的显示。

要配置字幕效果并编辑字幕菜单本身，包括以下任一查看器的菜单文本：

* `Universal_HTML5_Video` 查看者
* `Universal_HTML5_MixedMedia_dark` 查看者
* `Universal_HTML5_MixedMedia_light` 查看者

参见 [添加或编辑视频查看器预设](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset).

另请参阅 [添加和编辑查看器预设](application-setup.md#adding_and_editing_viewer_presets).

Adobe Dynamic Media Classic可以将字幕文件转换为JSON（JavaScript对象表示法）格式。 这种转换意味着，您可以将 JSON 文本作为视频的隐藏但完整的文本嵌入到网页中。然后，搜索引擎可以对内容进行爬网和索引，以使视频更容易被发现，并为客户提供有关视频内容的更多详细信息。

参见 [提供静态（非图像）内容](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/c-serving-static-nonimage-contents.html?lang=en#image-serving-api) 在 *Adobe图像服务API帮助* 有关在URL中使用JSON函数的更多信息。

**在视频中添加题注:**

1. 使用Adobe Dynamic Media Classic之外的第三方应用程序，根据您使用的查看器类型创建视频字幕文件。

   | 查看器类型 | 题注文件 |
   |--- |--- |
   | HTML5 | 如果您使用 HTML5 视频查看器，请确保您创建的题注文件遵循 WebVTT（Web 视频文本跟踪）标准。题注文件的扩展名为 .vtt。您可以了解有关 WebVTT 题注标准的详细信息。<br><br>[请参阅WebVTT](https://w3c.github.io/webvtt/)：Web视频字幕格式。 <br><br>你可以使用免费和付费的工具和服务在Adobe Dynamic Media Classic之外创作字幕文件。 例如，要创建不带样式的简单视频字幕文件，您可以使用以下免费的在线字幕创作和编辑工具： <br><br>[WebVTT题注生成器](https://testdrive-archive.azurewebsites.net/Graphics/CaptionMaker/Default.html) <br><br>为了获得最佳结果，请在Internet Explorer 9或更高版本、Google Chrome或Safari中使用该工具。 <br><br>在工具中， <b>输入视频文件的URL</b> 字段，粘贴视频文件的URL，然后选择 <b>加载</b>. <br><br>例如，如果视频文件使用的是Adobe Dynamic Media Classic URL，请双击单个视频资源（不是自适应视频集或主视频）以在“详细信息视图”中将其打开。 在“详细信息视图”的右侧面板中，展开“URL 和嵌入代码”。然后在“移动设备”组下方的“移动设备”（渐进式）右侧，选择 <b>复制URL</b>. 此过程将为您提供视频文件本身的URL，然后您可以将该URL粘贴到 <b>输入视频文件的URL</b> 字段。 随后，Internet Explorer、Chrome 或 Safari 就可以在本机播放视频。现在，按照屏幕上的站点说明创作并保存您的 WebVTT 文件。完成后，复制字幕文件内容并将其粘贴到纯文本编辑器中，并以VTT文件扩展名保存。 <br><br><b>注意：</b> 为了在全球范围内支持英语以外的语言的视频字幕，WebVTT标准要求您为要支持的每种语言创建单独的.vtt文件并调用。 <br><br>通常，您需要以视频文件的名称来命名题注 VTT 文件，并在后面附加 captions。这有助于使用现有的 Web 内容管理系统自动生成视频 URL。 |

1. 在Adobe Dynamic Media Classic中，上传WebVTT、DFXP或SMPTE XML字幕文件。

   参见 [上传文件](uploading-files.md#uploading_files).

1. 在左侧的“资源库”面板中，导航至要与上载的题注文件相关联的视频文件所在的资源文件夹。
1. 在“资源浏览”面板中，选择单个视频资源，然后选择该资源的缩略图图像下方 **[!UICONTROL 预览]** > **[!UICONTROL 查看器列表]**.
1. 在“查看器列表”表格中，找到名为的HTML5查看器 **Univeral_HTML5_Video**， **Universal_Media5_MixedMedia_darkHTML**，或 **Universal_HTML5_MixedMedia_light**，然后执行以下操作之一：

   * 要获得弹出式视频查看器体验，请选择 **[!UICONTROL 复制URL]** 最右边的名字。

      使用以下语法附加复制的视频的URL，以便将其与复制的URL关联到字幕文件：

      `&caption=<full Copy URL path to the caption file .vtt>,1`

      请注意 `,1` 在题注URL路径末尾。 紧跟路径中的VTT文件扩展名之后，您可以选择通过将设置为，启用或禁用视频播放器栏上的隐藏式字幕按钮 `1` 或 `0`，则不会显示任何内容。

   * 要获得嵌入式视频查看器体验，请选择 **[!UICONTROL 嵌入代码]** 最右边的名字。

      在“嵌入代码”对话框中，选择 **[!UICONTROL 复制到剪贴板]**.

      对于HTML5 `Universal_HTML5_Video`， `Universal_HTML5_MixedMedia_dark`，或 `Universal_HTML5_MixedMedia_light` 查看器，将复制的嵌入代码附加到以下内容：

      `videoViewer.setParam("caption","<full Copy URL path to the caption file .vtt>,1”`

      请注意 `,1` URL路径末尾。 在URL路径中的VTT文件扩展名之后，您可以选择通过将设置为，启用或禁用视频播放器栏上的字幕按钮 `1` 或 `0`，则不会显示任何内容。
