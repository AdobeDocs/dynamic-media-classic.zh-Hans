---
title: 自定义Media Portal屏幕
description: 了解如何在Adobe Dynamic Media Classic中自定义Media Portal屏幕。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
feature: Dynamic Media Classic,Collaboration,Asset Management
role: Admin,User
exl-id: b0c5f70a-2388-42aa-a1ed-fd745ff90518
topic: Collaboration, Content Management
level: Intermediate
source-git-commit: 00591bdbe721035e25d3dea245a2110f978d19aa
workflow-type: tm+mt
source-wordcount: '327'
ht-degree: 17%

---

# 自定义Media Portal屏幕{#customizing-the-media-portal-screen}

通过 Media Portal 样式设置，您可以在 Media Portal 屏幕中标上您公司的徽标和颜色。使用样式设置将您的公司品牌置于Media Portal上。

若要访问样式设置，请转到&#x200B;**[!UICONTROL 设置]** > **[!UICONTROL Media Portal设置]** > **[!UICONTROL 样式设置]**。 请确保选择&#x200B;**[!UICONTROL 保存]**&#x200B;以在设置完成后保存设置。 您可以选择&#x200B;**[!UICONTROL 还原]**&#x200B;以恢复默认设置。 当您做出选择时，“预览”面板会显示它们的显示方式。

* **[!UICONTROL 徽标]**：选择&#x200B;**[!UICONTROL 浏览]**，然后在“选择徽标图像”窗口中选择图形。

* **[!UICONTROL 应用程序]**：通过在“背景渐变颜色”的菜单上进行选择来创建渐变颜色混合。

* **[!UICONTROL 树]**：选择变换颜色和选择颜色。

* **[!UICONTROL 可折叠项]**：选择背景颜色、边框样式以及鼠标指针和所选颜色，这些颜色将显示在“详细信息”视图屏幕右侧的可折叠项。

* **[!UICONTROL 可折叠项标题]**：选择是否在可折叠项标题粗体中显示文本。

* **[!UICONTROL 数据网格]**：为数据网格中的标题行选择颜色。

* **[!UICONTROL 警报]**：选择警报消息框的背景颜色。

* **[!UICONTROL 进度条]**：为指示上载和下载进度的进度条选择一种颜色。

要让Media Portal用户查看您选择的样式设置，他们必须在访问Media Portal的URL中附加`?company=(company name)`。 例如，要查看样式设置，请访问PortalCo公司的Media Portal用户：

`https://s7sps1.scene7.com/MediaPortal`

请改用以下URL：

`https://s7sps1.scene7.com/MediaPortal?company=PortalCo`

通过在URL中包含公司名称，Media Portal可以识别用户希望访问的公司并相应地应用公司的样式设置。

您可以详细了解如何向 Media Portal 用户通知 URL 更改，以及如何设置欢迎电子邮件以使新用户收到正确的 Media Portal URL。

请参阅[为 Media Portal 用户设置欢迎电子邮件](adding-media-portal-users.md#setting_up_the_welcome_e_mail_message_for_media_portal_users)。
