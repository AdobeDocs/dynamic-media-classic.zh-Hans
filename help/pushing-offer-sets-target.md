---
title: 將優惠方案集推送到Adobe Target Standard/Premium
description: 瞭解如何從Adobe Dynamic Media Classic將優惠方案集推送到Adobe Target Standard/Premium。
uuid: 8c895a7c-21b4-4d85-8b0b-a3d2a420bf2e
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
discoiquuid: 39a05654-4f66-4f1e-aec5-ebe6d174353f
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 778fd54b-a9e5-40c5-aff1-a156a5c15923
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 0%

---

# 將優惠方案集推送到Adobe Target Standard/Premium {#pushing-offer-sets-to-target}

建立或編輯優惠方案集後，請依照以下步驟將其推送到Adobe Target Standard/Premium：

1. 在Test&amp;Target選件集畫面中，選取 **[!UICONTROL 推送優惠方案]**.
1. 輸入您的使用者端代碼和登入認證。
1. 選取 **[!UICONTROL 登入]**.

在轉移至Adobe Target Standard/Premium期間，前置詞 `S7_` 會自動附加至優惠方案名稱的開頭。 前置詞旨在確保您可以在Test&amp;Target選件清單中輕鬆找到Adobe Dynamic Media Classic選件。 例如，選件會顯示為 `S7_<name of offer set>_<offer name>`.

Adobe Dynamic Media Classic會推送至Adobe Target Standard/Premium Widget選件。 您可以在Adobe Target Standard/Premium以外使用Widget選件來託管您自己的選件內容。 Widget選件類似於Adobe Target Standard/Premium以外託管的標準選件。 它們可讓Adobe Target Standard/Premium部署儲存在伺服器上的選件內容，以便進行更精細的動態使用。 Widget選件可從URL擷取內容、快取該內容並提供約兩個小時的服務。 Widget提供一些動態內容產生功能，這是Adobe Target Standard/Preimium以外其他提供所沒有的功能。 如果提供選件的mbox包含mbox引數，例如 `mboxProductID` 和 `mbox.offerId`，則 `productId=[PRODUCT_ID]`和 `offerID=[OFFERID]` URL引數會附加至請求的URL。 這些引數可供Widget選件URL提供的服務使用，以傳回Adobe Target Standard/Premium以外使用您mbox之產品或訂單資訊的內容。 您也可以透過API存取Widget選件，以程式設計方式在Adobe Target Standard/Premium以外建立選件。
