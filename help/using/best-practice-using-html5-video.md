---
title: 使用HTML5视频查看器的最佳实践
description: 了解使用HTML5视频查看器的最佳实践。
uuid: 3c8924dc-7bea-4c25-b77b-005f57b71b64
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
discoiquuid: 4b11cab7-88cf-42dd-8554-2eea530753bb
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: ce49e4ce-8dc0-41e1-865a-249f23757553
topic: Content Management
level: Intermediate
source-git-commit: d82f816553f807b514f4690827dab672a6baf690
workflow-type: tm+mt
source-wordcount: '488'
ht-degree: 12%

---

# 使用HTML5视频查看器的最佳实践{#best-practice-using-the-html-video-viewer}

Adobe Dynamic Media Classic HTML5视频查看器预设是可靠的视频播放器。 在播放器的设计方面，您可以使用标准Web开发工具创建视频播放器的全部功能。 例如，您可以使用 HTML5 和 CSS 设计按钮、控件和自定义海报图像背景，以便通过自定义的界面外观吸引客户。

在查看器的播放端，它将自动检测浏览器的视频功能。然后，它使用HLS（HTTP实时流）提供视频，也称为自适应视频流。 或者，如果该传送方法不存在，则改用HTML5 progressive。

通过将以下功能组合到单个播放器中：

* 使用HTML5和CSS设计的播放组件
* 嵌入式播放
* 根据浏览器的功能使用自适应和渐进式流

您可以将富媒体内容的范围扩展到桌面和移动设备用户。 您还可以确保简化的视频体验。

另请参阅 [关于HTML5查看器](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/library/viewers-for-aem-assets-only/c-html5-aem-asset-viewers.html?lang=en#viewers-for-aem-assets-only) 在Adobe查看器参考指南中。

另请参阅 [查看器预设](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/550_viewer-presets_converted%20renamed_Done-AVS) 训练视频。

## 使用Adobe Dynamic Media Classic Video Viewer在桌面计算机和移动设备上播放视频 {#playback-of-video-on-desktop-computers-and-mobile-devices-using-the-scene-video-viewer}

对于桌面和移动设备自适应视频流，用于比特率切换的视频基于自适应视频集中的所有MP4视频。

使用HLS或渐进式视频进行视频播放。 HLS（HTTP实时流）是用于自适应视频流的Apple标准，可根据网络带宽容量自动调整播放。 它还允许客户在视频中的任何位置“搜寻”，而无需等待视频的其余部分下载。 另请参阅 [HTTP实时流](https://developer.apple.com/streaming/). 渐进式视频是通过将视频下载并本地存储到用户的桌面屏幕或移动设备来交付的。

下表介绍了使用Adobe Dynamic Media Classic Video Viewer在桌面计算机和移动设备上播放视频的设备、浏览器和方法。

| 设备 | 浏览器 | 视频播放模式 |
|--- |--- |--- |
| 桌面 | Internet Explorer 9和10 | 渐进式下载。 |
| 桌面 | Internet Explorer 11+ | HLS视频流。 |
| 桌面 | Firefox 23-44 | 渐进式下载。 |
| 桌面 | Firefox 45 或更高版本 | HLS视频流。 |
| 桌面 | 铬黄 | HLS视频流。 |
| 桌面 | Safari (Mac) | HLS视频流。 |
| 移动 | Chrome (Android™ 6或更低版本) | 渐进式下载。 |
| 移动 | Chrome (Android™ 7或更高版本) | HLS视频流。 |
| 移动 | Android™（默认浏览器） | 渐进式下载。 |
| 移动 | Safari (iOS) | HLS视频流。 |
| 移动 | Chrome (iOS) | HLS视频流。 |
| 移动 | BlackBerry® | HLS视频流。 |
