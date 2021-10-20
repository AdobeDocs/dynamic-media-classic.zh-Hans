---
title: 登录到 Adobe Analytics
description: 了解如何从Adobe Dynamic Media Classic登录Adobe Analytics。
uuid: 5614babe-1097-4228-a3dc-27e5a25366d5
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: e5b510a8-8b7f-4c60-869e-d664a8157e63
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 261b8f7c-c61c-4ce3-b9dc-8549347aca2e
source-git-commit: 876b4c61167b28f7d5e50a656564eafcbe5b9eab
workflow-type: tm+mt
source-wordcount: '845'
ht-degree: 1%

---

# 登录到 Adobe Analytics{#log-in-to-adobe-analytics}

在登录以配置Adobe Analytics报表并将Adobe Analytics报表变量与Adobe Dynamic Media Classic事件匹配之前，请确认您是Adobe Analytics中“Web服务访问”组的成员。 无论在界面中设置何种权限，此群组中的成员都可以通过Experience Cloud的Web服务API访问指定报表包中的所有报表。 要向组添加成员，请在Adobe Analytics中，转到 **[!UICONTROL 管理工具]** > **[!UICONTROL 用户管理]** > **[!UICONTROL 编辑群组]**.

登录后，您可以选择输入Experience Cloud组织ID以使用最新的视频分析实施。 如果您选择不输入您的ID，则视频报告仍然有效。 但是，这可能会导致数据无法与来自Adobe Dynamic Media Classic外部的该客户端的其他数据正确集成。

>[!NOTE]
>
>如果您的Adobe Analytics帐户已迁移到基于Adobe IMS的身份验证(Identity Management系统)以进行登录，则输入直接凭据将不起作用。

**要从Adobe Dynamic Media Classic登录Adobe Analytics，请执行以下操作：**

首先，将Dynamic Media Classic与Adobe Analytics OAuth集成。 Adobe Analytics OAuth与Dynamic Media Classic的集成通常仅针对每个用户完成一次。

1. 访问 [Adobe开发人员控制台](https://developer.adobe.com/console). 确保您的帐户拥有需要集成的组织的管理员权限。
1. 在主页的右上角附近，从下拉列表中，选择相应的公司。 (以下屏幕截图仅供参考；您选择的实际公司名称可能会有所不同。)

   ![创建新项目](assets/analytics-oauth1.png)

1. 执行以下任一操作：

   * 在页面顶部，从 **[!UICONTROL 主页]** 选项卡，选择 **[!UICONTROL 创建新项目]**.
   * 在页面顶部，从 **[!UICONTROL 项目]** 选项卡。 在页面的右角附近，选择 **[!UICONTROL 创建新项目]**.

1. 在项目的页面上，选择 **[!UICONTROL 添加API]**.
1. 在 **[!UICONTROL 添加API]** 页面，选择 **[!UICONTROL Adobe Analytics]**.
1. 在页面的右下角附近，选择 **[!UICONTROL 下一个]**.

   ![添加API](assets/analytics-oauth2.png)

1. 在 **[!UICONTROL 配置API]** 页面，选择 **[!UICONTROL 用户身份验证OAuth]**.
1. 在页面的右下角附近，选择 **[!UICONTROL 下一个]**.
1. 在 **[!UICONTROL 配置API]** 页面，选择 **[!UICONTROL OAUTH 2.0 Web]**.
1. 在 **[!UICONTROL 默认重定向URI]** 文本字段中，请完全按照所示输入以下路径：

   `https://exploreadobe.com/dynamic-media-upgrade/`

1. 在 **[!UICONTROL 重定向URI模式]** 文本字段中，请完全按照所示输入以下路径：

   `https://exploreadobe\.com/dynamic-media-upgrade/`

1. 在页面的右下角，选择 **[!UICONTROL 保存配置的API]**.
1. 在导航面板中，Adobe Analytics页面左侧的 **[!UICONTROL 凭据]**，选择 **[!UICONTROL OAuth Web]**.
1. 在 **[!UICONTROL 凭据详细信息]**，请执行以下操作：
   * 在 **[!UICONTROL 客户端ID]**，选择 **[!UICONTROL 复制]** 以复制值。 在Dynamic Media Classic桌面应用程序中，后续的Analytics配置需要此值。
   * 在 **[!UICONTROL 客户端密钥]**，选择 **[!UICONTROL 检索客户端密钥]** 以显示关联的值。 选择 **[!UICONTROL 复制]** 以复制值。 在Dynamic Media Classic桌面应用程序中，后续的Adobe Analytics配置需要此值。

**在Dynamic Media Classic桌面应用程序中配置Adobe Analytics**

>[!NOTE]
>
>在Dynamic Media Classic中初始配置Adobe Analytics后，您只有在以下情况中必须重做配置：
>
>* Analytics中会添加一个新报表，用户希望开始向该新报表发送数据。
>* 跟踪服务器已在Adobe Analytics中更新。
>* 报表中引入了新的跟踪变量，您希望将Dynamic Media Classic用户界面中的特定查看器变量链接到该新的Analytics变量。

>


1. 在Adobe Dynamic Media Classic桌面应用程序的右上角附近，转到 **[!UICONTROL 设置]** > **[!UICONTROL 应用程序设置]**.
1. 在左侧面板中，在 **[!UICONTROL 应用程序设置]**，选择 **[!UICONTROL Adobe Analytics]**.
1. 在 **[!UICONTROL Adobe Analytics配置]** 页面，选择 **[!UICONTROL Adobe Analytics登录]**.
1. 在 **[!UICONTROL Adobe Analytics登录]** 对话框中 **[!UICONTROL 客户端ID]** 字段和 **[!UICONTROL 客户端密钥]** 字段，请粘贴您之前复制的各个值。
1. 在对话框的右下角，选择“登录”并执行Adobe IMS(Identity Management服务)登录。

   成功登录后，将再次显示Adobe Analytics登录对话框以及 **[!UICONTROL 公司]** 下拉列表，由可供您使用的公司发起。

1. 从 **[!UICONTROL 公司]** 下拉列表中，选择公司。

   选择公司后， **[!UICONTROL SUITES]** 下拉列表（由选定公司可用的报表包启动）将变为可见。

1. 从 **[!UICONTROL SUITES]** 下拉列表中，选择一个报表包。

   >[!NOTE]
   >
   >默认情况下，用户必须意识到 **[!UICONTROL 公司]** 和 **[!UICONTROL SUITES]** 下拉列表为空。 因此，用户必须从每个列表中选择一个值。

1. 选择 **[!UICONTROL 确定]** 以便保存配置。

   >[!NOTE]
   >
   >的 **[!UICONTROL Adobe Analytics Server]** 字段会填充一个建议的第三方跟踪服务器，该服务器在您选择 **[!UICONTROL 确定]**. 如果您使用其他跟踪服务器，请在此字段中更新它以避免数据丢失。

1. 在Adobe Analytics配置页面的左下角，选择 **[!UICONTROL 保存]** 以确保更新Adobe Analytics帐户配置。

>[!MORELIKETHIS]
>
>* [配置Adobe Analytics报表](configuring-analytics-reports.md#configuring_adobe_analytics_reports)

