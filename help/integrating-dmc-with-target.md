---
title: 将Adobe Dynamic Media Classic与Adobe Target Standard/Premium集成
description: 了解如何将Adobe Dynamic Media Classic与Adobe Target Standard/Premium集成。
uuid: d1c07a52-b058-4ae3-a31d-44c43dc27f65
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
discoiquuid: 3b4add18-4191-475e-a3a3-0184367a25fc
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: c6f217fb-89cb-4c8d-aa7f-309fc42f7d46
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '149'
ht-degree: 0%

---

# 将Adobe Dynamic Media Classic与Adobe Target Standard/Premium集成 {#integrating-dmc-with-target}

集成之前 [!DNL Adobe Dynamic Media Classic] with [!DNL Target Standard/Premium]，则必须在 [!DNL Adobe Dynamic Media Classic] 应用程序常规设置屏幕。 要获取您的Target URL并在“应用程序常规设置”页面中输入它，请执行以下操作：

1. 在 [!DNL Adobe Experience Cloud]，登录到 [!DNL Target Standard/Premium] 帐户。
1. 登录后，在浏览器的地址栏中，将URL复制到（包括） `.com`.

   例如，如果 *虚构* 地址栏中的URL（URL路径始终包含正斜杠，而不是本例中的反斜杠）为 `https:\\www.myfictionalsite.com/categories/admin/home.do`，则仅复制 *虚构* URL: `https:\\www.myfictionalsite.com`.

1. 在 [!DNL Adobe Dynamic Media Classic]，转到 **[!UICONTROL 设置]** > **[!UICONTROL 应用程序设置]**.
1. 在“应用程序常规设置”页面的 **[!UICONTROL Test&amp;Target服务器名称]** 字段中，粘贴您在步骤2中复制的URL。
1. 选择 **[!UICONTROL 关闭]**.
