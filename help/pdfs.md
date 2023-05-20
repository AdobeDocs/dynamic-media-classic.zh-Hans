---
title: 使用PDF
description: 瞭解如何在Adobe Dynamic Media Classic中使用PDF。
uuid: 26d70d28-9393-49b1-9051-d70456deca67
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 5a073de3-6b1d-4c3e-8c03-9182f9f3874a
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 02892514-61fe-48ba-a2e3-eeb30580a1e4
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '710'
ht-degree: 36%

---

# 使用PDF{#working-with-pdfs}

PDF（可攜式檔案格式）檔案最常用於Adobe Dynamic Media Classic建立eCatalog。 上傳PDF檔案時，Adobe Dynamic Media Classic會依預設點陣化或擷取頁面，以便使用這些頁面建立豐富媒體。

當您上傳頁面擷取的PDF時，Adobe會強制實施以下限制：

| 限制型別 | 強制限制 | 於2022年12月31日變更為上限 |
| --- | --- | --- |
| PDF要考慮用於擷取的最大頁數 | 5000 （適用於新上傳） | 100 (適用於所有PDF) |

另請參閱 [Dynamic Media限制](/help/limitations.md).

## PDF 上载选项 {#pdf-upload-options}

当上载 PDF 文件时，您能够以多种方法设置其格式。可以裁切其页面、提取搜索词、输入像素/英寸分辨率以及选择颜色空间。PDF 文件中常常包含修剪边距、裁切标记、对齐标记以及其他打印机的标记。当上载 PDF 文件时，可以从页边裁切这些标记。

上傳PDF檔案的選項位於「上傳」頁面的「PDF選項」下方。

### 處理選項

**[!UICONTROL 點陣化]** - （預設）撕裂PDF檔案中的頁面，並將向量圖形轉換為點陣圖影像。 若要建立eCatalog，請選擇此選項。

**[!UICONTROL 擷取搜尋字詞]**  — 從PDF檔案中擷取文字，以便在eCatalog檢視器中依關鍵字搜尋檔案。

**[!UICONTROL 擷取連結]**  — 從PDF檔案中擷取連結，並將其轉換成eCatalog檢視器中使用的影像地圖。

**[!UICONTROL 使用多頁PDF自動產生eCatalog]**  — 自動從PDF檔案建立eCatalog。 eCatalog 以您上载的 PDF 文件命名。（只有当上载 PDF 文件时栅格化该文件，才可以使用此选项。）

### 分辨率

确定分辨率设置。该设置确定在 PDF 文件中每英寸显示多少像素。默认值为 150。

### 颜色空间选项

选择“颜色空间”菜单，并为 PDF 文件选择颜色空间。大多数 PDF 文件既包含 RGB 又包含 CMYK 彩色图像。对于联机查看，首选 RGB 颜色空间。

* **[!UICONTROL 自動偵測]**  — 保留PDF檔案的色域。

* **[!UICONTROL 強製為RGB]**  — 轉換成RGB色域。

* **[!UICONTROL 強製為CMYK]**  — 轉換成CMYK色彩空間。

* **[!UICONTROL 強製為灰階]**  — 轉換為灰階色彩空間。

### 色彩設定檔選項

* **[!UICONTROL 轉換為sRGB]**  — 轉換成sRGB （標準紅綠藍）。 在网页上显示图像时，推荐使用 sRGB 颜色空间。

* **[!UICONTROL 保留原始色域]**  — 保留原始色域。

* **[!UICONTROL 自訂來源]** > **[!UICONTROL 至]**  — 開啟選單，讓您能夠選擇「轉換自」和「轉換至」色域。 您可以選擇標準的Photoshop色域，或您上傳至Adobe Dynamic Media Classic的色域。

另请参阅[ ICC 配置文件](/help/icc-profiles.md#icc_profiles)。

## 從PDF檔案裁切空白字元 {#cropping-white-space-from-a-pdf-file}

1. 要在上载 PDF 文件时自动裁切其空白区域像素，请选择“裁切”菜单并选择“修剪”。
1. 指定以下选项：

   * **[!UICONTROL 修剪依據]**  — 選擇根據顏色或透明度裁切：

      * **[!UICONTROL 顏色]**  — 選擇「顏色」選項。 然後選取 **[!UICONTROL 轉角]** 功能表，然後以最能代表您要裁切之空白顏色的顏色，選擇PDF的轉角。

      * **[!UICONTROL 透明度]**  — 選擇「透明度」選項。
   * **[!UICONTROL 容許度]**  — 拖曳滑桿以指定從0到1的公差。

   * **[!UICONTROL 根據顏色修剪]**  — 指定0以裁切畫素，前提是這些畫素完全符合您在PDF角落選取的顏色。 数字越接近 1，允许的色差越大。

   * **[!UICONTROL 根據透明度修剪]**  — 指定0可裁切透明畫素；數字越接近1則透明度越高。


## 從PDF頁面側面裁切 {#cropping-from-the-sides-of-pdf-pages}

当上载 PDF 文件时，可以手动从 PDF 文件中删除页边的打印机标记。

1. 從「裁切」選單中選取 **[!UICONTROL 手動]**.
1. 在“上”、“下”、“左”、“右”文本框中输入像素设置，以便从页面的上、下及两边剪切。

页面被裁切部分的大小取决于您为 PDF 文件输入的“分辨率像素/英寸”选项。例如，假設您輸入150 （預設值）作為「解析度畫素/英吋」設定。 接著裁切頁面兩側75畫素。 在這種情況下，請輸入0.5英吋 已裁切。 若每英吋150畫素，75畫素等於半英吋。
