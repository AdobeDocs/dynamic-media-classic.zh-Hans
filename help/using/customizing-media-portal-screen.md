---
title: 自定义 Media Portal 屏幕
description: 了解如何在Adobe Dynamic Media Classic中自定义Media Portal屏幕。
uuid: bd1a65a6-723b-49d0-8eac-849da00e0e1a
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
discoiquuid: 8b000c25-c9c3-481e-9b25-96257471571f
feature: Dynamic Media Classic,Collaboration,Asset Management
role: Admin,User
exl-id: b0c5f70a-2388-42aa-a1ed-fd745ff90518
source-git-commit: 65e3b69bdcbd651a5f9ab100592217e61a8c05ef
workflow-type: tm+mt
source-wordcount: '346'
ht-degree: 32%

---

# 自定义 Media Portal 屏幕{#customizing-the-media-portal-screen}

通过 Media Portal 样式设置，您可以在 Media Portal 屏幕中标上您公司的徽标和颜色。使用样式设置将您的公司品牌置于Media Portal上。

要访问样式设置，请转到 **[!UICONTROL 设置]** > **[!UICONTROL Media Portal设置]** > **[!UICONTROL 样式设置]**. 确保选择 **[!UICONTROL 保存]** 以便在设置完成后保存设置。 您可以选择 **[!UICONTROL 恢复]** 以恢复默认设置。 当您做出选择时，“预览”面板会显示它们的显示方式。

* **[!UICONTROL 徽标]**  — 选择 **[!UICONTROL 浏览]**，然后在选择徽标图像窗口中选择图形。

* **[!UICONTROL 应用程序]**  — 通过在“背景渐变颜色”菜单中进行选择来创建渐变颜色混合。

* **[!UICONTROL 树]**  — 选择变换颜色（将指针移动到项目上时显示的颜色）和选择颜色（选择项目时显示的颜色）。

* **[!UICONTROL 可折叠项]**  — 为在“详细信息”视图中屏幕右侧显示的折叠选择背景颜色、边框样式以及变换颜色和所选颜色。

* **[!UICONTROL Accordion标题]**  — 选择是否在可折叠项标题粗体中显示文本。

* **[!UICONTROL 数据网格]**  — 选择数据网格中标题行的颜色。

* **[!UICONTROL 警报]**  — 选择警报消息框的背景颜色。

* **[!UICONTROL 进度条]**  — 为指示上传和下载进度的条形选择颜色。

要让Media Portal用户查看您选择的样式设置，他们必须附加 `?company=(company name)` 访问他们访问Media Portal的URL。 例如，要查看样式设置，访问 PortalCo 公司网站 (

`https://s7sps1.scene7.com/MediaPortal`

请改用以下URL：

`https://s7sps1.scene7.com/MediaPortal?company=PortalCo`

将公司名包含在 URL 中可以使 Media Portal 识别用户要访问的公司并相应地应用该公司的样式设置。

您可以详细了解如何向 Media Portal 用户通知 URL 更改，以及如何设置欢迎电子邮件以使新用户收到正确的 Media Portal URL。

请参阅[为 Media Portal 用户设置欢迎电子邮件](adding-media-portal-users.md#setting_up_the_welcome_e_mail_message_for_media_portal_users)。
