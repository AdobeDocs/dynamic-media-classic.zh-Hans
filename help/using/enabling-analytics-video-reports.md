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
source-git-commit: de6997fda88c4471625242ee9cca59b344cee945
workflow-type: tm+mt
source-wordcount: '221'
ht-degree: 0%

---

# 启用Adobe Analytics视频报表{#enabling-adobe-analytics-video-reports}

使用基于Adobe Analytics心率的视频报告，在Adobe Dynamic Media Classic中配置Adobe Analytics时，不必再启用四个视频查看器事件（播放、暂停、停止、里程碑）。 视频心率适用于开箱即用的Adobe Dynamic Media Classic HTML5视频和混合媒体查看器。 视频播放器会生成跟踪数据以供在Adobe Analytics视频报表中查看。

* 有关流媒体和“心率测量”的简介，请参阅[关于Adobe Analytics for Streaming Media](https://experienceleague.adobe.com/en/docs/media-analytics/using/media-overview)。

* Adobe Analytics视频报表与Adobe Dynamic Media Classic的集成支持解决方案变量，但不支持自定义变量。

  有关解决方案变量和自定义变量的详细信息，请参阅[音频和视频参数](https://experienceleague.adobe.com/en/docs/media-analytics/using/implementation/variables/audio-video-parameters)。

* 支持一分钟递增的现成区段。 但是，不支持自定义区段报告，例如客户定义的基于时间增量的里程碑、%里程碑或偏移里程碑。

  有关流媒体要求和设置的详细信息，请参阅[Adobe Analytics中的度量值流媒体](https://experienceleague.adobe.com/en/docs/media-analytics/using/media-overview)。

* 有关自定义变量和解决方案变量的信息，请参阅[媒体报表启用](https://experienceleague.adobe.com/en/docs/media-analytics/using/media-reports/media-reports-enable#media-reports)。

>[!NOTE]
>
>如果您许可的Adobe Analytics解决方案不包含视频心率，请继续使用本章中介绍的步骤，将Adobe Analytics变量分配给Adobe Dynamic Media Classic查看器事件和变量。
