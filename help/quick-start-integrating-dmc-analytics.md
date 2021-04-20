---
title: “快速开始:集成Dynamic Media Classic和Adobe Analytics”
description: 集成Dynamic Media Classic和Adobe Analytics的简介和快速开始，可帮助您快速入门和使用。
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Data Engineer,Administrator,Business Practitioner
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '679'
ht-degree: 45%

---


# 快速开始:集成Dynamic Media Classic和Adobe Analytics {#quick-start-integrating-dmc-analytics}

Adobe Analytics 是一款行业领先的产品，营销人员可用来评估、分析及优化整合自多个营销渠道的所有在线活动的数据。

将Adobe Analytics与Dynamic Media Classic集成后，您可以在网站上获得有关使用Dynamic Media Classic查看器的网站访客行为的报告。 例如，当网站访客在Dynamic Media经典缩放查看器中单击缩放目标时，Adobe Analytics会记录此操作。 Adobe Analytics报告可以在Dynamic Media Classic查看器中收集有关用户活动的累积信息。

通过使用 Adobe Analytics 报告，可以非常清楚地了解客户在网站上的活动。您可以确定哪些产品演示会改变客户的想法，哪些产品演示不会引起客户的兴趣。

另请参阅[在 Adobe Analytics 中测量视频](https://experienceleague.adobe.com/docs/media-analytics/using/media-overview.html)。

>[!NOTE]
>
>需要有效的Adobe Analytics帐户才能将Analytics与Dynamic Media Classic集成并生成Analytics报告。

**快速开始**

该快速入门旨在帮助您快速学会如何使用 Adobe Analytics 仪器包。

**1. 通过Dynamic Media Classic登录Adobe Analytics并下载Adobe Analytics报告变量**

>[!NOTE]
>
>在配置Adobe Analytics报表并将Adobe Analytics报表变量与Dynamic Media Classic事件匹配之前，请确认您已添加为Adobe Analytics中Web服务访问组的成员。 该组中的成员可以通过 Marketing Cloud 的 Web 服务 API 访问指定报表包中的所有报表，而无论是否在界面中设置了权限。要在组中添加成员，请在 Adobe Analytics 中单击“**管理工具**”>“**用户管理**”>“**编辑组**”。

确认您是Web服务访问组的成员后，在Dynamic Media Classic中，单击&#x200B;**设置** > **应用程序设置** > **Adobe Analytics**。 在“Adobe Analytics 配置”页中，单击“**Adobe Analytics 登录**”。

请参阅[登录到 Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics)。

在“Adobe Analytics登录”对话框中，键入您的Marketing Cloud组织ID（可选）和完整凭据，然后单击&#x200B;**登录**。 在“报告套件”下拉菜单中，选择要使用的报告套件的名称。

**2.将Adobe Analytics报表变量分配给Dynamic Media Classic查看器事件和Dynamic Media Classic变量**

在“Adobe Analytics 配置”页中，指定 Adobe Analytics 报告中所需的信息。对于每个您需要相关信息的Dynamic Media Classic查看器事件，选择Adobe Analytics变量（从您的报表包中）和Dynamic Media Classic变量。

* 查看器事件描述了要在报告中评估的用户活动。
* Dynamic Media Classic变量描述您希望报表传送的用户事件的数据。

“Adobe Analytics 配置”还提供了用于激活、编辑和删除查看器事件的工具。

在“Adobe Analytics配置”屏幕中单击“保存”后，用于测量用户活动的自定义跟踪代码将插入Dynamic Media Classic查看器中。 可以通过该功能在 Adobe Analytics 报告中跟踪用户活动。

请参阅[配置 Adobe Analytics 报告](configuring-analytics-reports.md#configuring_adobe_analytics_reports)。

**3.发布Dynamic Media Classic查看器**

发布Dynamic Media Classic查看器，以便查看器(带有用于跟踪Adobe Analytics报表中用户活动的代码)加载到Dynamic Media Classic服务器上。 在发布后，将在查看器中包含该信息，并且可用于 Adobe Analytics 分析。

请参阅[发布配置信息](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information)。

**4.将Dynamic Media Classic查看器放置到您的网站**

将包含Adobe Analytics跟踪代码的Dynamic Media Classic查看器放置到您的网站上。

**5.查看 Adobe Analytics 报告以测试 Adobe Analytics 集成**

要查看 Adobe Analytics 报告，请访问 Adobe Analytics 网站。通过“报告”页面可以查看数据及生成图形和图表，以便通过不同查看器来评估用户活动。

请参阅[查看 Adobe Analytics 报告以测试 Adobe Analytics 集成](testing-integration-viewing-analytics-report.md#testing_the_integration_by_viewing_an_adobe_analytics_report)。
