---
title: '"快速入门：视频"'
seo-title: '"快速入门：视频"'
description: 'null'
seo-description: 介绍和快速入门视频以帮助您快速入门和运行。
uuid: bf0ecf87-a1 f2-4e83-8041-df5192 dd26 a1
contentOwner: admin
content-type: 引用
products: SG_ EXPERIENCE MANAGER/Dynamic-Media-Scene-7
geptopics: SG_ SCENESELEFERENDER_ PK/类别/视频
discoiquuid: 6cf541b-e9 df-48eb-9a16-ca3 e1 f07238 e
translation-type: tm+mt
source-git-commit: de7d2608f94935f238a11d8310b97dddc5476f57

---


# 快速入门：视频{#quick-start-video}

Adobe Dynamic Media经典视频是一款端到端解决方案，可让您轻松发布高质量自适应视频以跨多个屏幕(包括桌面、iOS、Android、Blackberry和Windows移动设备)流式播放。自适应视频集可将同一视频以不同比特率和格式（如 400 kbps、800 kbps 和 1000 kbps）编码的不同版本分组在一起。台式计算机或移动设备可检测可用带宽。

例如，在 iOS 移动设备上，可检测 3G、4G 或 Wi-Fi 等带宽。然后，从自适应视频集内的不同视频比特率中自动选择正确的编码视频。视频将流式传输到台式机、移动设备或平板电脑。

另外，如果台式机或移动设备上的网络条件发生变化，则会自动动态切换视频质量。此外，如果客户在桌面上进入全屏模式，自适应视频集会以更好的分辨率响应，从而改善客户的查看体验。使用自适应视频集可为在多个屏幕和设备上播放Dynamic Media经典视频的客户提供最佳回放。

视频播放器用于确定要播放或选择的编码视频的逻辑取决于以下算法：

1. 视频播放器基于比特率最接近播放器本身中的“初始比特率”设置的比特率加载初始视频片段。
1. 视频播放器使用以下标准根据带宽速度变化进行切换：

   1. 播放器捕获低于或等于估计带宽的最高带宽流。
   1. 播放器只考虑80%的可用带宽。但是，如果它正在向上切换，它将以仅70%的速率转换，以避免估计过高并且必须立即切换。

