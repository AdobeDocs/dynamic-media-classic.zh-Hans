---
title: 字体
description: 了解如何在Dynamic Media Classic中使用字体。
uuid: bddec9c2-8530-4bbd-8db7-1562a347e482
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/support_files
discoiquuid: 97cecd6a-30aa-44fe-a611-fd71b02fd5ae
feature: Dynamic Media Classic
role: Business Practitioner
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '432'
ht-degree: 39%

---


# 字体{#fonts}

在某些情况下，Dynamic Media Classic要求您上传字体文件以输入或渲染特定字体中的文本。 例如，要在模板图层上将特定的字体用于文本，请上载字体文件。要以特定的字体显示 eCatalog 查看器页码，请上载字体文件。

Dynamic Media Classic支持以下字体类型：

* 所有 TrueType 字体
* PostScript®字体
* OpenType/TrueType 字体
* OpenType/PostScript 字体
* PhotoFont

上传字体文件后，您可以在“编辑信息”屏幕中更改其Dynamic Media Classic ID、字体名称和类型信息。

>[!NOTE]
>
>Dynamic Media Classic建议上传所有字体样式（粗体、斜体、粗体/斜体和常规），如果您计划在模板图层中使用字体。 Dynamic Media Classic需要这些字体样式来处理请求。 还建议上载与某种字体相关的所有 PostScript/Adobe Type 1 文件，因为其中的某些字体包含详细的字距调整信息。

## 上载字体文件 {#uploading-font-files}

使用与上载其他文件相同的方法上载字体文件。您可以将字体文件存储在任何Dynamic Media Classic文件夹中。 请参阅[上载文件](uploading-files.md#uploading_your_files)。

## 编辑字体文件信息  {#editing-font-file-information}

您可以更改字体的 ID 名称及其类型信息。编辑字体文件会有助于搜索，并且使得字体更易于识别。

在浏览面板中，选择您要在详细信息视图中编辑的字体文件，然后选择“文件”>“编辑信息”。此时将打开“编辑信息”屏幕。选择下列选项并且选择“提交”按钮。

**字** 体名称此名称在发布时标识字体。

**PostScript名** 称此名称是字体的完整PostScript名称。它通常指示粗细或样式。

**RTF名** 称此名称显示在创建模板文本图层的RTF编辑器的弹出菜单中。

**字体系** 列名称此名称列表字体名称，但不带样式、权重或字体类型指示符。

**字** 体样式选项为纯、粗、斜体和粗斜体。

**字** 体类型选项为TrueType和Adobe Type1。如果使用其他名称调用这些字体，可以输入该名称。

**字体类** 型缩写选项如下：

**用** 于PDF/PostScript渲染和图像服务的TTFTrueType字体文件。

**包** 含Adobe字体量度信息并用于图像服务的AFMAdobe PostScript字体文件。

**包** 含二进制字体量度信息的PFMAdobe PostScript字体文件。

**包** 含二进制字体轮廓信息的PFBAdobe PostScript字体文件，用于PDF/PostScript渲染和图像服务。
