---
title: 启用Adobe Analytics视频报表
description: 了解如何在Adobe Dynamic Media Classic中启用Adobe Analytics视频报告。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 9d017742-1ed2-411d-a8a6-438102bf1557
source-git-commit: 358284e6c9888e5188bec35eb7b5408563a71bad
workflow-type: tm+mt
source-wordcount: '250'
ht-degree: 12%

---

# 启用Adobe Analytics视频报表{#enabling-adobe-analytics-video-reports}

使用基于Adobe Analytics心率的视频报告，在Adobe Dynamic Media Classic中配置Adobe Analytics时，您不再必须启用四个视频查看器事件（播放、暂停、停止、里程碑）。 视频心率适用于开箱即用的Adobe Dynamic Media Classic HTML5视频和混合媒体查看器。 视频播放器生成跟踪数据以在 Adobe Analytics 视频报告中查看。

* 有关流媒体和“心率测量”的简介，请参阅 [关于适用于流媒体的 Adobe Analytics](https://experienceleague.adobe.com/docs/media-analytics/using/media-overview.html#about-adobe-analytics-for-streaming-media).

* Adobe Analytics视频报表与Adobe Dynamic Media Classic的集成支持解决方案变量，但不支持自定义变量。

   参见 [音频和视频参数](https://experienceleague.adobe.com/docs/media-analytics/using/metrics-and-metadata/audio-video-parameters.html#metrics-and-metadata) 有关解决方案变量和自定义变量的更多信息。

* 支持一分钟递增的现成区段。 不过，不支持自定义区段报告，例如，客户根据时间增量定义的里程碑（百分比里程碑）或偏移里程碑。

   有关流媒体要求和设置的更多信息，请参阅 [在Adobe Analytics中测量流媒体](https://experienceleague.adobe.com/docs/media-analytics/using/media-overview.html).

* 有关自定义变量和解决方案变量的信息，请参阅 [媒体报表启用](https://experienceleague.adobe.com/docs/media-analytics/using/media-reports/media-reports-enable.html?lang=en#media-reports).

>[!NOTE]
>
>如果您许可的Adobe Analytics解决方案不包含视频心率，则必须继续使用本章所述的步骤，将Adobe Analytics变量分配给Adobe Dynamic Media Classic查看器事件和变量。
