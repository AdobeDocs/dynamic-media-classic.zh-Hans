---
title: 配置 Adobe Analytics 报告
description: 了解如何配置Adobe Analytics报表。
uuid: bf210f68-dcb0-4e86-be04-0a8b2117ef2a
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: f4c8c2b3-cc95-416f-9a5d-da81c231dfc2
feature: Dynamic Media Classic
role: Data Engineer,Administrator,Business Practitioner
exl-id: d9fda3b8-7da8-4a30-a5f8-9bb34ec1b43d
translation-type: tm+mt
source-git-commit: 98463dbc24e141547d01bd3f71b1b9fe3a692c14
workflow-type: tm+mt
source-wordcount: '1196'
ht-degree: 46%

---

# 配置 Adobe Analytics 报告{#configuring-adobe-analytics-reports}

要向 Adobe Analytics 通知 Adobe Analytics 报告中所需的信息，请转到“Adobe Analytics 配置”屏幕。配置报表后，此屏幕列表将针对您需要的每个查看器事件显示相应的Adobe Analytics变量和Dynamic Media Classic变量。 这些查看器事件-Adobe Analytics变量 — Dynamic Media Classic变量组合决定报告哪些信息。

除了将查看器事件与变量关联外，Adobe Analytics配置屏幕还会优惠用于激活、编辑和删除查看器事件的工具。

>[!NOTE]
>
>在Adobe Analytics中更改Adobe Analytics报表设置时，请确保从Adobe Dynamic Media Classic中重新登录到Adobe Analytics，重新保存Adobe Analytics配置设置，然后重新发布。

请参阅[登录到 Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics)。

请参阅[发布配置信息](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information)。

## 将Adobe Analytics变量分配给Dynamic Media Classic查看器事件和变量{#assigning-adobe-analytics-variables-to-scene-viewer-events-and-variables}

使用Adobe Analytics配置屏幕将查看器事件与Adobe Analytics变量和Dynamic Media Classic变量关联。 对于每个查看器事件，选择一个Adobe Analytics变量和一个Dynamic Media Classic变量。 有关打开“Adobe Analytics 配置”屏幕的说明，请参阅[登录到 Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics)。

**将Adobe Analytics变量分配给Dynamic Media Classic查看器事件和变量**

