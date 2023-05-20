---
title: 登录到 Adobe Analytics
description: 瞭解如何從Adobe Dynamic Media Classic登入Adobe Analytics。
uuid: 5614babe-1097-4228-a3dc-27e5a25366d5
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: e5b510a8-8b7f-4c60-869e-d664a8157e63
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 261b8f7c-c61c-4ce3-b9dc-8549347aca2e
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '846'
ht-degree: 1%

---

# 登录到 Adobe Analytics{#log-in-to-adobe-analytics}

在您登入設定Adobe Analytics報表並將Adobe Analytics報表變數與Adobe Dynamic Media Classic事件相符之前，請先確認您是Adobe Analytics中「Web服務存取」群組的成員。 無論介面中設定的許可權為何，此群組中的成員皆可透過Experience Cloud的Web Services API存取指定報表套裝中的所有報表。 若要新增成員至群組，請在Adobe Analytics中前往 **[!UICONTROL 管理工具]** > **[!UICONTROL User Management]** > **[!UICONTROL 編輯群組]**.

登入時，您可以選擇輸入Experience Cloud組織ID，以使用最新的視訊分析實作。 如果您選擇不輸入ID，視訊報表仍可運作。 但是，這可能會導致資料無法正確與Adobe Dynamic Media Classic外部該使用者端的其他資料整合。

>[!NOTE]
>
>如果您的Adobe Analytics帳戶已移轉至Adobe IMS驗證(Identity Management系統)以進行登入，則無法輸入直接憑證。

## 從Adobe Dynamic Media Classic登入Adobe Analytics {#log-in-to-analytics-from-dmc}

首先，請整合Dynamic Media Classic與Adobe Analytics OAuth。 Adobe Analytics OAuth與Dynamic Media Classic的整合通常每個使用者只需完成一次。

1. 存取 [Adobe Developer主控台](https://developer.adobe.com/console). 確保您的帳戶擁有需要整合之組織的管理員許可權。
1. 在「首頁」右上角附近，從下拉式清單中選取適當的公司。 （下面的熒幕擷圖僅供參考；您選取的實際公司名稱可能會有所不同。）

   ![建立新專案](assets/analytics-oauth1.png)

1. 執行下列任一項作業：

   * 頁面頂端的 **[!UICONTROL 首頁]** 索引標籤，選取 **[!UICONTROL 建立新專案]**.
   * 頁面頂端的 **[!UICONTROL 專案]** 標籤。 在頁面的右角附近，選取 **[!UICONTROL 建立新專案]**.

1. 在專案的頁面上，選取 **[!UICONTROL 新增API]**.
1. 於 **[!UICONTROL 新增API]** 頁面，選取 **[!UICONTROL Adobe Analytics]**.
1. 在頁面的右下角附近，選取 **[!UICONTROL 下一個]**.

   ![新增API](assets/analytics-oauth2.png)

1. 於 **[!UICONTROL 設定API]** 頁面，選取 **[!UICONTROL 使用者驗證OAuth]**.
1. 在頁面的右下角附近，選取 **[!UICONTROL 下一個]**.
1. 於 **[!UICONTROL 設定API]** 頁面，選取 **[!UICONTROL OAUTH 2.0 Web]**.
1. 在 **[!UICONTROL 預設重新導向URI]** 文字欄位，請完全按照所示輸入以下路徑：

   `https://exploreadobe.com/dynamic-media-upgrade/`

1. 在 **[!UICONTROL 重新導向URI模式]** 文字欄位，請完全按照所示輸入以下路徑：

   `https://exploreadobe\.com/dynamic-media-upgrade/`

1. 在頁面的右下角，選取 **[!UICONTROL 儲存已設定的API]**.
1. 在導覽面板中，於Adobe Analytics頁面左側的下方 **[!UICONTROL 認證]**，選取 **[!UICONTROL OAuth Web]**.
1. 下 **[!UICONTROL 認證詳細資料]**，請執行下列動作：
   * 下 **[!UICONTROL 使用者端ID]**，選取 **[!UICONTROL 複製]** 以複製值。 您需要此值才能在後續的Dynamic Media Classic案頭應用程式中進行Analytics設定。
   * 下 **[!UICONTROL 使用者端密碼]**，選取 **[!UICONTROL 擷取使用者端密碼]** 以顯示相關值。 選取 **[!UICONTROL 複製]** 以複製值。 您需要此值才能在Dynamic Media Classic案頭應用程式中進行後續的Adobe Analytics設定。

## 在Adobe Dynamic Media Classic中設定Adobe Analytics {#configure-analytics-in-dmc}

>[!NOTE]
>
>在Dynamic Media Classic中進行Adobe Analytics的初始設定後，只有在下列情況下才必須重做設定：
>
>* Analytics中新增了新報表，使用者想要開始傳送資料至該新報表。
>* Adobe Analytics中的追蹤伺服器已更新。
>* 報表中引進了新的追蹤變數，您希望將Dynamic Media Classic使用者介面中的特定檢視器變數連結到該新Analytics變數。
>


1. 在Adobe Dynamic Media Classic案頭應用程式的右上角附近，前往 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]**.
1. 在左側面板中的 **[!UICONTROL 應用程式設定]**，選取 **[!UICONTROL Adobe Analytics]**.
1. 於 **[!UICONTROL Adobe Analytics設定]** 頁面，選取 **[!UICONTROL Adobe Analytics登入]**.
1. 在 **[!UICONTROL Adobe Analytics登入]** 對話方塊，在 **[!UICONTROL 使用者端ID]** 欄位和 **[!UICONTROL 使用者端密碼]** 欄位中，貼上您先前複製的個別值。
1. 在對話方塊的右下角，選取 **[!UICONTROL 登入]** 並執行您的Adobe IMS (Identity Management服務)登入。

   當您成功登入時，「Adobe Analytics登入」對話方塊會再次出現，同時顯示 **[!UICONTROL 公司]** 下拉式清單，由您可用的公司啟動。

1. 從 **[!UICONTROL 公司]** 從下拉式清單中選擇公司。

   選取公司後， **[!UICONTROL 套裝]** 由所選公司可用的報表套裝啟動的下拉式清單會變成可見。

1. 從 **[!UICONTROL 套裝]** 從下拉式清單中選擇報表套裝。

   >[!NOTE]
   >
   >依預設，使用者必須瞭解以下事實 **[!UICONTROL 公司]** 和 **[!UICONTROL 套裝]** 下拉式清單是空的。 因此，使用者必須從每個清單中選取一個值。

1. 選取 **[!UICONTROL 確定]** 以便儲存設定。

   >[!NOTE]
   >
   >此 **[!UICONTROL Adobe Analytics伺服器]** 欄位會填入在您選取時符合分析名稱空間的建議協力廠商追蹤伺服器 **[!UICONTROL 確定]**. 如果您使用不同的追蹤伺服器，請在此欄位中更新該伺服器，以避免資料遺失。

1. 在「Adobe Analytics設定」頁面的左下角，選取「 」 **[!UICONTROL 儲存]** 以確保更新您的Adobe Analytics帳戶設定。

>[!MORELIKETHIS]
>
>* [設定Adobe Analytics報表](configuring-analytics-reports.md#configuring_adobe_analytics_reports)

