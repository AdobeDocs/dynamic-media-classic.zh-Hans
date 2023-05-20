---
title: 將迴轉集連結至網頁
description: 瞭解如何將迴轉集連結至Adobe Dynamic Media Classic中的網頁。
uuid: d3c5773e-60c4-4e8b-9c48-e1e3eb8028d0
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/spin_sets
discoiquuid: 651b21ef-e322-4e6d-8e37-45ffd56f7a58
feature: Dynamic Media Classic,Viewers,Spin Sets
role: User
exl-id: af75547e-20e8-44c2-b165-01532d6e21d0
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '727'
ht-degree: 40%

---

# 將迴轉集連結至網頁{#linking-a-spin-set-to-a-web-page}

網站和應用程式會透過URL字串或內嵌程式碼存取Dynamic Media影像伺服器內容，包括迴轉集。 这些 URL 字符串在发布过程中被激活。若要將迴轉集的URL字串或內嵌程式碼放置在網頁和應用程式中，請從Adobe Dynamic Media Classic複製。

>[!NOTE]
>
>在发布资源之前，URL 处于非激活状态。

## 複製迴轉集URL {#copying-a-spin-set-url}

1. 在「資產瀏覽」面板的「顯示」下拉式清單中，選取 **[!UICONTROL 迴轉集]**.
1. 在左侧的“资源库”面板中，导航至要复制其嵌入代码的旋转集所在的资源文件夹。
1. 在“资源浏览”面板上方的工具栏右侧，执行以下任一操作：

   * 選取 **[!UICONTROL 格點檢視]**. 在“资源浏览”面板中，双击单个资源以便在详细信息视图中将其打开。在右側的「URL和內嵌程式碼」面板中，選取 **[!UICONTROL 複製URL]** 位於您想要的檢視器右側。
   * 選取 **[!UICONTROL 格點檢視]**. 在「資產瀏覽」面板中，選取單一資產，然後前往縮圖影像下方 **[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**.

      在「檢視器清單」頁面中，選取表格的「動作」欄下 **[!UICONTROL 複製URL]**.

   * 選取 **[!UICONTROL 清單檢視]**. 在「資產瀏覽」面板中，選取單一資產，然後在縮圖影像右側，前往 **[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**.

      在「檢視器清單」頁面中，選取表格的「動作」欄下 **[!UICONTROL 複製URL]**.

   * 選取 **[!UICONTROL 格點檢視]**， **[!UICONTROL 清單檢視]**，或 **[!UICONTROL 詳細資料檢視]**. 在相同工具列上，前往 **[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**.

      在「檢視器清單」頁面中，選取表格的「動作」欄下 **[!UICONTROL 複製URL]**.

## 將迴轉集URL新增至網頁 {#adding-spin-set-urls-to-your-web-page}

旋转集的部署方式与所有缩放查看器一样，即通过在缩放窗口中显示旋转集的动态页面（ASP 或 JSP）进行部署。對Adobe Dynamic Media Classic平台的URL呼叫遵循縮放檢視器上的相同通訊協定。 不过，查看器预设名称取决于您的管理员所定义的默认旋转集查看器预设。例如，以下非实时 URL 语法示例包括名为 `viewer.jsp` 的预设名称，而 SKU 参数现在为旋转集名称：

```as3
https://sample.scene7.com/s7ondemand/spin/viewer.jsp?company=S7Web&sku=backpack_spin
```

在此 URL 语法示例中（链接处于不活动状态），请注意 SKU 编号 (`sku=backpack_spin`)。之後的字串 `sku=` 是迴轉集名稱( `backpack spin`)。

## 複製迴轉集檢視器的內嵌程式碼 {#copying-the-embed-code-of-a-spin-set-viewer}

使用嵌入代码功能，您可以查看用于所选旋转集的查看器代码。您也可以将代码复制到剪贴板中，以便可以将其粘贴到网页中以部署查看器。在“嵌入代码”对话框中不允许编辑代码。

**复制旋转集查看器的嵌入代码:**

1. 在「資產瀏覽」面板的「顯示」下拉式清單中，選取 **[!UICONTROL 迴轉集]**.
1. 在左侧的“资源库”面板中，导航至要复制其嵌入代码的旋转集所在的资源文件夹。
1. 在“资源浏览”面板上方的工具栏右侧，执行以下任一操作：

   * 選取 **[!UICONTROL 格點檢視]**. 在“资源浏览”面板中，双击单个资源以便在详细信息视图中将其打开。在右側的「URL和內嵌程式碼」面板中，選取 **[!UICONTROL 內嵌程式碼]** 位於您想要的檢視器右側。
   * 選取 **[!UICONTROL 格點檢視]**. 在「資產瀏覽」面板中，選取單一資產，然後前往縮圖影像下方 **[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**.

      在「檢視器清單」頁面中，選取表格的「動作」欄下 **[!UICONTROL 內嵌程式碼]**.

   * 選取 **[!UICONTROL 清單檢視]**. 在「資產瀏覽」面板中，選取單一資產，然後在縮圖影像右側，前往 **[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**.

      在「檢視器清單」頁面中，選取表格的「動作」欄下 **[!UICONTROL 內嵌程式碼]**.

   * 選取 **[!UICONTROL 格點檢視]**， **[!UICONTROL 清單檢視]**，或 **[!UICONTROL 詳細資料檢視]**. 在相同工具列上，前往 **[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**.

      在「檢視器清單」頁面中，選取表格的「動作」欄下 **[!UICONTROL 內嵌程式碼]**.

1. 在內嵌程式碼對話方塊中，選取 **[!UICONTROL 複製到剪貼簿]**.

   在“嵌入代码”对话框中不允许编辑代码。

1. 選取 **[!UICONTROL 關閉]**.
