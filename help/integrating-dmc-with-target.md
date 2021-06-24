---
title: 将AdobeDynamic Media Classic与Adobe Target Standard/Premium集成
description: 了解如何将AdobeDynamic Media Classic与Adobe Target Standard/Premium相集成。
uuid: d1c07a52-b058-4ae3-a31d-44c43dc27f65
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
discoiquuid: 3b4add18-4191-475e-a3a3-0184367a25fc
feature: Dynamic Media Classic
role: Data Engineer,Administrator,Business Practitioner
exl-id: c6f217fb-89cb-4c8d-aa7f-309fc42f7d46
source-git-commit: 27d9a9b9f158846b54e4318119aec9e4dc9c4c0d
workflow-type: tm+mt
source-wordcount: '151'
ht-degree: 1%

---

# 将AdobeDynamic Media Classic与Adobe Target Standard/Premium集成 {#integrating-dmc-with-target}

在将[!DNL Dynamic Media Classic]与[!DNL Target Standard/Premium]集成之前，必须在[!DNL Dynamic Media Classic]应用程序常规设置屏幕中输入目标URL。 要获取您的Target URL并在“应用程序常规设置”页面中输入它，请执行以下操作：

1. 在[!DNL Adobe Experience Cloud]中，登录到您的[!DNL Target Standard/Premium]帐户。
1. 登录后，在浏览器的地址栏中，将URL复制到并包含`.com`。

   例如，如果地址栏中的&#x200B;*虚构* URL（URL路径始终包含正斜杠，而不是本例中的反斜杠）是`https:\\www.myfictionalsite.com/categories/admin/home.do`，则只复制&#x200B;*虚构* URL的此部分：`https:\\www.myfictionalsite.com`。

1. 在[!DNL Dynamic Media Classic]中，单击&#x200B;**[!UICONTROL 设置]** > **[!UICONTROL 应用程序设置]**。
1. 在“应用程序常规设置”页的&#x200B;**[!UICONTROL Test&amp;Target服务器名称]**&#x200B;字段中，粘贴您在步骤2中复制的URL。
1. 单击&#x200B;**[!UICONTROL 关闭]**。
