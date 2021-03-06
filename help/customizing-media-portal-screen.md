---
title: 自定义 Media Portal 屏幕
description: 了解如何在AdobeDynamic Media Classic中自定义媒体门户屏幕。
uuid: bd1a65a6-723b-49d0-8eac-849da00e0e1a
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
discoiquuid: 8b000c25-c9c3-481e-9b25-96257471571f
feature: Dynamic Media Classic,Collaboration,Asset Management
role: Admin,User
exl-id: b0c5f70a-2388-42aa-a1ed-fd745ff90518
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '346'
ht-degree: 32%

---

# 自定义 Media Portal 屏幕{#customizing-the-media-portal-screen}

通过 Media Portal 样式设置，您可以在 Media Portal 屏幕中标上您公司的徽标和颜色。使用样式设置将您的公司品牌策略放在媒体门户上。

要访问样式设置，请转到&#x200B;**[!UICONTROL 设置]** > **[!UICONTROL 媒体门户设置]** > **[!UICONTROL 样式设置]**。 确保在设置后选择&#x200B;**[!UICONTROL Save]**&#x200B;以保存设置。 您可以选择&#x200B;**[!UICONTROL Restore]**&#x200B;以恢复默认设置。 在您进行选择时，“预览”面板会显示它们的显示方式。

* **[!UICONTROL 徽标]**  — 选择 **[!UICONTROL 浏览]**，然后在“选择徽标图像”窗口中选择图形。

* **[!UICONTROL 应用]**  — 通过在“背景渐变颜色”菜单中进行选择，创建渐变颜色混合。

* **[!UICONTROL 树]**  — 选择一种变换颜色（将指针移动到项目上时显示的颜色）和选择颜色（选择项目时显示的颜色）。

* **[!UICONTROL 折叠]**  — 为“详细信息”视图屏幕右侧显示的折叠面板选择背景颜色、边框样式和滚动图像以及选定颜色。

* **[!UICONTROL 折叠项标题]**  — 选择是否在折叠项标题粗体中创建文本。

* **[!UICONTROL 数据网格]**  — 为数据网格中的标题行选择颜色。

* **[!UICONTROL 警报]**  — 为警报消息框选择背景颜色。

* **[!UICONTROL 进度栏]**  — 为栏选择指示上传和下载进度的颜色。

要使Media Portal用户能够查看您选择的样式设置，他们必须将`?company=(company name)`附加到访问Media Portal的URL后面。 例如，要查看样式设置，访问 PortalCo 公司网站 (

`https://s7sps1.scene7.com/MediaPortal`

请改用以下URL:

`https://s7sps1.scene7.com/MediaPortal?company=PortalCo`

将公司名包含在 URL 中可以使 Media Portal 识别用户要访问的公司并相应地应用该公司的样式设置。

您可以详细了解如何向 Media Portal 用户通知 URL 更改，以及如何设置欢迎电子邮件以使新用户收到正确的 Media Portal URL。

请参阅[为 Media Portal 用户设置欢迎电子邮件](adding-media-portal-users.md#setting_up_the_welcome_e_mail_message_for_media_portal_users)。
