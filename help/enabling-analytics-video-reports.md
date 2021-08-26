---
title: 启用Adobe Analytics视频报表
description: 了解如何在Adobe Analytics Classic中启用Dynamic Media视频报表。
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 9d017742-1ed2-411d-a8a6-438102bf1557
source-git-commit: 20a5e54a9f3fa442d3a993afae07aa5b1b13e9c3
workflow-type: tm+mt
source-wordcount: '245'
ht-degree: 13%

---

# 启用Adobe Analytics视频报表{#enabling-adobe-analytics-video-reports}

在Dynamic Media Classic中配置Adobe Analytics时，使用基于Adobe Analytics心率的视频报告功能，您不必再启用四个视频查看器事件（播放、暂停、停止、里程碑）。 视频心率适用于开箱即用的Dynamic Media Classic HTML5视频和混合媒体查看器。 视频播放器生成跟踪数据以在 Adobe Analytics 视频报告中查看。

* 有关流媒体和“心率测量”的简介，请参阅[关于适用于流媒体的Adobe Analytics](https://experienceleague.adobe.com/docs/media-analytics/using/media-overview.html#about-adobe-analytics-for-streaming-media)。

* 将Adobe Analytics视频报表与Dynamic Media Classic集成可支持解决方案变量，但不支持自定义变量。

   请参阅[音频和视频参数](https://experienceleague.adobe.com/docs/media-analytics/using/metrics-and-metadata/audio-video-parameters.html#metrics-and-metadata) ，以了解有关解决方案变量和自定义变量的更多信息。

* 支持以1分钟为增量的现成区段。 不过，不支持自定义区段报告，例如，客户根据时间增量定义的里程碑（百分比里程碑）或偏移里程碑。

   有关流媒体要求和设置的更多信息，请参阅[在Adobe Analytics中测量流媒体](https://experienceleague.adobe.com/docs/media-analytics/using/media-overview.html)。

* 有关自定义变量和解决方案变量的信息，请参阅[媒体报表启用](https://experienceleague.adobe.com/docs/media-analytics/using/media-reports/media-reports-enable.html?lang=en#media-reports)。

>[!NOTE]
>
>如果您的Adobe Analytics授权解决方案不包含视频心率，则必须继续使用本章中描述的步骤，将Adobe Analytics变量分配给Dynamic Media Classic查看器事件和变量。
