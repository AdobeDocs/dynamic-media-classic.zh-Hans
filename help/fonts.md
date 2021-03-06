---
title: 字体
description: 了解如何在AdobeDynamic Media Classic中使用字体。
uuid: bddec9c2-8530-4bbd-8db7-1562a347e482
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/support_files
discoiquuid: 97cecd6a-30aa-44fe-a611-fd71b02fd5ae
feature: Dynamic Media Classic
role: User
exl-id: 186f4c7f-16f6-42f5-bc0e-55362c55e794
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 28%

---

# 字体{#fonts}

有时，AdobeDynamic Media Classic会要求您上传字体文件，以输入或渲染特定字体的文本。 例如，要在模板图层上将特定的字体用于文本，请上载字体文件。要以特定的字体显示 eCatalog 查看器页码，请上载字体文件。

AdobeDynamic Media Classic支持以下字体类型：

* 所有 TrueType 字体
* PostScript®字体
* OpenType/TrueType 字体
* OpenType/PostScript 字体
* PhotoFont

上传字体文件后，您可以更改其AdobeDynamic Media Classic ID、字体名称，以及在“编辑信息”屏幕上键入信息。

>[!NOTE]
>
>AdobeDynamic Media Classic如果您计划在模板图层中使用字体，则建议上传所有字体样式（粗体、斜体、粗体/斜体和常规）。 AdobeDynamic Media Classic需要这些字体样式来处理请求。 还建议上载与某种字体相关的所有 PostScript/Adobe Type 1 文件，因为其中的某些字体包含详细的字距调整信息。

## 上传字体文件 {#uploading-font-files}

使用与上载其他文件相同的方法上载字体文件。您可以将字体文件存储在任何Adobe的Dynamic Media Classic文件夹中。 请参阅[上载文件](uploading-files.md#uploading_your_files)。

## 编辑字体文件信息 {#editing-font-file-information}

您可以更改字体的ID名称及其类型信息。 编辑字体文件会有助于搜索，并且使得字体更易于识别。

在“浏览”面板中，选择要在“详细信息视图”中编辑的字体文件，然后选择“文件”>“编辑信息”。 此时将打开“编辑信息”屏幕。选择以下选项，然后选择&#x200B;**[!UICONTROL Submit]**。

* **[!UICONTROL 字体名称]**  — 此名称在发布时标识字体。

* **[!UICONTROL PostScript名称]**  — 此名称是字体的完整PostScript名称。它通常指示粗细或样式。

* **[!UICONTROL RTF名称]**  — 此名称显示在RTF编辑器的弹出菜单中，其中创建了模板文本层。

* **[!UICONTROL 字体系列名称]**  — 此名称列出不带样式、粗细或字体类型指示符的字体名称。

* **[!UICONTROL 字体样式]**  — 选项为纯、粗体、斜体和粗体斜体。

* **[!UICONTROL 字体类型]**  — 选项为TrueType和Adobe Type1。如果使用其他名称调用这些字体，可以输入该名称。

* **[!UICONTROL 字体类型缩写]**  — 选项如下：

   * **[!UICONTROL TTF]**  — 用于PDF/PostScript渲染和图像提供的TrueType字体文件。

   * **[!UICONTROL AFM]**  — 包含Adobe字体量度信息并用于图像提供的Adobe PostScript字体文件。

   * **[!UICONTROL PFM]**  — 包含二进制字体量度信息的Adobe PostScript字体文件。

   * **[!UICONTROL PFB]**  — 包含二进制字体轮廓信息的Adobe PostScript字体文件，用于PDF/PostScript渲染和图像提供。
