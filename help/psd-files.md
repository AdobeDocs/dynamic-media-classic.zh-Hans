---
title: 使用 PSD 文件
seo-title: 使用 PSD 文件
description: 'null'
seo-description: 了解如何使用PSD文件。
uuid: 5836b660-6bca-46e7-ab39-1a31d1e0cff2
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 4086e3db-5aca-41a0-8f15-302afbf67ddb
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '1030'
ht-degree: 64%

---


# 使用 PSD 文件{#working-with-psd-files}

PSD(Photoshop文档文件)在Dynamic Media经典中最常用于创建模板。 上传PSD文件时，可以从文件自动创建Dynamic Media经典模板（在“上传”屏幕上选择“创建模板”选项）。

Dynamic Media经典(PSD)文件使用图层创建模板时，会从PSD文件创建多幅图像；它为每个图层创建一个图像。

## PSD 上载选项 {#psd-upload-options}

用于上载 PSD 文件的选项位于“Photoshop 选项”下方的“上载作业”选项中。您可以裁切文件、为其选择颜色配置文件、使用该文件创建模板，以及选择锚点。

以下选项在上载 PSD 文件时可用：

**裁剪** （位于“裁剪选项”下。）选择“修剪”将自动从 PSD 文件的边缘裁切空白区域；选择“手动”将裁切 PSD 文件的边：

**修** 剪根据菜单选择“修剪掉”，然后选择“颜色”或“透明度”。

如果选择“颜色”选项，请选择“角”菜单，并选择其颜色最接近于您要裁切的空白区域颜色的 PSD 角。

拖动滑块以指定容差，范围为 0 至 1：

基于颜色修剪时，如果指定为 0，则仅裁切与 PSD 角中选定颜色精确匹配的像素。数字越接近 1，允许的色差越大。

基于透明度修剪时，如果指定为 0，则仅裁切完全透明的像素；数字越接近 1，则裁切透明度越高的像素。

**手** 动输入要从图像的任何一侧或每一侧裁剪的像素数。图像被裁切部分的大小取决于图像文件中的 ppi（像素/英寸）设置。例如，如果图像显示 150 ppi，您在“上”、“下”、“左”、“右”文本框中输入 75，则将从图像各边裁切半英寸。

**颜色用户档案** (位于“颜色用户档案选项”下。)选择一个选项：

**转换为sRGB（默认）** 转换为sRGB（标准红绿蓝）。在网页上显示图像时，推荐使用 sRGB 颜色空间。

**保留原始颜** 色空间保留图像的原始色彩空间。

**“自定义自”>“** 至打开”菜单，因此您可以选择“转换自”和“转换为色彩空间”。您可以选择标准的Photoshop色彩空间或上传到Dynamic Media经典的色彩空间。 请参阅ICC 配置文件。

**维** 护图层将PSD中的图层（如果有）拆分为单个资源。资源图层仍然与 PSD 关联。查看方法是，在详细信息视图中打开 PSD 文件，然后选择图层面板。请参阅查看和编辑 PSD 文件中的图层。

**创** 建模板从PSD文件中的图层创建模板。

**提取** 文本提取文本，以便用户在查看器中搜索文本。

**将图层扩展到背** 景大小将已撕开的图像图层的大小扩展到背景图层的大小。

**图** 层命名PSD文件中的图层作为单独的图像上传。选择一个选项，在Dynamic Media经典中命名这些图像：

**图层** 名称在PSD文件中将图像命名为图层名称之后。例如，原始 PSD 文件中名为“Price Tag”的图层将成为名为“Price Tag”的图像。但是，如果 PSD 文件中的图层名称是默认 Photoshop 图层名称（“Background”、“Layer 1”、“Layer 2”等等），将以该文件中的图层编号而不是默认图层名称为图像命名。

**Photoshop和图** 层编号在PSD文件中将图像命名为图层编号之后，忽略原始图层名称。使用 Photoshop 文件名和附加的图层编号为图像命名。例如，在名为“Spring Ad.psd”的文件中，即使第二个图层在 Photoshop 中具有非默认名称，也会以“Spring Ad_2”命名该图层。

**Photoshop和图** 层名称在PSD文件后面命名图像，后跟图层名称或图层编号。如果 PSD 文件中的图层名称是默认的 Photoshop 图层名称，则将使用图层编号。例如，在 PSD 文件“SpringAd”中名为“Price Tag”的图层将命名为“Spring Ad_Price Tag”。具有默认名称“Layer 2”的图层命名为“Spring Ad_2”。

**锚** 点指定如何在从PSD文件生成的分层合成生成的模板中定位图像。默认情况下，锚点是中心。中心锚点允许替换图像尽可能占据相同的空间，无论替换图像的高宽比是多少。当引用模板并使用参数替换时，替换该图像的高宽比不同的图像有效地占据相同的空间。如果应用程序要求替换图像占据模板中分配的空间，请更改为其他设置。

## 查看和编辑 PSD 文件中的图层 {#viewing-and-editing-layers-in-a-psd-file}

如果您在上传PSD时选择了“维护图层”选项，Dynamic Media经典会将各个图层拆分为资产。 您可以在浏览面板的详细信息视图中打开 PSD 文件，以查看和编辑属于该文件的资源图层。

1. 在浏览面板中双击完整的 PSD 文件，则可以在详细信息视图中打开该文件。

   ***注&#x200B;**:确保打开完整资产，而不是某个PSD图层。*

1. 单击“图层”打开“图层”面板。在“图层”面板中将以单独的图像显示所有各图层。
1. 双击图层打开该图层并执行以下任一操作：

   * 单击“图像映射”图标在图层上创建图像映射。（请参阅[创建图像映射](creating-image-maps.md#creating_image_maps)。）
   * 单击“缩放目标”图标在图层上创建缩放目标。（请参阅[为引导式缩放创建缩放目标](creating-zoom-targets-guided-zoom.md#creating_zoom_targets_for_guided_zoom)。）
   * 单击“裁切”图标裁切图层。（请参阅[裁切图像](cropping-image.md#cropping_an_image)。）
   * 单击“锐化”锐化图层。（请参阅[锐化图像](sharpening-image.md#sharpening_an_image)。）
   * 单击“调整”调整图层。（请参阅[调整图像](adjusting-image.md#adjusting_an_image)。）

1. 单击“保存”或“另存为”。
1. 要查看或编辑其他图层，请单击图层预览底部的箭头。
1. 要退出图层详细信息视图，请单击“网格视图”图标。

