---
title: 管理eCatalogs中的資訊面板內容
description: 瞭解如何在Adobe Dynamic Media Classic中管理eCatalogs中的資訊面板內容。
uuid: 5aa634f9-0874-4bb5-a3d9-8ce4d5577941
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
discoiquuid: be277831-77cc-4011-ae30-e75c18eec99b
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: bfb9c5a4-5068-4adb-9fe2-a4ead8656289
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '866'
ht-degree: 59%

---

# 管理eCatalogs中的資訊面板內容{#managing-info-panel-content-in-ecatalogs}

除了在 eCatalog 中将图像映射文本用于变换之外，还可以使用“信息面板”添加大量变换文本（包括链接）。还可以使用定时缓存和计划内容更新来管理信息面板。

您可以使用Adobe Dynamic Media Classic中的下列功能來管理資訊面板設定和資料：

* “信息面板设置”面板可用来指定用于显示“信息面板”文本、默认错误响应以及信息缓存的小时数等信息的模板。此外，可以指定是否自动发布 eCatalog。
* 「資訊」「面板資料摘要」面板可讓您指定CSV檔案，其中包含您要顯示在「資訊」「面板」滑鼠指向效果文字中的文字，以及更新資訊的排程時間。
* “导入元数据”对话框（从“映射页面”视图访问）可用来导入包含变换文本信息的制表符分隔 TXT 文件。可以将该 TXT 选项或“数据输入”面板与“CSV 文件”选项结合，用于变换文本。
* “映射页面”视图提供了用于预览为特定图像映射而显示的 XML 的选项。

## 設定eCatalog的回應範本 {#set-up-a-response-template-for-ecatalogs}

可以选择三个预设响应模板之一用来在“信息面板”中显示文本。这些预设响应模板决定了在“信息面板”中显示信息的方式：列数和行数、字样大小、字体等等。可以选择预设响应模板，或者创建一个自己的模板。

>[!NOTE]
>
>也可以在“查看器预设”中设置响应模板。若要改用檢視器預設集中的回應範本，請新增 `fmt=1` 到檢視器預設集中的Information Server URL結尾。
>
>另請參閱 [設定eCatalog檢視器預設集](setting-ecatalog-viewer-presets.md#setting_up_ecatalog_viewer_presets).

1. 連按兩下eCatalog，使其在「詳細資料檢視」中開啟。
1. 選取 **[!UICONTROL 資訊面板設定]** 面板。
1. 选择“响应模板”：

   * 从“响应模板”菜单中选择预设。模板设计的 XML 显示在“用户模板”框中。
   * 若要建立您自己的回應範本，請選取 **[!UICONTROL 自訂]**. 在“用户模板”框中键入模板 XML 定义。可以将预设模板作为您自己的模板的基础。

1. （可選）在「預設回應」方塊中，輸入您要在Adobe Dynamic Media Classic擷取影像地圖資訊時發生錯誤，顯示的文字。 例如，如果系统收到公司名称和 eCatalog 名称，但是没有变换标识符，则将为用户显示该消息。
1. 在“响应 TTL”框中，输入要在缓存数据之前等待的小时数：

   * 如果在一整天内需要频繁更新数据，则设置一个较小的值。
   * 如果数据相对稳定并且不需要整天频繁更新，则设置一个较大的值。默认为十小时。

1. 選取 **[!UICONTROL 發佈]**.

## 匯入eCatalogs中資訊面板的來源內容 {#import-source-content-for-the-info-panel-in-ecatalogs}

可以为 eCatalog 的“信息面板”源文本使用逗号分隔值文件 (CSV) 或制表符分隔文件 (TXT)。制表符分隔文件必须使用 UTF16 (Unicode) 编码。使用不同的方法导入不同的文件类型。

格式化源内容时，谨记以下指导原则：

* 确保制表符分隔数据和逗号分隔数据包含变换模板所必需的列数。
* 确保数据的第一项或列是变换标识符（与图像映射 URL 的 rollover_key 值关联）。
* 確認識別碼之後的每個定位字元或逗號分隔專案都是您要取代至回應範本的專案。因此，第一欄會取代為$1$，第二欄會取代為$2$，依此類推。

### 從外部託管位置將CSV內容匯入eCatalog {#import-csv-content-into-ecatalogs-from-an-externally-hosted-location}

1. 連按兩下eCatalog，使其在「詳細資料檢視」中開啟。
1. 選取 **[!UICONTROL 資訊面板資料摘要]** 面板。
1. 在“外部承载的 CSV 文件位置”框中，输入 CSV 文件的 URL。可以将 URL 粘贴至该字段，或直接键入。
1. （可選）使用「排程更新」功能表指定更新內容的時間，然後選取 **[!UICONTROL 新增]**. 可以选择多个更新时间。每个更新时间显示在“更新时间”框中。(若要移除時間，請選取該時間，然後選取 **[!UICONTROL 刪除]**.)
1. （選用）選取 **[!UICONTROL 立即執行更新]** 立即更新內容。

### 导入制表符分隔文件或 CSV 文件 {#import-a-tab-delimited-or-csv-file}

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>SR changed this section 10/23/2012</p>

 -->

1. 連按兩下eCatalog，使其在「詳細資料檢視」中開啟。
1. 選取 **[!UICONTROL 資訊面板設定]** 面板。
1. 選取 **[!UICONTROL 上傳S7Info內容]**.
1. 選取 **[!UICONTROL 瀏覽]**，選取您要使用的Tab字元分隔的TXT檔案、CSV或SSV檔案，然後選取 **[!UICONTROL 開啟]**.
1. 選取 **[!UICONTROL 上傳]**.

Adobe Dynamic Media Classic會傳送電子郵件訊息給您，讓您知道上傳是否成功。

## 预览图像映射的变换键文本 {#preview-rollover-key-text-for-an-image-map}

使用“映射页面”屏幕，您可以快速、轻松地查看 eCatalog 特定页面上“图像映射”的“信息面板”文本。

1. 選取目錄的變換影像 **[!UICONTROL 編輯]** 按鈕。
1. 選取 **[!UICONTROL 對應頁面]**.
1. 在熒幕右側的表格頂端，選擇 **[!UICONTROL 資訊面板]** 從「顯示」功能表。

   变换键文本显示在包含“信息面板”文本的每个图像映射旁。
