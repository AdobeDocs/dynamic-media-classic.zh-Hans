---
title: 使用HTML5視訊檢視器的最佳實務
description: 瞭解使用HTML5視訊檢視器的最佳實務。
uuid: 3c8924dc-7bea-4c25-b77b-005f57b71b64
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
discoiquuid: 4b11cab7-88cf-42dd-8554-2eea530753bb
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: ce49e4ce-8dc0-41e1-865a-249f23757553
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '488'
ht-degree: 12%

---

# 使用HTML5視訊檢視器的最佳作法{#best-practice-using-the-html-video-viewer}

Adobe Dynamic Media Classic HTML5視訊檢視器預設集是強大的視訊播放器。 在播放器的設計方面，您可以使用標準Web開發工具來建立視訊播放器的完整功能。 例如，您可以使用 HTML5 和 CSS 设计按钮、控件和自定义海报图像背景，以便通过自定义的界面外观吸引客户。

在查看器的播放端，它将自动检测浏览器的视频功能。然後它會使用HLS （HTTP即時資料流），也稱為自我調整視訊資料流，提供視訊。 或者，如果該傳遞方法不存在，則改用HTML5 progressive。

將下列功能結合為單一播放器：

* 使用HTML5和CSS設計的播放元件
* 內嵌式播放
* 根據瀏覽器的功能使用最適化和漸進式串流

您可以將多媒體內容延伸至桌上型電腦和行動使用者。 您也可以確保簡化的視訊體驗。

另請參閱 [關於HTML5檢視器](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/library/viewers-for-aem-assets-only/c-html5-aem-asset-viewers.html?lang=en#viewers-for-aem-assets-only) 在Adobe檢視器參考指南中。

另請參閱 [檢視器預設集](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/550_viewer-presets_converted%20renamed_Done-AVS) 訓練影片。

## 使用Adobe Dynamic Media Classic視訊檢視器在桌上型電腦和行動裝置上播放視訊 {#playback-of-video-on-desktop-computers-and-mobile-devices-using-the-scene-video-viewer}

就桌上型電腦和行動最適化視訊串流而言，用於位元速率切換的視訊均以最適化視訊集中的所有MP4視訊為基礎。

使用HLS或漸進式視訊進行視訊播放。 HLS （HTTP即時資料流）是適用於最適化視訊資料流的Apple標準，可依據網路頻寬容量自動調整播放。 它也可讓客戶「搜尋」視訊中的任何位置，而不需要等候視訊的其餘部分下載。 另請參閱 [HTTP即時資料流](https://developer.apple.com/streaming/). 漸進式視訊是透過將視訊下載並儲存在使用者的案頭熒幕或行動裝置而提供。

下表說明使用Adobe Dynamic Media Classic Video Viewer在桌上型電腦和行動裝置上播放視訊的裝置、瀏覽器和方法。

| 设备 | 浏览器 | 視訊播放模式 |
|--- |--- |--- |
| 桌面 | Internet Explorer 9和10 | 漸進式下載。 |
| 桌面 | Internet Explorer 11+ | HLS視訊串流。 |
| 桌面 | Firefox 23-44 | 漸進式下載。 |
| 桌面 | Firefox 45 或更高版本 | HLS視訊串流。 |
| 桌面 | 鉻黃 | HLS視訊串流。 |
| 桌面 | Safari (Mac) | HLS視訊串流。 |
| 移动 | Chrome (Android™ 6或更舊版本) | 漸進式下載。 |
| 移动 | Chrome (Android™ 7或更新版本) | HLS視訊串流。 |
| 移动 | Android™ （預設瀏覽器） | 漸進式下載。 |
| 移动 | Safari (iOS) | HLS視訊串流。 |
| 移动 | Chrome (iOS) | HLS視訊串流。 |
| 移动 | BlackBerry® | HLS視訊串流。 |
