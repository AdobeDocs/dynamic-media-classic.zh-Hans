---
title: 使用HTML5视频查看器的最佳实践
description: 了解使用HTML5视频查看器的最佳实践。
uuid: 3c8924dc-7bea-4c25-b77b-005f57b71b64
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
discoiquuid: 4b11cab7-88cf-42dd-8554-2eea530753bb
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: ce49e4ce-8dc0-41e1-865a-249f23757553
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 13%

---

# 使用HTML5视频查看器的最佳实践{#best-practice-using-the-html-video-viewer}

AdobeDynamic Media Classic HTML5视频查看器预设是强大的视频播放器。 在播放器的设计方面，您可以使用标准Web开发工具创建视频播放器的整个功能。 例如，您可以使用 HTML5 和 CSS 设计按钮、控件和自定义海报图像背景，以便通过自定义的界面外观吸引客户。

在查看器的播放端，它将自动检测浏览器的视频功能。然后，它使用HLS（HTTP实时流）（也称为自适应视频流）来提供视频。 或者，如果不存在该提交方法，则改用HTML5渐进式。

通过将以下功能组合到单个播放器中：

* 使用HTML5和CSS设计的播放组件
* 嵌入式播放
* 基于浏览器功能的自适应和渐进式流的使用

您可以将富媒体内容的范围扩展到桌面和移动设备用户。 您还可以确保简化的视频体验。

另请参阅《Adobe查看器参考指南》中的[关于HTML5查看器](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/library/viewers-for-aem-assets-only/c-html5-aem-asset-viewers.html?lang=en#viewers-for-aem-assets-only)。

## 使用AdobeDynamic Media Classic视频查看器在台式计算机和移动设备上播放视频 {#playback-of-video-on-desktop-computers-and-mobile-devices-using-the-scene-video-viewer}

对于桌面和移动设备自适应视频流播放，用于比特率切换的视频基于自适应视频集中的所有MP4视频。

使用HLS或渐进式视频时，会发生视频播放。 HLS（HTTP实时流播放）是Apple的自适应视频流播放标准，可根据网络带宽容量自动调整播放。 它还允许客户“搜寻”视频中的任意点，而无需等待视频的其余部分下载。 另请参阅[HTTP实时流](https://developer.apple.com/streaming/)。 通过将视频下载到本地并将其存储到用户的桌面屏幕或移动设备，来传送渐进式视频。

下表介绍了使用Dynamic Media Classic视频查看器在台式计算机和移动设备上播放视频的设备、浏览器和Adobe方法。

| 设备 | 浏览器 | 视频播放模式 |
|--- |--- |--- |
| 桌面 | Internet Explorer 9和10 | 渐进式下载。 |
| 桌面 | Internet Explorer 11+ | HLS视频流。 |
| 桌面 | Firefox 23-44 | 渐进式下载。 |
| 桌面 | Firefox 45 或更高版本 | HLS视频流。 |
| 桌面 | 铬黄 | HLS视频流。 |
| 桌面 | Safari(Mac) | HLS视频流。 |
| 移动 | Chrome(Android™ 6或更早版本) | 渐进式下载。 |
| 移动 | Chrome(Android™ 7或更高版本) | HLS视频流。 |
| 移动 | Android™（默认浏览器） | 渐进式下载。 |
| 移动 | Safari(iOS) | HLS视频流。 |
| 移动 | Chrome(iOS) | HLS视频流。 |
| 移动 | BlackBerry® | HLS视频流。 |
