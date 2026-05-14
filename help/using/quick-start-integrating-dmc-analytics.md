---
title: 快速入门：集成Adobe Dynamic Media Classic和Adobe Analytics
description: 有关如何集成Adobe Dynamic Media Classic和Adobe Analytics的简介和快速入门。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Developer,Admin,User
exl-id: a8fa2414-af01-4a58-bb33-dfd12c1056cc
topic: Integrations
level: Experienced
autotag-review: '2026-05-13T20:10:08.073Z'
TQID: 'https://experienceleague.adobe.com/DnpXpIqOz1HSLxZAoEOTHG65PSqTWLK7R--OzJj3FcY'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
level_v2:
  - id: d378ca77-2da1-4f39-ad92-1917fe974a38
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
source-git-commit: 81e92d0e8963cccb5b058328cb7601925f7ace4f
workflow-type: tm+mt
source-wordcount: 699
ht-degree: 23%

---

# 快速入门：集成Adobe Dynamic Media Classic和Adobe Analytics {#quick-start-integrating-dmc-analytics}

Adobe Analytics 是一款行业领先的产品，营销人员可用来评估、分析及优化整合自多个营销渠道的所有在线活动的数据。

将Adobe Analytics与Adobe Dynamic Media Classic集成后，您可以在网站上使用Adobe Dynamic Media Classic查看器获取有关网站访客行为的报表。 例如，当网站访客在Adobe Dynamic Media Classic缩放查看器中选择缩放目标时，Adobe Analytics将记录此操作。 Adobe Analytics报表可收集有关Adobe Dynamic Media Classic查看器中用户活动的累积信息。

通过使用 Adobe Analytics 报告，可以非常清楚地了解客户在网站上的活动。 您可以确定哪些产品演示文稿会导致转化，哪些不吸引客户兴趣。

另请参阅Adobe Analytics中的[度量值视频](https://experienceleague.adobe.com/zh-hans/docs/media-analytics/using/media-overview)。

>[!NOTE]
>
>要将Analytics与Adobe Dynamic Media Classic集成并生成Analytics报表，需要有效的Adobe Analytics帐户。

本快速入门指南旨在通过Adobe Analytics工具包帮助您快速启动和运行。

## &#x200B;1. 通过Adobe Dynamic Media Classic登录Adobe Analytics并下载Adobe Analytics报表变量

>[!NOTE]
>
>验证您是否已被添加为Adobe Analytics中Web服务访问组的成员。 请在配置Adobe Analytics报表之前进行此验证。 此外，在将Adobe Analytics报表变量与Adobe Dynamic Media Classic事件匹配之前。 此组中的成员可以访问指定报表包中的所有报表。 无论界面中设置的权限如何，您都可以使用Experience Cloud的Web服务API来执行此操作。 若要向组添加成员，请在Adobe Analytics中转到&#x200B;**[!UICONTROL 管理工具]** > **[!UICONTROL 用户管理]** > **[!UICONTROL 编辑组]**。

确认您是Web服务访问组成员后，在Adobe Dynamic Media Classic中，转到&#x200B;**[!UICONTROL 设置]** > **[!UICONTROL 应用程序设置]** > **[!UICONTROL Adobe Analytics]**。 在“Adobe Analytics配置”页面上，选择&#x200B;**[!UICONTROL Adobe Analytics登录]**。

请参阅[登录Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics)。

在“Adobe Analytics登录”对话框中，键入您的Experience Cloud组织ID（可选）和完整凭据，然后选择&#x200B;**[!UICONTROL 登录]**。 在“报告套件”下拉菜单中，选择要使用的报告套件的名称。

## &#x200B;2. 将Adobe Analytics报表变量分配给Adobe Dynamic Media Classic查看器事件和Adobe Dynamic Media Classic变量

在“Adobe Analytics 配置”页中，指定 Adobe Analytics 报告中所需的信息。 对于您想要了解的相关信息的每个Adobe Dynamic Media Classic查看器事件，请选择一个Adobe Analytics变量（从报表包中）和一个Adobe Dynamic Media Classic变量。

* 查看器事件描述了要在报告中评估的用户活动。
* Adobe Dynamic Media Classic变量描述您希望报表交付的用户事件的相关数据。

“Adobe Analytics 配置”还提供了用于激活、编辑和删除查看器事件的工具。

在Adobe Analytics配置页面中选择&#x200B;**[!UICONTROL 保存]**&#x200B;后，将在Adobe Dynamic Media Classic查看器中插入用于测量用户活动的自定义跟踪代码。 可以通过该功能在 Adobe Analytics 报告中跟踪用户活动。

请参阅[配置Adobe Analytics报表](configuring-analytics-reports.md#configuring_adobe_analytics_reports)。

## &#x200B;3. 发布Adobe Dynamic Media Classic查看器

发布Adobe Dynamic Media Classic查看器，以便在Adobe Dynamic Media Classic服务器上加载查看器（在Adobe Analytics报表中带有用于跟踪用户活动的代码）。 发布后，此信息将包含在查看器中。 可将其用于Adobe Analytics的分析。

请参阅[发布配置信息](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information)。

## &#x200B;4. 将Adobe Dynamic Media Classic查看器放置在您的网站上

将带有Adobe Analytics跟踪代码的Adobe Dynamic Media Classic查看器放在您的网站上。

## &#x200B;5. 查看 Adobe Analytics 报告以测试 Adobe Analytics 集成

要查看 Adobe Analytics 报告，请访问 Adobe Analytics 网站。 通过“报告”页面可以查看数据及生成图形和图表，以便通过不同查看器来评估用户活动。

查看[通过查看Adobe Analytics报表来测试Adobe Analytics集成](testing-integration-viewing-analytics-report.md#testing_the_integration_by_viewing_an_adobe_analytics_report)。
