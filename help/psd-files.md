---
title: 使用 PSD 文件
seo-title: 使用 PSD 文件
description: 'null'
seo-description: 了解如何处理PSD文件。
uuid: 5836b660-6bca-46e7-ab39-1a31 d1 e0 cff2
contentOwner: admin
content-type: 引用
products: SG_ EXPERIENCE MANAGER/Dynamic-Media-Scene-7
geptopics: SG_ SCENESELEFERENDER_ PK/categories/master_ files
discoiquuid: 4086e3db-5aca-41a0-8f15-302afbf67ddb
translation-type: tm+mt
source-git-commit: a1722c15d3c049f05959d895e85297d47d730872

---


# 使用 PSD 文件{#working-with-psd-files}

PSD(Photoshop文档文件)常用于动态媒体经典中创建模板。上传PSD文件时，可以从文件中自动创建Dynamic Media经典模板(在上传屏幕上选择“创建模板”选项)。

如果您使用 PSD 文件创建模板，SPS 会通过具有多个图层的该文件创建多个图像；它将为每个图层创建一个图像。

## PSD 上载选项 {#psd-upload-options}

用于上载 PSD 文件的选项位于“Photoshop 选项”下方的“上载作业”选项中。您可以裁切文件、为其选择颜色配置文件、使用该文件创建模板，以及选择锚点。

以下选项在上载 PSD 文件时可用：

**裁剪(** 位于裁剪选项下)。选择“修剪”将自动从 PSD 文件的边缘裁切空白区域；选择“手动”将裁切 PSD 文件的边：

**修剪** 选择“修剪离开基于”菜单，然后选择“颜色”或“透明度”。

如果选择“颜色”选项，请选择“角”菜单，并选择其颜色最接近于您要裁切的空白区域颜色的 PSD 角。

拖动滑块以指定容差，范围为 0 至 1：

基于颜色修剪时，如果指定为 0，则仅裁切与 PSD 角中选定颜色精确匹配的像素。数字越接近 1，允许的色差越大。

基于透明度修剪时，如果指定为 0，则仅裁切完全透明的像素；数字越接近 1，则裁切透明度越高的像素。

**手动** 输入从图像的任一边或每侧裁剪的像素数。图像被裁切部分的大小取决于图像文件中的 ppi（像素/英寸）设置。例如，如果图像显示 150 ppi，您在“上”、“下”、“左”、“右”文本框中输入 75，则将从图像各边裁切半英寸。

**颜色配置文件** (位于“颜色配置文件选项”下)。选择一个选项：

**转换为sRGB(默认)** 转换为sRGB(标准红绿蓝)。在网页上显示图像时，推荐使用 sRGB 颜色空间。

**保留原始颜色空间** 保留图像的原始色彩空间。

**“自定义自”&gt;“打开** 菜单”，以便您可以选择“从中转换”和“转换为色彩空间”。您可以选择标准 Pgotoshop 颜色空间或上载到 SPS 的颜色空间。请参阅ICC 配置文件。

**保持图层** 将PSD中的图层(如果有)呈现到单个资源中。资源图层仍然与 PSD 关联。查看方法是，在详细信息视图中打开 PSD 文件，然后选择图层面板。请参阅查看和编辑 PSD 文件中的图层。

**创建模板** 从PSD文件中的图层创建模板。

**提取文本** 提取文本，以便用户可以在查看器中搜索文本。

**将图层扩展到背景大小** 将撕裂的图像层的大小扩展到背景图层的大小。

**PSD文件中的图层命名** 图层以单独的图像上传。在 Scene7 Publishing System 中选择选项以命名这些图像。

**图层名称** 在PSD文件中其图层名称之后命名图像。例如，原始 PSD 文件中名为“Price Tag”的图层将成为名为“Price Tag”的图像。但是，如果 PSD 文件中的图层名称是默认 Photoshop 图层名称（“Background”、“Layer 1”、“Layer 2”等等），将以该文件中的图层编号而不是默认图层名称为图像命名。

**Photoshop和图层编号** 在PSD文件中的图层编号之后命名图像，忽略原始图层名称。使用 Photoshop 文件名和附加的图层编号为图像命名。例如，在名为“Spring Ad.psd”的文件中，即使第二个图层在 Photoshop 中具有非默认名称，也会以“Spring Ad_2”命名该图层。

**Photoshop和图层名称** 在PSD文件后面命名图像，后跟图层名称或图层编号。如果 PSD 文件中的图层名称是默认的 Photoshop 图层名称，则将使用图层编号。例如，在 PSD 文件“SpringAd”中名为“Price Tag”的图层将命名为“Spring Ad_Price Tag”。具有默认名称“Layer 2”的图层命名为“Spring Ad_2”。

**锚点** 指定图像在从PSD文件生成的分层合成生成的模板中定位的方式。默认情况下，锚点是中心。中心锚点允许替换图像尽可能占据相同的空间，无论替换图像的高宽比是多少。当引用模板并使用参数替换时，替换该图像的高宽比不同的图像有效地占据相同的空间。如果应用程序要求替换图像占据模板中分配的空间，请更改为其他设置。

## 查看和编辑 PSD 文件中的图层 {#viewing-and-editing-layers-in-a-psd-file}

如果您在上传PSD时选择了“维护图层”选项，则Dynamic Media经典将各个图层翻录到资源中。您可以在浏览面板的详细信息视图中打开 PSD 文件，以查看和编辑属于该文件的资源图层。

1. 在浏览面板中双击完整的 PSD 文件，则可以在详细信息视图中打开该文件。

   ***注意**：确保打开完整的资源，而不是打开其中一个PSD图层。*

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

