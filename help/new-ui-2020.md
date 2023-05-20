---
title: Adobe Dynamic Media Classic案頭應用程式
description: Adobe Dynamic Media Classic使用者現在可以體驗使用者介面的完整重新整理。 此體驗提供更新的登入功能，內含寶貴資源的連結，加上此更新不再依賴瀏覽器中的AdobeFlash技術。
contentOwner: rbrough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic
role: Admin,User
exl-id: d61ea80a-a98e-43e6-9e2e-4389962134f1
source-git-commit: 6bdf08b98c5c8167f4a4da49452efa977beb136e
workflow-type: tm+mt
source-wordcount: '1089'
ht-degree: 0%

---

# Adobe Dynamic Media Classic案頭應用程式 — 現已推出 {#new-ui-2020}

另請參閱 [Adobe Dynamic Media Classic案頭應用程式](/help/dynamic-media-classic-desktop-app.md) 若要檢閱系統需求，請下載並安裝新的應用程式，然後登入該應用程式。

## _上次修訂日期：2020年6月30日_

Adobe Dynamic Media Classic使用者現在可以使用新的登入體驗，不再仰賴瀏覽器中的AdobeFlash技術。

## 常见问题

+++**_2020年12月31日當瀏覽器停止支援AdobeFlash時，會對Adobe Dynamic Media Classic (前身為Scene7)造成任何影響嗎？_**
AdobeFlash Player是網頁瀏覽器外掛程式，可讓網頁瀏覽器使用在Adobe Flash Platform上開發的內容。 Adobe Dynamic Media Classic的網頁使用者介面(目前標籤為 [!DNL Scene7 Publishing System] 或 [!DNL SPS] （在產品中）需要AdobeFlash Player。 2020年12月31日棄用AdobeFlash後，Adobe Dynamic Media Classic客戶將無法再登入網頁使用者介面。 由於這項變更，Adobe已提供客戶案頭應用程式，以取代瀏覽器體驗。
+++

+++**_如何存取新的案頭應用程式？_**
新的案頭應用程式以 `.dmg` macOS安裝程式或 `.exe` Windows®安裝程式。

另請參閱 [Adobe Dynamic Media Classic案頭應用程式](/help/dynamic-media-classic-desktop-app.md) 若要檢閱系統需求，請下載並安裝新應用程式，然後登入該應用程式。
+++

<!-- NEWSLETTER IS DEAD The download links are also available by way of the [Adobe Dynamic Media Classic newsletter subscription page.](https://www.adobe.com/subscription/dynamic-media-newsletter.html) -->

+++**_新的案頭應用程式如何運作？_**
下載、安裝及啟動案頭應用程式後，系統會顯示重新整理的登入體驗。 透過輸入您現有的使用者名稱和密碼，並根據您的地區選擇適當的伺服器，您可以登入Adobe Dynamic Media Classic。 整體體驗與您慣用的熟悉網頁瀏覽器版本相同。 從案頭應用程式，您可以存取Adobe Dynamic Media Classic生產和中繼環境。 如果您擁有此功能的認證，也可以存取Media Portal。

>[!IMPORTANT]
>
>只能安裝案頭應用程式的一個執行個體 *和* 在指定電腦上同時啟用。 不過，您可以跨電腦安裝的數量並沒有限制。

+++

+++**_如果我使用Adobe Dynamic Media Classic API存取產品，但未透過網頁使用者介面登入，該怎麼辦？_**
Adobe Dynamic Media Classic的基礎API沒有變更。
+++

+++**_這項全新的案頭應用程式體驗是否需要移轉或變更協力廠商整合？_**
否. Adobe Dynamic Media Classic客戶不需移轉或變更任何協力廠商整合，即可使用新的案頭應用程式。
+++

+++**_此變更是否會影響我的自動化指令碼？_**
否. 對自動化指令碼沒有影響。 新版案頭應用程式的運作和行為方式，與您熟悉的瀏覽器式體驗類似。
+++

+++**_新的Adobe Dynamic Media Classic案頭應用程式能否在Mac和個人電腦上運作？_**&#x200B;是的。新版案頭應用程式是跨平台解決方案，適用於Mac和電腦。 Linux®是 *not* 支援。
+++

+++**_我的公司有嚴格的安全要求。 新的Adobe Dynamic Media Classic案頭應用程式如何處理這些需求？_**
Adobe致力於確保其產品符合客戶的安全需求。 新的Adobe Dynamic Media Classic案頭應用程式持續為客戶提供符合所有Adobe安全性標準的高度安全體驗。
+++

+++**_我的公司不允許我在電腦上安裝軟體與應用程式。 您建議我如何存取新的案頭應用程式？_**
有些公司不允許您未經核准，將軟體與應用程式下載並安裝至您的系統。 在這種情況下，請及早與您的IT團隊合作，以取得存取新Adobe Dynamic Media Classic案頭應用程式的許可權。 請記住，在2020年12月31日之後，瀏覽器版本將被棄用。 請務必避免等到最後一分鐘才下載新的案頭應用程式。
+++

+++**_新案頭應用程式的多個執行個體可以同時開啟嗎？_**
否，建置新Adobe Dynamic Media Classic案頭應用程式的AIR技術會限制使用者在指定時間開啟多個應用程式例項。
+++

+++**_對於可透過本機電腦上傳至Adobe Dynamic Media Classic的檔案數量是否有任何限制？_**
在Windows®上使用新的Adobe Dynamic Media Classic案頭應用程式時，您最多可以使用以下工具一次上傳150個檔案： **[!UICONTROL 上傳]** 對話方塊。 此限制已在2020年底之前解決。 有 *否* macOS平台上的上傳限制。
+++

+++**_新的Adobe Dynamic Media Classic案頭應用程式是否需要新的SKU？ 是否涉及授權成本？_**
使用新的Adobe Dynamic Media Classic案頭應用程式不需變更SKU或授權。
+++

+++**_如何啟用Adobe Dynamic Media Classic案頭應用程式升級？_**
在2020年6月30日發行Adobe Dynamic Media Classic案頭應用程式後，如果Adobe發行新版本，客戶必須下載新版本並照常安裝(取代現有的應用程式於 **[!UICONTROL 應用]**)。 您會透過Adobe帳戶團隊和應用程式內升級通知機制收到新版本的通知，通知使用者已升級。
+++

+++**_我該如何取得Adobe Dynamic Media Classic案頭應用程式相關問題的協助？_**
如有任何使用應用程式的問題，請聯絡Adobe支援。
+++

+++**_我想確認我正在最佳化我的多媒體策略。 如何進一步瞭解Adobe Dynamic Media Classic？_**
Adobe Dynamic Media Classic是功能豐富的強大解決方案，專為增強您的多媒體策略而設計。 為確保您能充分運用所有功能，請務必探索以下實用資源：

* [Adobe Dynamic Media Classic最佳實務教學課程](https://experienceleague.adobe.com/docs/experience-manager-learn/dynamic-media-classic-tutorial/overview.html)
* [Adobe部落格](https://blog.adobe.com/)<!-- (https://blog.adobe.com/tag/dynamic-media/) -->
* [AdobeDynamic Media電子報封存](https://experienceleague.adobe.com/docs/dynamic-media-classic/using/dynamic-media-newsletter.html)

+++

<!-- HIDDEN AUGUST 2, 2021 BECAUSE THE NEWSLETTER WAS DISCONTINUED Plus, [subscribe to the Dynamic Media newsletter](https://www.adobe.com/subscription/dynamic-media-newsletter.html) to stay current on the latest news, information, training opportunities, powerful features available to you such as [Smart Imaging](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/imaging-faq.html#dynamic), and the complementary audit program. -->

+++**_我想進一步瞭解如何使用Adobe Experience Manager Assets升級至AdobeDynamic Media。 我可以在哪裡找到更多資訊？_**
若要進一步瞭解升級至新一代多媒體創作、發佈及動態傳送的好處，請造訪 [AdobeDynamic Media入口網站以進行升級](https://exploreadobe.com/dynamic-media-upgrade/).
+++

>[!MORELIKETHIS]
>
>* [登入和登出Adobe Dynamic Media Classic案頭應用程式](/help/signing-out.md)
>* [下載並安裝Adobe Dynamic Media Classic案頭應用程式](/help/dynamic-media-classic-desktop-app.md)


<!-- SAVE - OLD LINK TO BEST PRACTICES GUIDE IN PDF https://www.adobe.com/content/dam/www/us/en/marketing/experience-manager-assets/dynamic-media/adobe-dynamic-media-classic-best-practices-guide.pdf -->