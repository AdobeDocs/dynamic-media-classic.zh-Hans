---
title: 快速入门： Adobe Dynamic Media Classic中的视频
description: Adobe Dynamic Media Classic简介和快速入门视频可帮助您快速启动和运行。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: 1157400c-b33a-422e-848c-258660ddc748
topic: Content Management
level: Beginner
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '1441'
ht-degree: 24%

---

# 快速入门： Adobe Dynamic Media Classic中的视频{#quick-start-video}

Adobe Dynamic Media Classic Video是一款端到端解决方案，可让您轻松发布高质量自适应视频，以便跨多个屏幕(包括台式机、iOS、Android™、BlackBerry®和Windows®移动设备)进行流式传输。 自适应视频集可将同一视频以不同比特率和格式（如 400 kbps、800 kbps 和 1000 kbps）编码的不同版本分组在一起。台式计算机或移动设备可检测可用带宽。

例如，在 iOS 移动设备上，可检测 3G、4G 或 Wi-Fi 等带宽。然后，从自适应视频集内的不同视频比特率中自动选择正确的编码视频。视频将流式传输到台式机、移动设备或平板电脑。

另外，如果台式机或移动设备上的网络条件发生变化，则会自动动态切换视频质量。此外，如果客户在桌面上进入全屏模式，则自适应视频集将使用更好的分辨率进行响应，从而改善客户的观看体验。 使用自适应视频集可以尽可能提供最佳播放。 它最适合在多个屏幕和设备上播放Adobe Dynamic Media Classic视频的客户。

视频播放器用于确定要播放或选择的编码视频的逻辑取决于以下算法：

1. 视频播放器根据比特率加载初始视频片段，该比特率最接近在播放器本身中为“初始比特率”设置的值。
1. 视频播放器根据使用下列条件对带宽速度所做的更改进行切换：

   1. 播放器选择低于或等于估计带宽的最高带宽流。
   1. 播放器仅考虑可用带宽的80%。 然而，如果它正在切换，则更保守的是70%，以避免高估，并立即切换回来。

