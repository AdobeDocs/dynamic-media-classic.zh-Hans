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
source-git-commit: d18dbbf89a1bfe4df46cbe7d56cdf6f442595ddb
workflow-type: tm+mt
source-wordcount: '762'
ht-degree: 1%

---

# 登录到 Adobe Analytics{#log-in-to-adobe-analytics}

在登录以配置Adobe Analytics报表并匹配Adobe Analytics报表变量以AdobeDynamic Media Classic事件之前，请确认您是Adobe Analytics中Web服务访问组的成员。 无论在界面中设置何种权限，此群组中的成员都可以通过Experience Cloud的Web服务API访问指定报表包中的所有报表。 要向组添加成员，请在Adobe Analytics中，转到&#x200B;**[!UICONTROL 管理工具]** > **[!UICONTROL 用户管理]** > **[!UICONTROL 编辑组]**。

登录后，您可以选择输入Experience Cloud组织ID以使用最新的视频分析实施。 如果您选择不输入您的ID，则视频报告仍然有效。 但是，这可能会导致数据无法与外部AdobeDynamic Media Classic中该客户端的其他数据正确集成。

>[!NOTE]
>
>如果您的Adobe Analytics帐户已迁移到基于Adobe IMS的身份验证(Identity Management系统)以进行登录，则输入直接凭据将不起作用。

**要从Adobe Dynamic Media Classic登录Adobe Analytics，请执行以下操作：**

首先，将Dynamic Media Classic与Adobe Analytics OAuth集成。 Adobe Analytics OAuth与Dynamic Media Classic的集成通常仅针对每个用户完成一次。

1. 访问[Adobe开发人员控制台](https://developer.adobe.com/console)。 确保您的帐户拥有需要集成的组织的管理员权限。
1. 在主页的右上角附近，从下拉列表中，选择相应的公司。 (以下屏幕截图仅供参考；您选择的实际公司名称可能会有所不同。)

   ![创建新项目](assets/analytics-oauth1.png)

1. 执行以下任一操作：

   * 在页面顶部的&#x200B;**[!UICONTROL Home]**&#x200B;选项卡中，选择&#x200B;**[!UICONTROL 新建项目]**。
   * 在页面顶部的&#x200B;**[!UICONTROL 项目]**&#x200B;选项卡中。 在页面的右角附近，选择&#x200B;**[!UICONTROL 新建项目]**。

1. 在项目的页面上，选择&#x200B;**[!UICONTROL 添加API]**。
1. 在&#x200B;**[!UICONTROL 添加API]**&#x200B;页面上，选择&#x200B;**[!UICONTROL Adobe Analytics]**。
1. 在页面的右下角附近，选择&#x200B;**[!UICONTROL Next]**。

   ![添加API](assets/analytics-oauth2.png)

1. 在&#x200B;**[!UICONTROL 配置API]**&#x200B;页面上，选择&#x200B;**[!UICONTROL 用户身份验证OAuth]**。
1. 在页面的右下角附近，选择&#x200B;**[!UICONTROL Next]**。
1. 在&#x200B;**[!UICONTROL 配置API]**&#x200B;页面上，选择&#x200B;**[!UICONTROL OAUTH 2.0 Web]**。
1. 在&#x200B;**[!UICONTROL 默认重定向URI]**&#x200B;文本字段中，完全按照所示输入以下路径：

   `https://exploreadobe.com/dynamic-media-upgrade/`

1. 在&#x200B;**[!UICONTROL 重定向URI模式]**&#x200B;文本字段中，完全按照所示输入以下路径：

   `https://exploreadobe\.com/dynamic-media-upgrade/`

1. 在页面的右下角，选择&#x200B;**[!UICONTROL 保存配置的API]**。
1. 在导航面板的Adobe Analytics页面左侧的&#x200B;**[!UICONTROL 凭据]**&#x200B;下，选择&#x200B;**[!UICONTROL OAuth Web]**。
1. 在&#x200B;**[!UICONTROL 凭据详细信息]**&#x200B;下，执行以下操作：
   * 在&#x200B;**[!UICONTROL 客户端ID]**&#x200B;下，选择&#x200B;**[!UICONTROL 复制]**&#x200B;以复制值。 在Dynamic Media Classic桌面应用程序中，后续的Analytics配置需要此值。
   * 在&#x200B;**[!UICONTROL 客户端密钥]**&#x200B;下，选择&#x200B;**[!UICONTROL 检索客户端密钥]**&#x200B;以显示关联的值。 选择&#x200B;**[!UICONTROL Copy]**&#x200B;以复制值。 在Dynamic Media Classic桌面应用程序中，后续的Adobe Analytics配置需要此值。

**在Dynamic Media Classic桌面应用程序中配置Adobe Analytics**

>[!NOTE]
>
>在Dynamic Media Classic中初始配置Adobe Analytics后，您唯一必须重做配置的时间如下：
>
>* Analytics中会添加一个新报表，用户希望开始向该新报表发送数据。
>* 跟踪服务器已在Adobe Analytics中更新。
>* 报表中引入了新的跟踪变量，您希望将Dynamic Media Classic用户界面中的特定查看器变量链接到该新的Analytics变量。

>


1. 在AdobeDynamic Media Classic桌面应用程序的右上角附近，转到&#x200B;**[!UICONTROL 设置]** > **[!UICONTROL 应用程序设置]**。
1. 在左侧面板的&#x200B;**[!UICONTROL 应用程序设置]**&#x200B;下，选择&#x200B;**[!UICONTROL Adobe Analytics]**。
1. 在&#x200B;**[!UICONTROL Adobe Analytics配置]**&#x200B;页面上，选择&#x200B;**[!UICONTROL Adobe Analytics登录]**。
1. 在&#x200B;**[!UICONTROL Adobe Analytics登录]**&#x200B;对话框的客户端ID字段和客户端密钥字段中，粘贴您之前复制的各个值。
1. 执行IMS登录。

   成功登录后，将显示由可供您使用的公司启动的&#x200B;**[!UICONTROL 公司]**&#x200B;下拉列表。

1. 从&#x200B;**[!UICONTROL 公司]**&#x200B;下拉列表中，选择公司。

   选择公司后，将显示由选定公司可用的报表包启动的&#x200B;**[!UICONTROL SUITES]**&#x200B;下拉列表。

1. 从&#x200B;**[!UICONTROL SUITES]**&#x200B;下拉列表中，选择一个报表包。

   >[!NOTE]
   >
   >默认情况下，用户必须了解以下事实： **[!UICONTROL COMPANIES]**&#x200B;和&#x200B;**[!UICONTROL SUITES]**&#x200B;下拉列表都为空。 因此，用户必须从每个列表中选择一个值。—>

1. 选择&#x200B;**[!UICONTROL OK]**&#x200B;以保存配置。

>[!MORELIKETHIS]
>
>* [配置Adobe Analytics报表](configuring-analytics-reports.md#configuring_adobe_analytics_reports)

