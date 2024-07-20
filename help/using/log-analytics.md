---
title: 登录到Adobe Analytics
description: 了解如何从Adobe Dynamic Media Classic登录到Adobe Analytics。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 261b8f7c-c61c-4ce3-b9dc-8549347aca2e
topic: Integrations, Development
level: Experienced
source-git-commit: de6997fda88c4471625242ee9cca59b344cee945
workflow-type: tm+mt
source-wordcount: '847'
ht-degree: 0%

---

# 登录到Adobe Analytics{#log-in-to-adobe-analytics}

验证您是否是Adobe Analytics中的Web服务访问组的成员。 请在登录以配置Adobe Analytics报表并将Adobe Analytics报表变量与Adobe Dynamic Media Classic事件匹配之前执行此操作。 此组中的成员可以访问指定报表包中的所有报表。 无论界面中设置的权限如何，都使用Experience Cloud的Web服务API来执行此操作。 若要向组添加成员，请在Adobe Analytics中转到&#x200B;**[!UICONTROL 管理工具]** > **[!UICONTROL 用户管理]** > **[!UICONTROL 编辑组]**。

登录时，您可以选择输入Experience Cloud组织ID以使用最新的视频分析实施。 如果您选择不输入ID，则视频报表仍可正常工作。 但是，它可能会导致数据无法与Adobe Dynamic Media Classic外部适用于该客户端的其他数据正确集成。

>[!NOTE]
>
>如果您的Adobe Analytics帐户已迁移到基于Adobe IMS的身份验证(Identity Management System)以进行登录，则无法输入直接凭据。

## 从Adobe Dynamic Media Classic登录到Adobe Analytics {#log-in-to-analytics-from-dmc}

首先，将Dynamic Media Classic与Adobe Analytics OAuth集成。 Adobe Analytics OAuth与Dynamic Media Classic的集成通常每个用户只执行一次。

