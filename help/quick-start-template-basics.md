---
title: '"快速入门：模板基础"'
description: 模板基础知识的简介和快速开始，可帮助您快速入门和使用。
uuid: 16d78cbb-f762-4263-aea9-5712eb933693
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: dd0fbb39-3f6a-496b-a9b6-63b11dcb823a
feature: Dynamic Media Classic
role: Business Practitioner
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '789'
ht-degree: 71%

---


# Quick Start: Template Basics{#quick-start-template-basics}

模板基础是动态创建和可寻址的分层图像文件，如图像编辑应用程序(如Adobe Photoshop)中的分层文件。 与包含图层的静态文件（如 PSD 文件）不同，模板可以包括参数。通过各种参数，图像的不同方面都可以寻址及自定义。

模板可以包含任意数量的图像图层和文本图层。您可以将包含图层（如分层的PSD文件）的静态文件转换为模板，并在Dynamic Media Classic中创建模板。 您可以使用上传到Dynamic Media Classic中的字体在模板中创建文本图层。 将文本添加到模板中之后，可以通过更改其对齐方式、字体、字体大小以及颜色来设置字体格式。

通过“参数”屏幕，可以将模板的任意方面转换为可寻址的参数。此时，可以更改要在模板中使用的分层图像或文本值。这些参数是通过 URL 字符串传递的，因此可以通过更改任意参数，动态自定义从图像服务器生成的回复图像。

**快速开始**

本快速入门旨在帮助您快速学会如何使用模板基础。

**1. 上载文件**

首先请为模板上载 PSD 文件或图像文件。Dynamic Media Classic除了支持PSD外，还支持许多图像文件格式，但建议模板使用无损的TIFF和PNG图像，因为它们允许透明。

如果构建模板时使用的是 PSD 文件，请在上载 PSD 文件时，从“上载作业选项”对话框中选择“创建模板”选项。还选择“图层命名”选项，告诉Dynamic Media Classic在将PSD图层上传到Dynamic Media Classic时如何命名这些图层。

如果使用的是图像文件，可以在上载时在图像中裁切图像，以及从剪切路径创建蒙版。

选择全局导航栏上的“上传”按钮，将PSD文件或其他图像文件从您的计算机上传到Dynamic Media Classic上的文件夹。 请参阅[上载模板文件](uploading-template-files.md#uploading_template_files)。

**2.创建模板**

要从 PSD 文件创建模板，请在上载文件时选择“创建模板”选项。要从图像创建模板，请选择“构建”>“模板基础”，输入画布的宽度和高度，选择“设计器”或“开发者”，然后将图像拖到“模板”屏幕上。也可以先选择图像，然后再选择“构建”>“模板基础”。“模板”屏幕提供的工具可用于：

* 添加图像图层。要添加图层，请将图像拖到“模板”屏幕中。
* 添加文本图层。选择文本工具  并拖动来绘制文本图层框；然后使用“文本”屏幕上的工具来设置文本格式。
* 更改图层大小和位置。
* 更改图层顺序。
* 将阴影和发光效果应用于图像图层和文本图层。

请参阅[创建模板](creating-template.md#creating_a_template)。

**3.创建模板参数**

接下来是将图层属性参数化，从而确定 URL 字符串中包含哪些图层属性。您可以通过这些参数尽可能灵活地使用模板。图层属性参数化之后，可以动态进行更改。

要参数化图层，请在“模板”屏幕中打开模板，并选择图层名称旁边的“参数”按钮。在“参数”屏幕上，选择要添加的各个参数旁边的选项。请参阅[创建模板参数](creating-template-parameters.md#creating_template_parameters)。

**4.发布模板**

发布模板时，模板会放置在Dynamic Media图像服务器上，以便能够动态地将其交付到您的网站或应用程序。 发布还会激活URL，以从Dynamic Media图像服务器将模板调用到您的网站或应用程序。

请确保发布与模板相关的所有图像。

要发布模板，请将其标记为发布，然后在全局导航栏上选择“发布”按钮。然后选择“开始发布”按钮。请参阅[发布模板](publishing-templates.md#publishing_templates)。

**5.将模板链接至网页**

Dynamic Media Classic为模板创建URL，并在将模板发布到Dynamic Media图像服务器时激活URL。 可以从“模板预览”屏幕复制这些 URL 字符串。

在浏览面板中选择模板，然后单击“预览”按钮，打开“模板预览”屏幕。然后选择“图像预设”来发送模板，并选择“复制 URL”按钮。从“预览”屏幕复制 URL 后，可以将其用于您的网站或应用程序中。请参阅[将模板链接至网页](linking-template-web-page.md#linking_a_template_to_a_web_page)。
