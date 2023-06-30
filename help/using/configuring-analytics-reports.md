---
title: 配置Adobe Analytics报表
description: 了解如何在Adobe Dynamic Media Classic中配置Adobe Analytics报表。
uuid: bf210f68-dcb0-4e86-be04-0a8b2117ef2a
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: f4c8c2b3-cc95-416f-9a5d-da81c231dfc2
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: d9fda3b8-7da8-4a30-a5f8-9bb34ec1b43d
topic: Integrations, Development
level: Experienced
source-git-commit: 5d8b7cb8b4616a998346675d7324b568634698fb
workflow-type: tm+mt
source-wordcount: '1231'
ht-degree: 27%

---

# 配置Adobe Analytics报表{#configuring-adobe-analytics-reports}

要告知Adobe Analytics您想在Adobe Analytics报表中查看哪些信息，请转到Adobe Analytics配置屏幕。 配置报表后，此屏幕会为每个您希望了解相关信息的查看器事件列出相应的Adobe Analytics变量和Adobe Dynamic Media Classic变量。 这些查看器事件 — Adobe Analytics变量 — Adobe Dynamic Media Classic变量组合决定了报告的信息。

除了将查看器事件与变量关联之外，“Adobe Analytics配置”屏幕还提供了用于激活、编辑和删除查看器事件的工具。

>[!NOTE]
>
>每当您在Adobe Analytics中更改Adobe Analytics报表设置时，请确保从Adobe Dynamic Media Classic中重新登录到Adobe Analytics，重新保存Adobe Analytics配置设置，然后重新发布。

请参阅[登录到 Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics)。

参见 [发布配置信息](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information).

## 将Adobe Analytics变量分配给Adobe Dynamic Media Classic查看器事件和变量 {#assigning-adobe-analytics-variables-to-scene-viewer-events-and-variables}

使用Adobe Analytics配置屏幕将查看器事件与Adobe Analytics变量和Adobe Dynamic Media Classic变量关联。 对于每个查看器事件，选择一个Adobe Analytics变量和一个Adobe Dynamic Media Classic变量。 有关打开“Adobe Analytics 配置”屏幕的说明，请参阅[登录到 Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics)。

**要将Adobe Analytics变量分配给Adobe Dynamic Media Classic查看器事件和变量，请执行以下操作：**

