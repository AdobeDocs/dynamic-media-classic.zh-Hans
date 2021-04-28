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
exl-id: bf695fee-821c-4396-829a-d57ccf475b0c
translation-type: tm+mt
source-git-commit: c5c8c4f96f18339734f4441733cdb1e7f34d3071
workflow-type: tm+mt
source-wordcount: '779'
ht-degree: 34%

---

# Quick Start: Template Basics{#quick-start-template-basics}

模板基础是动态创建和可寻址的分层图像文件，如图像编辑应用程序(如Adobe Photoshop)中的分层文件。 与包含图层的静态文件（如 PSD 文件）不同，模板可以包括参数。通过各种参数，图像的不同方面都可以寻址及自定义。

模板可以包含任意数量的图像图层和文本图层。您可以将包含图层（如分层的PSD文件）的静态文件转换为模板，并在Dynamic Media Classic中创建模板。 您可以使用上传到Dynamic Media Classic中的字体在模板中创建文本图层。 将文本添加到模板中之后，可以通过更改其对齐方式、字体、字体大小以及颜色来设置字体格式。

使用“参数”页，您可以将模板的任何方面转换为可寻址的参数。 此时，可以更改要在模板中使用的分层图像或文本值。这些参数是通过 URL 字符串传递的，因此可以通过更改任意参数，动态自定义从图像服务器生成的回复图像。

本快速入门旨在帮助您快速学会如何使用模板基础。

## 1.上传文件

首先请为模板上载 PSD 文件或图像文件。Dynamic Media Classic除了支持PSD外，还支持许多图像文件格式，但建议模板使用无损的TIFF和PNG图像，因为它们允许透明。

如果您使用PSD文件来构建模板，请在上传PSD文件时，在&#x200B;**[!UICONTROL 上传作业选项]**&#x200B;对话框中选择&#x200B;**[!UICONTROL 创建模板]**。 还可以选择&#x200B;**[!UICONTROL 图层命名]**&#x200B;选项，以便Dynamic Media Classic了解在将PSD图层上传到Dynamic Media Classic时如何命名这些图层。

如果使用的是图像文件，可以在上载时在图像中裁切图像，以及从剪切路径创建蒙版。

在“全局导航”栏上，单击&#x200B;**[!UICONTROL 上传]**，将PSD文件或其他图像文件从计算机上传到Dynamic Media Classic上的文件夹。 请参阅[上载模板文件](uploading-template-files.md#uploading_template_files)。

## 2.创建模板

要从PSD文件创建模板，请在上传文件时选择&#x200B;**[!UICONTROL 创建模板]**。 要从图像创建模板，请在全局导航栏上，单击&#x200B;**[!UICONTROL 构建]** > **[!UICONTROL 模板基础]**，输入画布的宽度和高度度量。 在页面的右上角附近，选择&#x200B;**[!UICONTROL Designer]**&#x200B;或&#x200B;**[!UICONTROL Developer]**，然后将图像拖到“模板”页面上。 您还可以在单击&#x200B;**[!UICONTROL 构建]** > **[!UICONTROL 模板基础]**&#x200B;之前选择图像&#x200B;*。*“模板”页面优惠工具用于：

* 添加图像图层。要添加图层，请将图像拖入“模板”页面。
* 添加文本图层。单击&#x200B;**[!UICONTROL 文本工具]**&#x200B;图标。 拖动指针，为文本图层创建框；然后，使用“文本”页面上的工具设置文本格式。
* 更改图层大小和位置。
* 更改图层顺序。
* 将阴影和发光效果应用于图像图层和文本图层。

请参阅[创建模板](creating-template.md#creating_a_template)。

## 3.创建模板参数

接下来是将图层属性参数化，从而确定 URL 字符串中包含哪些图层属性。您可以通过这些参数尽可能灵活地使用模板。图层属性参数化之后，可以动态进行更改。

要参数化图层，请在“模板”页中打开该模板，然后单击图层名称旁的&#x200B;**[!UICONTROL 参数]**。 在“参数”页上，选择要添加的每个参数旁边的选项。 请参阅[创建模板参数](creating-template-parameters.md#creating_template_parameters)。

## 4.发布模板

发布模板时，模板会放置在Dynamic Media图像服务器上，以便能够动态地将其交付到您的网站或应用程序。 发布还会激活URL，以从Dynamic Media图像服务器将模板调用到您的网站或应用程序。

请确保发布与模板相关的所有图像。

要发布模板，请将其标记为发布，并在全局导航栏上单击&#x200B;**[!UICONTROL 发布]**。 然后单击&#x200B;**[!UICONTROL 提交发布]**。 请参阅[发布模板](publishing-templates.md#publishing_templates)。

## 5.将模板链接到网页

Dynamic Media Classic为模板创建URL，并在将模板发布到Dynamic Media图像服务器时激活URL。 您可以从“模板”预览页复制这些URL字符串。

在浏览面板中选择您的模板，然后单击&#x200B;**[!UICONTROL 预览]**&#x200B;以打开“模板”预览页。 选择用于传送模板的图像预设，然后单击&#x200B;**[!UICONTROL 复制URL]**。 从预览页复制URL后，即可在网站或应用程序中使用它。 请参阅[将模板链接至网页](linking-template-web-page.md#linking_a_template_to_a_web_page)。
