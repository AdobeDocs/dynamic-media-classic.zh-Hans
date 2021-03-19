---
title: 启用 Adobe Analytics 视频报告
description: 了解如何启用Adobe Analytics视频报表。
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: 数据工程师，管理员，业务从业者
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '252'
ht-degree: 19%

---


# 启用 Adobe Analytics 视频报告{#enabling-adobe-analytics-video-reports}

在Dynamic Media Classic中配置Adobe Analytics时，使用基于Adobe Analytics心率的视频报告，您不再需要启用四个视频查看器事件（播放、暂停、停止、里程碑）。 视频心率可与现成的Dynamic Media Classic HTML5视频和混合媒体查看器配合使用。 视频播放器生成跟踪数据以在 Adobe Analytics 视频报告中查看。

* 有关流媒体和“心率测量”的介绍，请参阅[关于Adobe Analytics for Streaming Media](https://experienceleague.adobe.com/docs/media-analytics/using/media-overview.html#about-adobe-analytics-for-streaming-media)。

* 将Adobe Analytics视频报表与Dynamic Media Classic集成支持解决方案变量，但不支持自定义变量。

   有关解决方案变量和自定义变量的详细信息，请参阅[音频和视频参数](https://experienceleague.adobe.com/docs/media-analytics/using/metrics-and-metadata/audio-video-parameters.html#metrics-and-metadata)。

* 支持一分钟增量的现成区段。不过，不支持自定义区段报告，例如，客户根据时间增量定义的里程碑（百分比里程碑）或偏移里程碑。

   有关流媒体要求和设置的详细信息，请参阅[在Adobe Analytics中测量流媒体](https://experienceleague.adobe.com/docs/media-analytics/using/media-overview.html)。

* 有关自定义变量和解决方案变量的信息，请参阅[媒体报表enablement](https://experienceleague.adobe.com/docs/media-analytics/using/media-reports/media-reports-enable.html?lang=en#media-reports)。

>[!NOTE]
>
>如果您的Adobe Analytics许可解决方案不包括视频心率，则您需要继续使用本章中描述的步骤，将Adobe Analytics变量分配给Dynamic Media Classic查看器事件和变量。

