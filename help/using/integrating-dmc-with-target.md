---
title: 将Adobe Dynamic Media Classic与Adobe Target Standard/Premium集成
description: 了解如何将Adobe Dynamic Media Classic与Adobe Target Standard/Premium集成。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: c6f217fb-89cb-4c8d-aa7f-309fc42f7d46
topic: Integrations, Development
level: Experienced
source-git-commit: 914fde11270dc731a261da3305b29dd573584d93
workflow-type: tm+mt
source-wordcount: '149'
ht-degree: 0%

---

# 将Adobe Dynamic Media Classic与Adobe Target Standard/Premium集成 {#integrating-dmc-with-target}

在您可以集成 [!DNL Adobe Dynamic Media Classic] 替换为 [!DNL Target Standard/Premium]，您必须在以下位置输入目标URL： [!DNL Adobe Dynamic Media Classic] “应用程序常规设置”屏幕。 要获取Target URL并在“应用程序常规设置”页面中输入它，请执行以下操作：

1. 在 [!DNL Adobe Experience Cloud]，登录到您的 [!DNL Target Standard/Premium] 帐户。
1. 登录后，在浏览器的地址栏中，将URL复制到并包括 `.com`.

   例如，如果 *虚构* 地址栏中的URL（URL路径始终包含正斜杠，而不是本示例中的反斜杠）为 `https:\\www.myfictionalsite.com/categories/admin/home.do`，仅复制 *虚构* URL： `https:\\www.myfictionalsite.com`.

1. 在 [!DNL Adobe Dynamic Media Classic]，转到 **[!UICONTROL 设置]** > **[!UICONTROL 应用程序设置]**.
1. 在应用程序常规设置页面上，在 **[!UICONTROL Test&amp;Target服务器名称]** 字段中，粘贴您在步骤2中复制的URL。
1. 选择 **[!UICONTROL 关闭]**.