1. 访问[Adobe Developer Console](https://developer.adobe.com/console)。 确保您的帐户对需要集成的组织具有管理员权限。
1. 在主页右上角附近，从下拉列表中选择相应的公司。 （下面的屏幕截图仅供参考；您选择的实际公司名称可能会有所不同。）

   ![创建新项目](assets/analytics-oauth1.png)

1. 执行以下任一操作：

   * 在页面顶部，从&#x200B;**[!UICONTROL 主页]**&#x200B;选项卡中选择&#x200B;**[!UICONTROL 创建新项目]**。
   * 在页面顶部的&#x200B;**[!UICONTROL 项目]**&#x200B;选项卡中。 在页面的右角附近，选择&#x200B;**[!UICONTROL 创建新项目]**。

1. 在项目的页面上，选择&#x200B;**[!UICONTROL 添加API]**。
1. 在&#x200B;**[!UICONTROL 添加API]**&#x200B;页面上，选择&#x200B;**[!UICONTROL Adobe Analytics]**。
1. 在页面的右下角附近，选择&#x200B;**[!UICONTROL 下一步]**。

   ![添加API](assets/analytics-oauth2.png)

1. 在&#x200B;**[!UICONTROL `Configure API`]**&#x200B;页面上，选择&#x200B;**[!UICONTROL 用户身份验证OAuth]**。
1. 在页面的右下角附近，选择&#x200B;**[!UICONTROL 下一步]**。
1. 在&#x200B;**[!UICONTROL `Configure API`]**&#x200B;页面上，选择&#x200B;**[!UICONTROL OAUTH 2.0 Web]**。
1. 在&#x200B;**[!UICONTROL 默认重定向URI]**&#x200B;文本字段中，完全按照所示输入以下路径：

   `https://exploreadobe.com/dynamic-media-upgrade/`

1. 在&#x200B;**[!UICONTROL 重定向URI模式]**&#x200B;文本字段中，完全按照所示输入以下路径：

   `https://exploreadobe\.com/dynamic-media-upgrade/`

1. 在页面的右下角，选择&#x200B;**[!UICONTROL 保存配置的API]**。
1. 在Adobe Analytics页面左侧的导航面板中，在&#x200B;**[!UICONTROL 凭据]**&#x200B;下，选择&#x200B;**[!UICONTROL OAuth Web]**。
1. 在&#x200B;**[!UICONTROL 凭据详细信息]**&#x200B;下，执行以下操作：
   * 在&#x200B;**[!UICONTROL 客户端ID]**&#x200B;下，选择&#x200B;**[!UICONTROL 复制]**&#x200B;以复制值。 您需要此值才能在随后的Dynamic Media Classic桌面应用程序中进行后续Analytics配置。
   * 在&#x200B;**[!UICONTROL 客户端密钥]**&#x200B;下，选择&#x200B;**[!UICONTROL 检索客户端密钥]**&#x200B;以显示关联的值。 选择&#x200B;**[!UICONTROL 复制]**&#x200B;以复制值。 您需要此值才能在随后的Dynamic Media Classic桌面应用程序中进行后续的Adobe Analytics配置。

## 在Adobe Dynamic Media Classic中配置Adobe Analytics {#configure-analytics-in-dmc}

>[!NOTE]
>
>在Dynamic Media Classic中对Adobe Analytics进行初始配置后，只有在以下情况下才必须重做配置：
>
>* 在Analytics中添加了一个新报表，用户希望开始向该新报表发送数据。
>* Adobe Analytics中更新了跟踪服务器。
>* 报表中引入了一个新的跟踪变量，您希望将Dynamic Media Classic用户界面中的特定查看器变量链接到这个新的Analytics变量。
>

1. 在Adobe Dynamic Media Classic桌面应用程序的右上角附近，转到&#x200B;**[!UICONTROL 设置]** > **[!UICONTROL 应用程序设置]**。
1. 在左侧面板的&#x200B;**[!UICONTROL 应用程序设置]**&#x200B;下，选择&#x200B;**[!UICONTROL Adobe Analytics]**。
1. 在&#x200B;**[!UICONTROL Adobe Analytics配置]**&#x200B;页面上，选择&#x200B;**[!UICONTROL Adobe Analytics登录]**。
1. 在&#x200B;**[!UICONTROL Adobe Analytics登录]**&#x200B;对话框的&#x200B;**[!UICONTROL 客户端ID]**&#x200B;字段和&#x200B;**[!UICONTROL 客户端密钥]**&#x200B;字段中，粘贴您之前复制的相应值。
1. 在对话框的右下角，选择&#x200B;**[!UICONTROL 登录]**&#x200B;并执行Adobe IMS (Identity Management服务)登录。

   成功登录后，“Adobe Analytics登录”对话框将再次与&#x200B;**[!UICONTROL 公司]**&#x200B;下拉列表一起显示，下拉列表由您可用的公司启动。

1. 从&#x200B;**[!UICONTROL 公司]**&#x200B;下拉列表中选择公司。

   选择公司后，由选定公司可用的报表包启动的&#x200B;**[!UICONTROL 报表包]**&#x200B;下拉列表将变得可见。

1. 从&#x200B;**[!UICONTROL SUITES]**&#x200B;下拉列表中选择一个报表包。

   >[!NOTE]
   >
   >默认情况下，用户必须了解&#x200B;**[!UICONTROL COMPANIES]**&#x200B;和&#x200B;**[!UICONTROL SUITES]**&#x200B;下拉列表都是空的。 因此，用户必须从每个列表中选择一个值。

1. 选择&#x200B;**[!UICONTROL 确定]**，以便保存配置。

   >[!NOTE]
   >
   >**[!UICONTROL Adobe Analytics Server]**&#x200B;字段由建议的第三方跟踪服务器填充，当您选择&#x200B;**[!UICONTROL 确定]**&#x200B;时，该服务器与您的Analytics命名空间相匹配。 如果您使用其他跟踪服务器，请在此字段中更新它以避免数据丢失。

1. 在“Adobe Analytics配置”页面的左下角，选择&#x200B;**[!UICONTROL 保存]**&#x200B;以确保更新您的Adobe Analytics帐户配置。

>[!MORELIKETHIS]
>
>* [配置Adobe Analytics报表](configuring-analytics-reports.md#configuring_adobe_analytics_reports)
