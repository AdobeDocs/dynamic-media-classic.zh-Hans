---
title: 建立eCatalog影像地圖
description: 瞭解如何在Adobe Dynamic Media Classic中建立eCatalog影像地圖。
uuid: 943ad3f7-a885-4bc2-88cb-77083384bdf8
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
discoiquuid: 4cf63359-63b5-4da7-9498-335d91b4776c
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: 5e7f39a5-36a6-40df-8752-064a582c9346
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '1492'
ht-degree: 40%

---

# 建立eCatalog影像地圖{#creating-ecatalog-image-maps}

「影像地圖」是eCatalog頁面上的區域，您可以用滑鼠滑鼠滑動，或選取它來觸發各種動作。 例如，當您將指標移到「影像地圖」上時，您會看到專案的滑鼠指向效果文字說明。 當您選取「影像地圖」時，會起始另一個動作。 例如，您可以打开网页，以便查看器可以更多地了解一个项目或购买它，您还可以启动视频来查看使用中的项目。

## 繪製eCatalog影像地圖 {#drawing-ecatalog-image-maps}

对于 eCatalog，可以在 eCatalog 屏幕的“映射页面”选项卡上绘制图像映射。该屏幕包括显示 eCatalog 页面的图像映射区域，右侧显示“图像映射”列表。创建图像映射时，其名称会输入到“图像映射”列表中。

1. 選取eCatalog的變換 **[!UICONTROL 編輯]** 按鈕。
1. 選取 **[!UICONTROL 對應頁面]**.
1. 在“映射页面”屏幕的左侧，选择所需页面。
1. 在“图像映射”区域中，绘制一个矩形或多边形（多个边）图像映射：

   * **矩形地圖**  — 選取「矩形影像地圖」工具並在頁面上拖曳以建立矩形。

   * **多邊形地圖**  — 選取「多邊形影像地圖」工具，然後視需要多次選取影像周邊。 當您選取時，Adobe Dynamic Media Classic會繪製影像地圖的邊界。

      繪製「影像地圖」後，Adobe Dynamic Media Classic會在「影像地圖」清單中為其指定一個名稱。 若要形成名稱，Adobe Dynamic Media Classic會在您正在使用的eCatalog頁面名稱后面附加一個序號。

1. （選用）從「影像地圖」清單的 [!UICONTROL 名稱] 欄中，您可以為「影像地圖」輸入新名稱。 输入的名称中不能包含空格。
1. 您可以讓檢視者在選取「影像地圖」時開啟新的網頁。 在“图像映射”列表面板中的“URL”列中输入网页的 URL。

   若要更輕鬆地輸入URL （Href範本），請選取 **[!UICONTROL 編輯]** 並輸入範本。

