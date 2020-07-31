---
title: 登录到 Adobe Analytics
seo-title: 登录到 Adobe Analytics
description: 'null'
seo-description: 了解如何登录Adobe Analytics。
uuid: 5614babe-1097-4228-a3dc-27e5a25366d5
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: e5b510a8-8b7f-4c60-869e-d664a8157e63
translation-type: tm+mt
source-git-commit: ff112497b41f71b77f4afa47d331a1a9bc1e2d07
workflow-type: tm+mt
source-wordcount: '357'
ht-degree: 37%

---


# 登录到 Adobe Analytics{#log-in-to-adobe-analytics}

在登录以配置Adobe Analytics报告并将Adobe Analytics报告变量与Dynamic Media经典事件匹配之前，请验证您是否已添加为Adobe AnalyticsWeb服务访问组的成员。 该组中的成员可以通过 Marketing Cloud 的 Web 服务 API 访问指定报表包中的所有报表，而无论是否在界面中设置了权限。要在组中添加成员，请在 Adobe Analytics 中单击“**管理工具**”>“**用户管理**”>“**编辑组**”。

登录后，您可以选择输入Marketing Cloud组织ID以使用最新的视频分析实施。 如果您选择不输入ID，视频报告仍然有效。 但是，它可能导致数据无法与来自外部Dynamic Media经典的该客户端的其他数据正确集成。

>[!NOTE]
>
>如果您的Adobe Analytics帐户已迁移到Adobe基于IMS的身份验证(Identity Management系统)进行登录，则输入直接凭据将不起作用。

**登录到 Adobe Analytics**

1. 在Dynamic Media经典页面的右上角附近，点按设置>应 **[!UICONTROL 用程序设置]**。
1. In the left pane, under **[!UICONTROL Application Setup]**, tap **[!UICONTROL Adobe Analytics]**.
1. In the Adobe Analytics Configuration page, tap **[!UICONTROL Adobe Analytics Login]**.
1. 在“Adobe Analytics **[!UICONTROL 登录名]** ”对话框中，在“密码”文本字段中输入您的公司名、Marketing Cloud组织ID（可选）、 *用户名和密码* 密钥 **** 。

   您可以从Analytics *管理员* 控制台检索共享密钥。 请参 [阅如何获取用户帐户的API凭据](https://helpx.adobe.com/analytics/kb/how-to-get-api-credentials-for-user-accounts-.html)。

1. 按一下&#x200B;**[!UICONTROL 登入]**。
1. 在“报 **[!UICONTROL 表包]** ”下拉菜单中，选择一个报表包，然后单击 **[!UICONTROL 确定]**。

   >[!NOTE]
   >
   >首次登录到 Adobe Analytics 时，“报告套件”下拉列表是空白的。首次登录时无法选择报告套件。在首次登录后，先注销，然后返回到 Adobe Analytics 屏幕。重新登录后即可选择报告套件。

>[!MORELIKETHIS]
>
>* [配置 Adobe Analytics 报告](configuring-analytics-reports.md#configuring_adobe_analytics_reports)

