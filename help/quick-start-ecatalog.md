---
title: 「快速入門：eCatalogs」
description: eCatalogs簡介和快速入門，可幫助您在Adobe Dynamic Media Classic中快速上手並執行eCatalog技術。
uuid: 1ec41927-3df6-4845-8d9d-bb92cf6dca08
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
discoiquuid: 781dacd0-ef0c-42b7-92e0-12791994874d
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: 9e2df814-465d-412a-a032-ef3e8cb462ba
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '1559'
ht-degree: 36%

---

# 快速入門：eCatalogs{#quick-start-ecatalogs}

eCatalog 是数字网络版本的印刷材料，例如目录、小册子、传单、产品手册或广告传单。eCatalog 显示在网站的 eCatalog 查看器中。该查看器会模拟阅读印刷材料的体验。

另請觀看下列訓練影片：

* [快速入門1：eCatalogs](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/561_Quick%20Start%20-%20Part%201_converted%20renamed_eCatalogs-AVS)
* [快速入門2：eCatalogs](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/562_Quick%20Start%20-%20Part%202_converted%20renamed_eCatalogs-AVS)

根據您為eCatalog選擇的設定，檢視器可讓您執行下列動作：

* 在目錄中搜尋一或多個關鍵字。 搜尋結果會在目錄左側的搜尋面板中顯示為縮圖清單。 每個可點按的縮圖代表目錄跨頁，其中會找到反白顯示的搜尋字詞。

* 透過社群媒體分享目錄；下載目錄以離線檢視；啟用「我的最愛」以標籤您要快速返回的專案，或列印目錄。
* 使用目錄或頁面格線檢視來瀏覽目錄；按一下頁面中邊緣可向前或向後瀏覽頁面。
* 放大、缩小及平移以仔细查看页面上的物品。
* 將指標移到頁面區域（稱為影像地圖）上，以便看到包含專案相關資訊的快顯視窗。
* 選取頁面區域，開啟包含專案詳細資訊的新網頁。
* 写入附注，并将其附加到 eCatalog 页面。
* 如果您想要啟動相關網頁或內容資訊面板，請點選影像地圖圖示。
* 使用手势交互，包括捏合缩放和点刷转页。
* 按关键字搜索物品。

![向使用者顯示的eCatalog。 A) eCatalog開啟頁面。 B)eCatalog已翻到第2頁。](/help/assets/ec_cat_viewer_popup.png)

若要建立eCatalog，您通常會使用在Adobe Acrobat或其他列印程式中建立的高解析度PDF檔案，但您也可以從影像檔案建立eCatalog。

创建 eCatalog 过程中，可以按照所选顺序排列页面或跨页。也可以声明需要单页、双页跨页，还是多页跨页。您可以為頁面區域建立影像地圖，讓檢視者可以選取頁面上的某個區域，並在您的網站上開啟新頁面。 可以使用 eCatalog 屏幕内的“信息面板”设置来管理显示的变换文本。也可以从 100 多个不同的配置选项中选择，以配置 eCatalog 查看器。您可以为特殊受众定制查看器的功能和外观。

>[!NOTE]
>
>如果您是Dynamic Media - Scene7模式使用者，並且想要使用eCatalog，請編輯 `pdfbrochure` CRXDE Lite中的值。 若要這麼做，請在Adobe Experience Manager中前往 **[!UICONTROL 工具]** > **[!UICONTROL 一般]** > **[!UICONTROL CRXDE Lite]**. 在左側面板導覽樹狀結構中，導覽至 `/conf/global/settings/cloudconfigs/dmscene7/jcr:content/mimeTypes/application_pdf`.
>
>在右下方的窗格中， **[!UICONTROL 屬性]** 索引標籤中，選取 `jobParam` 列。 設定值 `pdfbrochure` 從 `false` 至 `true`. 如在 `pdfbrochure=true`
>
>在CRXDE Lite頁面的左上角，選取 **[!UICONTROL 全部儲存]**.
>
>您現在可以在Adobe Dynamic Media Classic中撰寫eCatalogs。

本 eCatalog 快速入门旨在帮助您快速学会如何使用 eCatalog。按照步骤 1 到 7 操作。每個步驟之後，都會有主題標題的互動參照，讓您在其中找到更多資訊。

## 1.上傳PDF檔案

eCatalog 通常由 Adobe PDF 文件生成。由于 PDF 文件要用于印刷，因此通常包含 CMYK 图像。Adobe Dynamic Media Classic會偵測這些影像，並使用標準CMYK色彩設定檔進行轉換。 不過，您必須上傳並使用自訂色彩設定檔。

在全域導覽列上，選取 **[!UICONTROL 上傳]** 以開始上傳eCatalog的PDF檔案或影像。 可以从桌面或通过 FTP 上载文件；如果上载大量文件或大于 100 MB 的文件，则推荐使用 FTP。

“上载”屏幕的“PDF 选项”下面提供了一些选项，用于上载分辨率合适并且颜色空间正确的 PDF 文件。推荐使用 150 PPI 的分辨率。上载 PDF 文件时，可以选择“自动生成 eCatalog”选项来创建 eCatalog。

