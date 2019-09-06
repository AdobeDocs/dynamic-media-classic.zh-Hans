---
title: 启用 Adobe Analytics 视频报告
seo-title: 启用 Adobe Analytics 视频报告
description: 'null'
seo-description: 了解如何启用Adobe Analytics视频报告。
uuid: 078594b2-7d53-47148-ff3 b5 c3 a5 e36
contentOwner: admin
content-type: 引用
products: SG_ EXPERIENCE MANAGER/Dynamic-Media-Scene-7
geptopics: SG_ SCENEESFERENONDAND_ PK/categories/adobe_ analytics_ contracting_ kit
discoiquuid: 18644a53-92da-40ab-b961-318d8832 c54 d
translation-type: tm+mt
source-git-commit: 32f5e03766466ceaafe58780e9e80dbdd4a0c3dd

---


# 启用 Adobe Analytics 视频报告{#enabling-adobe-analytics-video-reports}

使用基于Adobe Analytics心跳的视频报表，在Dynamic Media经典中配置Adobe Analytics时，您不再需要启用四个视频查看器事件(播放、暂停、停止、里程碑)。Video Heartbat可与现成的动态媒体经典HTML视频和MixedMedia查看器一起使用。视频播放器生成跟踪数据以在 Adobe Analytics 视频报告中查看。

* 将Adobe Analytics视频报告与Dynamic Media Classic集成在一起支持解决方案变量，但不支持自定义变量。

   See [Configure Analytics Video Reporting](https://microsite.omniture.com/t2/help/en_US/sc/appmeasurement/hbvideo/video_analytics_config.html) for more information about solution variables and custom variables.

* 支持一分钟增量的现成区段。不过，不支持自定义区段报告，例如，客户根据时间增量定义的里程碑（百分比里程碑）或偏移里程碑。

For more information about Video Heartbeat requirements and setup, see [Measuring Video in Adobe Analytics using Video Heartbeat](https://microsite.omniture.com/t2/help/en_US/sc/appmeasurement/hbvideo/).

>[!NOTE]
>
>如果您的Adobe Analytics的许可解决方案不包含Video Heartbat，您需要继续使用本章中描述的步骤，将Adobe Analytics变量分配给Dynamic Media经典查看器事件和变量。

