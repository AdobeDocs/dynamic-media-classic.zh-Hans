---
title: 设置缩放查看器预设
description: 了解如何在Adobe Dynamic Media Classic中设置缩放查看器预设。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/zoom
feature: Dynamic Media Classic,Viewers,Zoom
role: User
exl-id: ddaaff6c-5447-408e-9c92-bcdfd1a0e72e
topic: Content Management
level: Intermediate
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '629'
ht-degree: 48%

---

# 设置缩放查看器预设{#setting-up-zoom-viewer-presets}

缩放查看器预设可确定缩放查看器的样式、行为和外观。Adobe Dynamic Media Classic提供了多个用于自定义查看器和为查看器设置外观的选项。 Adobe Dynamic Media Classic附带默认的基本（快速）、弹出和自定义缩放查看器预设。 如果您是管理员，则可以创建公司缩放查看器预设或编辑默认预设，并使用新名称保存该预设。

所有缩放查看器都带有用于放大、缩小、平移并在缩放后将图像重置为原始状态的按钮。这些按钮的外观以及窗口本身的显示方式取决于您选择的缩放查看器预设。 您可以使用不同的颜色、边框、字体及图像设置来配置缩放查看器预设。配置引导式缩放查看器时，还可以选择缩放目标的放置位置。缩放目标指的是用户单击后可缩放到指定区域的缩略图。

## 关于缩放查看器预设 {#about-zoom-viewer-presets}

Adobe Dynamic Media Classic提供以下缩放查看器预设：

* **缩放查看器：基本**：提供对原始图像的基本缩放。

* **缩放查看器：弹出**：在原始图像旁边显示缩放区域的第二个图像。 没有控件可以使用，用户只需将选取范围移动到他们要查看的区域上即可。

在确定此查看器的完整带宽使用量时，请考虑在查看器中有主图像和弹出图像。弹出图像大小取决于主图像大小（舞台宽度和高度）和缩放因子。为防止弹出文件大小变得太大，需对这两个值进行平衡：如果您的主图像大小很大，请降低缩放系数值。（弹出宽度和弹出高度决定了弹出窗口的大小，但不决定提供给查看器的弹出图像的大小。）

例如，如果您的主图像大小是 350 X 350 像素，缩放系数为 3，则生成的弹出图像是 1050 X 1050 像素。如果您的主图像大小是 300 X 300 像素，缩放系数为 4，则弹出图像是 1200 X 1200 像素。根据 JPEG 品质设置（推荐的设置介于 80-90），您可以显著地减少文件大小。建议的缩放系数为 2.5 至 4，取决于您的主图像的大小。

Adobe Dynamic Media Classic建议为弹出缩放查看器预设使用以下参数：

* **放大的图像大小**：约1500 x 1500像素，不超过2000 x 2000像素。

* **图像大小**：100 KB或更低，不超过150 KB（压缩文件以使其低于150 KB）。

* **缩放查看器：自定义**：提供带图像的引导式或无引导式缩放、带多个视图的图像集或色板集。

## 创建和编辑缩放查看器预设 {#creating-and-editing-zoom-viewer-presets}

1. 在全局导航栏上，转到 **[!UICONTROL 设置]** > **[!UICONTROL 查看器预设]**.
1. 执行以下任一操作：

   * **创建预设**：选择 **[!UICONTROL 添加]**. 在“添加查看器预设”对话框中，选择一个平台，选择一个缩放查看器，然后选择 **[!UICONTROL 添加]**. 在“预设名称”框中输入预设的名称。

   * **编辑预设**：选择缩放查看器预设，然后选择 **[!UICONTROL 编辑]**.

1. 根据需要指定设置。

   要查看选项的说明，请选择 **[!UICONTROL 信息提示]** 图标。

   当您更新和更改设置时，“预览”页面将显示查看器。

1. 选择 **[!UICONTROL 保存]** 或 **[!UICONTROL 另存为]**.
1. 在“查看器预设”页面上，检查您创建的缩放查看器预设或引导式缩放查看器预设。 如果需要调整，请选择 **[!UICONTROL 编辑]**，更改设置 `Configure Viewer` 页面，然后选择 **[!UICONTROL 保存]**.

有关在“查看器预设”屏幕上管理查看器预设的信息，请参阅[查看器预设](application-setup.md#viewer_presets)。

>[!MORELIKETHIS]
>
>* [创建和编辑查看器预设](application-setup.md#adding_and_editing_viewer_presets)