1. 从Adobe Dynamic Media Classic登录Adobe Analytics并选择报表包后，在Adobe Analytics配置页面的右侧表列中，通过选择激活查看器事件 **[!UICONTROL 启用]**.
1. 在变量列下，通过选择所需查看器事件的箭头按钮来显示变量对选择器。

   请参阅[查看器事件](configuring-analytics-reports.md#viewer_events)。

1. 添加Adobe Dynamic Media Classic变量。

   参见 [Adobe Dynamic Media Classic变量](configuring-analytics-reports.md#scene7_variables).

1. 添加一个 Adobe Analytics 变量。
1. （可选）要添加其他变量对，请选择 **[!UICONTROL 添加]**.
1. 选择 **[!UICONTROL 保存]**.

   选择后 **[!UICONTROL 保存]**、查看器事件、其Adobe Analytics变量及其Adobe Dynamic Media Classic变量将在Adobe Analytics配置屏幕中列出。

1. 在右下角，选择 **[!UICONTROL 关闭]**.
1. 转到 **[!UICONTROL Publish]** > **[!UICONTROL 提交发布]** 以运行图像服务发布。

   必须进行发布，以便查看器中包含的信息在Adobe Dynamic Media Classic服务器上可用。

### 查看器事件 {#viewer-events}

查看器事件描述用户使用Adobe Dynamic Media Classic查看器执行的操作。 当用户启动特定操作（例如选择缩略图或启动或停止视频）时，查看者“广播”事件到网页，以及与该事件关联的数据。

下表介绍了可添加到Adobe Analytics配置屏幕的查看器事件。

| 查看器事件 | HTML5 查看器平台支持和查看器 | 说明 |
| --- | --- | --- |
| LOAD | **X**（eCatalog、弹出、旋转集、视频、缩放） | 当用户启动查看器时 |
| PAGE | **X** (eCatalog) | 在eCatalogs中，用户翻页时；在定向缩放查看器中，用户选择其他目标或色板时。 |
| SWAP | **X**（eCatalog、弹出、旋转集、视频、缩放） | 当用户选择其他缩略图查看其他图像时。 |
| ITEM | **X** (eCatalog) | 在支持已定义变换的图像映射的查看器中，用户将指针悬停在图像映射上以读取变换文本时。 |
| HREF | **X** (eCatalog) | 在支持“图像映射”的查看器中，用户在“图像映射”中选择URL时。 |
| TARGET | | 在目标缩放查看器中，用户选择要缩放到部分图像的缩放目标时。 |
| SEARCH | | 在 eCatalog 中用户执行关键词搜索时。 |
| PLAY | **X**（视频） | 在视频查看器中，当用户选择“播放”开始播放视频时。<br><br>**注意：** 如果您使用的是基于Adobe Analytics心率的视频报告，则在Adobe Dynamic Media Classic中配置Adobe Analytics时，不需要将任何变量映射到此查看器事件。 视频心率适用于开箱即用的Adobe Dynamic Media Classic HTML5 Video和MixedMedia查看器。 视频播放器生成跟踪数据以在 Adobe Analytics 视频报告中查看。参见 [启用Adobe Analytics视频报表](enabling-analytics-video-reports.md). |
| PAUSE | **X**（视频） | 在视频查看器中，当用户选择 **[!UICONTROL 暂停]** 冻结视频。<br><br>**注意：** 如果您使用的是基于Adobe Analytics心率的视频报告，则在Adobe Dynamic Media Classic中配置Adobe Analytics时，不需要将任何变量映射到此查看器事件。 视频心率适用于开箱即用的Adobe Dynamic Media Classic HTML5 Video和MixedMedia查看器。 视频播放器生成跟踪数据以在 Adobe Analytics 视频报告中查看。参见 [启用Adobe Analytics视频报表](enabling-analytics-video-reports.md). |
| STOP | **X**（视频） | 在视频查看器中，当用户选择 **[!UICONTROL 停止]** 停止播放视频。<br><br>**注意：** 如果您使用的是基于Adobe Analytics心率的视频报告，则在Adobe Dynamic Media Classic中配置Adobe Analytics时，不需要将任何变量映射到此查看器事件。 视频心率适用于开箱即用的Adobe Dynamic Media Classic HTML5 Video和MixedMedia查看器。 视频播放器生成跟踪数据以在 Adobe Analytics 视频报告中查看。参见 [启用Adobe Analytics视频报表](enabling-analytics-video-reports.md). |
| MILESTONE | **X**  (视频) | 在视频查看器中，用户在观看到视频的 0%、25%、50%、75% 或 100% 时会生成里程碑事件。<br><br>**注意：** 如果您使用的是基于Adobe Analytics心率的视频报告，则在Adobe Dynamic Media Classic中配置Adobe Analytics时，不需要将任何变量映射到此查看器事件。 视频心率适用于开箱即用的Adobe Dynamic Media Classic HTML5 Video和MixedMedia查看器。 视频播放器生成跟踪数据以在 Adobe Analytics 视频报告中查看。参见 [启用Adobe Analytics视频报表](enabling-analytics-video-reports.md). |
| 样本 | **X** （弹出、缩放） | 此查看器事件映射到Adobe Dynamic Media Classic中的页面查看器事件。 |
| 缩放 | **X**（eCatalog、旋转集、缩放） | Adobe Analytics 不进行跟踪。 |
| 平移 | **X**（eCatalog、旋转集、缩放） | Adobe Analytics 不进行跟踪。 |
| 旋转 | **X**（旋转集） | Adobe Analytics 不进行跟踪。 |

### Adobe Dynamic Media Classic变量 {#scene-variables}

对于Adobe Analytics配置屏幕上的每个查看器事件，选择一个Adobe Analytics变量和 *Adobe Dynamic Media Classic变量*. Adobe Dynamic Media Classic变量表示可为报表获取的数据。 例如，`searchTerm` 变量可列出在 eCatalog 搜索中使用的关键字。

下表介绍了Adobe Dynamic Media Classic变量：

| Adobe Dynamic Media Classic变量 | 说明 |
| --- | --- |
| asset | Adobe Dynamic Media Classic资源ID或视频路径文件。 |
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

* **激活**  — 选择 **[!UICONTROL 启用]** 激活或 **[!UICONTROL 禁用]** 取消激活选定的查看器事件。

* **编辑**  — 选择一个查看器事件并选择 **[!UICONTROL 查看/编辑]** 变量灰色按钮。 在“Adobe Dynamic Media Classic变量”和“Adobe Analytics变量”下拉列表中，从各自的列表中选择一个不同的变量。 有关更多信息，请参阅 [将Adobe Analytics变量分配给Adobe Dynamic Media Classic查看器事件和变量](#assigning-adobe-analytics-variables-to-scene-viewer-events-and-variables).

* **删除**  — 选择一个查看器事件，然后选择 **[!UICONTROL 查看/编辑]** 变量灰色按钮。 选择 **[!UICONTROL 删除]**.
