---
title: 自定义 Media Portal 屏幕
description: 了解如何自定义媒体门户屏幕。
uuid: bd1a65a6-723b-49d0-8eac-849da00e0e1a
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
discoiquuid: 8b000c25-c9c3-481e-9b25-96257471571f
translation-type: tm+mt
source-git-commit: ca12c96d3a76cfa52fd930d190476cb6fc4f4ac7
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 52%

---


# 自定义 Media Portal 屏幕{#customizing-the-media-portal-screen}

通过 Media Portal 样式设置，您可以在 Media Portal 屏幕中标上您公司的徽标和颜色。使用样式设置将您公司的图章放在 Media Portal 上。

要访问样式设置，请选择“**设置**”>“**Media Portal 设置**”>“**样式设置**”。设置后请确保单击“**保存**”以保存设置。您可以单击“**还原**”恢复默认设置。当您做出选择时，“预览”面板会向您显示您选择的样式。

**标** 志单击“浏览”，然后在“选择标志图像”窗口中选择图形。

**应** 用程序通过选择“背景渐变颜色”菜单创建渐变混色。

**树选** 择一种变换颜色（将指针移到某个项目上时显示的颜色）和一种选择颜色（选择某个项目时显示的颜色）。

**折叠** 面板为显示在屏幕右侧的折叠面板选择背景颜色、边框样式、翻转和选定颜色(在“详细信息”视图中)。

**折叠** 标题选择是否在折叠标题中加粗文本。

**数** 据网格为数据网格中的标题行选择颜色。

**警** 报为警报消息框选择背景颜色。

**进度** 栏为栏选择一种颜色，用于指示上传和下载的进度。

要使Media Portal用户能够看到您选择的样式设置，他们必须将`?company=(company name)`追加到访问Media Portal的URL。 例如，要查看样式设置，访问 PortalCo 公司网站 (

`https://s7sps1.scene7.com/MediaPortal`

) 的 Media Portal 应使用以下 URL：

`https://s7sps1.scene7.com/MediaPortal?company=PortalCo`

将公司名包含在 URL 中可以使 Media Portal 识别用户要访问的公司并相应地应用该公司的样式设置。

您可以详细了解如何向 Media Portal 用户通知 URL 更改，以及如何设置欢迎电子邮件以使新用户收到正确的 Media Portal URL。

请参阅[为 Media Portal 用户设置欢迎电子邮件](adding-media-portal-users.md#setting_up_the_welcome_e_mail_message_for_media_portal_users)。
