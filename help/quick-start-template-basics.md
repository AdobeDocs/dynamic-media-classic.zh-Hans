---
title: '"快速入门：模板基础"'
description: 模板基础知识简介和快速入门，可帮助您快速启动并运行。
uuid: 16d78cbb-f762-4263-aea9-5712eb933693
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: dd0fbb39-3f6a-496b-a9b6-63b11dcb823a
feature: Dynamic Media Classic
role: User
exl-id: bf695fee-821c-4396-829a-d57ccf475b0c
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '782'
ht-degree: 34%

---

# 快速入门：模板基础{#quick-start-template-basics}

模板基础知识是动态创建和可寻址的分层图像文件，如图像编辑应用程序(如Adobe Photoshop)中的分层文件。 与包含图层的静态文件（如 PSD 文件）不同，模板可以包括参数。通过各种参数，图像的不同方面都可以寻址及自定义。

模板可以包含任意数量的图像图层和文本图层。您可以将包含层（如分层PSD文件）的静态文件转换为模板，并在AdobeDynamic Media Classic中创建模板。 您可以使用上传到AdobeDynamic Media Classic的字体在模板中创建文本层。 将文本添加到模板中之后，可以通过更改其对齐方式、字体、字体大小以及颜色来设置字体格式。

使用“参数”页面，您可以将模板的任何方面转换为可寻址参数。 此时，可以更改要在模板中使用的分层图像或文本值。这些参数是通过 URL 字符串传递的，因此可以通过更改任意参数，动态自定义从图像服务器生成的回复图像。

本快速入门旨在帮助您快速学会如何使用模板基础。

## 1.上传文件

首先请为模板上载 PSD 文件或图像文件。AdobeDynamic Media Classic除了支持PSD之外，还支持许多图像文件格式，但建议模板使用无损的TIFF和PNG图像，因为它们允许透明。

如果使用PSD文件来构建模板，请在上传PSD文件时，在&#x200B;**[!UICONTROL 上传作业选项]**&#x200B;对话框中选择&#x200B;**[!UICONTROL 创建模板]**。 此外，还选择&#x200B;**[!UICONTROL 层命名]**&#x200B;选项，以便AdobeDynamic Media Classic了解在将PSD层上传到AdobeDynamic Media Classic时如何命名这些层。

如果使用的是图像文件，可以在上载时在图像中裁切图像，以及从剪切路径创建蒙版。

在全局导航栏上，单击&#x200B;**[!UICONTROL Upload]** ，将PSD文件或其他图像文件从您的计算机上传到AdobeDynamic Media Classic上的文件夹。 请参阅[上载模板文件](uploading-template-files.md#uploading_template_files)。

## 2.创建模板

要从PSD文件创建模板，请在上传文件时选择&#x200B;**[!UICONTROL 创建模板]**。 要从图像创建模板，请在全局导航栏上单击&#x200B;**[!UICONTROL 生成]** > **[!UICONTROL 模板基础知识]**，输入画布的宽度和高度测量。 在页面的右上角附近，选择&#x200B;**[!UICONTROL Designer]**&#x200B;或&#x200B;**[!UICONTROL Developer]**，然后将图像拖动到“模板”页面上。 您还可以在单击&#x200B;**[!UICONTROL 生成]** > **[!UICONTROL 模板基础知识]**&#x200B;之前选择图像&#x200B;*。*“模板”页面提供了以下工具：

* 添加图像图层。要添加图层，请将图像拖到“模板”页面中。
* 添加文本图层。单击&#x200B;**[!UICONTROL 文本工具]**&#x200B;图标。 拖动指针为文本层创建框；然后，在“文本”(Text)页面上使用工具设置文本格式。
* 更改图层大小和位置。
* 更改图层顺序。
* 将阴影和发光效果应用于图像图层和文本图层。

请参阅[创建模板](creating-template.md#creating_a_template)。

## 3.创建模板参数

接下来是将图层属性参数化，从而确定 URL 字符串中包含哪些图层属性。您可以通过这些参数尽可能灵活地使用模板。图层属性参数化之后，可以动态进行更改。

要对层进行参数化，请在“模板”页中打开模板，然后单击层名称旁边的&#x200B;**[!UICONTROL 参数]**。 在参数页面上，选择要添加的每个参数旁边的选项。 请参阅[创建模板参数](creating-template-parameters.md#creating_template_parameters)。

## 4.发布模板

发布模板会将其放置在Dynamic Media图像服务器上，以便能够将其动态交付到您的网站或应用程序。 发布还会激活URL，以将模板从Dynamic Media图像服务器调用到您的网站或应用程序。

请确保发布与模板相关的所有图像。

要发布模板，请将其标记为发布，然后在“全局导航”栏上单击&#x200B;**[!UICONTROL Publish]**。 然后，单击&#x200B;**[!UICONTROL 提交发布]**。 请参阅[发布模板](publishing-templates.md#publishing_templates)。

## 5.将模板链接到网页

Dynamic Media Classic会为模板创建URL，并在您将模板发布到Dynamic Media图像服务器时激活这些URL。 您可以从“模板预览”页面复制这些URL字符串。

在“浏览”面板中选择您的模板，然后单击&#x200B;**[!UICONTROL 预览]**&#x200B;以打开“模板预览”页面。 选择用于传送模板的图像预设，然后单击&#x200B;**[!UICONTROL 复制URL]**。 从“预览”页面复制URL后，即可在您的网站或应用程序中使用它。 请参阅[将模板链接至网页](linking-template-web-page.md#linking_a_template_to_a_web_page)。
