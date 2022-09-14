---
title: 将缩放查看器链接到网页
description: 了解如何在Adobe Dynamic Media Classic中将缩放查看器链接到网页。
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

# 将缩放查看器链接到网页{#linking-zoom-viewers-to-your-web-pages}

您的网站和应用程序可通过URL字符串或嵌入代码访问Dynamic Media图像服务器内容，包括主图像和关联的缩放目标，以及缩放查看器预设。 这些 URL 字符串在发布过程中被激活。要将这些URL字符串或嵌入的代码置于网页和应用程序中，请从Adobe Dynamic Media Classic复制它们。

>[!NOTE]
>
>在发布资源之前，URL 处于非激活状态。

## 复制缩放查看器URL {#copying-a-zoom-viewer-url}

1. 在左侧的“资源库”面板中，导航至要复制其 URL 的缩放查看器所在的资源文件夹。
1. 在“资源浏览”面板上方的工具栏右侧，执行以下任一操作：

   * 选择 **[!UICONTROL 网格视图]** 或 **[!UICONTROL 列表视图]**. 在“资源浏览”面板中，双击单个资源以便在详细信息视图中将其打开。在右侧的URL和嵌入代码面板中，选择 **[!UICONTROL 复制URL]** 查看者的右侧。
   * 选择 **[!UICONTROL 网格视图]**. 在资产浏览面板中，选择一个资产，然后在缩略图图像下方，转到 **[!UICONTROL 预览]** > **[!UICONTROL 查看器列表]**.

      在“查看器列表”页面的表的“操作”列下，选择 **[!UICONTROL 复制URL]**.

   * 选择 **[!UICONTROL 列表视图]**. 在资产浏览面板中，选择一个资产，然后在缩略图图像的右侧，转到 **[!UICONTROL 预览]** > **[!UICONTROL 查看器列表]**.

      在“查看器列表”页面的表的“操作”列下，选择 **[!UICONTROL 复制URL]**.

   * 选择 **[!UICONTROL 网格视图]**, **[!UICONTROL 列表视图]**&#x200B;或 **[!UICONTROL 详细信息视图]**. 在同一工具栏上，转到 **[!UICONTROL 预览]** > **[!UICONTROL 查看器列表]**.

      在“查看器列表”页面的表的“操作”列下，选择 **[!UICONTROL 复制URL]**.

## 将缩放查看器URL添加到网页 {#adding-zoom-viewer-urls-to-your-web-page}

通常，访客会首先选择缩放图标来缩放网站上的图像（通常该图标会显示放大镜的图像）。 选择该图标会启动一个动态网页（ASP 或 JSP），该网页在弹出窗口中显示该图像。弹出窗口是访客实际缩放该图像的位置。

有关更多详细信息和代码示例，请参阅 [《嵌入HTML查看器参考指南》中的“嵌入Adobe5基本缩放查看器”](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/library/viewers-aem-assets-dmc/basic-zoom/c-html5-20-basic-zoom-viewer-about.html#section-e1c3106f5b3e445d9b95be337c2f94e2).

## 复制缩放查看器的嵌入副本 {#copying-the-embed-copy-of-a-zoom-viewer}

使用嵌入代码功能，您可以查看用于所选缩放查看器的查看器代码。您也可以将代码复制到剪贴板中，以便可以将其粘贴到网页中以部署查看器。不允许在“嵌入代码”对 话框中编辑代码 。

**复制缩放查看器的嵌入代码:**

1. 在左侧的“资源库”面板中，导航至要复制其嵌入代码的缩放查看器所在的资源文件夹。
1. 在“资源浏览”面板上方的工具栏右侧，执行以下任一操作：

   * 选择 **[!UICONTROL 网格视图]**. 在“资源浏览”面板中，双击单个资源以便在详细信息视图中将其打开。在右侧的URL和嵌入代码面板中，选择 **[!UICONTROL 嵌入代码]** 查看者的右侧。
   * 选择 **[!UICONTROL 网格视图]**. 在资产浏览面板中，选择一个资产，然后在缩略图图像下方，转到 **[!UICONTROL 预览]** > **[!UICONTROL 查看器列表]**.

      在“查看器列表”页面的表的“操作”列下，选择 **[!UICONTROL 嵌入代码]**.

   * 选择 **[!UICONTROL 列表视图]**. 在资产浏览面板中，选择一个资产，然后在缩略图图像的右侧，转到 **[!UICONTROL 预览]** > **[!UICONTROL 查看器列表]**.

      在“查看器列表”页面的表的“操作”列下，选择 **[!UICONTROL 嵌入代码]**.

   * 选择 **[!UICONTROL 网格视图]**, **[!UICONTROL 列表视图]**&#x200B;或 **[!UICONTROL 详细信息视图]**. 在同一工具栏上，转到 **[!UICONTROL 预览]** > **[!UICONTROL 查看器列表]**.

      在“查看器列表”页面的表的“操作”列下，选择 **[!UICONTROL 嵌入代码]**.

1. 在“嵌入代码”对话框中，选择 **[!UICONTROL 复制到剪贴板]**.

   在“嵌入代码”对话框中不允许编辑代码。

1. 选择 **[!UICONTROL 关闭]**.
