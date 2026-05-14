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
autotag-review: '2026-05-13T19:59:42.608Z'
TQID: 'https://experienceleague.adobe.com/eGKamqA47mITzfyTuHoFYLfWEXOP0jAl5XWDpihGjZA'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
  - id: d378ca77-2da1-4f39-ad92-1917fe974a38
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 0d05ca7402db1d8894db1127088905143fb97cff
workflow-type: tm+mt
source-wordcount: 528
ht-degree: 31%

---

# ICC 配置文件{#icc-profiles}

ICC（国际颜色联盟）配置文件是一个文件，用于描述如何正确地将图像文件从一个色彩空间转换到另一个色彩空间。 ICC 配置文件有助于为图像获取正确的颜色。 例如，要正确显示设计用于在计算机显示器上打印的图像，可以选择ICC配置文件。 该配置文件将图像转换到不同的颜色空间并确保颜色正确地联机显示。

在Adobe Dynamic Media Classic中，您可以选择在上传图像时将ICC配置文件转换为其他颜色空间。 默认情况下，所有标准Photoshop ICC配置文件在Adobe Dynamic Media Classic上均可用。 要在“上载”屏幕中查看颜色配置文件的名称，请选择“颜色配置文件”菜单。 然后选择“自定义从>到”，再从“转换至”和“转换到”菜单中选择 ICC 配置文件的名称。

在上传[&#128279;](image-editing-options-upload.md#image-editing-options-at-upload)中查看图像编辑选项。

除了使用默认的ICC配置文件外，您还可以将其他ICC配置文件上传到Adobe Dynamic Media Classic，以便用于色彩空间转换。 在“浏览”面板中切换到“详细视图”以调查ICC配置文件的配置文件类、色彩空间类型和PCS类型。

总之，ICC配置文件的要点如下：

* ICC配置文件为图像文件启用不同色彩空间之间的正确色彩转换。
* Adobe Dynamic Media Classic整合了所有标准的Photoshop ICC配置文件，以实现强大的图像转换。
* 自定义ICC配置文件可增加灵活性，以满足高级色彩空间转换需求。
* 在详细信息视图中查看配置文件类和PCS类型等详细信息有助于管理ICC设置。
* 上传ICC配置文件非常简单，并且可确保跨Dynamic Media Classic中的文件夹进行访问。


## 上传ICC配置文件 {#uploading-icc-profiles}

通过与上载文件时所使用的技术相同的技术上载 ICC 配置文件。 您可以将ICC配置文件存储在任何Adobe Dynamic Media Classic文件夹中。

查看[上传您的文件](uploading-files.md#uploading_your_files)。

## 检查ICC配置文件 {#examining-an-icc-profile}

要检查ICC配置文件，请在“浏览”面板中选择它，并在“详细信息视图”中显示它。 “详细信息视图”提供有关ICC配置文件的以下信息：

* **[!UICONTROL 配置文件类]**： ICC定义每个类以覆盖应用程序类型。 例如，输入配置文件适用于数码相机和扫描仪等设备。 输出配置文件适用于打印机。

* **[!UICONTROL 色彩空间类型]**：此数字是配置文件的“输入”色彩空间，由ICC定义。 颜色空间类型定义颜色空间的组件的数量和对这些组件的解释。 例如，RGB 是具有三个组件（红色、绿色和蓝色）的颜色空间。 颜色空间类型不定义空间的特定颜色特征（例如，原色的色度）。

* **[!UICONTROL PCS类型]**：此PCS类型是配置文件的“输出”颜色空间 — 其配置文件连接空间。 例如，颜色配置文件可以将 RGB 转换成 PCS，然后转化成 CMYK。

对于用于标记颜色或图像的输入、显示或输出配置文件，PCS类型为XYZ或Lab。 将该配置文件解释成在 ICC 规范中定义的相应的特定颜色空间。
