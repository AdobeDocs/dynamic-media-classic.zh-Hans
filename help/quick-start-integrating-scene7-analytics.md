---
title: '“快速开始: 将Dynamic Media经典与AdobeAnalytics'
seo-title: '“快速开始: 将Dynamic Media经典与AdobeAnalytics'
description: 'null'
seo-description: 集成Dynamic Media经典和Adobe Analytic的简介和快速开始，帮助您快速入门和运行。
uuid: 3f9e2c91-15d4-4b53-8220-9b1ca57c0b1d
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: abec9a85-013c-4030-b129-bf27a89cb464
translation-type: tm+mt
source-git-commit: 2fb7e34b734dba1e0bd1d150580d7d6c74ee1b79
workflow-type: tm+mt
source-wordcount: '685'
ht-degree: 47%

---


# 快速开始: 将Dynamic Media经典与AdobeAnalytics集成 {#quick-start-integrating-scene-and-adobe-analytics}

Adobe Analytics 是一款行业领先的产品，营销人员可用来评估、分析及优化整合自多个营销渠道的所有在线活动的数据。

在将AdobeAnalytics与Scene7 Publishing System集成之后，您可以在网站上获取有关使用Dynamic Media经典查看器的网站访客行为的报告。 例如，当网站访客在Dynamic Media经典缩放查看器中单击缩放目标时，AdobeAnalytics会记录此操作。 AdobeAnalytics报告可以收集Dynamic Media经典查看器中有关用户活动的累积信息。

通过使用 Adobe Analytics 报告，可以非常清楚地了解客户在网站上的活动。您可以确定哪些产品演示会改变客户的想法，哪些产品演示不会引起客户的兴趣。

另请参阅[在 Adobe Analytics 中测量视频](https://docs.adobe.com/content/help/en/media-analytics/using/media-overview.html)。

>[!NOTE]
>
>要将 Adobe Analytics 与 Scene7 Publishing System 集成在一起并生成 Analytics 报告，需要使用有效的 Analytics 帐户。

**快速开始**

该快速入门旨在帮助您快速学会如何使用 Adobe Analytics 仪器包。

**1. Log in to Adobe Analytics by way of Dynamic Media Classic and download Adobe Analytics report variables**

>[!NOTE]
>
>在配置AdobeAnalytics报告并将AdobeAnalytics报告变量与Dynamic Media经典事件匹配之前，请先验证您已添加为AdobeAnalytics的Web服务访问组的成员。 该组中的成员可以通过 Marketing Cloud 的 Web 服务 API 访问指定报表包中的所有报表，而无论是否在界面中设置了权限。要在组中添加成员，请在 Adobe Analytics 中单击“**管理工具**”>“**用户管理**”>“**编辑组**”。

After you have verified that you are a member of the Web Service Access group, in Dynamic Media Classic, click **Setup** > **Application Setup** > **Adobe Analytics**. 在“Adobe Analytics 配置”页中，单击“**Adobe Analytics 登录**”。

请参阅[登录到 Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics)。

在AdobeAnalytics登录对话框中，键入您的Marketing Cloud组织ID（可选）和完整凭据，然后单击登 **录**。 在“报告套件”下拉菜单中，选择要使用的报告套件的名称。

**2. 将AdobeAnalytics报表变量分配给Dynamic Media经典查看器事件和Dynamic Media经典变量**

在“Adobe Analytics 配置”页中，指定 Adobe Analytics 报告中所需的信息。对于每个您想要相关信息的Dynamic Media经典查看器事件，选择AdobeAnalytics变量（从您的报表包中）和Dynamic Media经典变量。

* 查看器事件描述了要在报告中评估的用户活动。
* Dynamic Media经典变量描述您希望报表传送的用户事件的相关数据。

“Adobe Analytics 配置”还提供了用于激活、编辑和删除查看器事件的工具。

在AdobeAnalytics配置屏幕中单击“保存”后，将在Dynamic Media经典查看器中插入用于测量用户活动的自定义跟踪代码。 可以通过该功能在 Adobe Analytics 报告中跟踪用户活动。

请参阅[配置 Adobe Analytics 报告](configuring-analytics-reports.md#configuring_adobe_analytics_reports)。

**3. 发布Dynamic Media经典查看器**

发布Dynamic Media经典查看器，以便查看器(带有用于跟踪AdobeAnalytics报告中的用户活动的代码)加载到Dynamic Media经典服务器上。 在发布后，将在查看器中包含该信息，并且可用于 Adobe Analytics 分析。

请参阅[发布配置信息](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information)。

**4. 将Dynamic Media经典查看器放置到您的网站中**

将Dynamic Media经典查看器与AdobeAnalytics跟踪代码放在您的网站上。

**5. 查看 Adobe Analytics 报告以测试 Adobe Analytics 集成**

要查看 Adobe Analytics 报告，请访问 Adobe Analytics 网站。通过“报告”页面可以查看数据及生成图形和图表，以便通过不同查看器来评估用户活动。

请参阅[查看 Adobe Analytics 报告以测试 Adobe Analytics 集成](testing-integration-viewing-analytics-report.md#testing_the_integration_by_viewing_an_adobe_analytics_report)。
