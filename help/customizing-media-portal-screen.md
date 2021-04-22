---
title: 自定义 Media Portal 屏幕
description: 了解如何自定义Media Portal屏幕。
uuid: bd1a65a6-723b-49d0-8eac-849da00e0e1a
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
discoiquuid: 8b000c25-c9c3-481e-9b25-96257471571f
feature: Dynamic Media Classic，协作，资产管理
role: Administrator,Business Practitioner
exl-id: b0c5f70a-2388-42aa-a1ed-fd745ff90518
translation-type: tm+mt
source-git-commit: 4e79c98b92dfa4e1a9890ed8a291cdf564126466
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 46%

---

# 自定义 Media Portal 屏幕{#customizing-the-media-portal-screen}

通过 Media Portal 样式设置，您可以在 Media Portal 屏幕中标上您公司的徽标和颜色。使用样式设置将您的公司品牌放在Media Portal上。

要访问样式设置，请选择“**[!UICONTROL 设置]**”>“**[!UICONTROL Media Portal 设置]**”>“**[!UICONTROL 样式设置]**”。设置后请确保单击“**[!UICONTROL 保存]**”以保存设置。您可以单击“**[!UICONTROL 还原]**”恢复默认设置。当您做出选择时，“预览”面板会向您显示您选择的样式。

* **徽标**  — 单击“ **** 浏览”，然后在“选择徽标图像”窗口中选择图形。

* **应用**  — 通过在“背景渐变颜色”菜单上进行选择，创建渐变颜色混合。

* **树**  — 选择一种变换颜色（将指针移到项目上时显示的颜色）和一种选择颜色（选择项目时显示的颜色）。

* **折叠**  — 为显示在屏幕右侧的折叠面板选择背景颜色、边框样式、变换颜色和选定颜色(在“详细信息”视图中)。

* **Accordion Header**  — 选择是否将accordion头中的文本设置为粗体。

* **Datagrid**  — 为数据网格中的标题行选择颜色。

* **警报**  — 为警报消息框选择背景颜色。

* **进度栏**  — 为栏选择指示上载和下载进度的颜色。

要使Media Portal用户查看您选择的样式设置，他们必须将`?company=(company name)`附加到访问Media Portal的URL。 例如，要查看样式设置，访问 PortalCo 公司网站 (

`https://s7sps1.scene7.com/MediaPortal`

请改用以下URL:

`https://s7sps1.scene7.com/MediaPortal?company=PortalCo`

将公司名包含在 URL 中可以使 Media Portal 识别用户要访问的公司并相应地应用该公司的样式设置。

您可以详细了解如何向 Media Portal 用户通知 URL 更改，以及如何设置欢迎电子邮件以使新用户收到正确的 Media Portal URL。

请参阅[为 Media Portal 用户设置欢迎电子邮件](adding-media-portal-users.md#setting_up_the_welcome_e_mail_message_for_media_portal_users)。
