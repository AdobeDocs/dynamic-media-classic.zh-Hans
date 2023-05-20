---
title: 使用PSD檔案
description: 瞭解如何在Adobe Dynamic Media Classic中使用PSD檔案。
uuid: 5836b660-6bca-46e7-ab39-1a31d1e0cff2
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 4086e3db-5aca-41a0-8f15-302afbf67ddb
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: e3b8c4b9-e9c4-4d7f-84de-2efb456755a1
source-git-commit: dc1ec666b208cec8fffe836d64ed501f6ccf4e7b
workflow-type: tm+mt
source-wordcount: '1003'
ht-degree: 25%

---

# 使用PSD檔案{#working-with-psd-files}

<!--   USED TO BE AN OPTION UNDER COLOR PROFILE OPTIONS * **Convert To sRGB (default)** - Converts to sRGB (Standard Red Green Blue). sRGB is the recommended color space for displaying images on web pages. -->

PSD (Photoshop檔案檔案)最常用於Adobe Dynamic Media Classic中建立範本。 上傳PSD檔案時，您可以從檔案中自動建立Adobe Dynamic Media Classic範本（在「上傳」畫面上選取「建立範本」選項）。

如果您使用檔案來建立範本，Adobe Dynamic Media Classic會從含有圖層的PSD檔案建立多個影像；它會為每個圖層建立一個影像。

## PSD 上载选项 {#psd-upload-options}

上傳PSD檔案的選項位於「上傳工作選項」對話方塊中的「Photoshop選項」下。 您可以裁切文件、为其选择颜色配置文件、使用该文件创建模板，以及选择锚点。

以下选项在上载 PSD 文件时可用：

* **裁切選項**  — 位於 **[!UICONTROL 裁切選項]**. 選取 **[!UICONTROL Trim]** 自動裁切PSD檔案邊緣的空白字元；選取 **[!UICONTROL 手動]** 裁切PSD檔案的側邊：

   * **[!UICONTROL Trim]**  — 選取 **[!UICONTROL 修剪依據]** 功能表，然後選擇 **[!UICONTROL 顏色]** 或 **[!UICONTROL 透明度]**.
   如果您選擇 **[!UICONTROL 顏色]** 選項，選取「轉角」選單，然後選擇最能代表您要裁切之空白區域顏色的PSD轉角。

   拖曳滑桿以指定從0到1的公差。 基于颜色修剪时，如果指定为 0，则仅裁切与 PSD 角中选定颜色精确匹配的像素。数字越接近 1，允许的色差越大。若要根據透明度進行裁剪，請指定0來裁切透明畫素；數字越接近1則透明度越高。

   * **[!UICONTROL 手動]**  — 輸入影像任何一面或兩面裁切的畫素數。 图像被裁切部分的大小取决于图像文件中的 ppi（像素/英寸）设置。例如，如果影像顯示150 ppi，而您在「上」、「右」、「下」和「左」文字方塊中輸入75，則以0.5英吋。 會從影像的每一側裁切。


* **色彩設定檔選項**  — 位於 **[!UICONTROL 色彩設定檔選項]**.

   * **[!UICONTROL 默认护色]**

   * **[!UICONTROL 保留原始色域]**  — 保留影像的原始色域。

   * **[!UICONTROL 自訂來源]** > **[!UICONTROL 至]**  — 開啟選單，讓您能夠選擇「轉換自」和「轉換至」色域。 您可以選擇標準的Photoshop色域，或您上傳至Adobe Dynamic Media Classic的色域。 请参阅[ICC 配置文件](/help/icc-profiles.md)。

