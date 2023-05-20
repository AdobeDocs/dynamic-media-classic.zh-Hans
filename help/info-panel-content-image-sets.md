---
title: 管理影像集中的資訊面板內容
description: 瞭解如何管理Adobe Dynamic Media Classic影像集中的資訊面板內容。
uuid: ed7b4344-f180-41fc-a95a-62a9767dc056
contentOwner: rbrough
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
content-type: reference
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sets
discoiquuid: ba5d1fb1-af54-471c-a471-853ace7f72fd
feature: Dynamic Media Classic,Viewers,Image Sets
role: User
exl-id: 09fafdb4-51e2-4719-83b6-056f79d1ba9e
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '767'
ht-degree: 51%

---

# 管理影像集中的資訊面板內容{#managing-info-panel-content-in-image-sets}

除了在图像集中将图像映射文本用于变换之外，还可以使用“信息面板”添加大量变换文本（包括链接）。还可以使用定时缓存和计划内容更新来管理信息面板。

您可以使用Adobe Dynamic Media Classic中的下列功能來管理資訊面板設定和資料：

* “信息面板设置”面板可用来指定用于显示“信息面板”文本、默认错误响应以及信息缓存的小时数等信息的模板。此外，可以指定是否自动发布图像集。
* 「資訊」「面板資料摘要」面板可讓您指定CSV檔案，其中包含您要顯示在資訊面板滑鼠指向效果文字中的文字，以及更新資訊的排程時間。
* “导入元数据”对话框可用来导入包含变换文本信息的制表符分隔 TXT 文件。您可以針對滑鼠指向效果文字，使用此TXT選項或具有CSV檔案選項的「資訊面板資料摘要」面板。

## 設定影像集的回應範本 {#set-up-a-response-template-for-image-sets}

可以选择三个预设响应模板之一用来在“信息面板”中显示文本。这些预设响应模板决定了在“信息面板”中显示信息的方式：列数和行数、字样大小、字体等等。可以选择预设响应模板，或者创建一个自己的模板。

**若要設定「影像集」的回應範本，請執行下列動作：**

1. 連按兩下「影像集」，使其在「詳細資料檢視」中開啟。
1. 選取 **[!UICONTROL 資訊面板設定]**.
1. 在“响应模板”下拉列表中，执行下列操作之一：

   * 若要使用預設回應，請選取 **[!UICONTROL 預設]**. 模板设计的 XML 在“用户模板”文本框中灰显。
   * 若要建立您自己的回應範本，請選取 **[!UICONTROL 自訂]**. 在“用户模板”文本框中，键入模板 XML 定义。您可以使用已在该文本框定义的默认模板作为您自己的响应的基模板。

1. （可選）在「預設回應」方塊中，輸入您要在Adobe Dynamic Media Classic擷取影像地圖資訊時發生錯誤，顯示的文字。 例如，如果系统收到公司名称和图像集名称，但是没有变换标识符，则将为用户显示该消息。
1. 在“响应 TTL”文本字段中，输入要在缓存数据之前等待的小时数。

   * 如果在一整天内需要频繁更新数据，则设置一个较小的值。
   * 如果数据相对稳定并且不需要整天频繁更新，则设置一个较大的值。默认为十小时。

1. 選取 **[!UICONTROL 上傳]** 若要根據rollover_key值將資訊面板內容上傳至s7info。
1. 在「S7Info上傳」對話方塊中，瀏覽至您要使用的檔案，然後選取 **[!UICONTROL 上傳]**.

   支援的檔案格式為使用UTF-16編碼的TAB分隔檔案和使用ASCII編碼的CSV檔案。 对于 CSV 文件，必须对非 ASCII 字符进行 HTML 编码。

1. 在「資訊面板設定」面板中，選取 **[!UICONTROL 發佈]**.

## 匯入影像集中資訊面板的來源內容 {#import-source-content-for-the-info-panel-in-image-sets}

您可以将采用 ASCII 编码（必须对非 ASCII 字符进行 HTML 编码）的 CSV（逗号分隔值）文件或制表符分隔文件用于图像集信息面板的源文本。制表符分隔文件必须使用 UTF-16 (Unicode) 编码。使用不同的方法导入不同的文件类型。

格式化源内容时，谨记以下指导原则：

* 以Tab和逗號分隔的資料可包含變換範本所需數量的欄。
* 第一個專案或資料欄是滑鼠指向效果識別碼（與影像地圖URL中的rollover_key值相關聯）。
* 確認識別碼之後的每個定位字元或逗號分隔專案都是您要取代至回應範本的專案。因此，第一欄會取代為$1$，第二欄會取代為$2$，依此類推)。

### 從外部託管位置將CSV內容匯入影像集 {#import-csv-content-into-image-sets-from-an-externally-hosted-location}

1. 連按兩下「影像集」，使其在「詳細資料檢視」中開啟。
1. 選取 **[!UICONTROL 資訊面板資料摘要]**.
1. 在“外部承载的 CSV 文件位置 (HTTP)”文本字段中，输入指向 CSV 文件的 URL。
1. （選擇性）在「排程更新」欄位中，指定更新內容的時間，然後選取 **[!UICONTROL 新增]**.

   可以选择多个更新时间。每个更新时间显示在“更新时间”文本框中。若要移除排定的時間，請選取該時間，然後選取 **[!UICONTROL 刪除]**.

1. （選用）選取 **[!UICONTROL 執行更新]** 立即更新內容。
