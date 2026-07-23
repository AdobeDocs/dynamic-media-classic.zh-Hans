---
title: 使用HTML5视频查看器的最佳实践
description: 了解使用HTML5视频查看器的最佳实践。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: ce49e4ce-8dc0-41e1-865a-249f23757553
topic: Content Management
level: Intermediate
autotag-review: '2026-05-13T17:39:23.475Z'
TQID: 'https://experienceleague.adobe.com/wGnoHGEOQLVV-rnoKBOE8wzphK3VaM-vr9YB1Y-gT8c'
product_v2: id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
source-git-commit: 5fdabd28c4d0defdf9f145b581c89640cc1f6118
workflow-type: tm+mt
source-wordcount: 482
ht-degree: 2%

---

# 使用HTML5视频查看器的最佳实践{#best-practice-using-the-html-video-viewer}

Adobe Dynamic Media Classic HTML5视频查看器预设是高性能视频播放器。 对于播放器设计，您可以使用标准Web开发工具创建视频播放器的整个功能。 要自定义外观，您可以使用HTML5和CSS设计按钮、控件以及自定义海报图像。

对于查看器播放，会自动检测浏览器的视频功能。 然后，它使用HLS（HTTP实时流）提供视频，也称为自适应视频流。 或者，如果不存在该投放方法，则改用HTML5 progressive。

通过将以下功能组合到单个播放器中：

* 使用HTML5和CSS设计的播放组件。
* 嵌入式播放。
* 根据浏览器的功能使用自适应流和渐进式流。

您可以提高富媒体内容对桌面和移动设备用户的可用性。 还可确保简化视频体验。

另请参阅HTML查看器参考指南中的[关于Adobe5查看器](https://experienceleague.adobe.com/en/docs/dynamic-media-developer-resources/library/viewers-for-aem-assets-only/c-html5-aem-asset-viewers#viewers-for-aem-assets-only)。

另请观看[查看器预设](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/550_viewer-presets_converted%20renamed_Done-AVS)培训视频。

## 使用Adobe Dynamic Media Classic Video Viewer在桌面计算机和移动设备上播放视频 {#playback-of-video-on-desktop-computers-and-mobile-devices-using-the-scene-video-viewer}

对于桌面和移动设备自适应视频流，用于比特率切换的视频基于自适应视频集中的所有MP4视频。

使用HLS或渐进式视频进行视频播放。 HLS （HTTP实时流）是用于自适应视频流的Apple标准，可根据网络带宽容量自动调整播放。 它还允许用户导航到视频中的任意点，而无需等待下载视频的其余部分。 另请参阅[HTTP实时流式传输](https://developer.apple.com/streaming/)。 该系统通过将渐进式视频下载并本地存储到用户的桌面屏幕或移动设备来发送渐进式视频。

下表介绍了使用Adobe Dynamic Media Classic Video Viewer在台式计算机和移动设备上播放视频的设备、浏览器和方法。

| 设备 | 浏览器 | 视频播放模式 |
|--- |--- |--- |
| 桌面 | Internet Explorer 9和10 | 渐进式下载。 |
| 桌面 | Internet Explorer 11+ | HLS视频流。 |
| 桌面 | Firefox 23-44 | 渐进式下载。 |
| 桌面 | Firefox 45或更高版本 | HLS视频流。 |
| 桌面 | Chrome | HLS视频流。 |
| 桌面 | Safari (Mac) | HLS视频流。 |
| 移动 | Chrome（Android™ 6或更早版本） | 渐进式下载。 |
| 移动 | Chrome （Android™ 7或更高版本） | HLS视频流。 |
| 移动 | ™（默认浏览器） | 渐进式下载。 |
| 移动 | Safari (iOS) | HLS视频流。 |
| 移动 | Chrome (iOS) | HLS视频流。 |
| 移动 | BlackBerry® | HLS视频流。 |
