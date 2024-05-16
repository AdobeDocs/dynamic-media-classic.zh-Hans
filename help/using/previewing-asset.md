---
title: 预览资源
description: 了解如何在Adobe Dynamic Media Classic中预览资源。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
feature: Dynamic Media Classic,Asset Management,Viewers
role: User
exl-id: 7e6f652c-b197-4171-b11b-f532795f7cf2
topic: Content Management
level: Intermediate
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '1008'
ht-degree: 12%

---

# 预览资源{#previewing-an-asset}

您可以使用预览功能查看客户查看数字资产时如何显示。 “预览”使用分配给资源的默认查看器。默认查看器在“应用程序设置”中进行配置。

请参阅 [配置默认查看器](application-setup.md#configuring_default_viewers).

如果预览模板资产时带有参数图层，则可以更改参数或更改图像预设。 因为您所做的更改是嵌入式的，所以可以立即从相同的“预览”窗口查看结果。

另请参阅 [Adobe查看器参考库示例](https://landing.adobe.com/en/na/dynamic-media/ctir-2755/live-demos.html).

**要预览资源，请执行以下操作：**

1. 在左侧的资产库面板中，导航到包含要预览的资产的资产文件夹。
1. 执行以下任一操作：

   * 在“资源”窗口的工具栏右侧，选择 **[!UICONTROL 网格视图]**.
   * 在“资源”窗口的工具栏右侧，选择 **[!UICONTROL 列表视图]**.
   * 在“资源”窗口的工具栏右侧，选择 **[!UICONTROL 详细信息视图]**.

1. 根据您使用的视图，执行以下操作之一：

   * 在网格视图或列表视图的资源窗口中，选择单个资源，然后选择 **[!UICONTROL 预览]** 在缩略图图像附近。
   * 在“网格视图”、“列表视图”或“详细信息视图”的“资源”窗口上方的工具栏上，选择 **[!UICONTROL 预览]**.

## 根据查看器平台类型预览资源 {#previewing-an-asset-based-on-viewer-platform-type}

您可以使用查看器列表预览资源在特定查看器平台类型(如HTML5)上的显示方式。 并不是所有平台都可在查看器列表中找到，这取决于您选择要预览的资源类型和关联的查看器。

您还可以使用查看器列表复制查看器的URL，或者查看并复制查看器代码以嵌入到网页中。

对于给定的查看器平台，“查看器列表”窗口允许您直观地查看查看器可以使用哪些设备，如平板电脑和智能手机。

**要根据查看器平台类型预览资源，请执行以下操作：**

1. 在左侧的资产库面板中，导航到包含要预览的资产的资产文件夹。
1. 执行以下任一操作：

   * 在“资源”窗口的工具栏右侧，选择 **[!UICONTROL 网格视图]**. 在“资源”窗口中，选择单个资源，然后转到缩略图图像下方 **[!UICONTROL 预览]** > **[!UICONTROL 查看器列表]**.
   * 在“资源”窗口的工具栏右侧，选择 **[!UICONTROL 列表视图]**. 在“资源”窗口中，选择单个资源，然后转到缩略图图像右侧的 **[!UICONTROL 预览]** > **[!UICONTROL 查看器列表]**.
   * 在“资源”窗口的工具栏右侧，选择 **[!UICONTROL 详细信息视图]**. 在同一工具栏上，转到 **[!UICONTROL 预览]** > **[!UICONTROL 查看器列表]**.

1. （可选）在“查看器列表”窗口中，选择列标题 **[!UICONTROL 名称]** 或 **[!UICONTROL 平台类型]** 以按升序或降序对列进行排序。
1. 在“查看器列表”窗口的表的“操作”列下，选择 **[!UICONTROL 预览]** 查看选定查看器和平台类型中资产的显示方式。

   关闭显示的预览。

1. （可选）在“查看器列表”窗口中，在底部的“用于生成副本URL的URL编码”下拉列表中选择“URL编码”。 此编码在复制资产时应用到资产的URL。
1. （可选）请执行下列操作之一：

   * 在“查看器列表”窗口的表的“操作”列下，选择 **[!UICONTROL 复制URL]** 选定的查看器和平台类型。

     当您选择时 **[!UICONTROL 复制URL]**，则其关联的URL会自动复制到剪贴板。

   * 在“查看器列表”窗口的表的“操作”列下，选择 **[!UICONTROL 嵌入代码]**.

     当您选择时 **[!UICONTROL 嵌入代码]**，将打开嵌入代码窗口，您可以在其中查看查看器代码。 不允许在该窗口中编辑代码。您还可以将代码复制到剪贴板，以便将其粘贴到网页中。

     关闭显示的预览。

1. 在Viewer List窗口的右下角，选择 **[!UICONTROL 关闭]** 以返回资产屏幕。

## 预览基于其图像预设的图像资源 {#previewing-an-image-asset-based-on-its-image-preset}

您可以预览基于其图像预设的图像资源，以了解当以不同大小动态交付到您的网站或应用程序时您的图像是什么样的。

图像预设是预定义设置的集合。 这些设置可更改导出图像时图像外观的大小、图像质量、格式、分辨率和其他方面。

请参阅 [设置图像预设](setting-image-presets.md#setting_up_image_presets).

请参阅 [创建和启用图像预设](creating-enabling-image-presets.md#creating_and_enabling_image_presets).

**要根据图像预设预览图像资源，请执行以下操作：**

1. 在左侧的资产库面板中，导航到包含要预览的图像资产的“资产”文件夹。
1. 执行以下任一操作：

   * 在“资源”窗口的工具栏右侧，选择 **[!UICONTROL 网格视图]**. 在“资源”窗口中，选择单个图像资源，然后转到缩略图图像下方的 **[!UICONTROL 预览]** > **[!UICONTROL 图像预设列表]**.
   * 在“资源”窗口的工具栏右侧，选择 **[!UICONTROL 列表视图]**. 在“资源”窗口中，选择单个图像资源，然后转到缩略图图像右侧的 **[!UICONTROL 预览]** > **[!UICONTROL 图像预设列表]**.
   * 在“资源”窗口的工具栏右侧，选择 **[!UICONTROL 详细信息视图]**. 在同一工具栏上，转到 **[!UICONTROL 预览]** > **[!UICONTROL 图像预设列表]**.

1. 在“图像预设列表”窗口的表中，选择您要嵌入右侧窗格预览其图像资源的预设类型名称。
1. （可选）在“图像预设列表”窗口的 **[!UICONTROL 用于生成副本URL的URL编码]** 下拉列表。
1. 选择URL编码，以在复制图像资源时应用于图像资源的URL。
1. （可选）在“图像预设列表”窗口中，在预览窗格的右上角区域中选择 **[!UICONTROL 复制URL]** 所选预设类型。

   当您选择时 **[!UICONTROL 复制URL]**，则其关联的URL会自动复制到剪贴板。

1. 在“图像预设列表”窗口的右下角，选择 **[!UICONTROL 关闭]** 以返回资产屏幕。
