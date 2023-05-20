---
title: 创建图像映射
description: 瞭解如何在Adobe Dynamic Media Classic中建立影像地圖。
uuid: 0dcc4956-006e-4a74-9d6a-6d4bb23790ce
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 4eddf983-38cb-4f00-b3be-85c20bdd6f69
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: deafbd03-06bc-4d7e-87a1-5620ebcac426
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '2430'
ht-degree: 46%

---

# 创建图像映射 {#creating-image-maps}

图像映射是图像、eCatalog 页面上的区域或旋转集中的图像，显示含文本的变换面板。當使用者選取影像地圖時，就會觸發某種動作。 例如，将启动网页，供用户了解产品的更多相关信息。當使用者將指標移到「影像地圖」上時，其周圍會出現一個外框。

除了在Adobe Dynamic Media Classic中建立影像地圖功能外，您也可以在Adobe Acrobat或Adobe InDesign中設計目錄時建立影像地圖。

當您建立「影像地圖」時，可以執行下列任一項作業：

* 输入变换文本。
* 输入用于启动网页的 JavaScript 和 URL。
* 为图像映射创建 URL 模板。
* 将图像映射复制到其他图像、eCatalog 页面或旋转集。
* 把图像映射导出到 CSV 或 XML。
* 從定位字元分隔檔案或XML檔案匯入影像中繼資料。
* 定义万维网联盟所确定的其他操作。
* 预览图像映射。

## 繪製和調整影像地圖 {#drawing-and-adjusting-an-image-map}

1. 执行以下任一操作：

   * 如果您在「格點檢視」或「清單檢視」中處理影像，請在「編輯」下拉式清單中選取 **[!UICONTROL 影像地圖]**. 或者，在「詳細資料檢視」中開啟它，然後選取 **[!UICONTROL 影像地圖]** 影像上方。
   * 如果您在「格點檢視」或「清單檢視」中使用迴轉集，請選取 **[!UICONTROL 編輯]**. 或者，在「詳細資料檢視」中開啟它，然後選取 **[!UICONTROL 編輯]**. 選取影像資產，然後選取 **[!UICONTROL 影像地圖]**.
   * 如果您正在使用eCatalog，請在「格點檢視」、「清單檢視」、「詳細資料檢視」中選取 **[!UICONTROL 編輯]**. 選取 **[!UICONTROL 對應頁面]** 標籤。

   ![影像地圖影像](assets/ma_image_map.png)

1. 绘制矩形或多边形（多条边）图像映射：

   * **矩形地圖**  — 選取「矩形影像地圖」工具並在頁面上拖曳以建立矩形。 若要將點新增至矩形對映（因此將其變更為多邊形對映），請按下Ctrl，然後將插入工具置於所需位置並選取。

   * **多邊形地圖**  — 選取「多邊形影像地圖」工具，並選取要包圍的影像區域周邊上的點。 使用多边形密度滑块改变多边形中的点密度。如果选择其他映射，将记住原始密度。如果在多边形中添加、删除或移动任何点，将丢失原始密度，同时滑块重置为其最大值。

1. 如果需要，在“图像映射”列表中为图像映射输入名称。繪製影像地圖後，Adobe Dynamic Media Classic會為其指定一個名稱。

   若要建立名稱，Adobe Dynamic Media Classic會在您使用的影像或eCatalog頁面名稱后面附加一個序號。 您可以输入您选择的名称。