有关它的技术信息，请参阅 [https://android.googlesource.com/platform/frameworks/av/+/master/media/libstagefright/httplive/LiveSession.cpp](https://android.googlesource.com/platform/frameworks/av/+/master/media/libstagefright/httplive/LiveSession.cpp) 的算法逻辑。

要管理单一视频和自适应视频集，Dynamic Media经典支持以下各项：

* 上载很多支持的视频格式和音频格式的视频，并将视频编码为 MP4 H.264 格式以在多个屏幕中进行播放。您可以使用预定义的动态媒体经典自适应视频预设、单个视频编码预设或自定义自己的编码，以控制视频的质量和大小。

   生成自适应视频集时，它包括MP视频。

   `**Note:**` 主/源视频以及任何其他源格式视频 *不* 会添加到自适应视频集。

* Universal_ HTML5_ Video、Universal_ HTML5_ MixedMedia_ dark和Universal_ HTML5_ Video、Universal_ HTML5_ MixedMedia_ light查看器和视频章节导航中的视频字幕(Universal_ HTML5_ MixedMedia_ light和Universal_ HTML5_ MixedMedia_ light查看器)。

   请参阅[在视频中添加题注](adding-captions-video.md)。

   请参阅[在视频中添加章节标记](adding-chapter-markers-video.md)。

* 利用对元数据的全面支持来组织、浏览和搜索视频，从而高效地管理视频资源。
* 将自适应视频集传送到网站以及台式机和移动设备，包括 iPhone、iPad、Android™、Blackberry 和 Windows Phone。

   在各种不同的 iOS 平台上支持自适应视频流。

   请参阅“ [Adobe查看器参考指南](https://marketing.adobe.com/resources/help/en_US/s7/viewers_ref/)”中的最新支持。

   Dynamic Media Classic支持针对MP H.264视频的移动视频回放。您可以在以下网站中找到支持该视频格式的 Blackberry 设备：

   请参阅 [Blackberry上支持的视频格式](https://support.blackberry.com/kb/articleDetail?ArticleNumber=000005482)。

   您可以在以下网站找到支持该视频格式的 Windows 设备：

   请参阅 [Windows Phone上支持的视频格式](https://msdn.microsoft.com/en-us/library/ff462087(v=vs.92).aspx)。

* 使用Dynamic Media经典查看器预设播放视频，其中包括：

   * 单视频查看器。
   * 兼有视频和图像内容的混合媒体查看器。

* 配置视频播放器来满足您的品牌需求。
* 通过简单的 URL 或嵌入代码将视频集成到您的网站、移动站点或移动应用程序中。

**快速入门**

以下分步工作流程说明旨在帮助您在Dynamic Media经典中快速设置和运行自适应视频集。每个步骤的后面都有一个交叉引用，可以跳转到相应的主题标题，供您了解更多信息。

**1. 上载和编码视频**

可以使用以下两种方案之一上载并生成自适应视频集：

* **上传预编码视频** -如果您的视频已经在Dynamic Media经典外部进行编码，请单击 **全局导航栏** 上的“上传”以浏览MP视频文件并将其直接上传到Scene Publishing System。然后，单击“**构建**”&gt;“**自适应视频集**”。浏览至您的视频文件。将需要的视频文件拖放到“自适应视频集”表中，然后保存此视频集。
* **上传主源视频** -如果您的视频未编码，请单击 **全局导航栏** 上的“上传”以上传主视频源文件(非MP4)，并让Scene Publishing System将它们编码为MP文件。在“上载作业选项”对话框中，在“eVideo 选项”下面选择“**自适应视频**。

   通过使用此首选的选项，可以创建一个自适应视频集以自动将正确编码预设应用于视频（不论是 16:9 还是 4:3），以便与您上载的视频尺寸相匹配。提交上载作业时，系统会自动为您创建一个自适应视频集，其中包含三个具有正确高宽比的视频编码。

   或者，在相同的“作业选项”对话框中，在“eVideo 选项”下面展开“**单个编码预设**”，然后从“**台式机**”、“**移动设备（iPhone、iPad、Android）**”和“**平板电脑（iPad、Android）**”中选择所需的单个视频编码预设以创建 MP4 文件。

* 或者，您可以使用重新处理功能重新处理主视频。已将最新编码的视频添加到现有的自适应视频集。

请参阅[上载和编码视频](uploading-encoding-videos.md#uploading_and_encoding_videos)。

**可选**

动态媒体经典提供大量预定义的视频编码预设。这些预定义的预设反映了目前使用的最常见编码设置，并针对在目标屏幕上播放进行了优化。

不过，如果需要进一步自定义，管理员可以创建视频预设，以便为最终用户自定义视频大小和播放体验。管理员可以从“设置”&gt;“应用程序设置”&gt;“视频预设”&gt;“单个编码预设”下面的“视频预设”页中添加和管理视频预设。“视频预设”页提供用于添加、编辑、删除和激活视频预设的选项。

请参阅[使用视频编码预设](uploading-encoding-videos.md#working_with_video_encoding_presets)。

**2. 在视频查看器中预览视频**

要查看在台式机、网站或移动设备上为最终用户播放视频的方式，请在浏览面板中选择视频，然后单击“**预览**”。

请参阅[在视频查看器中预览视频](previewing-videos-video-viewer.md#previewing_videos_in_a_video_viewer)。

您可以在“预览”屏幕上播放视频。还可以选择不同的视频查看器，以了解视频在不同播放器中的播放效果。作为最佳做法，请使用 HTML5 视频播放器在台式机、平板电脑和移动设备上进行多屏幕播放。

**可选**

查看器预设自定义-动态媒体经典提供预定义的查看器预设，用于交付视频。这些预设决定了查看器的外观及其播放控件的工作方式。要自定义视频查看器，管理员可以从“视频预设”页中添加和管理视频预设。要打开该页，请在 Scene7 Publishing System 的右上角，单击“设置”&gt;“查看器预设”。“查看器预设”页提供用于添加、编辑、删除和激活查看器预设的命令。

请参阅[使用视频查看器预设](previewing-videos-video-viewer.md#working_with_video_viewer_presets)。

**3. 将视频部署到网站和移动站点**

要将视频集成到您的网站，您可以执行以下操作之一：

* 在自己的弹出或模式窗口中显示视频，此时，应使用复制 URL 功能。

   要获取视频的 URL，请在网格视图或列表视图的浏览面板中选择该视频。Click Preview, and then click Copy URL to the right of `Universal_HTML5_Viewer`.

   在单击“复制 URL”时，该 URL 将复制到剪贴板中。将此代码放置在网站、移动站点或应用程序的 HTML 中。

   ***注意**：URL仅在您发布视频或自适应视频集后才会激活。*

* 显示网页中嵌入的视频，此时，应使用嵌入代码功能。

   要获取视频的嵌入代码，请在网格视图或列表视图的浏览面板中选择该视频。单击“预览”&gt;“查看器列表”。在表的“操作”列下面，单击 `Universal_HTML5_Video` 右侧的“嵌入代码”。不允许编辑代码。

   单击“关闭”，然后将嵌入代码粘贴在网页中。

   ***注意**：嵌入代码只在发布视频或自适应视频集后激活。*

请参阅[将视频部署到网站和移动站点](deploying-video-websites-mobile-sites.md#deploying_video_to_your_websites_and_mobile_sites)。

>[!MORELIKETHIS]
>
>* [视频编码最佳做法](uploading-encoding-videos.md#best_practices_for_video_encoding)