有关算法的技术信息，请参阅[https://android.googlesource.com/platform/frameworks/av/+/master/media/libstagefright/httplive/LiveSession.cpp](https://android.googlesource.com/platform/frameworks/av/+/master/media/libstagefright/httplive/LiveSession.cpp)上的算法逻辑。

对于管理单个视频和自适应视频集，Adobe Dynamic Media Classic支持以下内容：

* 上传多种受支持视频格式的视频。 并且，将音频格式和视频编码上传到MP4 H.264格式，以便跨多个屏幕播放。 您可以使用预定义的Adobe Dynamic Media Classic自适应视频预设、单个视频编码预设，或自定义自己的编码来控制视频的质量和大小。

请参阅[激活或停用自适应视频预设](/help/using/application-setup.md#activating-or-deactivating-adaptive-video-presets)

另请参阅[视频预设](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/549_video-presets_converted%20renamed_Done-AVS)培训视频。

生成自适应视频集时，该视频集包含MP4视频。

>[!NOTE]
>
>主/源视频和任何其他源格式视频&#x200B;*不是*&#x200B;添加到自适应视频集。

* Univeral_HTML5_Video、Universal_HTML5_MixedMedia_dark和Universal_HTML5_MixedMedia_light查看器中的视频字幕以及Universal_HTML5_Video、Universal_HTML5_MixedMedia_dark和Universal_HTML5_MixedMedia_light查看器中的视频章节导航。

  请参阅[向视频添加字幕](adding-captions-video.md)。

  请参阅[向视频添加章节标记](adding-chapter-markers-video.md)。

* 利用对元数据的全面支持来组织、浏览和搜索视频，从而高效地管理视频资源。
* 将自适应视频集交付到Web以及桌面和移动设备，包括iPhone、iPad、Android™、BlackBerry®和Windows® phone。

  各种iOS平台支持自适应视频流。

  请参阅[Adobe查看器参考指南](https://experienceleague.adobe.com/en/docs/dynamic-media-developer-resources)中的最新支持。

  Adobe Dynamic Media Classic支持MP4 H.264视频的移动视频播放。<!-- LINK IS 404; NO SUITABLE REPLACEMENT WAS FOUND You can find BlackBerry&reg; devices that support this video format at the following website: -->

  <!-- See [Supported video formats on BlackBerry&reg;](https://support.blackberry.com/kb/articleDetail?ArticleNumber=000005482). -->

  您可以在以下位置找到支持此视频格式的Windows®设备：

  [Windows® Phone上支持的视频格式](https://learn.microsoft.com/en-us/windows/uwp/audio-video-camera/supported-codecs)。

* 使用Adobe Dynamic Media Classic查看器预设播放视频，包括以下内容：

   * 单个视频查看器。
   * 兼有视频和图像内容的混合媒体查看器。

* 配置视频播放器来满足您的品牌需求。
* 将视频与简单URL或嵌入代码集成到您的网站、移动网站或移动应用程序。

请观看以下培训视频：
* [MP4视频概述](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/563_MP4%20Video%20Overview_converted%20renamed_eVideos-AVS)

* [MP4视频预览](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/564_MP4%20Video%20Preview_converted%20renamed_eVideos-AVS)

* [MP4视频上传](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/565_MP4%20Video%20Upload_converted%20renamed_eVideos-AVS)

* [流概述](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/567_Streaming%20Overview_master_eVideos_converted%20renamed_eVideos-AVS)

**快速入门**

以下分步工作流描述旨在帮助您在Adobe Dynamic Media Classic中快速启动和运行自适应视频集。 每一步之后，都会交叉引用主题标题，您可以在其中查找更多信息。

## 1.上传视频并进行编码

可以使用以下两种方案之一上载并生成自适应视频集：

* **上载预先编码的视频**：如果您的视频已在Adobe Dynamic Media Classic外部编码，请在全局导航栏上选择&#x200B;**[!UICONTROL 上载]**。 浏览MP4视频文件并将其直接上传到Adobe Dynamic Media Classic。 然后，转到&#x200B;**[!UICONTROL 生成]** > **[!UICONTROL 自适应视频集]**。 浏览至您的视频文件。将所需的视频文件拖放到“自适应视频集”表中，然后保存该集。
* **上载主源视频**：如果视频未编码，请在全局导航栏上选择&#x200B;**[!UICONTROL 上载]**&#x200B;上载主视频源文件（非MP4）。 Adobe Dynamic Media Classic会为您将它们编码为MP4文件。 在&#x200B;**[!UICONTROL 上载作业选项]**&#x200B;对话框的&#x200B;**[!UICONTROL EVideo选项]**&#x200B;下，选择&#x200B;**[!UICONTROL 自适应视频]**。

  通过此首选选项，您可以创建自适应视频集。 正确的编码预设将自动应用于视频，无论是16:9还是4:3，以匹配您上传的视频尺寸。 在提交上载作业时，将自动为您创建自适应视频集，该视频集包含三个具有正确长宽比的编码视频设置。

  或者，在同一&#x200B;**[!UICONTROL 作业选项]**&#x200B;对话框中，在&#x200B;**[!UICONTROL EVideo选项]**&#x200B;下，展开&#x200B;**[!UICONTROL 单个编码预设]**。 选择所需的各个视频编码预设。 您可以选择&#x200B;**桌面**、**移动设备(iPhone、iPad、Android™)**&#x200B;和&#x200B;**平板电脑(iPad、Android™)**&#x200B;来创建MP4文件。

* 或者，您可以使用&#x200B;**[!UICONTROL 重新处理]**&#x200B;功能重新处理主视频。 已将最新编码的视频添加到现有的自适应视频集。

查看[上传视频并为其编码](uploading-encoding-videos.md#uploading_and_encoding_videos)。

**可选**

Adobe Dynamic Media Classic提供了大量预定义的视频编码预设。 这些预定义预设反映了当前使用的最常见视频编码设置，并且针对目标页面上的播放进行了优化。

不过，如果需要进一步自定义，管理员可以创建视频预设，以便为最终用户自定义视频大小和播放体验。管理员可以从&#x200B;**[!UICONTROL 设置]** > **[!UICONTROL 应用程序设置]** > **[!UICONTROL 视频预设]** > **[!UICONTROL 单个编码预设]**&#x200B;下的视频预设页面添加和管理视频预设。 “视频预设”页提供用于添加、编辑、删除和激活视频预设的选项。

请参阅[使用视频编码预设](uploading-encoding-videos.md#working_with_video_encoding_presets)。

## 2.在视频查看器中预览视频

要查看视频如何在桌面、网站或移动设备上为最终用户播放，请在“浏览”面板中选择该视频。 然后选择&#x200B;**[!UICONTROL 预览]**。

请参阅[在视频查看器中预览视频](previewing-videos-video-viewer.md#previewing_videos_in_a_video_viewer)。

您可以在“预览”页面上播放视频。 您还可以选择不同的视频查看器，以了解您的视频在不同播放器中的显示方式。 作为最佳做法，请使用 HTML5 视频播放器在台式机、平板电脑和移动设备上进行多屏幕播放。

**可选**

查看器预设自定义： Adobe Dynamic Media Classic提供了用于交付视频的预定义查看器预设。 这些预设决定了查看器的外观及其播放控件的工作方式。要自定义视频查看器，管理员可以从“视频预设”页中添加和管理视频预设。若要打开此页面，请在Adobe Dynamic Media Classic的右上角，转到&#x200B;**[!UICONTROL 设置]** > **[!UICONTROL 查看器预设]**。 “查看器预设”页提供用于添加、编辑、删除和激活查看器预设的命令。

请参阅[使用视频查看器预设](previewing-videos-video-viewer.md#working_with_video_viewer_presets)。

另请参阅[视频预设](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/549_video-presets_converted%20renamed_Done-AVS)培训视频。

## 3.将视频部署到您的网站和移动站点

要将视频集成到您的网站，您可以执行以下操作之一：

* 在其自己的弹出窗口或模式窗口中显示视频，在此情况下，请使用&#x200B;**[!UICONTROL 复制URL]**&#x200B;功能。

  要获取视频的URL，请在网格视图或列表视图中，在浏览面板中选择它。 选择&#x200B;**[!UICONTROL 预览]**，然后选择&#x200B;**[!UICONTROL 右侧的]**&#x200B;复制URL`Universal_HTML5_Viewer`。

  当您选择&#x200B;**[!UICONTROL 复制URL]**&#x200B;时，该URL将被复制到剪贴板。 将此代码放置在网站、移动站点或应用程序的 HTML 中。

  >[!NOTE]
  >
  >只有在发布视频或自适应视频集后，才会激活 URL。

* 显示嵌入到网页上的视频，在此情况下，使用&#x200B;**[!UICONTROL 嵌入代码]**&#x200B;功能。

  要获取视频的嵌入代码，请在网格视图或列表视图中，在浏览面板中选择视频。 转到&#x200B;**[!UICONTROL 预览]** > **[!UICONTROL 查看器列表]**。 在表的“操作”列下，选择&#x200B;**[!UICONTROL 右侧的]**&#x200B;嵌入代码`Universal_HTML5_Video`。 不允许编辑代码。

  选择&#x200B;**[!UICONTROL 关闭]**&#x200B;并将嵌入代码粘贴到一个或多个网页中。

  >[!NOTE]
  >
  >只有在发布视频或自适应视频集后，才会激活嵌入代码。

查看[将视频部署到您的网站和移动站点](deploying-video-websites-mobile-sites.md#deploying_video_to_your_websites_and_mobile_sites)。

>[!MORELIKETHIS]
>
>* [视频编码最佳做法](uploading-encoding-videos.md#best_practices_for_video_encoding)
