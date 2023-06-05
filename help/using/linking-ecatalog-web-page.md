---
title: 将eCatalog链接到网页
description: 了解如何将eCatalog链接到Adobe Dynamic Media Classic中的网页。
uuid: 90098a90-180b-477a-8533-24a52a93200b
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
discoiquuid: 140640f2-3ca4-4b6c-a240-5f01be87fa9c
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: aee72576-1e3e-401c-953d-cc2be27f7dfd
source-git-commit: 65e3b69bdcbd651a5f9ab100592217e61a8c05ef
workflow-type: tm+mt
source-wordcount: '691'
ht-degree: 38%

---

# 将eCatalog链接到网页{#linking-an-ecatalog-to-a-web-page}

您的网站和应用程序通过URL字符串或嵌入代码访问Dynamic Media Image Server内容，包括eCatalog。 这些 URL 字符串在发布过程中被激活。要将eCatalog的URL字符串或嵌入代码置于网页和应用程序中，请从Adobe Dynamic Media Classic复制该字符串或嵌入代码。

>[!NOTE]
>
>在发布资源之前，URL 处于非激活状态。

## 复制eCatalog URL {#copying-an-ecatalog-url}

1. 在资产浏览面板的显示下拉列表中，选择 **[!UICONTROL 目录]**.
1. 在左侧的“资源库”面板中，导航至要复制其嵌入代码的 eCatalog 所在的资源文件夹。
1. 在“资源浏览”面板上方的工具栏右侧，执行以下任一操作：

   * 选择 **[!UICONTROL 网格视图]**. 在“资源浏览”面板中，双击单个资源以便在详细信息视图中将其打开。在右侧的“URL和嵌入代码”面板中，选择 **[!UICONTROL 复制URL]** 位于所需查看器的右侧。
   * 选择 **[!UICONTROL 网格视图]**. 在“资源浏览”面板中，选择单个资源，然后转到缩略图图像下方 **[!UICONTROL 预览]** > **[!UICONTROL 查看器列表]**.

      在“查看器列表”页的表的“操作”列下，选择 **[!UICONTROL 复制URL]**.

   * 选择 **[!UICONTROL 列表视图]**. 在“资源浏览”面板中，选择单个资源，然后转到缩略图图像右侧的 **[!UICONTROL 预览]** > **[!UICONTROL 查看器列表]**.

      在“查看器列表”页的表的“操作”列下，选择 **[!UICONTROL 复制URL]**.

   * 选择 **[!UICONTROL 网格视图]**， **[!UICONTROL 列表视图]**，或 **[!UICONTROL 详细信息视图]**. 在同一工具栏上，转到 **[!UICONTROL 预览]** > **[!UICONTROL 查看器列表]**.

      在“查看器列表”页的表的“操作”列下，选择 **复制URL**.

## 将eCatalog URL添加到网页 {#adding-ecatalog-urls-to-your-web-page}

部署 eCatalog 的最常用方法是在网页上放入一个 eCatalog 缩略图封面形式的链接。与 IT 团队合作，以确保在一个居中弹出的空白窗口中启动 eCatalog。请您的 IT 团队协助在浏览器中不显示工具栏和地址栏。

有关更多详细信息和代码示例，请参阅 [Adobe查看器参考指南中的嵌入HTML5 eCatalog查看器](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/library/viewers-aem-assets-dmc/ecatalog/c-html5-20-ecatalog-viewer-about.html#section-e1c3106f5b3e445d9b95be337c2f94e2).

## 复制eCatalog查看器的嵌入代码 {#copying-the-embed-code-of-an-ecatalog-viewer}

使用嵌入代码功能，您可以查看用于所选 eCatalog 的查看器代码。 您也可以将代码复制到剪贴板中，以便可以将其粘贴到网页中以部署查看器。在“嵌入代码”对话框中不允许编辑代码。

**复制 eCatalog 查看器的嵌入代码:**

1. 在资产浏览面板的显示下拉列表中，选择 **[!UICONTROL 目录]**.
1. 在左侧的“资源库”面板中，导航至要复制其嵌入代码的 eCatalog 所在的资源文件夹。
1. 在“资源浏览”面板上方的工具栏右侧，执行以下任一操作：

   * 选择 **[!UICONTROL 网格视图]**. 在“资源浏览”面板中，双击单个资源以便在详细信息视图中将其打开。在右侧的URL面板中，选择 **[!UICONTROL 嵌入代码]**.
   * 选择 **[!UICONTROL 网格视图]**. 在“资源浏览”面板中，选择单个资源，然后转到缩略图图像下方 **[!UICONTROL 预览]** > **[!UICONTROL 查看器列表]**.

      在“查看器列表”页的表的“操作”列下，选择 **[!UICONTROL 嵌入代码]**.

   * 选择 **[!UICONTROL 列表视图]**. 在“资源浏览”面板中，选择单个资源，然后转到缩略图图像右侧的 **[!UICONTROL 预览]** > **[!UICONTROL 查看器列表]**.

      在“查看器列表”页的表的“操作”列下，选择 **[!UICONTROL 嵌入代码]**.

   * 选择 **[!UICONTROL 网格视图]**， **[!UICONTROL 列表视图]**，或 **[!UICONTROL 详细信息视图]**. 在同一工具栏上，转到 **[!UICONTROL 预览]** > **[!UICONTROL 查看器列表]**.

      在“查看器列表”页的表的“操作”列下，选择 **[!UICONTROL 嵌入代码]**.

1. 在“嵌入代码”对话框中，选择 **[!UICONTROL 复制到剪贴板]**.

   在“嵌入代码”对话框中不允许编辑代码。

1. 选择 **[!UICONTROL 关闭]**.
