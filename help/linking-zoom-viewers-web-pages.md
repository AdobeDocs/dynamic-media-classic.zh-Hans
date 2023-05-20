---
title: 將縮放檢視器連結至您的網頁
description: 瞭解如何將縮放檢視器連結至Adobe Dynamic Media Classic中的網頁。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/zoom
feature: Dynamic Media Classic,Viewers,Zoom
role: User
exl-id: 2073d95b-1600-481f-8038-d29e8acacf7d
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '685'
ht-degree: 34%

---

# 將縮放檢視器連結至您的網頁{#linking-zoom-viewers-to-your-web-pages}

您的網站和應用程式會透過URL字串或內嵌程式碼存取Dynamic Media影像伺服器內容（包括主要影像和相關聯的縮放目標）以及縮放檢視器預設集。 这些 URL 字符串在发布过程中被激活。若要將這些URL字串或內嵌程式碼放置在網頁和應用程式中，請從Adobe Dynamic Media Classic複製它們。

>[!NOTE]
>
>在发布资源之前，URL 处于非激活状态。

## 複製縮放檢視器URL {#copying-a-zoom-viewer-url}

1. 在左侧的“资源库”面板中，导航至要复制其 URL 的缩放查看器所在的资源文件夹。
1. 在“资源浏览”面板上方的工具栏右侧，执行以下任一操作：

   * 選取 **[!UICONTROL 格點檢視]** 或 **[!UICONTROL 清單檢視]**. 在“资源浏览”面板中，双击单个资源以便在详细信息视图中将其打开。在右側的「URL和內嵌程式碼」面板中，選取 **[!UICONTROL 複製URL]** 位於您想要的檢視器右側。
   * 選取 **[!UICONTROL 格點檢視]**. 在「資產瀏覽」面板中，選取單一資產，然後前往縮圖影像下方 **[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**.

      在「檢視器清單」頁面中，選取表格的「動作」欄下 **[!UICONTROL 複製URL]**.

   * 選取 **[!UICONTROL 清單檢視]**. 在「資產瀏覽」面板中，選取單一資產，然後在縮圖影像右側，前往 **[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**.

      在「檢視器清單」頁面中，選取表格的「動作」欄下 **[!UICONTROL 複製URL]**.

   * 選取 **[!UICONTROL 格點檢視]**， **[!UICONTROL 清單檢視]**，或 **[!UICONTROL 詳細資料檢視]**. 在相同工具列上，前往 **[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**.

      在「檢視器清單」頁面中，選取表格的「動作」欄下 **[!UICONTROL 複製URL]**.

## 新增縮放檢視器URL至您的網頁 {#adding-zoom-viewer-urls-to-your-web-page}

通常，訪客會先選取「縮放」圖示（通常該圖示會顯示放大鏡的影像），以縮放網站上的影像。 选择该图标会启动一个动态网页（ASP 或 JSP），该网页在弹出窗口中显示该图像。弹出窗口是访客实际缩放该图像的位置。

如需詳細資訊和程式碼範例，請參閱 [Adobe檢視器參考指南中的內嵌HTML5基本縮放檢視器](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/library/viewers-aem-assets-dmc/basic-zoom/c-html5-20-basic-zoom-viewer-about.html#section-e1c3106f5b3e445d9b95be337c2f94e2).

## 複製縮放檢視器的內嵌復本 {#copying-the-embed-copy-of-a-zoom-viewer}

使用嵌入代码功能，您可以查看用于所选缩放查看器的查看器代码。您也可以将代码复制到剪贴板中，以便可以将其粘贴到网页中以部署查看器。在“嵌入代码”对话框中不允许编辑代码。

**复制缩放查看器的嵌入代码:**

1. 在左侧的“资源库”面板中，导航至要复制其嵌入代码的缩放查看器所在的资源文件夹。
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
