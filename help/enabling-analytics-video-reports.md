---
title: 启用 Adobe Analytics 视频报告
seo-title: 启用 Adobe Analytics 视频报告
description: 'null'
seo-description: 了解如何启用Adobe Analytics视频报告。
uuid: 078594b2-7d53-4714-8128-ff3b5c3a5e36
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: 18644a53-92da-40ab-b961-318d8332c54d
translation-type: tm+mt
source-git-commit: 32f5e03766466ceaafe58780e9e80dbdd4a0c3dd

---


# 启用 Adobe Analytics 视频报告{#enabling-adobe-analytics-video-reports}

使用基于Adobe Analytics心跳的视频报告，在Dynamic Media Classic中配置Adobe Analytics时，您不再需要启用四个视频查看器事件（播放、暂停、停止、里程碑）。 视频心率可与开箱即用的Dynamic Media Classic HTML5视频和混合媒体查看器配合使用。 视频播放器生成跟踪数据以在 Adobe Analytics 视频报告中查看。

* Adobe Analytics视频报告与Dynamic Media Classic的集成支持解决方案变量，但不支持自定义变量。

   See [Configure Analytics Video Reporting](https://microsite.omniture.com/t2/help/en_US/sc/appmeasurement/hbvideo/video_analytics_config.html) for more information about solution variables and custom variables.

* 支持一分钟增量的现成区段。不过，不支持自定义区段报告，例如，客户根据时间增量定义的里程碑（百分比里程碑）或偏移里程碑。

For more information about Video Heartbeat requirements and setup, see [Measuring Video in Adobe Analytics using Video Heartbeat](https://microsite.omniture.com/t2/help/en_US/sc/appmeasurement/hbvideo/).

>[!NOTE]
>
>如果Adobe Analytics的许可解决方案不包括视频心率，则您需要继续使用本章中描述的步骤，将Adobe Analytics变量分配给Dynamic Media Classic查看器事件和变量。

