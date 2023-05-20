---
title: 「快速入門：Adobe Target Standard/Premium整合」
description: Adobe Target Standard/Premium簡介和快速入門，可幫助您在Adobe Dynamic Media Classic中快速上手並執行Adobe Target Standard/Premium整合技術。
uuid: d8f79fbf-8be1-44fa-8058-3508060fcd70
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_classic_integration
discoiquuid: f8c25768-cf59-45ec-8193-522404191d57
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 4745ace5-7825-468e-8a82-bfbbcf1b0440
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '515'
ht-degree: 7%

---

# 快速入門： Adobe Target Standard/Premium整合{#quick-start-target-integration}

Adobe Target Standard/Premium將控制權直接交由行銷人員手中，以快速並持續執行多個A/B和多變數測試、測量成效，並透過分段、目標定位和Automated Personalization提高線上內容的關聯性。

Adobe Dynamic Media Classic可讓您為Adobe Target Standard/Premium行銷活動建立優惠方案和優惠方案集。 例如，您可以建立包含相同多媒體資產的三個變體的選件集。 接著，您可以讓Adobe Target Standard/Premium判斷哪個資產可提供較好的轉換提升度。 您可以通过基本模板或各个图像创建优惠和优惠套餐。將選件集推送或儲存至Adobe Target Standard/Premium （選件會與mbox和體驗相關聯）後，Adobe Target Standard/Premium就可以執行行銷活動。 這些行銷活動會決定網站的哪些變數最適合點進和轉換。

若要進一步自訂動態Adobe Dynamic Media Classic內容，請使用Adobe Target Standard/PremiumHTML選件。 請參閱 [Adobe Target Standard/Premium產品檔案](https://experienceleague.adobe.com/docs/target.html) 以取得詳細資訊。

>[!NOTE]
>
>必須具備有效的Adobe Target Standard/Premium帳戶，才能將Adobe Target Standard/Premium與Adobe Dynamic Media Classic搭配使用。

本快速入門旨在協助您快速上手Adobe Target Standard/PremiumHTML選件集。 请执行步骤 1 到 3。每個步驟之後，都會有主題標題的互動參照，讓您在其中找到更多資訊。

## 1.在「應用程式一般設定」頁面中輸入您的Adobe Target Standard/Premium URL

Adobe Dynamic Media Classic需要您的Adobe Target Standard/Premium URL才能與Adobe Target Standard/Premium整合。 複製您的Adobe Target Standard/Premium URL部分，最多可複製並包含 `.com`，並在Adobe Dynamic Media Classic中輸入 **[!UICONTROL 應用程式一般設定]** 頁面，在 **[!UICONTROL 伺服器]** 群組， **[!UICONTROL Test&amp;Target伺服器名稱]** 文字欄位。 另請參閱 [將Adobe Dynamic Media Classic與Adobe Target Standard/Premium整合](integrating-dmc-with-target.md#integrating-dmc-with-target).

## 2.建立優惠方案集

使用参数化模板或图像来创建优惠套餐。您可以在Test&amp;Target選件集頁面上建立HTML選件集。 若要開啟此頁面，請選取您的範本或影像，然後在全域導覽列上，前往 **[!UICONTROL 建置]** > **[!UICONTROL Test&amp;Target選件集]**.

若要使用範本建立優惠方案，請選取 **[!UICONTROL 新增並預覽]**. 在新增和預覽頁面上，變更引數值。

若要建立包含影像的選件，請將影像拖曳至Test&amp;Target選件集頁面。 選取 **[!UICONTROL 預覽]** 並為影像或選件集中的所有影像選擇影像預設集。

创建优惠套餐后请将其保存。

另請參閱 [建立優惠方案集](creating-offer-set.md#creating_an_offer_set).

## 3.將優惠方案集推送至Adobe Target Standard/Premium

在Test&amp;Target選件集頁面中，選取 **[!UICONTROL 推送優惠方案]**，並在Test&amp;Target登入對話方塊中輸入登入認證。 另請參閱 [將優惠方案集推送到Adobe Target Standard/Premium](pushing-offer-sets-target.md#pushing_offer_sets_to_target).