* **Photoshop 选项**

   * **[!UICONTROL 保留圖層]**  — 將PSD中的圖層（如果有的話）擷取到個別資產中。 资源图层仍然与 PSD 关联。您可以在「詳細資料檢視」中開啟PSD檔案，並選取圖層面板來檢視它們。 请参阅查看和编辑 PSD 文件中的图层。

   * **[!UICONTROL 建立範本]**  — 從PSD檔案中的圖層建立範本。

   * **[!UICONTROL 擷取文字]**  — 擷取文字，讓使用者能在檢視器中搜尋文字。

   * **[!UICONTROL 將圖層延伸至背景大小]**  — 將擷取的影像圖層大小延伸至背景圖層大小。

   * **[!UICONTROL 圖層命名]** -PSD檔案中的圖層會以個別影像上傳。 若要在Adobe Dynamic Media Classic中命名這些影像，請從下列選項中選擇：

      * **[!UICONTROL 圖層名稱]**  — 在PSD檔案中，以影像的圖層名稱來命名影像。 例如，原始 PSD 文件中名为“Price Tag”的图层将成为名为“Price Tag”的图像。不過，如果PSD檔案中的圖層名稱是預設的Photoshop圖層名稱（「背景」、「圖層1」、「圖層2」等），則會以影像在PSD檔案中的圖層編號來命名影像。 <!-- not their default layer names -->

      * **[!UICONTROL Photoshop和圖層編號]**  — 將影像命名為PSD檔案中的圖層編號後方，略過原始圖層名稱。 使用 Photoshop 文件名和附加的图层编号为图像命名。例如，檔案的第二層，稱為 `Spring Ad.psd` 已命名 `Spring Ad_2` 即使它在Photoshop中有非預設名稱。

      * **[!UICONTROL Photoshop和圖層名稱]**  — 在PSD檔案後面加上圖層名稱或圖層編號來命名影像。 如果 PSD 文件中的图层名称是默认的 Photoshop 图层名称，则将使用图层编号。例如，名為 `Price Tag` 在名為的PSD檔案中 `SpringAd` 已命名 `Spring Ad_Price Tag`. 系統會呼叫預設名稱為「圖層2」的圖層 `Spring Ad_2`.
   * **[!UICONTROL 錨點]**  — 指定影像在範本中的錨定方式，範本是從PSD檔案產生的分層構成產生的。 默认情况下，锚点是中心。中心锚点允许替换图像尽可能占据相同的空间，无论替换图像的高宽比是多少。当引用模板并使用参数替换时，替换该图像的高宽比不同的图像有效地占据相同的空间。如果应用程序要求替换图像占据模板中分配的空间，请更改为其他设置。


## 在PSD檔案中檢視和編輯圖層 {#viewing-and-editing-layers-in-a-psd-file}

如果您在上傳PSD時選取了「保留圖層」選項，Adobe Dynamic Media Classic會將個別圖層擷取到資產中。 您可以在「詳細資訊檢視」的「瀏覽」面板中開啟檔案，以檢視和編輯屬於PSD檔案的資產圖層。

>[!NOTE]
>
>Adobe Dynamic Media Classic在巢狀圖層群組中最多可支援五個層級。

1. 在「瀏覽」面板中，按兩下完整PSD檔案。 檔案會在「詳細資料檢視」中開啟。

   >[!NOTE]
   >
   >请确保您打开的是完整资源，而不是某一个 PSD 图层。

1. 選取 **[!UICONTROL 圖層]**. 在“图层”面板中将以单独的图像显示所有各图层。
1. 連按兩下圖層，然後執行下列任一項作業：

   * 若要在圖層上建立影像地圖，請選取 **[!UICONTROL 影像地圖]** 圖示。 (請參閱 [建立影像地圖](creating-image-maps.md#creating_image_maps).)
   * 若要在圖層上建立縮放目標，請選取 **[!UICONTROL 縮放目標]** 圖示。 (請參閱 [建立引導式縮放的縮放目標](creating-zoom-targets-guided-zoom.md#creating_zoom_targets_for_guided_zoom).)
   * 若要裁切圖層，請選取 **[!UICONTROL 裁切]** 圖示。 (請參閱 [裁切影像](cropping-image.md#cropping_an_image).)
   * 若要銳利化圖層，請選取 **[!UICONTROL 銳利化]**. (請參閱 [銳利化影像](sharpening-image.md#sharpening_an_image).)
   * 若要調整圖層，請選取 **[!UICONTROL 調整]**. (請參閱 [調整影像](adjusting-image.md#adjusting_an_image).)

1. 選取 **[!UICONTROL 儲存]** 或 **[!UICONTROL 另存為]**.
1. 若要檢視或編輯不同的圖層，請選取圖層預覽底部的箭頭。
1. 若要退出圖層「詳細資料檢視」，請選取 **[!UICONTROL 格點檢視]** 圖示。
