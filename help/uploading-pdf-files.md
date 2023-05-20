---
title: 上傳PDF檔案
description: 瞭解如何在Adobe Dynamic Media Classic中上傳與eCatalog相關聯的PDF檔案。
uuid: 9e178bb2-ac09-427a-b61a-aad4e87a5837
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 0097cba5-c886-4115-bc35-7ae7a500202f
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: a787d6b5-48c8-4cf7-b136-60ba3d3eb2f2
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '831'
ht-degree: 36%

---

# 上傳PDF檔案{#uploading-the-pdf-files}

通常Adobe PDF檔案是eCatalog的來源。 這些檔案包含所有影像資訊、字型和向量圖形。 也可以利用图像来构建 eCatalog。準備好要上傳的PDF檔案後，在全域導覽列上，選取 **[!UICONTROL 上傳]** 以開始上傳PDF。

當您上傳頁面擷取的PDF時，Adobe會強制實施以下限制：

| PDF限制型別 | 強制限制 | 於2022年12月31日變更為上限 |
| --- | --- | --- |
| PDF要考慮用於擷取的最大頁數 | 5000 （適用於新上傳） | 100 (適用於所有PDF) |

另請參閱 [Dynamic Media限制](/help/limitations.md).

## 準備PDF檔案 {#preparing-your-pdf-files}

先準備PDF檔案，再上傳至Adobe Dynamic Media Classic：

* 若要讓檔案上傳更輕鬆，請將所有檔案放在電腦或網路上的同一個資料夾中。
* 按照页面的字母数字顺序命名文件。如果对页面进行排序，则在文件上载之后，更容易按正确顺序放置页面。
* 若要檢視PDF頁面是否包含裁切標籤、註冊目標或色條，請檢查頁面。 这些标记决定了印刷文档时的切纸位置，将 eCatalog 放到网络中之前，必须删除这些标记。當您上傳PDF檔案時，Adobe Dynamic Media Classic會提供裁切標籤的選項。
* 如果希望观众按关键字搜索 eCatalog，应确认您的 PDF 文件是否已“平面化”。从平面化的 PDF 文件中无法提取搜索词。要确认 PDF 是否平面化，尝试选择其中的文本。如果您無法選取文字，PDF會平面化，且檢視器無法依您在eCatalog中的關鍵字進行搜尋。
* 由于 PDF 文件要用于印刷，因此通常包含 CMYK 图像。依預設，Adobe Dynamic Media Classic可以聰明地偵測這些CMYK影像，並使用內部CMYK色彩設定檔來轉換它們。 但如果需要，也可以使用自定颜色配置文件来转换 CMYK 图像。

   另請參閱 [ICC （國際色彩聯盟）設定檔](icc-profiles.md#icc_profiles).

## 最佳实践 PDF 上载选项 {#best-practice-pdf-upload-options}

有关不同上载方法的详细信息，请参阅[上载文件](uploading-files.md#uploading_your_files)。

選取您要上傳的檔案，然後選取這些檔案 *最佳實務* PDF選項：

* **裁切選項**  — 在上傳工作選項對話方塊中，選取 **[!UICONTROL 裁切選項]**. 如果PDF頁面包含裁切標籤、註冊標籤或其他標籤，請於 **[!UICONTROL 裁切]** 下拉式清單，選擇 **[!UICONTROL 手動]**. 输入要从页面的上侧、右侧、下侧及左侧裁切的像素数。裁切標籤通常設定為半英吋邊界。 假設您選擇 **[!UICONTROL 150]** （建議使用）做為每英吋畫素解析度，並在「上」、「右」、「下」和「左」文字方塊中輸入75、75、75和75。 在這種情況下，它會從邊界裁切半英吋（150 ppi，1的一半等於75畫素）。

* **處理中**  — 在上傳工作選項對話方塊中，選取 **[!UICONTROL PDF選項]**. 在 **[!UICONTROL 處理中]** 下拉式清單，選擇 **[!UICONTROL 點陣化]**. PDF 文件必须经过栅格化才能在 eCatalog 中显示所有页面和图像。

* **擷取搜尋字詞（選擇性）**  — 在上傳工作選項對話方塊中，選取 **[!UICONTROL PDF選項]**. 在「擷取」下拉式清單中，選擇 **[!UICONTROL 搜尋字詞]** 如果您希望檢視者能夠在eCatalog中依關鍵字搜尋。

* **從多頁PDF自動產生eCatalog （選用）**  — 在上傳工作選項對話方塊中，選取 **[!UICONTROL PDF選項]**. 選取 **[!UICONTROL 從多頁PDF自動產生eCatalog]** 以上傳時自動建立eCatalog。 可以直接进入 eCatalog 屏幕，并开始使用 eCatalog，无需先选择 PDF 文件及选择“构建”命令。eCatalog 用 PDF 文件的名称命名。

* **解析度**  — 在上傳工作選項對話方塊中，選取 **[!UICONTROL PDF選項]**. 在 **[!UICONTROL 解析度]** 文字欄位，輸入值。 Adobe Dynamic Media Classic建議每英吋150畫素。

* **色域**  — 在上傳工作選項對話方塊中，選取 **[!UICONTROL PDF選項]**. 在「色域」下拉式清單中，選擇 **[!UICONTROL 自動偵測]**. 通常，为印刷输出创建的 PDF 采用 CMYK；而用于在线查看的 PDF 则采用 RGB。如果 PDF 使用两个颜色空间，可以选择“强制渲染为 RGB”或“强制渲染为 CMYK”来选择特定颜色空间。例如，当页面图形使用 CMYK 颜色空间，但图片使用 RGB 时，PDF 使用这两个颜色空间。如果上载了 ICC 配置文件，则其名称显示在“颜色空间”菜单上，您可以在其中选择该名称。

   另請參閱 [ICC （國際色彩聯盟）設定檔](/help/icc-profiles.md).

* **色彩設定檔選項**  — 在上傳工作選項對話方塊中，選取 **[!UICONTROL 色彩設定檔選項]**，然後選擇「色彩設定檔」選項：

   * **保留原始色域**  — 保留原始色域。

   * **自訂從>到**  — 開啟子功能表，讓您選擇 **[!UICONTROL 轉換自]** 和 **[!UICONTROL 轉換為]** 色域。 您可以選擇標準的Photoshop色域，或您上傳至Adobe Dynamic Media Classic的色域。

<!-- * **Convert To SRGB** - Converts to SRGB (Standard Red Green Blue). SRGB is the recommended color space for displaying images on web pages. -->

另請參閱 [ICC （國際色彩聯盟）設定檔](icc-profiles.md#icc_profiles).

>[!NOTE]
>
>有关所有 PDF 选项的详细信息，请参阅[PDF 上载选项](pdfs.md#pdf_upload_options)。
