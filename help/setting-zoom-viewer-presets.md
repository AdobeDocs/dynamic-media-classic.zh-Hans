---
title: 设置缩放查看器预设
seo-title: 设置缩放查看器预设
description: 'null'
seo-description: 了解如何设置缩放查看器预设。
uuid: 202d80cb-8282-45d4-89e8-942c8677aa93
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/zoom
discoiquuid: 5023a933-e229-4d3c-8e91-3ac5e9f4970b
translation-type: tm+mt
source-git-commit: 6fff3699f8a08af433df3f3a7790a11bf9d05b00

---


# 设置缩放查看器预设{#setting-up-zoom-viewer-presets}

缩放查看器预设可确定缩放查看器的样式、行为和外观。Dynamic Media Classic优惠了许多用于自定义查看器和设置查看器外观的选项。 Dynamic Media Classic附带默认的基本（快速）缩放查看器预设和自定义缩放查看器预设。 如果您是管理员，则可以创建新的公司缩放查看器预设，或编辑默认预设并使用新名称保存。

所有缩放查看器都带有用于放大、缩小、平移并在缩放后将图像重置为原始状态的按钮。按钮和窗口的显示效果具体取决于所选的缩放查看器预设。您可以使用不同的颜色、边框、字体及图像设置来配置缩放查看器预设。配置引导式缩放查看器时，还可以选择缩放目标的放置位置。缩放目标指的是用户单击后可缩放到指定区域的缩略图。

## 关于缩放查看器预设 {#about-zoom-viewer-presets}

Dynamic Media Classic优惠了以下缩放查看器预设：

* **缩放查看器：基本**&#x200B;对原始图像提供基本缩放。

* **缩放查看器：飞出在**&#x200B;原始图像旁边显示缩放区域的第二幅图像。 没有控件可以使用，用户只需将选取范围移动到他们要查看的区域上即可。

在确定此查看器的完整带宽使用量时，请考虑在查看器中有主图像和弹出图像。弹出图像大小取决于主图像大小（舞台宽度和高度）和缩放因子。为防止弹出文件大小变得太大，需对这两个值进行平衡：如果您的主图像大小很大，请降低缩放系数值。（弹出宽度和弹出高度决定了弹出窗口的大小，但不决定提供给查看器的弹出图像的大小。）

例如，如果您的主图像大小是 350 X 350 像素，缩放系数为 3，则生成的弹出图像是 1050 X 1050 像素。如果您的主图像大小是 300 X 300 像素，缩放系数为 4，则弹出图像是 1200 X 1200 像素。根据 JPEG 品质设置（推荐的设置介于 80-90），您可以显著地减少文件大小。建议的缩放系数为 2.5 至 4，取决于您的主图像的大小。

Dynamic Media Classic建议用于弹出缩放查看器预设的以下参数：

* **放大图像大**&#x200B;小约1500 x 1500像素，不超过2000 x 2000像素。

* **图像大小**&#x200B;为100KB或以下，不超过150KB（压缩文件以使其保持在150KB以下）。

* **缩放查看器：自定**&#x200B;义提供对图像、具有多个视图的图像集或色板集的引导式或未引导式缩放。

## 创建并编辑缩放查看器预设 {#creating-and-editing-zoom-viewer-presets}

请按照以下步骤创建或编辑缩放查看器预设：

1. 单击“**设置**”>“**查看器预设**”。
1. 执行以下任一操作：

   * **创建预设单击**“添加”。 在“添加查看器预设”对话框中，选择一个平台，选择缩放查看器，然后单击“添加”。 在“预设名称”框中输入预设的名称。

   * **编辑预设选**&#x200B;择缩放查看器预设，然后单击编 **辑**。

1. 根据需要指定设置。

   要查看选项的说明，请单击选项旁的“信息提示”图标 。

   更新和更改设置时，预览屏幕将显示查看器。

1. 单击“**保存**”或“**另存为**”。
1. 在“查看器预设”屏幕上，检查创建的缩放查看器预设或引导式缩放查看器预设。If it needs adjusting, click **Edit**, change settings on the Configure Viewer screen, and click **Save**.

有关在“查看器预设”屏幕上管理查看器预设的信息，请参阅[查看器预设](application-setup.md#viewer_presets)。

>[!MORELIKETHIS]
>
>* [Creating and editing Viewer Presets](application-setup.md#adding_and_editing_viewer_presets)

