---
title: 字体
seo-title: 字体
description: 'null'
seo-description: 了解如何在Dynamic Media Classic中使用字体。
uuid: bddec9c2-8530-4bbd-8db7-1562a347e482
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/support_files
discoiquuid: 97cecd6a-30aa-44fe-a611-fd71b02fd5ae
translation-type: tm+mt
source-git-commit: d5bf894d56687561c93ef08762bc19d3597225e6

---


# 字体{#fonts}

在某些情况下，Scene7 Publishing System 要求您上载字体文件，以便使用特定的字体输入或渲染文本。例如，要在模板图层上将特定的字体用于文本，请上载字体文件。要以特定的字体显示 eCatalog 查看器页码，请上载字体文件。

Dynamic Media Classic支持以下字体类型：

* 所有 TrueType 字体
* PostScript®字体
* OpenType/TrueType 字体
* OpenType/PostScript 字体
* PhotoFont

上载字体文件之后，您可以在“编辑信息”屏幕中更改其 SPS ID、字体名称和类型信息。

>[!NOTE]
>
>如果您计划在模板图层中使用字体，Dynamic Media Classic建议上传所有字体样式（粗体、斜体、粗体／斜体和常规）。 Dynamic Media Classic需要这些字体样式来处理请求。 还建议上载与某种字体相关的所有 PostScript/Adobe Type 1 文件，因为其中的某些字体包含详细的字距调整信息。

## 上载字体文件 {#uploading-font-files}

使用与上载其他文件相同的方法上载字体文件。您可以将字体文件存储在任何 SPS 文件夹中。请参阅[上载文件](uploading-files.md#uploading_your_files)。

## 编辑字体文件信息 {#editing-font-file-information}

您可以更改字体的 ID 名称及其类型信息。编辑字体文件会有助于搜索，并且使得字体更易于识别。

在浏览面板中，选择您要在详细信息视图中编辑的字体文件，然后选择“文件”>“编辑信息”。此时将打开“编辑信息”屏幕。选择下列选项并且选择“提交”按钮。

**字体名称** 此名称在字体发布时标识字体。

**PostScript名称** 此名称是字体的完整PostScript名称。 它通常指示粗细或样式。

**RTF名称** ：此名称显示在创建模板文本层的RTF编辑器的弹出菜单中。

**字体系列名称** 此名称列表字体名称，但不带样式、权重或字体类型指示符。

**字体样式** “纯”、“粗体”、“斜体”和“粗斜体”选项。

**字体类型** “TrueType”和“Adobe Type 1”选项。 如果使用其他名称调用这些字体，可以输入该名称。

**字体类型缩写** ：选项如下所示：

**用于PDF** /PostScript渲染和图像服务的TTF TrueType字体文件。

**AFM** Adobe PostScript字体文件，其中包含Adobe Font Metrics信息并用于图像服务。

**包含二进制字体度量信息的PFM** Adobe PostScript字体文件。

**PFB** Adobe PostScript字体文件，包含二进制字体轮廓信息并用于PDF/PostScript渲染和图像服务。