1. 在从Dynamic Media Classic中登录Adobe Analytics并选择报表包后，在Adobe Analytics配置页的右表列中，单击&#x200B;**[!UICONTROL 启用]**&#x200B;以激活查看器事件。
1. 在“变量”列下，单击所需的查看器事件的箭头按钮，显示变量对选择器。

   请参阅[查看器事件](configuring-analytics-reports.md#viewer_events)。

1. 添加Dynamic Media Classic变量。

   请参阅[Dynamic Media Classic变量](configuring-analytics-reports.md#scene7_variables)。

1. 添加一个 Adobe Analytics 变量。
1. （可选）要添加其他变量对，请单击“**添加**”。
1. 单击“**保存**”。

   单击“保存”后，查看器事件、其Adobe Analytics变量及其Dynamic Media Classic变量将列在“Adobe Analytics配置”屏幕中。

1. 在右下角单击“**关闭**”。
1. 单击“**发布**”>“**提交发布**”运行图像服务发布。

   必须进行发布，以便查看器中包含的信息在Dynamic Media Classic服务器上可用。

### 查看器事件 {#viewer-events}

查看器事件描述了用户使用Dynamic Media Classic查看器执行的操作。 当用户启动某些操作（如单击缩略图或启动或停止视频）时，查看器将事件“广播”到网页，以及与该事件关联的数据。

下表描述了可添加到“Adobe Analytics 配置”屏幕中的查看器事件。

| 查看器事件 | HTML5 查看器平台支持和查看器 | 说明 |
|--- |--- |--- |
| LOAD | **X**（eCatalog、弹出、旋转集、视频、缩放） | 用户启动查看器时。 |
| PAGE | **X** (eCatalog) | 在 eCatalog 中用户翻页时；在目标缩放查看器中用户单击其他目标或颜色样本时。 |
| SWAP | **X**（eCatalog、弹出、旋转集、视频、缩放） | 用户单击其他缩略图以查看其他图像时。 |
| ITEM | **X** (eCatalog) | 在支持已定义变换的图像映射的查看器中，用户将指针悬停在图像映射上以读取变换文本时。 |
| HREF | **X** (eCatalog) | 在支持图像映射的查看器中，用户在图像映射中单击 URL 时。 |
| TARGET |  | 在目标缩放查看器中，当用户单击缩放目标以将其缩放为图像的一部分时。 |
| SEARCH |  | 在 eCatalog 中用户执行关键词搜索时。 |
| PLAY | **X**（视频） | 在视频查看器中，用户单击“播放”开始播放视频时。<br><br>**注意：** 如果您使用基于Adobe Analytics心率的视频报告，则在Dynamic Media Classic中配置Adobe Analytics时，无需将任何变量映射到此查看器事件。视频心率可与现成的Dynamic Media Classic HTML5视频和混合媒体查看器配合使用。 视频播放器生成跟踪数据以在 Adobe Analytics 视频报告中查看。请参阅[启用Adobe Analytics视频报表](enabling-analytics-video-reports.md)。 |
| PAUSE | **X**（视频） | 在视频查看器中，用户单击“暂停”以暂停视频时。<br><br>**注意：** 如果您使用基于Adobe Analytics心率的视频报告，则在Dynamic Media Classic中配置Adobe Analytics时，无需将任何变量映射到此查看器事件。视频心率可与现成的Dynamic Media Classic HTML5视频和混合媒体查看器配合使用。 视频播放器生成跟踪数据以在 Adobe Analytics 视频报告中查看。请参阅[启用Adobe Analytics视频报表](enabling-analytics-video-reports.md)。 |
| STOP | **X**（视频） | 在视频查看器中，用户单击“停止”会停止播放视频。<br><br>**注意：** 如果您使用基于Adobe Analytics心率的视频报告，则在Dynamic Media Classic中配置Adobe Analytics时，无需将任何变量映射到此查看器事件。视频心率可与现成的Dynamic Media Classic HTML5视频和混合媒体查看器配合使用。 视频播放器生成跟踪数据以在 Adobe Analytics 视频报告中查看。请参阅[启用Adobe Analytics视频报表](enabling-analytics-video-reports.md)。 |
| MILESTONE | **X**  (视频) | 在视频查看器中，用户在观看到视频的 0%、25%、50%、75% 或 100% 时会生成里程碑事件。<br><br>**注意：** 如果您使用基于Adobe Analytics心率的视频报告，则在Dynamic Media Classic中配置Adobe Analytics时，无需将任何变量映射到此查看器事件。视频心率可与现成的Dynamic Media Classic HTML5视频和混合媒体查看器配合使用。 视频播放器生成跟踪数据以在 Adobe Analytics 视频报告中查看。请参阅[启用Adobe Analytics视频报表](enabling-analytics-video-reports.md)。 |
| 样本 | X （弹出、缩放） | 此查看器事件将映射到Dynamic Media Classic中的PAGE查看器事件。 |
| 缩放 | **X**（eCatalog、旋转集、缩放） | Adobe Analytics 不进行跟踪。<br> |
| 平移 | **X**（eCatalog、旋转集、缩放） | Adobe Analytics 不进行跟踪。<br> |
| 旋转 | **X**（旋转集） | Adobe Analytics 不进行跟踪。<br> |


### Dynamic Media Classic变量{#scene-variables}

对于“Adobe Analytics配置”屏幕上的每个查看器事件，选择Adobe Analytics变量和&#x200B;*Dynamic Media Classic变量*。 Dynamic Media经典变量表示可为报表获取的数据。 例如，`searchTerm` 变量可列出在 eCatalog 搜索中使用的关键字。

下表介绍了Dynamic Media Classic变量。

| Dynamic Media Classic变量 | 说明 |
|--- |:--- |
| asset | Dynamic Media经典资源ID或视频路径文件。 |
| viewerId | 指定给各个不同的查看器类型的任意编号。 |
| pageLabel | 在 eCatalog 中，查看器显示的页面。 |
| label | 标签值（字符串）。 |
| frame | 图像集中的页面或页面引用。 |
| rollover_keyRaw | 完整的 HREF 值，不仅是已处理部分。 |
| rollover_keyProc | 在图像映射中引用的项目的 ID（对 href 和项目事件有效）。 |
| searchTerm | 在 eCatalog 搜索中使用的搜索词。 |
| timeStamp | 在视频查看器中选择的“播放”、“停止”和“暂停”。 |
| progress | 完成的里程碑事件的百分比。 |
| targetId | ID 值（数值）。 |

## 激活、编辑和删除查看器事件 {#activating-editing-and-deleting-viewer-events}

可以在“Adobe Analytics 配置”屏幕上激活、编辑和删除查看器事件：

* **激**
活单 **** 击启用以激活或 **** 禁用以取消激活选定的查看器事件。

* **编**
辑选择查看器事件，然后单击 **[!UICONTROL 视图/]** 编辑变量灰色按钮。在Dynamic Media经典变量和Adobe Analytics变量下拉列表中，从每个列表选择不同的变量。 有关详细信息，请参阅将Adobe Analytics变量分配给Dynamic Media Classic查看器事件和变量。

* **删**
除选择查看器事件，然后单击 **[!UICONTROL 视图/]** 编辑变量灰色按钮。单击“**[!UICONTROL 删除]**”。