另請參閱 [使用範本輸入JavaScript和URL](creating-image-maps.md#using_a_template_to_enter_javascript_and_urls).

1. （選用）在「顯示」下拉式清單中，選取 **[!UICONTROL 變換文字]**，然後輸入您希望使用者在影像地圖上移動指標時於熒幕顯示的文字。
1. （選用）在「顯示」下拉式清單中，選取 **[!UICONTROL 其他動作]**，並輸入屬性，以在使用者在影像地圖上移動指標時觸發模糊或聚焦動作。

   另請參閱 [定義影像地圖的其他動作](creating-image-maps.md#defining_other_actions_for_image_maps).

1. 選取 **[!UICONTROL 儲存]**.
1. （選用）選取 **[!UICONTROL 預覽]** 以檢視具有預設eCatalog檢視器預設集的eCatalog。

若要刪除「影像地圖」，請在「影像地圖」清單中選取其名稱，然後選取 **[!UICONTROL 刪除]**. 要在页面中临时禁用图像映射而不删除该图像映射，可以在“图像映射”列表面板上取消选择图像映射的“开”选项。

## 在eCatalog中內嵌多媒體 {#embedding-rich-media-in-an-ecatalog}

可以使用 eCatalog 的富媒体选项向已添加到 eCatalog 的图像映射添加 MP4 格式的视频或旋转集。當使用者選取eCatalog中的「影像地圖」區域時，會顯示相關的迴轉集或影片。 如果想要客户查看使用中的项目，或者从不同的角度和透视图查看项目，此功能将特别有用。

您也可以選擇在客戶將指標移動到您的影像地圖上時顯示工具提示文字，讓他們知道自己選擇什麼。

**要在 eCatalog 中嵌入富媒体:**

1. 绘制 eCatalog 图像映射。

   另請參閱 [繪製eCatalog影像地圖](creating-ecatalog-image-maps.md#drawing_ecatalog_image_maps).

1. 在「顯示」下拉式清單中，選取 **[!UICONTROL 多媒體]**.
1. 在左侧的“添加资源”面板中，导航到要嵌入的旋转集或视频（MP4 格式）资源所在的文件夹。
1. 将资源拖动到图像映射上。
1. （選用）在「影像地圖」清單面板的 **[!UICONTROL 工具提示]** 欄標題，輸入檢視者在將指標移至「影像地圖」上方時，要在熒幕上看到的文字。
1. 選取 **[!UICONTROL 儲存]**.

## 编辑 eCatalog 图像映射 {#editing-ecatalog-image-maps}

从 eCatalog 屏幕的“映射页面”选项卡上开始，使用以下方法来编辑 eCatalog 图像映射：

* **調整位置**  — 選取「平移」工具，並將指標移到地圖邊框附近，但不會移到邊框上。 当指针显示为四向箭头时，将图像映射拖动到新位置。

   另請參閱 [調整影像地圖的位置、形狀和大小](creating-image-maps.md#adjusting_the_position_shape_and_size_of_image_maps).

* **變更形狀和大小**  — 若要調整矩形影像地圖的大小，請選取平移工具。 然后将指针移动到边框或角上，看到双向箭头图标时进行拖动。要调整多边形图像映射的大小，请拖动正方形选择手柄。若要建立選取範圍控點，請選取「影像地圖」的邊框並拖曳。

   另請參閱 [調整影像地圖的位置、形狀和大小](creating-image-maps.md#adjusting_the_position_shape_and_size_of_image_maps).

* **刪除影像地圖**  — 選取「平移」工具，選取「影像地圖」以選取它，然後選取 **[!UICONTROL 刪除]**.

   若要從eCatalog中移除所有影像地圖，請選取 **[!UICONTROL 排序頁面]** 標籤，然後選取 **[!UICONTROL 清除地圖]**.

* **處理重疊的影像地圖**  — 拖曳以變更「影像地圖」清單上的「影像地圖」順序。

   另請參閱 [處理重疊的影像地圖](creating-image-maps.md#handling_overlapping_image_maps).

* **複製影像地圖至其他頁面**  — 選取 **[!UICONTROL 將地圖複製到]** （請確定您位於「地圖頁面」索引標籤上）。 在「選取影像」畫面上，選取您要複製「影像地圖」的一個或多個頁面，然後選取 **[!UICONTROL 選取]**.

   另請參閱 [將影像地圖複製至其他影像](creating-image-maps.md#copying_image_maps).

>[!NOTE]
>
>除了將影像地圖複製到eCatalog中的不同頁面之外，您還可以將eCatalog中的所有影像地圖複製到不同的eCatalog。 另請參閱 [在eCatalog之間複製影像地圖](creating-ecatalog-image-maps.md#copying_image_maps_between_ecatalogs).

## 檢閱和匯入影像地圖資料 {#reviewing-and-importing-image-map-data}

“映射摘要”屏幕提供了关于您的 eCatalog 的元数据。也可以从“映射摘要”屏幕开始为 eCatalog 批量导入图像映射数据。用这种方法导入图像映射数据可以简化图像映射 URL 及变换文本的输入。

若要檢視「地圖摘要」畫面，請在eCatalog畫面的「地圖頁面」標籤上選取 **[!UICONTROL 摘要]**.

### 检查图像映射数据摘要 {#review-image-map-data-summary}

1. 在「對應頁面」畫面上，選取「 」 **[!UICONTROL 摘要]**.

   “映射摘要”屏幕显示 eCatalog 中图像映射、URL、变换文本说明以及其他操作的数量。

1. 如果出現滑鼠指向效果索引鍵錯誤，請選取 **[!UICONTROL Rollover_Key錯誤]** 欄，檢視您的試算表中必須變更哪些專案才能更正錯誤。 可以选择并复制该消息的文本，并将其粘贴到电子表格中。
1. 選取 **[!UICONTROL 預覽]** 因此您可以在eCatalog Viewer中檢查頁面；選取X以關閉「摘要」畫面並返回「對應頁面」畫面，或選取 **[!UICONTROL 關閉]** 以返回「瀏覽」。

### 导入图像映射数据 {#import-image-map-data}

可以将整个 eCatalog 的数据导入到“映射摘要”屏幕中，而不必在每个页面都输入图像映射数据。可以通过制表符分隔的文件或 XML DTD 的形式导入图像映射数据。文件中的字段必须与“映射摘要”屏幕中显示的顺序相同：“名称”、“TOC 标签”、“映射”、“URL”、“变换文本”、“其他操作”和“搜索字符串”。导入图像映射数据可以免去创建每个图像映射时在“图像映射”列表中输入数据的麻烦。

>[!NOTE]
>
>在导入图像映射数据之前，必须已经创建图像映射。

在“映射摘要”屏幕上开始，按照以下步骤为创建的图像映射导入图像映射数据：

1. 選取 **[!UICONTROL 匯入地圖資料]**.
1. 在「匯入中繼資料」對話方塊中，選取 **[!UICONTROL 瀏覽]**，然後選取定位點分隔或XML DTD檔案。
1. 在“作业名称”字段中，键入文件的名称（注意保留其扩展名）。
1. 選取 **[!UICONTROL 上傳]**.

## 在eCatalog之間複製影像地圖 {#copying-image-maps-between-ecatalogs}

可以将 eCatalog 中的所有图像映射复制到其他 eCatalog 中。这种复制图像映射的方法是在相同的 eCatalog 的外语翻译之间复制图像映射的方便方法。為了成功複製，Adobe Dynamic Media Classic建議您在具有相同頁數和相同影像的eCatalog之間複製。

>[!NOTE]
>
>如果图像映射所复制到的 eCatalog 已经包含图像映射，复制时将删除原有的图像映射。

若要將一個eCatalog中的所有影像地圖複製到另一個eCatalog，請執行下列動作：

1. 選取包含您要複製之影像地圖的eCatalog，然後選取eCatalog的變換影像 **[!UICONTROL 編輯]** 按鈕。
1. 在「排序頁面」標籤上，選取 **[!UICONTROL 複製地圖]**.
1. 在「選取資產」對話方塊中，選取您要複製「影像地圖」的eCatalog，然後選取 **[!UICONTROL 選取]**.

如果目標eCatalog （您複製影像地圖的eCatalog）具有不同數量的頁面或不同大小的影像，Adobe Dynamic Media Classic會顯示警告訊息。 選取 **[!UICONTROL 繼續]** 以複製影像地圖，無論是否有警告。
