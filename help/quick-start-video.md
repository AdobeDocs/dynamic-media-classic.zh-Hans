---
title: “快速入门：视频在Adobe Dynamic Media Classic中”
description: Adobe Dynamic Media Classic视频简介和快速入门，可帮助您快速启动并运行。
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: 1157400c-b33a-422e-848c-258660ddc748
source-git-commit: 352b1c383195fa03294ad3501207d63f3cfe3e42
workflow-type: tm+mt
source-wordcount: '1806'
ht-degree: 28%

---

# 快速入门：视频在Adobe Dynamic Media Classic{#quick-start-video}

Adobe Dynamic Media Classic Video是一种端到端解决方案，可轻松发布高质量自适应视频，以便在多个屏幕(包括台式机、iOS、Android™、BlackBerry®和Windows®移动设备)上进行流播放。 自适应视频集可将同一视频以不同比特率和格式（如 400 kbps、800 kbps 和 1000 kbps）编码的不同版本分组在一起。台式计算机或移动设备可检测可用带宽。

例如，在 iOS 移动设备上，可检测 3G、4G 或 Wi-Fi 等带宽。然后，从自适应视频集内的不同视频比特率中自动选择正确的编码视频。视频将流式传输到台式机、移动设备或平板电脑。

另外，如果台式机或移动设备上的网络条件发生变化，则会自动动态切换视频质量。此外，如果客户在桌面上进入全屏模式，自适应视频集将使用更好的分辨率做出响应，从而改善客户的观看体验。 对于在多个屏幕和设备上播放Adobe Dynamic Media Classic视频的客户，使用自适应视频集可为您提供最佳的播放方式。

视频播放器用于确定要播放或选择的编码视频的逻辑取决于以下算法：

1. 视频播放器根据与播放器本身中为“初始比特率”设置的值最接近的比特率来加载初始视频片段。
1. 视频播放器根据带宽速度的更改使用以下条件进行切换：

   1. 播放器会选取低于或等于估计带宽的最高带宽流。
   1. 播放器仅考虑可用带宽的80%。 但是，如果它正在切换，则更为保守，仅为70%，以避免过高估计，并且必须立即重新切换。

