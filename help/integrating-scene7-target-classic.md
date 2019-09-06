---
title: 将Adobe Dynamic Media经典与Adobe Target Classic集成
seo-title: 将Adobe Dynamic Media经典与Adobe Target Classic集成
description: 'null'
seo-description: 了解如何将Adobe Dynamic Media经典与Adobe Target Classic集成。
uuid: d1c07a52-b058-4ae3-a31 d-44c43 dc27 f65
contentOwner: admin
content-type: 引用
products: SG_ EXPERIENCE MANAGER/Dynamic-Media-Scene-7
geptopics: SG_ SCENESELEFERENDER_ PK/categories/target_ classic_ integration
discoiquuid: 3b4add18-4191-475e-a3 a3-018467a25 fc
translation-type: tm+mt
source-git-commit: d5bf894d56687561c93ef08762bc19d3597225e6

---


# 将Adobe Dynamic Media经典与Adobe Target Classic集成{#integrating-adobe-scene-with-adobe-target-classic}

在将Dynamic Media经典与Target Classic集成之前，必须在Dynamic Media经典应用程序常规设置屏幕中输入Target经典URL。请按照以下步骤获取Target经典URL并在“应用程序常规设置”屏幕中输入它：

1. 转到位于以下地址的Target经典登录页面：https://admin.testandtarget.omniture.com。
1. 输入凭据，然后单击 **“登录”**。
1. 登录后，在浏览器的地址栏中，复制 URL 中直到 *.com* 的部分。

   For example, if the *fictional* URL (URLs paths always contain forward slashes, not back slashes as in this example) in the address bar is `https:\\www.mysite.com/categories/admin/home.do`, copy only this portion of the *fictional* URL: `https:\\www.mysite.com`.

   在第步中，您将复制的URL部分粘贴到Dynamic Media经典应用程序常规设置屏幕中。

1. 在Dynamic Media经典中，单击 **“设置** ”&gt; **“应用程序设置**”。
1. 在“应用程序常规设置”页面的“目标经典服务器名称”字段中，粘贴您在步骤中复制的URL。
1. 单击“**关闭**”。

