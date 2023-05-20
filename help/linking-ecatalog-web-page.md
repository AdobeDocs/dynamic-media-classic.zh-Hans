---
title: 將eCatalog連結至網頁
description: 瞭解如何將eCatalog連結至Adobe Dynamic Media Classic中的網頁。
uuid: 90098a90-180b-477a-8533-24a52a93200b
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
discoiquuid: 140640f2-3ca4-4b6c-a240-5f01be87fa9c
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: aee72576-1e3e-401c-953d-cc2be27f7dfd
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '691'
ht-degree: 38%

---

# 將eCatalog連結至網頁{#linking-an-ecatalog-to-a-web-page}

您的網站和應用程式會透過URL字串或內嵌程式碼存取Dynamic Media影像伺服器內容，包括eCatalog。 这些 URL 字符串在发布过程中被激活。若要將eCatalog的URL字串或內嵌程式碼放置在網頁和應用程式中，請從Adobe Dynamic Media Classic複製。

>[!NOTE]
>
>在发布资源之前，URL 处于非激活状态。

## 複製eCatalog URL {#copying-an-ecatalog-url}

1. 在「資產瀏覽」面板的「顯示」下拉式清單中，選取 **[!UICONTROL 目錄]**.
1. 在左侧的“资源库”面板中，导航至要复制其嵌入代码的 eCatalog 所在的资源文件夹。
1. 在“资源浏览”面板上方的工具栏右侧，执行以下任一操作：

   * 選取 **[!UICONTROL 格點檢視]**. 在“资源浏览”面板中，双击单个资源以便在详细信息视图中将其打开。在右側的「URL和內嵌程式碼」面板中，選取 **[!UICONTROL 複製URL]** 位於您想要的檢視器右側。
   * 選取 **[!UICONTROL 格點檢視]**. 在「資產瀏覽」面板中，選取單一資產，然後前往縮圖影像下方 **[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**.

      在「檢視器清單」頁面中，選取表格的「動作」欄下 **[!UICONTROL 複製URL]**.

   * 選取 **[!UICONTROL 清單檢視]**. 在「資產瀏覽」面板中，選取單一資產，然後在縮圖影像右側，前往 **[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**.

      在「檢視器清單」頁面中，選取表格的「動作」欄下 **[!UICONTROL 複製URL]**.

   * 選取 **[!UICONTROL 格點檢視]**， **[!UICONTROL 清單檢視]**，或 **[!UICONTROL 詳細資料檢視]**. 在相同工具列上，前往 **[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**.

      在「檢視器清單」頁面中，選取表格的「動作」欄下 **複製URL**.

## 將eCatalog URL新增至您的網頁 {#adding-ecatalog-urls-to-your-web-page}

部署 eCatalog 的最常用方法是在网页上放入一个 eCatalog 缩略图封面形式的链接。与 IT 团队合作，以确保在一个居中弹出的空白窗口中启动 eCatalog。请您的 IT 团队协助在浏览器中不显示工具栏和地址栏。

如需詳細資訊和程式碼範例，請參閱 [Adobe檢視器參考指南中的內嵌HTML5 eCatalog檢視器](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/library/viewers-aem-assets-dmc/ecatalog/c-html5-20-ecatalog-viewer-about.html#section-e1c3106f5b3e445d9b95be337c2f94e2).

## 複製eCatalog檢視器的內嵌程式碼 {#copying-the-embed-code-of-an-ecatalog-viewer}

使用嵌入代码功能，您可以查看用于所选 eCatalog 的查看器代码。 您也可以将代码复制到剪贴板中，以便可以将其粘贴到网页中以部署查看器。在“嵌入代码”对话框中不允许编辑代码。

**复制 eCatalog 查看器的嵌入代码:**

1. 在「資產瀏覽」面板的「顯示」下拉式清單中，選取 **[!UICONTROL 目錄]**.
1. 在左侧的“资源库”面板中，导航至要复制其嵌入代码的 eCatalog 所在的资源文件夹。
1. 在“资源浏览”面板上方的工具栏右侧，执行以下任一操作：

   * 選取 **[!UICONTROL 格點檢視]**. 在“资源浏览”面板中，双击单个资源以便在详细信息视图中将其打开。在右側的URL面板中，選取 **[!UICONTROL 內嵌程式碼]**.
   * 選取 **[!UICONTROL 格點檢視]**. 在「資產瀏覽」面板中，選取單一資產，然後前往縮圖影像下方 **[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**.

      在「檢視器清單」頁面中，選取表格的「動作」欄下 **[!UICONTROL 內嵌程式碼]**.

   * 選取 **[!UICONTROL 清單檢視]**. 在「資產瀏覽」面板中，選取單一資產，然後在縮圖影像右側，前往 **[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**.

      在「檢視器清單」頁面中，選取表格的「動作」欄下 **[!UICONTROL 內嵌程式碼]**.

   * 選取 **[!UICONTROL 格點檢視]**， **[!UICONTROL 清單檢視]**，或 **[!UICONTROL 詳細資料檢視]**. 在相同工具列上，前往 **[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**.

      在「檢視器清單」頁面中，選取表格的「動作」欄下 **[!UICONTROL 內嵌程式碼]**.

1. 在內嵌程式碼對話方塊中，選取 **[!UICONTROL 複製到剪貼簿]**.

   在“嵌入代码”对话框中不允许编辑代码。

1. 選取 **[!UICONTROL 關閉]**.
