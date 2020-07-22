---
title: '"最佳做法：使用 HTML5 视频查看器"'
seo-title: '"最佳做法：使用 HTML5 视频查看器"'
description: 'null'
seo-description: 了解使用HTML5视频查看器的最佳实践。
uuid: 3c8924dc-7bea-4c25-b77b-005f57b71b64
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
discoiquuid: 4b11cab7-88cf-42dd-8554-2eea530753bb
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 30%

---


# 最佳做法：使用 HTML5 视频查看器{#best-practice-using-the-html-video-viewer}

Dynamic Media经典HTML5视频查看器预设是功能强大的视频播放器。 在播放器的设计方面，您可以使用标准Web开发工具创建视频播放器的所有功能。 例如，您可以使用 HTML5 和 CSS 设计按钮、控件和自定义海报图像背景，以便通过自定义的界面外观吸引客户。

在查看器的播放端，它将自动检测浏览器的视频功能。然后，它使用HLS（自适应视频流）提供视频。 或者，如果该投放方法不存在，则改用HTML5渐进式。

将使用 HTML5 和 CSS 设计播放组件的功能合并到一个单独播放器中实现了嵌入播放，并可根据浏览器功能选择使用自适应流和渐进式流，从而将富媒体内容的范围扩展到台式机用户和移动用户并确保视频体验一体化。

另请参 [阅《Adobe查看器参考指南](https://docs.adobe.com/content/help/en/dynamic-media-developer-resources/library/viewers-for-aem-assets-only/c-html5-aem-asset-viewers.html) 》中的“关于HTML5查看器”。

## 使用Dynamic Media经典视频查看器在桌面计算机和移动设备上播放视频 {#playback-of-video-on-desktop-computers-and-mobile-devices-using-the-scene-video-viewer}

对于桌面和移动自适应视频流播放，比特率切换所使用的视频基于自适应视频集中的所有MP4视频。

使用HLS或渐进式视频进行视频回放。 HLS（HTTP实时流）是自适应视频流播放的Apple标准，可根据网络带宽容量自动调整播放。 它还允许客户“搜索”视频中的任何点，而无需等待视频的其余部分下载。 另请参 [阅HTTP实时流](https://developer.apple.com/streaming/)。 渐进式视频通过下载视频并将其本地存储到用户的桌面屏幕或移动设备来交付。

下表介绍了使用Dynamic Media经典视频查看器在桌面计算机和移动设备上播放视频的设备、浏览器和方法。

| 设备 | 浏览器 | 视频播放模式 |
|--- |--- |--- |
| 德斯科普 | Internet Explorer 9和10 | 渐进式下载。 |
| 桌面 | Internet Explorer 11+ | HLS视频流。 |
| 桌面 | Firefox 23-44 | 渐进式下载。 |
| 桌面 | Firefox 45 或更高版本 | HLS视频流。 |
| 桌面 | 铬黄 | HLS视频流。 |
| 桌面 | Safari(Mac) | HLS视频流。 |
| 移动 | Chrome（Android 6或更早版本） | 渐进式下载。 |
| 移动 | Chrome（Android 7或更高版本） | HLS视频流。 |
| 移动 | Android（默认浏览器） | 渐进式下载。 |
| 移动 | Safari(iOS) | HLS视频流。 |
| 移动 | Chrome(iOS) | HLS视频流。 |
| 移动 | Blackberry | HLS视频流。 |
