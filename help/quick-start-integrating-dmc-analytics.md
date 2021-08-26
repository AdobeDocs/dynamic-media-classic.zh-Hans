---
title: “快速入门：集成AdobeDynamic Media Classic和Adobe Analytics”
description: 集成AdobeDynamic Media Classic和Adobe Analytics的简介和快速入门，可帮助您快速启动并运行。
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: a8fa2414-af01-4a58-bb33-dfd12c1056cc
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '686'
ht-degree: 39%

---

# 快速入门：集成AdobeDynamic Media Classic和Adobe Analytics {#quick-start-integrating-dmc-analytics}

Adobe Analytics 是一款行业领先的产品，营销人员可用来评估、分析及优化整合自多个营销渠道的所有在线活动的数据。

将Adobe Analytics与AdobeDynamic Media Classic集成后，您可以在网站上获取有关使用AdobeDynamic Media Classic查看器的网站访客行为的报表。 例如，当网站访客在AdobeDynamic Media Classic缩放查看器中单击缩放目标时，Adobe Analytics会记录此操作。 Adobe Analytics报表可以在AdobeDynamic Media Classic查看器中收集有关用户活动的累积信息。

通过使用 Adobe Analytics 报告，可以非常清楚地了解客户在网站上的活动。您可以确定哪些产品演示可导致转化，哪些产品演示不吸引客户兴趣。

另请参阅[在 Adobe Analytics 中测量视频](https://experienceleague.adobe.com/docs/media-analytics/using/media-overview.html)。

>[!NOTE]
>
>要将Analytics与AdobeAdobe Analytics Classic集成并生成Analytics报表，需要具有有效的Dynamic Media帐户。

该快速入门旨在帮助您快速学会如何使用 Adobe Analytics 仪器包。

## 1.通过AdobeAdobe Analytics Classic和下载Adobe Analytics报表变量，登录到Dynamic Media

>[!NOTE]
>
>在配置Adobe Analytics报表并匹配Adobe Analytics报表变量以AdobeDynamic Media Classic事件之前，请确认您已作为Adobe Analytics中Web服务访问组的成员添加。 该组中的成员可以通过 Marketing Cloud 的 Web 服务 API 访问指定报表包中的所有报表，而无论是否在界面中设置了权限。要在组中添加成员，请在 Adobe Analytics 中单击“**[!UICONTROL 管理工具]**”>“**[!UICONTROL 用户管理]**”>“**[!UICONTROL 编辑组]**”。

确认您是Web服务访问组的成员后，在AdobeDynamic Media Classic中，单击&#x200B;**[!UICONTROL 设置]** > **[!UICONTROL 应用程序设置]** > **[!UICONTROL Adobe Analytics]**。 在“Adobe Analytics 配置”页中，单击“**[!UICONTROL Adobe Analytics 登录]**”。

请参阅[登录到 Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics)。

在“Adobe Analytics登录”对话框中，键入您的Marketing Cloud组织ID（可选）和完整凭据，然后单击&#x200B;**[!UICONTROL 登录]**。 在“报告套件”下拉菜单中，选择要使用的报告套件的名称。

## 2.将Adobe Analytics报表变量分配给AdobeDynamic Media Classic查看器事件和AdobeDynamic Media Classic变量

在“Adobe Analytics 配置”页中，指定 Adobe Analytics 报告中所需的信息。对于您想要了解的每个AdobeDynamic Media Classic查看器事件，请选择一个Adobe Analytics变量（从您的报表包中）和一个AdobeDynamic Media Classic变量。

* 查看器事件描述了要在报告中评估的用户活动。
* AdobeDynamic Media Classic变量描述您希望报表交付的用户事件数据。

“Adobe Analytics 配置”还提供了用于激活、编辑和删除查看器事件的工具。

在“Adobe Analytics配置”页面中单击&#x200B;**[!UICONTROL Save]**&#x200B;后，将在AdobeDynamic Media Classic查看器中插入用于测量用户活动的自定义跟踪代码。 可以通过该功能在 Adobe Analytics 报告中跟踪用户活动。

请参阅[配置 Adobe Analytics 报告](configuring-analytics-reports.md#configuring_adobe_analytics_reports)。

## 3.发布AdobeDynamic Media Classic查看器

发布您的AdobeDynamic Media Classic查看器，以便查看器(包含用于跟踪Adobe Analytics报表中用户活动的代码)加载到AdobeDynamic Media Classic服务器上。 在发布后，将在查看器中包含该信息，并且可用于 Adobe Analytics 分析。

请参阅[发布配置信息](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information)。

## 4.将AdobeDynamic Media Classic查看器放入您的网站

将具有Adobe Analytics跟踪代码的AdobeDynamic Media Classic查看器放置到您的网站上。

## 5.通过查看Adobe Analytics报表来测试Adobe Analytics集成

要查看 Adobe Analytics 报告，请访问 Adobe Analytics 网站。通过“报告”页面可以查看数据及生成图形和图表，以便通过不同查看器来评估用户活动。

请参阅[查看 Adobe Analytics 报告以测试 Adobe Analytics 集成](testing-integration-viewing-analytics-report.md#testing_the_integration_by_viewing_an_adobe_analytics_report)。
