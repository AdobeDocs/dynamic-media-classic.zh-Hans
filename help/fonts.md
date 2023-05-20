---
title: 字体
description: 瞭解如何在Adobe Dynamic Media Classic中使用字型。
uuid: bddec9c2-8530-4bbd-8db7-1562a347e482
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/support_files
discoiquuid: 97cecd6a-30aa-44fe-a611-fd71b02fd5ae
feature: Dynamic Media Classic
role: User
exl-id: 186f4c7f-16f6-42f5-bc0e-55362c55e794
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 28%

---

# 字体{#fonts}

有時候，Adobe Dynamic Media Classic會要求您上傳字型檔案，以輸入或轉譯特定字型的文字。 例如，要在模板图层上将特定的字体用于文本，请上载字体文件。要以特定的字体显示 eCatalog 查看器页码，请上载字体文件。

Adobe Dynamic Media Classic支援下列字型型別：

* 所有 TrueType 字体
* PostScript®字型
* OpenType/TrueType 字体
* OpenType/PostScript 字体
* PhotoFont

上傳字型檔案後，您可以變更其Adobe Dynamic Media Classic ID、字型名稱，並在「編輯資訊」畫面上輸入資訊。

>[!NOTE]
>
>如果您打算在範本圖層中使用字型，Adobe Dynamic Media Classic建議上傳所有字型樣式（粗體、斜體、粗體/斜體及一般）。 Adobe Dynamic Media Classic需要這些字型樣式來處理請求。 还建议上载与某种字体相关的所有 PostScript/Adobe Type 1 文件，因为其中的某些字体包含详细的字距调整信息。

## 上傳字型檔案 {#uploading-font-files}

使用与上载其他文件相同的方法上载字体文件。您可以將字型檔案儲存在任何Adobe Dynamic Media Classic資料夾中。 请参阅[上载文件](uploading-files.md#uploading_your_files)。

## 編輯字型檔案資訊 {#editing-font-file-information}

您可以變更字型的ID名稱及其型別資訊。 编辑字体文件会有助于搜索，并且使得字体更易于识别。

在「瀏覽」面板中，選取要在「詳細資料檢視」中編輯的字型檔案，然後選擇「檔案」>「編輯資訊」。 此时将打开“编辑信息”屏幕。選擇下列選項，然後選取 **[!UICONTROL 提交]**.

* **[!UICONTROL 字型名稱]**  — 此名稱可識別發佈時的字型。

* **[!UICONTROL PostScript名稱]**  — 此名稱是字型的完整PostScript名稱。 它通常指示粗细或样式。

* **[!UICONTROL RTF名稱]**  — 此名稱會出現在建立範本文字圖層的RTF編輯器中的彈出式選單上。

* **[!UICONTROL 字型系列名稱]**  — 此名稱會列出字型名稱，但沒有樣式、粗細或字型型別指示器。

* **[!UICONTROL 字型樣式]**  — 選項為純、粗體、斜體及粗斜體。

* **[!UICONTROL 字型型別]**  — 選項為TrueType和Adobe Type1。 如果使用其他名称调用这些字体，可以输入该名称。

* **[!UICONTROL 字型型別縮寫]**  — 選項如下：

   * **[!UICONTROL TTF]**  — 用於PDF/PostScript轉譯和影像伺服的TrueType字型檔案。

   * **[!UICONTROL AFM]**  — 包含Adobe字型量度資訊且用於影像伺服的Adobe PostScript字型檔案。

   * **[!UICONTROL PFM]**  — 包含二進位字型量度資訊的Adobe PostScript字型檔案。

   * **[!UICONTROL PFB]**  — 包含二進位字型輪廓資訊的Adobe PostScript字型檔案，用於PDF/PostScript轉譯和影像提供。
