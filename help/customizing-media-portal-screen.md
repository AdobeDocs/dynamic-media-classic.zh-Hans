---
title: 自定义 Media Portal 屏幕
seo-title: 自定义 Media Portal 屏幕
description: 'null'
seo-description: 了解如何自定义Media Portal屏幕。
uuid: bd a65a6-723b-49d-8eac-849da00e0e1a
contentOwner: admin
content-type: 引用
products: SG_ EXPERIENCE MANAGER/Dynamic-Media-Scene-7
geptopics: SG_ SCENESELEFERENDER_ PK/categories/media_ Portal
discoiquuid: 8b000c25-c9 c3-481e-9b25-96257471571f
translation-type: tm+mt
source-git-commit: 75f006fd81b0fe2dad5479cdd98e45eaada46b2a

---


# 自定义 Media Portal 屏幕{#customizing-the-media-portal-screen}

通过 Media Portal 样式设置，您可以在 Media Portal 屏幕中标上您公司的徽标和颜色。使用样式设置将您公司的图章放在 Media Portal 上。

要访问样式设置，请选择“**设置**”&gt;“**Media Portal 设置**”&gt;“**样式设置**”。设置后请确保单击“**保存**”以保存设置。您可以单击“**还原**”恢复默认设置。当您做出选择时，“预览”面板会向您显示您选择的样式。

**Logo** 单击“浏览”并在“选择标志图像”窗口中选择一个图形。

**应用程序** 通过在“背景渐变颜色”菜单上做出选择来创建渐变颜色混合。

**树** 选择翻转颜色(将指针移到项目上时显示的颜色)和选区颜色(选择项目时显示的颜色)。

**Accordion** 选择背景颜色、边框样式和翻转以及可折叠的颜色，这些颜色显示在屏幕右侧的“详细信息”视图中。

**折叠标题** 选择是否使折叠标题中的文本成为粗体。

**数据网格** 为数据网格中的标题行选择颜色。

**警报** 为警报消息框选择背景颜色。

**进度栏** 选择指示上传和下载进度的栏颜色。

For Media Portal users to see the style settings you choose, they must append `?company=(company name)` to the URL with which they access Media Portal. 例如，要查看样式设置，访问 PortalCo 公司网站 (

`https://s7sps1.scene7.com/MediaPortal`

) 的 Media Portal 应使用以下 URL：

`https://s7sps1.scene7.com/MediaPortal?company=PortalCo`

将公司名包含在 URL 中可以使 Media Portal 识别用户要访问的公司并相应地应用该公司的样式设置。

您可以详细了解如何向 Media Portal 用户通知 URL 更改，以及如何设置欢迎电子邮件以使新用户收到正确的 Media Portal URL。

请参阅[为 Media Portal 用户设置欢迎电子邮件](adding-media-portal-users.md#setting_up_the_welcome_e_mail_message_for_media_portal_users)。
