---
title: 自定义 Media Portal 屏幕
description: 瞭解如何在Adobe Dynamic Media Classic中自訂Media Portal畫面。
uuid: bd1a65a6-723b-49d0-8eac-849da00e0e1a
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
discoiquuid: 8b000c25-c9c3-481e-9b25-96257471571f
feature: Dynamic Media Classic,Collaboration,Asset Management
role: Admin,User
exl-id: b0c5f70a-2388-42aa-a1ed-fd745ff90518
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '346'
ht-degree: 32%

---

# 自定义 Media Portal 屏幕{#customizing-the-media-portal-screen}

通过 Media Portal 样式设置，您可以在 Media Portal 屏幕中标上您公司的徽标和颜色。使用樣式設定將您的公司品牌放在Media Portal上。

若要存取樣式設定，請前往 **[!UICONTROL 設定]** > **[!UICONTROL Media Portal設定]** > **[!UICONTROL 樣式設定]**. 請務必選取 **[!UICONTROL 儲存]** 以在完成設定後加以儲存。 您可以選取 **[!UICONTROL 還原]** 以恢復預設設定。 當您做出選擇時，「預覽」面板會顯示它們的顯示方式。

* **[!UICONTROL 標誌]**  — 選取 **[!UICONTROL 瀏覽]**，然後在「選取標誌影像」視窗中選擇圖形。

* **[!UICONTROL 應用]**  — 在「背景漸層顏色」選單中進行選擇，建立漸層顏色混合。

* **[!UICONTROL 樹狀]**  — 選擇滑鼠指向效果色彩（將指標移到專案上時顯示的色彩）和選取範圍色彩（選取專案時顯示的色彩）。

* **[!UICONTROL 收合式選單]**  — 選擇背景顏色、邊框樣式、滑鼠指向效果及選取的顏色，以利在「詳細資訊」檢視中顯示在熒幕右側的摺疊式功能表。

* **[!UICONTROL 收合式選單標題]**  — 選擇是否以摺疊式功能表頁首粗體顯示文字。

* **[!UICONTROL 資料格]**  — 選擇資料網格中標題列的顏色。

* **[!UICONTROL 警報]**  — 選擇警示訊息方塊的背景顏色。

* **[!UICONTROL 進度列]**  — 選擇指示上傳和下載進度的橫條色彩。

若要Media Portal使用者檢視您選擇的樣式設定，他們必須附加 `?company=(company name)` 存取他們用來存取Media Portal的URL。 例如，要查看样式设置，访问 PortalCo 公司网站 (

`https://s7sps1.scene7.com/MediaPortal`

請改用以下URL：

`https://s7sps1.scene7.com/MediaPortal?company=PortalCo`

将公司名包含在 URL 中可以使 Media Portal 识别用户要访问的公司并相应地应用该公司的样式设置。

您可以详细了解如何向 Media Portal 用户通知 URL 更改，以及如何设置欢迎电子邮件以使新用户收到正确的 Media Portal URL。

请参阅[为 Media Portal 用户设置欢迎电子邮件](adding-media-portal-users.md#setting_up_the_welcome_e_mail_message_for_media_portal_users)。