另請參閱 [上傳PDF檔案](uploading-pdf-files.md#uploading_the_pdf_files).

## 2.建立eCatalog

在「瀏覽」面板中選取PDF或影像檔案，以建立您的eCatalog。 選取 **[!UICONTROL 建置]**，然後選擇 **[!UICONTROL eCatalogs]**.

在eCatalog頁面的 **[!UICONTROL 排序頁面]** 索引標籤中，選取「版面」選項： **[!UICONTROL 1欄式]**， **[!UICONTROL 2欄式]**，或 **[!UICONTROL 自訂]**. 可以通过拖动的方式，或者在大型 eCatalog 中在“移至”菜单中选择页面名称，来重新排列页面或跨页。

要添加页面，在“资源库”中选择一个文件夹，然后将其中的 PDF 或图像文件拖动到“排序页面”屏幕中。您可以提供自訂頁面名稱或匯入許多頁面名稱，而不是預設頁碼。

選取 **[!UICONTROL 儲存]**，輸入eCatalog的名稱，選擇用來儲存的Adobe Dynamic Media Classic資料夾，然後選取 **[!UICONTROL 儲存]**. 每次變更頁面順序或編輯eCatalog時，請按一下以儲存變更 **[!UICONTROL 儲存]**.

另請參閱 [建立eCatalog](creating-ecatalog.md).

## 3.建立影像地圖

「影像地圖」為eCatalog頁面新增了另一個面向。 图像映射是页面上的一个区域，可提供关于某个物品的更多信息。当观众在“图像映射”上滚动鼠标指针时，他们会看到物品的说明。单击“图像映射”会激活一个外部引用，该引用打开一个新的网页，您可以从中了解关于某个物品的更多信息。

要创建图像映射，打开 eCatalog 屏幕。然後前往 **[!UICONTROL 對應頁面]** 標籤，並使用「矩形影像地圖」工具或「多邊形影像地圖」工具將地圖框架化。 可以使用“平移”工具  拖动映射边框来调整“图像映射”的位置和大小。

在設定「影像地圖」的框架後，輸入當您選取「影像地圖」時要前往的URL位址。 也可以输入当您将指针移动到图像映射上时所显示的变换文本。

另請參閱 [建立eCatalog影像地圖](creating-ecatalog-image-maps.md#creating-ecatalog-image-maps).

另請參閱 [使用影像地圖在eCatalog中內嵌多媒體](creating-ecatalog-image-maps.md#embedding-rich-media-in-an-ecatalog).

可以在 eCatalog 屏幕中使用“信息面板”设置来建立和管理图像映射文本。

另請參閱 [管理eCatalogs中的資訊面板內容](/help/info-panel-content-ecatalog.md).

## 4.設定eCatalog檢視器預設集

最终用户在“eCatalog 查看器中”看到您的 eCatalog。如果您是管理员，还可以配置 eCatalog 查看器。可以更改其轮廓颜色，并选择新的“外观”来确立 eCatalog 品牌。Adobe Dynamic Media Classic隨附數個「最佳實務」 eCatalog檢視器預設集。 可以选择这些预设中的一个预设来显示 eCatalog。如果您是管理员，还可以创建自己的 eCatalog 查看器预设。

若要建立eCatalog檢視器預設集，請在全域導覽列上選取 **[!UICONTROL 設定]**，然後選擇 **[!UICONTROL 檢視器預設集]**. 選取 **[!UICONTROL 新增]**，選擇平台，然後選取 **[!UICONTROL eCatalog]** > **[!UICONTROL 檢視器]**.

另請參閱 [設定eCatalog檢視器預設集](setting-ecatalog-viewer-presets.md#setting-up-ecatalog-viewer-presets).

## 5.在eCatalog檢視器中預覽eCatalog

eCatalog 查看器预设决定了 eCatalog 查看器的样式和行为。

若要瞭解eCatalog檢視器預設集如何顯示您的eCatalog，請在「瀏覽」面板中選取您的eCatalog，然後選取 **[!UICONTROL 預覽]**. “预览”屏幕随即在默认查看器中打开。

注意方向、配色方案、更改页面的控件的外观以及页面翻转时的显示效果。

另請參閱 [在eCatalog檢視器中預覽eCatalog](previewing-ecatalogs-ecatalog-viewer.md#previewing-ecatalogs-in-the-ecatalog-viewer).

## 6.發佈eCatalog和相關PDF

發佈eCatalog和相關PDF時，會將它置於Dynamic Media影像伺服器上，以便傳送至您的網站和應用程式。 在發佈程式中，Adobe Dynamic Media Classic會啟動eCatalog的URL字串。 使用此URL從Dynamic Media影像伺服器呼叫eCatalog至您的網站或應用程式。

在「瀏覽」面板中將eCatalog和PDF標籤為發佈後，選取「全域導覽」列上的「發佈」按鈕以啟動發佈。 在「發佈」畫面上，選取「 」 **[!UICONTROL 提交發佈]**.

另請參閱 [發佈eCatalog和相關PDF](publishing-ecatalogs-associated-pdfs.md#publishing-ecatalogs-and-associated-pdfs).

## 7.將eCatalog連結至網頁

當您將eCatalog發佈至Adobe Dynamic Media Classic影像伺服器時，Dynamic Media會啟用顯示所需的URL圖說文字字串。 您可以選取面板中的URL，從「預覽」畫面和「瀏覽」面板（在「詳細資料檢視」中）複製此URL字串。 复制 URL 字符串之后，该 URL 便可用于您的网站和应用程序。

与您的 IT 团队合作，将 eCatalog 链接放在网页中的合适位置。當使用者選取連結時，eCatalog檢視器會出現，使用者可以瀏覽您的eCatalog。

另請參閱 [將eCatalog連結至網頁](linking-ecatalog-web-page.md#linking-an-ecatalog-to-a-web-page).
