---
title: ICC（国际颜色联盟）配置文件
description: 了解Adobe Dynamic Media Classic中的ICC配置文件。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/support_files
feature: Dynamic Media Classic
role: User
exl-id: 989f2761-f5d0-4ece-b2a6-f7b4577aa8a2
topic: Administration, Content Management
level: Intermediate
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '452'
ht-degree: 41%

---

# ICC 配置文件{#icc-profiles}

ICC（国际颜色联盟）配置文件是一个文件，用于描述如何正确地将图像文件从一个色彩空间转换到另一个色彩空间。 ICC 配置文件有助于为图像获取正确的颜色。例如，要正确显示设计用于在计算机显示器上打印的图像，可以选择ICC配置文件。 该配置文件将图像转换到不同的颜色空间并确保颜色正确地联机显示。

在Adobe Dynamic Media Classic中，您可以选择在上传图像时将ICC配置文件转换为其他颜色空间。 默认情况下，所有标准Photoshop ICC配置文件在Adobe Dynamic Media Classic上均可用。 要在“上载”屏幕中查看颜色配置文件的名称，请选择“颜色配置文件”菜单。然后选择“自定义自”>“到”，并在“转换自”和“转换至”菜单中选择一个ICC配置文件名称。

请参阅 [上传时图像编辑选项](image-editing-options-upload.md#image-editing-options-at-upload).

除了使用默认的ICC配置文件外，您还可以将其他ICC配置文件上传到Adobe Dynamic Media Classic，以便用于色彩空间转换。 在“浏览”面板中切换到“详细信息视图”以调查ICC配置文件的配置文件类、色彩空间类型和PCS类型。

## 上传ICC配置文件 {#uploading-icc-profiles}

通过与上载文件时所使用的技术相同的技术上载 ICC 配置文件。您可以将ICC配置文件存储在任何Adobe Dynamic Media Classic文件夹中。

请参阅 [上传文件](uploading-files.md#uploading_your_files).

## 检查ICC配置文件 {#examining-an-icc-profile}

要检查ICC配置文件，请在“浏览”面板中选择它，并在“详细信息视图”中显示它。 “详细信息视图”提供有关ICC配置文件的以下信息：

* **[!UICONTROL 配置文件类]**：ICC（国际颜色联盟）定义每个类以涵盖一种类型的应用程序。 例如，输入配置文件应用于数码相机和扫描仪等设备，输出配置文件应用于打印机。

* **[!UICONTROL 色彩空间类型]**：此数字是配置文件的“输入”颜色空间，由ICC定义。 颜色空间类型定义颜色空间的组件的数量和对这些组件的解释。例如，RGB 是具有三个组件（红色、绿色和蓝色）的颜色空间。颜色空间类型不定义空间的特定颜色特征（例如，原色的色度）。

* **[!UICONTROL PCS类型]**：此PCS类型是配置文件的“输出”颜色空间 — 其配置文件连接空间。 例如，颜色配置文件可以将 RGB 转换成 PCS，然后转化成 CMYK。

对于有助于标记颜色或图像的输入、显示或输出配置文件，PCS 类型是 XYZ 或 Lab。将该配置文件解释成在 ICC 规范中定义的相应的特定颜色空间。
