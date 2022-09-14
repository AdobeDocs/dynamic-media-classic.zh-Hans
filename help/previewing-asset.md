---
title: 预览资产
description: 了解如何在Adobe Dynamic Media Classic中预览资产。
uuid: 4a01be21-e37f-4d79-9220-f4e177e9179a
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: 17d0bfd6-fc62-4ed6-8a51-7ac1a6bb96cc
feature: Dynamic Media Classic,Asset Management,Viewers
role: User
exl-id: 7e6f652c-b197-4171-b11b-f532795f7cf2
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '1012'
ht-degree: 37%

---

# 预览资产{#previewing-an-asset}

您可以使用预览功能查看客户查看数字资产时的显示方式。 “预览”使用分配给资源的默认查看器。默认查看器在“应用程序设置”中进行配置。

请参阅 [配置默认查看器](application-setup.md#configuring_default_viewers).

如果您预览的模板资产包含参数层，则可以更改参数或更改图像预设。 因为您所做的更改是嵌入式的，所以可以立即从相同的“预览”窗口查看结果。

另请参阅 [Adobe查看器参考库示例](https://landing.adobe.com/zh-Hans/na/dynamic-media/ctir-2755/live-demos.html).

**预览资源:**

1. 在左侧“资源库”面板中，导航到包含要预览的资源的“资源”文件夹。
1. 执行以下任一操作：

   * 在资产窗口的工具栏右侧的上方，选择 **[!UICONTROL 网格视图]**.
   * 在资产窗口的工具栏右侧的上方，选择 **[!UICONTROL 列表视图]**.
   * 在资产窗口的工具栏右侧的上方，选择 **[!UICONTROL 详细信息视图]**.

1. 根据您所使用的视图，执行以下操作之一：

   * 在网格视图或列表视图的“资产”窗口中，选择一个资产，然后选择 **[!UICONTROL 预览]** 在缩略图图像附近。
   * 在网格视图、列表视图或详细信息视图的“资产”窗口上方的工具栏中，选择 **[!UICONTROL 预览]**.

## 根据查看器平台类型预览资产 {#previewing-an-asset-based-on-viewer-platform-type}

可以使用“查看器列表”预览资源在特定查看器平台类型（如 HTML5）上的显示情况。并不是所有平台都可在查看器列表中找到，这取决于您选择要预览的资源类型和关联的查看器。

您也可以使用查看器列表来复制查看器的 URL 或者查看和复制查看器代码以嵌入到网页中。

对于给定的查看器平台，“查看器列表”窗口可让您直观地查看可供使用的设备（如平板电脑和智能手机）。

**基于查看器平台类型预览资源:**

1. 在左侧“资源库”面板中，导航到包含要预览的资源的“资源”文件夹。
1. 执行以下任一操作：

   * 在资产窗口的工具栏右侧的上方，选择 **[!UICONTROL 网格视图]**. 在“资产”窗口中，选择一个资产，然后在缩略图图像下方，转到 **[!UICONTROL 预览]** > **[!UICONTROL 查看器列表]**.
   * 在资产窗口的工具栏右侧的上方，选择 **[!UICONTROL 列表视图]**. 在“资产”窗口中，选择一个资产，然后在缩略图图像的右侧，转到 **[!UICONTROL 预览]** > **[!UICONTROL 查看器列表]**.
   * 在资产窗口的工具栏右侧的上方，选择 **[!UICONTROL 详细信息视图]**. 在同一工具栏上，转到 **[!UICONTROL 预览]** > **[!UICONTROL 查看器列表]**.

1. （可选）在“查看器列表”窗口中，选择列标题 **[!UICONTROL 名称]** 或 **[!UICONTROL 平台类型]** 按升序或降序对列进行排序。
1. 在“查看器列表”窗口的表的“操作”列下，选择 **[!UICONTROL 预览]** 查看选定查看器和平台类型的资产显示方式。

   关闭显示的预览。

1. （可选）在“查看器列表”窗口底部的“用于生成副本 URL 的 URL 编码”下拉列表中，选择要在复制资源的 URL 时应用的 URL 编码。
1. （可选）请执行下列操作之一：

   * 在“查看器列表”窗口的表的“操作”列下，选择 **[!UICONTROL 复制URL]** ，以查看选定的查看器和平台类型。

      选择 **[!UICONTROL 复制URL]**，则其关联的URL会自动复制到剪贴板。

   * 在“查看器列表”窗口的表的“操作”列下，选择 **[!UICONTROL 嵌入代码]**.

      选择 **[!UICONTROL 嵌入代码]**，此时会打开嵌入代码窗口，您可以在其中查看查看器代码。 不允许在该窗口中编辑代码。您也可以将代码复制到剪贴板中，以便可以将其粘贴到网页中。

      关闭显示的预览。

1. 在“查看器列表”窗口的右下角，选择 **[!UICONTROL 关闭]** ，以返回到资产屏幕。

## 根据图像预设预览图像资产 {#previewing-an-image-asset-based-on-its-image-preset}

您可以基于图像预设来预览图像资源，从而查看在图像以不同大小动态地传送到网站或应用程序时的显示情况。

图像预设是一组预定义的设置，用于更改图像在导出时的外观大小、图像质量、格式、分辨率以及其他方面。

请参阅 [设置图像预设](setting-image-presets.md#setting_up_image_presets).

请参阅 [创建并启用图像预设](creating-enabling-image-presets.md#creating_and_enabling_image_presets).

**基于图像预设预览图像资源:**

1. 在左侧“资源库”面板中，导航到包含要预览的图像资源的“资源”文件夹。
1. 执行以下任一操作：

   * 在资产窗口的工具栏右侧的上方，选择 **[!UICONTROL 网格视图]**. 在“资产”窗口中，选择单个图像资产，然后在缩略图图像下方，转到 **[!UICONTROL 预览]** > **[!UICONTROL 图像预设列表]**.
   * 在资产窗口的工具栏右侧的上方，选择 **[!UICONTROL 列表视图]**. 在“资产”窗口中，选择一个图像资产，然后在缩略图的右侧，转到 **[!UICONTROL 预览]** > **[!UICONTROL 图像预设列表]**.
   * 在资产窗口的工具栏右侧的上方，选择 **[!UICONTROL 详细信息视图]**. 在同一工具栏上，转到 **[!UICONTROL 预览]** > **[!UICONTROL 图像预设列表]**.

1. 在“图像预设列表”窗口的表中，选择您要嵌入右侧窗格预览其图像资源的预设类型名称。
1. （可选）在“图像预设列表”窗口的 **[!UICONTROL 用于生成复制URL的URL编码]** 下拉列表中，选择要在复制图像资产时应用于其URL的URL编码。
1. （可选）在“图像预设列表”窗口的预览窗格的右上角，选择 **[!UICONTROL 复制URL]** 的值。

   选择 **[!UICONTROL 复制URL]**，则其关联的URL会自动复制到剪贴板。

1. 在“图像预设列表”窗口的右下角，选择 **[!UICONTROL 关闭]** ，以返回到资产屏幕。
