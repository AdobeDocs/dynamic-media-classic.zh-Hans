---
title: ICC 配置文件
seo-title: ICC 配置文件
description: 'null'
seo-description: 了解ICC配置文件。
uuid: 708ff ad-9a47-4e3e-b643-5b19648 f726 b
contentOwner: admin
content-type: 引用
products: SG_ EXPERIENCE MANAGER/Dynamic-Media-Scene-7
geptopics: SG_ SCENESELEFERENDER_ PK/categories/support_ files
discoiquuid: 44f1b4c4-6d7f-4e0f-84ce-11d26745e0f0
translation-type: tm+mt
source-git-commit: 75f006fd81b0fe2dad5479cdd98e45eaada46b2a

---


# ICC 配置文件{#icc-profiles}

ICC （国际色彩联盟）配置文件是描述如何正确地将图像文件从一个颜色空间转换到另一个颜色空间的文件。ICC 配置文件有助于为图像获取正确的颜色。例如，到正确地显示用于在计算机显示器上打印的图像，可以选择 ICC 配置文件。该配置文件将图像转换到不同的颜色空间并确保颜色正确地联机显示。

在 Scene7 Publishing System 中，在上载图像时，可以选择一个 ICC 配置文件以将图像转换到不同的颜色空间。默认情况下在 SPS 上所有标准的 Photoshop ICC 配置文件都是可用的。要在“上载”屏幕中查看颜色配置文件的名称，请选择“颜色配置文件”菜单。然后选择“自定义从&gt;到”，再从“转换至”和“转换到”菜单中选择 ICC 配置文件的名称。请参阅[上载时的图像编辑选项](image-editing-options-upload.md#image-editing-options-at-upload)。

除使用默认的 ICC 配置文件外，您还可以向 SPS 上载其他 ICC 配置文件，使其可用于颜色空间转换。在浏览面板中切换到详细信息视图，以便调查 ICC 配置文件的配置文件类、颜色空间类型和 PCS 类型。

## 上载 ICC 配置文件 {#uploading-icc-profiles}

通过与上载文件时所使用的技术相同的技术上载 ICC 配置文件。您可以将 ICC 配置文件存储在任何 SPS 文件夹中。请参阅[上载文件](uploading-files.md#uploading_your_files)。

## 检查 ICC 配置文件 {#examining-an-icc-profile}

要检查 ICC 配置文件，请在浏览面板中选择该文件并在详细信息视图中进行显示。详细信息视图提供有关 ICC 配置文件的以下信息：

**个人资料类** ICC(国际颜色联合协会)定义每个类以涵盖某种应用程序。例如，输入配置文件应用于数码相机和扫描仪等设备，输出配置文件应用于打印机。

**色彩空间类型** 此编号是配置文件的“输入”颜色空间，由ICC定义。颜色空间类型定义颜色空间的组件的数量和对这些组件的解释。例如，RGB 是具有三个组件（红色、绿色和蓝色）的颜色空间。颜色空间类型不定义空间的特定颜色特征（例如，原色的色度）。

**PCS类型** 此PCS类型是配置文件的“输出”颜色空间—其配置文件连接空间。例如，颜色配置文件可以将 RGB 转换成 PCS，然后转化成 CMYK。

对于有助于标记颜色或图像的输入、显示或输出配置文件，PCS 类型是 XYZ 或 Lab。将该配置文件解释成在 ICC 规范中定义的相应的特定颜色空间。