1. 如果您希望使用者在選取「影像地圖」時開啟新網頁，請在「影像地圖」清單中輸入URL。

   请参见[输入 JavaScript 和 URL](creating-image-maps.md#using_a_template_to_enter_javascript_and_urls)。

1. 要在用户将指针移动到图像映射上时显示变换文本，请在“图像映射”列表中输入文本。在「影像地圖」清單中，選取 **[!UICONTROL 顯示]** 功能表並選取 **[!UICONTROL 變換文字]**. 然後輸入您希望使用者在熒幕上看到的文字。 可以在文字处理程序中写入文本，然后将其复制到“变换文本”字段中。

1. 如果您希望在用户将鼠标移动到图像映射上时发生其他操作效果，请定义该操作。在 **[!UICONTROL 顯示]** 下拉式清單，選取 **[!UICONTROL 其他動作]**. 输入操作的属性。(前往 **[!UICONTROL 顯示]** > **[!UICONTROL 兩者]** 為「影像地圖」建立滑鼠指向效果文字和動作)。

   另請參閱 [定義影像地圖的其他動作](creating-image-maps.md#defining_other_actions_for_image_maps).

1. （可选）请执行下列操作之一：

   * 若要預覽影像地圖，請選取 **[!UICONTROL 預覽]**.
   * 若要刪除「影像地圖」或多邊形頂點，請選取影像上的形狀，然後選取 **[!UICONTROL 刪除]**. 或者，針對eCatalog，在「訂單頁面」標籤上選取 **[!UICONTROL 清除地圖]** 以從所有頁面中移除影像地圖。
   * 要将某个图像映射临时从图像、旋转集中的图像或 eCatalog 页面中移走而不删除，请在“图像映射”列表中取消选中相应的“开”选项。

1. 選取 **[!UICONTROL 儲存]**.

### 調整影像地圖的位置、形狀和大小 {#adjusting-the-position-shape-and-size-of-image-maps}

要更改图像映射的位置、形状和大小，请选择“图像映射”按钮 。然後，選取 **[!UICONTROL 平移]** 工具並遵循下列指示：

* **變更位置**  — 將指標移到「影像地圖」邊框附近，但不移到「影像地圖」邊框上方。 当您看见四向箭头图标时，将映射拖到新位置。

* **變更大小與形狀**  — 如何變更「影像地圖」的形狀和大小，取決於您是使用矩形或多邊形的「影像地圖」：

>[!TIP]
>
>您可以拖动屏幕底部的“大小”滑块以更改视图，使您更轻松地查看图像映射。

* **矩形影像地圖**  — 將指標移到「影像地圖」的側邊或角落上方。 当您看见双向箭头图标时，开始拖动。拖动时，按住 Shift 键，以更改大小，但保持高宽比（形状）不变。

* **多邊形影像地圖**  — 拖曳方形選取範圍控點。 若要建立選取範圍控點，請選取「影像地圖」的框線並開始拖曳。

### 處理重疊的影像地圖 {#handling-overlapping-image-maps}

如果您的图像或 eCatalog 页面包括多个图像映射且映射重叠，您可以确定映射的重叠方式。为此，请更改“图像映射”列表上映射的顺序。将它们的名称拖到列表上的更高或更低位置。名称在列表中的高低位置决定其图像映射是否重叠其他图像映射。

### 导入图像映射数据 {#importing-image-map-data}

可以将图像、旋转集或 eCatalog 的数据导入到“映射摘要”屏幕中，而不必在每个页面上都输入图像映射数据。可以通过制表符分隔的文件或 XML DTD 的形式导入图像映射数据。文件中的字段必须与“映射摘要”屏幕中显示的顺序相同：“名称”、“TOC 标签”、“映射”、“URL”、“变换文本”、“其他操作”和“搜索字符串”。导入图像映射数据可以免去创建每个图像映射时在“图像映射”列表中输入数据的麻烦。

**导入图像映射数据:**

1. 转到“图像映射”编辑器页（对于图像或旋转集中的图像）或 eCatalog 编辑屏幕的“映射页面”选项卡。
1. 選取 **[!UICONTROL 匯入中繼資料]**.
1. 在「上傳中繼資料」對話方塊中，選取「影像」或「影像地圖」，從所需的資產屬性型別上傳中繼資料。
1. 在“生成文件”下拉列表中，选择要创建的文件类型。
1. （選用）選取 **[!UICONTROL 產生]** 以根據您要建立的檔案型別預覽產生的資料。 選取 **[!UICONTROL 關閉]** 返回「上傳中繼資料」對話方塊。
1. 浏览至您要上载的文件。在“文件名”文本字段中，指定所生成文件的名称。
1. （可选）在“作业名称”字段中，指定元数据上载作业的名称。
1. 選取 **[!UICONTROL 上傳]**.

### 複製影像地圖 {#copying-image-maps}

您可以将图像映射从一个图像或 eCatalog 页面复制到另一个。使用 **[!UICONTROL 複製影像地圖]** 以搶先一步建立它們。 您也可以複製「影像地圖」，以在共用版面或對應結構的影像或頁面中重新建立它們。

例如，在 eCatalog 中复制图像映射是一种在相同 eCatalog 的不同外语版本之间复制所有图像映射的简便方式。为获得最佳结果，如果您在具有相同数量的页面和相同图像的不同 eCatalog 之间复制，则复制是最成功的。如果您複製的eCatalog已經包含「影像地圖」，則製作複製時會刪除這些「影像地圖」。

**复制图像映射:**

1. 转到“图像映射”编辑器页（对于图像或旋转集中的图像）或 eCatalog 编辑屏幕的“映射页面”选项卡。
1. 選取 **[!UICONTROL 將地圖複製到]**.
1. 根据您是从图像复制图像映射还是从 eCatalog 复制图像映射，执行下列操作之一：

   * （图像）在“选择图像”屏幕中，选择您要将图像映射复制到的图像。
   * (eCatalog) 在“选择资源”屏幕中，选择您要将图像映射复制到的图像或 eCatalog 页面。

1. 選擇 **[!UICONTROL 選取]**.

## 使用範本輸入JavaScript和URL {#using-a-template-to-enter-javascript-and-urls}

您可以定义 URL 模板（也称为 Href 模板），以便在输入图像映射 URL 时更轻松更有效。如果您的大部分图像映射 URL 都共享通用的固定格式，请定义 URL 模板。在输入固定 URL 部分以作为 URL 模板后，每次创建图像映射时，无需输入该部分 URL。您的 URL 模板也可以包含 JavaScript 命令、路径名和参数。根據預設，URL範本包含專有的Adobe Dynamic Media Classic JavaScript處理常式，稱為 `loadProduct` 會在新視窗中開啟影像。

>[!NOTE]
>
>將JavaScript程式碼新增至影像地圖的HREF屬性時，該程式碼會在使用者端的電腦上執行。 因此，請確定JavaScript程式碼是安全的。

### 关于 URL 模板 {#about-url-templates}

URL 模板的工作方式是，在模板中使用两个美元符号 (&#39;$$&#39;) 代替“图像映射”列表中 URL 列的内容：

```as3
Javascript:loadProduct(‘$$’);void(0);
```

您可以在URL範本的影像地圖之間放置所有不會變更的值。 仅仅将那些会在 URL 列中发生变化的值添加到“图像映射”列表中。例如：

* URL範本 —  `javascript:loadProduct(‘https://www.examplesitehere.com/$$’);void(0);`
* URL值 —  `product.htm`
* 實際產生的URL - `javascript:loadProduct(‘https://www.examplesitehere.com/product.html);void(0);`

依預設，URL範本包含專有的Adobe Dynamic Media Classic JavaScript處理常式，稱為 `loadProduct` 會開啟含有URL目的地的新視窗。 不過，您可以使用任何JavaScript程式碼來取代此JavaScript處理常式，或使用下列Adobe Dynamic Media Classic處理常式之一：

* `loadProductCW`  — 顯示在目前視窗的URL欄中指定的URL目標。 该处理函数主要用于集成到网站中的页面的 eCatalog。

* `loadProductPW`  — 在父視窗（開啟目前視窗的頁面）的URL欄中顯示指定的URL目標。 当前窗口仍处于打开状态，但父窗口切换为显示 URL 目标。

   >[!NOTE]
   >
   >处理程序 `loadProductPW` 不支持 DHTML 和 HTML5 查看器。

### 建立URL範本 {#creating-a-url-template}

1. 在“映射编辑器”屏幕（图像或旋转集）或 eCatalog 屏幕 (eCatalog) 的“映射页面”选项卡上，选择“URL 模板”选项旁边的“编辑”。将打开“编辑映射模板”对话框。
1. 輸入JavaScript程式碼和完整URL （以美元符號取代變數部分） [$$])。 您可以按一下滑鼠右鍵並選擇 **[!UICONTROL 貼上]**.
1. 選取 **[!UICONTROL 儲存]**.

### 處理URL範本 {#handling-url-templates}

“映射编辑器”页面（图像和旋转集）和 eCatalog 屏幕 (eCatalog) 的“映射页面”选项卡提供以下用于处理 URL 模板的命令：

* **URL範本選項**  — 選取「URL範本」選項，將您的URL範本套用至影像或eCatalog頁面上的所有影像地圖。

* **範本選項**  — 如果您不希望個別影像對映使用URL範本，請取消選取「URL影像對映」清單中的「範本」選項。

## 定義影像地圖的其他動作 {#defining-other-actions-for-image-maps}

您可以選取 **[!UICONTROL 顯示]** 功能表並選擇 **[!UICONTROL 其他動作]** 以觸發滑鼠指向效果文字和網頁啟動以外的動作。 当用户将指针移动到图像映射上时，您可以启动一个操作。这些操作是万维网联盟 HTML 规范为客户端图像映射定义的属性。它们是：

* **`accesskey`**  — 當使用者按下鍵盤上的指定按鍵時觸發動作。

* **`onfocus`**  — 當影像地圖收到焦點時觸發事件 — 透過游標、Tab鍵或按存取鍵。 例如，当图像映射被激活时，您可以启动网页，当图像映射被取消激活时，您可以将其关闭。

* **`onblur`**  — 當影像地圖失去焦點時觸發事件（游標或Tab鍵瀏覽皆然）。

**定义图像映射的其他操作:**

1. 在「地圖編輯器」畫面（影像和迴轉集）或eCatalog畫面(eCatalog)的「地圖頁面」標籤上，選取 **[!UICONTROL 顯示]** 功能表並選取 **[!UICONTROL 其他動作]**.
1. 使用由万维网联盟 HTML 规范指定的语法，在“图像映射”列表的“其他操作”列中添加支持的属性。
1. 選取 **[!UICONTROL 儲存]**.

選取 **[!UICONTROL 顯示]** 功能表並選取 **[!UICONTROL 兩者]** 如果您希望「影像地圖」有滑鼠指向效果文字和動作。

## 在Adobe Acrobat或Adobe InDesign中建立影像地圖 {#creating-image-maps-in-adobe-acrobat-or-adobe-indesign}

在 Adobe Acrobat 或 Adobe InDesign 中设计 eCatalog 时，您可以创建图像映射。

在Adobe Acrobat或Adobe InDesign中，建立您想要「影像地圖」出現的超連結參考，並指定影像地圖的URL位置。 選取「擷取連結」選項，將PDF檔案上傳至Adobe Dynamic Media Classic時，會自動將連結轉換為影像地圖。

如需詳細資訊，請參閱Adobe InDesign說明或Adobe Acrobat說明。

### 在 Adobe InDesign 中创建图像映射 {#to-create-image-maps-in-adobe-indesign}

1. 在Adobe InDesign中，前往 **[!UICONTROL Windows®]** > **[!UICONTROL 互動式]** > **[!UICONTROL 超連結]**.
1. 在「超連結」面板中，選取您要製作成「影像地圖」的文字、框架或圖形。
1. 選取 **[!UICONTROL 新增超連結]** 從面板選單中。
1. 在新增超連結對話方塊中，從 **[!UICONTROL 連結至]** 功能表，選擇 **[!UICONTROL URL]**.
1. 在URL方塊中鍵入或貼上產品ID。
1. 選取 **[!UICONTROL 確定]**. (Adobe Dynamic Media Classic會使用影像地圖URL範本完成URL。)

   >[!NOTE]
   >
   >您不需要在Adobe InDesign中設定外觀選項。 您可以在Adobe Dynamic Media Classic中指定外觀。

1. 对于您想要创建的所有图像映射，重复步骤 2 到 6。
1. 将文件导出为 PDF。
1. 將PDF上傳至Adobe Dynamic Media Classic。
1. 在 **[!UICONTROL PDF選項]**，選取 **[!UICONTROL 擷取連結]**.

### 在 Adobe Acrobat 中创建图像映射 {#to-create-image-maps-in-adobe-acrobat}

1. 在Adobe Acrobat中，前往 **[!UICONTROL 工具]** > **[!UICONTROL 進階編輯]** > **[!UICONTROL 連結工具]**.
1. 拖动以创建图像映射。
1. 在建立連結方塊中，選取 **[!UICONTROL 自訂連結]**，並選取 **[!UICONTROL 下一個]**.

>[!NOTE]
>
>您不需要在Adobe Acrobat中設定外觀選項。 您可以在Adobe Dynamic Media Classic中指定外觀。

1. 在「連結屬性」方塊中，選取 **[!UICONTROL 動作]**.
1. 選取 **[!UICONTROL 開啟網頁連結]** 從「選取動作」功能表，然後選取 **[!UICONTROL 新增]**.
1. 在「編輯URL」方塊中輸入「影像地圖」的產品ID，然後選取 **[!UICONTROL 確定]**. (Adobe Dynamic Media Classic會使用影像地圖URL範本完成URL。)
1. 对于您想要创建的所有图像映射，重复步骤 1 到 7。
1. 保存文件。
1. 將PDF上傳至Adobe Dynamic Media Classic，然後從「PDF選項」中選取「擷取連結」 。