有关算法的技术信息，请参阅[https://android.googlesource.com/platform/frameworks/av/+/master/media/libstagefright/httplive/LiveSession.cpp](https://android.googlesource.com/platform/frameworks/av/+/master/media/libstagefright/httplive/LiveSession.cpp)上算法的逻辑。

要管理单个视频和自适应视频集，Adobe Dynamic Media Classic支持以下功能：

* 上载很多支持的视频格式和音频格式的视频，并将视频编码为 MP4 H.264 格式以在多个屏幕中进行播放。您可以使用预定义的Adobe Dynamic Media Classic自适应视频预设、单个视频编码预设，或自定义您自己的编码以控制视频的质量和大小。

请参阅[激活或停用自适应视频预设](/help/application-setup.md#activating-or-deactivating-adaptive-video-presets)

另请参阅[视频预设](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/549_video-presets_converted%20renamed_Done-AVS)培训视频。

生成自适应视频集时，它将包含MP4视频。

>[!NOTE]
>
>主控/源视频和任何其他源格式视频均&#x200B;*未*&#x200B;添加到自适应视频集。

* 在Univeral_HTML5_Video、Universal_HTML5_MixedMedia_dark和Universal_HTML5_MixedMedia_light查看器中设置视频字幕，并在Universal_HTML5_Video、Universal_HTML5_MixedMedia_dark和Universal_HTML5_MixedMedia_light查看器中设置视频章节导航。

   请参阅[向视频添加字幕](adding-captions-video.md)。

   请参阅[向视频](adding-chapter-markers-video.md)添加章节标记。

* 利用对元数据的全面支持来组织、浏览和搜索视频，从而高效地管理视频资源。
* 将自适应视频集交付到Web和桌面，以及移动设备，包括iPhone、iPad、Android™、BlackBerry®和Windows®手机。

   各种iOS平台均支持自适应视频流播放。

   请参阅[Adobe查看器参考指南](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources.html)中的最新支持。

   Adobe Dynamic Media Classic支持为MP4 H.264视频播放移动设备视频。 您可以在以下网站上找到支持此视频格式的BlackBerry®设备：

   请参阅[BlackBerry®](https://support.blackberry.com/kb/articleDetail?ArticleNumber=000005482)上支持的视频格式。

   您可以在以下位置找到支持此视频格式的Windows®设备：

   请参阅[Windows® Phone](https://docs.microsoft.com/en-us/)上支持的视频格式。

* 使用Adobe Dynamic Media Classic查看器预设播放视频，包括以下内容：

   * 单视频查看器。
   * 兼有视频和图像内容的混合媒体查看器。

* 配置视频播放器来满足您的品牌需求。
* 通过简单的 URL 或嵌入代码将视频集成到您的网站、移动站点或移动应用程序中。

请观看以下培训视频：
* [MP4视频概述](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/563_MP4%20Video%20Overview_converted%20renamed_eVideos-AVS)

* [MP4视频预览](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/564_MP4%20Video%20Preview_converted%20renamed_eVideos-AVS)

* [MP4视频上传](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/565_MP4%20Video%20Upload_converted%20renamed_eVideos-AVS)

* [流概述](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/567_Streaming%20Overview_master_eVideos_converted%20renamed_eVideos-AVS)

**快速入门**

以下工作流分步描述旨在帮助您在Adobe Dynamic Media Classic中快速设置并运行自适应视频集。 每个步骤的后面都有一个交叉引用，可以跳转到相应的主题标题，供您了解更多信息。

## 1.上传和编码视频

可以使用以下两种方案之一上载并生成自适应视频集：

* **上传预编码视频**  — 如果您的视频已在Adobe Dynamic Media Classic外部进行编码，请在全局导航栏中选择 **** Upload以浏览MP4视频文件，并将其直接上传到Adobe Dynamic Media Classic。然后，转到&#x200B;**[!UICONTROL Build]** > **[!UICONTROL 自适应视频集]**。 浏览至您的视频文件。将需要的视频文件拖放到“自适应视频集”表中，然后保存此视频集。
* **上传主控源视频**  — 如果您的视频未进行编码，请在全局导航栏中选择 **** 上传，以上传主控视频源文件（非MP4）。Adobe Dynamic Media Classic会为您将其编码为MP4文件。 在&#x200B;**[!UICONTROL 上传作业选项]**&#x200B;对话框的&#x200B;**[!UICONTROL EVideo选项]**&#x200B;下，选择&#x200B;**[!UICONTROL 自适应视频]**。

   通过使用此首选的选项，可以创建一个自适应视频集以自动将正确编码预设应用于视频（不论是 16:9 还是 4:3），以便与您上载的视频尺寸相匹配。在您提交上传作业时，系统会自动为您创建自适应视频集，该视频集包含三个以正确宽高比进行编码的视频设置。

   或者，在同一&#x200B;**[!UICONTROL 作业选项]**&#x200B;对话框的&#x200B;**[!UICONTROL EVideo选项]**&#x200B;下，展开&#x200B;**[!UICONTROL 单个编码预设]**。从&#x200B;**Desktop**、**Mobile(iPhone、iPad、Android™)**&#x200B;和&#x200B;**Tablet(iPad、Android™)**&#x200B;中选择您需要的单个视频编码预设，以便创建MP4文件。

* 或者，您也可以使用&#x200B;**[!UICONTROL Reprocess]**&#x200B;功能重新处理主控视频。 已将最新编码的视频添加到现有的自适应视频集。

请参阅[上传和编码视频](uploading-encoding-videos.md#uploading_and_encoding_videos)。

**可选**

Adobe Dynamic Media Classic提供了大量预定义的视频编码预设。 这些预定义的预设反映了当前使用的最常见视频编码设置，并针对在目标页面上播放进行了优化。

不过，如果需要进一步自定义，管理员可以创建视频预设，以便为最终用户自定义视频大小和播放体验。管理员可以从位于&#x200B;**[!UICONTROL 设置]** > **[!UICONTROL 应用程序设置]** > **[!UICONTROL 视频预设]** > **[!UICONTROL 单个编码预设]**&#x200B;下的“视频预设”页面添加和管理视频预设。 “视频预设”页提供用于添加、编辑、删除和激活视频预设的选项。

请参阅[使用视频编码预设](uploading-encoding-videos.md#working_with_video_encoding_presets)。

## 2.在视频查看器中预览视频

要查看视频在桌面、您的网站或移动设备上对最终用户的播放方式，请在浏览面板中选择视频，然后选择&#x200B;**[!UICONTROL 预览]**。

请参阅[在视频查看器中预览视频](previewing-videos-video-viewer.md#previewing_videos_in_a_video_viewer)。

您可以在预览页面上播放视频。 您还可以选择不同的视频查看器，以了解您的视频在不同播放器中的显示方式。 作为最佳做法，请使用 HTML5 视频播放器在台式机、平板电脑和移动设备上进行多屏幕播放。

**可选**

查看器预设自定义 — Adobe Dynamic Media Classic提供了预定义的查看器预设来传送视频。 这些预设决定了查看器的外观及其播放控件的工作方式。要自定义视频查看器，管理员可以从“视频预设”页中添加和管理视频预设。要打开此页面，请在Adobe Dynamic Media Classic的右上角，转到&#x200B;**[!UICONTROL Setup]** > **[!UICONTROL Viewer Presets]**。 “查看器预设”页提供用于添加、编辑、删除和激活查看器预设的命令。

请参阅[使用视频查看器预设](previewing-videos-video-viewer.md#working_with_video_viewer_presets)。

另请参阅[视频预设](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/549_video-presets_converted%20renamed_Done-AVS)培训视频。

## 3.将视频部署到您的网站和移动网站

要将视频集成到您的网站，您可以执行以下操作之一：

* 在其自身的弹出窗口或模式窗口中显示视频，在这种情况下，使用&#x200B;**[!UICONTROL 复制URL]**&#x200B;功能。

   要获取视频的 URL，请在网格视图或列表视图的浏览面板中选择该视频。选择&#x200B;**[!UICONTROL 预览]**，然后选择`Universal_HTML5_Viewer`右侧的&#x200B;**[!UICONTROL 复制URL]**。

   选择&#x200B;**[!UICONTROL 复制URL]**&#x200B;后，该URL将会复制到剪贴板。 将此代码放置在网站、移动站点或应用程序的 HTML 中。

   >[!NOTE]
   >
   >只有在发布视频或自适应视频集后，才会激活 URL。

* 显示嵌入到网页上的视频，在这种情况下，使用&#x200B;**[!UICONTROL 嵌入代码]**&#x200B;功能。

   要获取视频的嵌入代码，请在网格视图或列表视图的浏览面板中选择该视频。转到&#x200B;**[!UICONTROL 预览]** > **[!UICONTROL 查看器列表]**。 在表的“操作”列下，选择`Universal_HTML5_Video`右侧的&#x200B;**[!UICONTROL 嵌入代码]**。 不允许编辑代码。

   选择&#x200B;**[!UICONTROL 关闭]**&#x200B;并将嵌入代码粘贴到您的网页中。

   >[!NOTE]
   >
   >只有在发布视频或自适应视频集后，才会激活嵌入代码。

请参阅[将视频部署到您的网站和移动站点](deploying-video-websites-mobile-sites.md#deploying_video_to_your_websites_and_mobile_sites)。

>[!MORELIKETHIS]
>
>* [视频编码最佳做法](uploading-encoding-videos.md#best_practices_for_video_encoding)

