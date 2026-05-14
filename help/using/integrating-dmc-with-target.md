---
title: 将Adobe Dynamic Media Classic与Adobe Target Standard/Premium集成
description: 了解如何将Adobe Dynamic Media Classic与Adobe Target Standard/Premium集成。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
feature: Dynamic Media Classic
role: Developer,Admin,User
exl-id: c6f217fb-89cb-4c8d-aa7f-309fc42f7d46
topic: Integrations, Development
level: Experienced
autotag-review: '2026-05-13T19:51:50.750Z'
TQID: 'https://experienceleague.adobe.com/csg3qawhCOMv6niWQHp9vyGgpJBcVuOOhExioDeURuA'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
level_v2:
  - id: d378ca77-2da1-4f39-ad92-1917fe974a38
source-git-commit: 0d05ca7402db1d8894db1127088905143fb97cff
workflow-type: tm+mt
source-wordcount: 150
ht-degree: 0%

---

# 将Adobe Dynamic Media Classic与Adobe Target Standard/Premium集成 {#integrating-dmc-with-target}

必须先在[!DNL Adobe Dynamic Media Classic]应用程序常规设置屏幕中输入目标URL，然后才能将[!DNL Adobe Dynamic Media Classic]与[!DNL Target Standard/Premium]集成。 要获取Target URL并在“应用程序常规设置”页面中输入它，请执行以下操作：

1. 在[!DNL Adobe Experience Cloud]中，登录到您的[!DNL Target Standard/Premium]帐户。
1. 登录后，在浏览器的地址栏中，将URL复制到并包括`.com`。

   例如，如果地址栏中的&#x200B;*虚构* URL （URL路径始终包含正斜杠，而不是本示例中的反斜杠）为`https:\\www.myfictionalsite.com/categories/admin/home.do`，则仅复制&#x200B;*虚构* URL的以下部分： `https:\\www.myfictionalsite.com`。

1. 在[!DNL Adobe Dynamic Media Classic]中，转到&#x200B;**[!UICONTROL 设置]** > **[!UICONTROL 应用程序设置]**。
1. 在“应用程序常规设置”页面的&#x200B;**[!UICONTROL Test&amp;Target服务器名称]**&#x200B;字段中，粘贴您在步骤2中复制的URL。
1. 选择&#x200B;**[!UICONTROL 关闭]**。
