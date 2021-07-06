---
title: ICC 配置文件
description: 了解ICC配置文件。
uuid: 708ff2ad-9a47-4e3e-b643-5b19648f726b
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/support_files
discoiquuid: 44f1b4c4-6d7f-4e0f-84ce-11d26745e0f0
feature: Dynamic Media Classic
role: User
exl-id: 989f2761-f5d0-4ece-b2a6-f7b4577aa8a2
source-git-commit: df689ff5a127bfbc400ca5331168d1ff7bb0b42e
workflow-type: tm+mt
source-wordcount: '442'
ht-degree: 71%

---

# ICC 配置文件{#icc-profiles}

ICC （国际色彩联盟）配置文件是描述如何正确地将图像文件从一个颜色空间转换到另一个颜色空间的文件。ICC 配置文件有助于为图像获取正确的颜色。例如，到正确地显示用于在计算机显示器上打印的图像，可以选择 ICC 配置文件。该配置文件将图像转换到不同的颜色空间并确保颜色正确地联机显示。

在Dynamic Media Classic中，您可以选择ICC配置文件，以在上传图像时将图像转换为不同的色彩空间。 默认情况下，所有标准Photoshop ICC配置文件均在Dynamic Media Classic上可用。 要在“上载”屏幕中查看颜色配置文件的名称，请选择“颜色配置文件”菜单。然后选择“自定义从>到”，再从“转换至”和“转换到”菜单中选择 ICC 配置文件的名称。

请参阅[上载时的图像编辑选项](image-editing-options-upload.md#image-editing-options-at-upload)。

除了使用默认的ICC配置文件外，您还可以将其他ICC配置文件上传到Dynamic Media Classic，并使其可用于色彩空间转换。 在浏览面板中切换到详细信息视图，以便调查 ICC 配置文件的配置文件类、颜色空间类型和 PCS 类型。

## 上载 ICC 配置文件 {#uploading-icc-profiles}

通过与上载文件时所使用的技术相同的技术上载 ICC 配置文件。您可以将ICC配置文件存储在任何Dynamic Media Classic文件夹中。

请参阅[上载文件](uploading-files.md#uploading_your_files)。

## 检查 ICC 配置文件 {#examining-an-icc-profile}

要检查 ICC 配置文件，请在浏览面板中选择该文件并在详细信息视图中进行显示。详细信息视图提供有关 ICC 配置文件的以下信息：

* **配置文件类**  - ICC（国际颜色联盟）定义每个类以涵盖应用程序类型。例如，输入配置文件应用于数码相机和扫描仪等设备，输出配置文件应用于打印机。

* **色彩空间类型**  — 此数字是配置文件的“输入”色彩空间，由ICC定义。颜色空间类型定义颜色空间的组件的数量和对这些组件的解释。例如，RGB 是具有三个组件（红色、绿色和蓝色）的颜色空间。颜色空间类型不定义空间的特定颜色特征（例如，原色的色度）。

* **PCS类型**  — 此PCS类型是配置文件的“输出”颜色空间，即其配置文件连接空间。例如，颜色配置文件可以将 RGB 转换成 PCS，然后转化成 CMYK。

对于有助于标记颜色或图像的输入、显示或输出配置文件，PCS 类型是 XYZ 或 Lab。将该配置文件解释成在 ICC 规范中定义的相应的特定颜色空间。
