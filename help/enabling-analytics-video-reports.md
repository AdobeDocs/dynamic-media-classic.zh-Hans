---
title: 启用 Adobe Analytics 视频报告
seo-title: 启用 Adobe Analytics 视频报告
description: 'null'
seo-description: 了解如何启用Adobe Analytics视频报告。
uuid: 078594b2-7d53-4714-8128-ff3b5c3a5e36
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: 18644a53-92da-40ab-b961-318d8332c54d
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '215'
ht-degree: 26%

---


# 启用 Adobe Analytics 视频报告{#enabling-adobe-analytics-video-reports}

使用基于Adobe Analytics心跳的视频报告，在Dynamic Media经典中配置Adobe Analytics时，您不再需要启用四个视频查看器事件（播放、暂停、停止、里程碑）。 视频心跳可以与现成的Dynamic Media经典HTML5视频和混合媒体查看器配合使用。 视频播放器生成跟踪数据以在 Adobe Analytics 视频报告中查看。

* 将Adobe Analytics视频报表与Dynamic Media经典集成支持解决方案变量，但不支持自定义变量。

   有关解决方案变量和自定义变量的详细信息，请参阅[配置分析视频报告](https://microsite.omniture.com/t2/help/en_US/sc/appmeasurement/hbvideo/video_analytics_config.html)。

* 支持一分钟增量的现成区段。不过，不支持自定义区段报告，例如，客户根据时间增量定义的里程碑（百分比里程碑）或偏移里程碑。

有关视频心跳要求和设置的详细信息，请参阅[使用视频心跳测量Adobe Analytics的视频](https://microsite.omniture.com/t2/help/en_US/sc/appmeasurement/hbvideo/)。

>[!NOTE]
>
>如果您的Adobe Analytics许可解决方案不包括视频心跳，您需要继续使用本章中描述的步骤，将Adobe Analytics变量分配给Dynamic Media经典查看器事件和变量。

