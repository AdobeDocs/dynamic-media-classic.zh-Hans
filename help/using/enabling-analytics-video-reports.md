---
title: 启用Adobe Analytics视频报表
description: 了解如何在Adobe Dynamic Media Classic中启用Adobe Analytics视频报表。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 9d017742-1ed2-411d-a8a6-438102bf1557
topic: Development, Integrations
level: Experienced
source-git-commit: 1b90beb99b161b76da81403f5aed9755b3a92c8b
workflow-type: tm+mt
source-wordcount: '249'
ht-degree: 5%

---

# 启用Adobe Analytics视频报表{#enabling-adobe-analytics-video-reports}

使用基于Adobe Analytics心率的视频报告，在Adobe Dynamic Media Classic中配置Adobe Analytics时，不必再启用四个视频查看器事件（播放、暂停、停止、里程碑）。 视频心率适用于开箱即用的Adobe Dynamic Media Classic HTML5视频和混合媒体查看器。 视频播放器生成跟踪数据以在 Adobe Analytics 视频报告中查看。

* 有关流媒体和“心率测量”的介绍，请参阅 [关于适用于流媒体的Adobe Analytics](https://experienceleague.adobe.com/docs/media-analytics/using/media-overview.html).

* Adobe Analytics视频报表与Adobe Dynamic Media Classic的集成支持解决方案变量，但不支持自定义变量。

  请参阅 [音频和视频参数](https://experienceleague.adobe.com/docs/media-analytics/using/implementation/variables/audio-video-parameters.html) 有关解决方案变量和自定义变量的更多信息。

* 支持一分钟递增的现成区段。 但是，不支持自定义区段报告，例如客户定义的基于时间增量的里程碑、%里程碑或偏移里程碑。

  有关流媒体要求和设置的更多信息，请参阅 [在Adobe Analytics中测量流媒体](https://experienceleague.adobe.com/docs/media-analytics/using/media-overview.html).

* 有关自定义变量和解决方案变量的信息，请参阅 [媒体报表启用](https://experienceleague.adobe.com/docs/media-analytics/using/media-reports/media-reports-enable.html?lang=en#media-reports).

>[!NOTE]
>
>如果您的Adobe Analytics许可解决方案不包含视频心率，则必须继续使用本章中介绍的步骤，将Adobe Analytics变量分配给Adobe Dynamic Media Classic查看器事件和变量。
