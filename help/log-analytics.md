---
title: 登录到 Adobe Analytics
description: 了解如何从AdobeDynamic Media Classic登录Adobe Analytics。
uuid: 5614babe-1097-4228-a3dc-27e5a25366d5
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: e5b510a8-8b7f-4c60-869e-d664a8157e63
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 261b8f7c-c61c-4ce3-b9dc-8549347aca2e
source-git-commit: e3c2dcaa245e486ada62edd554db5a39d495483e
workflow-type: tm+mt
source-wordcount: '361'
ht-degree: 20%

---

# 登录到 Adobe Analytics{#log-in-to-adobe-analytics}

在登录以配置Adobe Analytics报表并匹配Adobe Analytics报表变量以AdobeDynamic Media Classic事件之前，请确认您是Adobe Analytics中Web服务访问组的成员。 无论在界面中设置何种权限，此群组中的成员都可以通过Experience Cloud的Web服务API访问指定报表包中的所有报表。 要向组添加成员，请在Adobe Analytics中，转到&#x200B;**[!UICONTROL 管理工具]** > **[!UICONTROL 用户管理]** > **[!UICONTROL 编辑组]**。

登录后，您可以选择输入Experience Cloud组织ID以使用最新的视频分析实施。 如果您选择不输入您的ID，则视频报告仍然有效。 但是，这可能会导致数据无法与外部AdobeDynamic Media Classic中该客户端的其他数据正确集成。

>[!NOTE]
>
>如果您的Adobe Analytics帐户已迁移到基于Adobe IMS的身份验证(Identity Management系统)以进行登录，则输入直接凭据将不起作用。

**登录到 Adobe Analytics:**

1. 在AdobeDynamic Media Classic页面的右上角附近，转到&#x200B;**[!UICONTROL 设置]** > **[!UICONTROL 应用程序设置]**。
1. 在左窗格的&#x200B;**[!UICONTROL 应用程序设置]**&#x200B;下，点按&#x200B;**[!UICONTROL Adobe Analytics]**。
1. 在Adobe Analytics配置页面中，点按&#x200B;**[!UICONTROL Adobe Analytics登录]**。
1. 在&#x200B;**[!UICONTROL Adobe Analytics登录]**&#x200B;对话框中，在&#x200B;**[!UICONTROL 密码]**&#x200B;文本字段中输入公司名称、Experience Cloud组织ID（可选）、用户名和&#x200B;*共享密钥*&#x200B;键。

   您可以从AnalyticsAdmin Console中检索&#x200B;*共享密钥*&#x200B;密钥。 请参阅[如何获取用户帐户的API凭据](https://github.com/AdobeDocs/analytics-2.0-apis/blob/master/create-oauth-client.md)。

1. 选择&#x200B;**[!UICONTROL 登录]**。
1. 在&#x200B;**[!UICONTROL 报表包]**&#x200B;下拉菜单中，选择一个报表包，然后选择&#x200B;**[!UICONTROL 确定]**。

   >[!NOTE]
   >
   >首次登录到 Adobe Analytics 时，“报告套件”下拉列表是空白的。首次登录时无法选择报告套件。在首次登录后，先注销，然后返回到 Adobe Analytics 屏幕。重新登录后即可选择报告套件。

>[!MORELIKETHIS]
>
>* [配置Adobe Analytics报表](configuring-analytics-reports.md#configuring_adobe_analytics_reports)

