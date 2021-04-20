---
title: 使用 PDF
description: 了解如何在Dynamic Media Classic中使用PDF。
uuid: 26d70d28-9393-49b1-9051-d70456deca67
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 5a073de3-6b1d-4c3e-8c03-9182f9f3874a
feature: Dynamic Media Classic,Asset Management
role: Business Practitioner
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '677'
ht-degree: 55%

---


# 使用 PDF{#working-with-pdfs}

Dynamic Media Classic中最常使用PDF(可移植文档格式)文件创建电子目录。 当您上传PDF文件、Dynamic Media Classic栅格化或翻页时，默认情况下会对页面进行栅格化或翻页，以便这些页面可用于构建富媒体。

## PDF 上载选项 {#pdf-upload-options}

当上载 PDF 文件时，您能够以多种方法设置其格式。可以裁切其页面、提取搜索词、输入像素/英寸分辨率以及选择颜色空间。PDF 文件中常常包含修剪边距、裁切标记、对齐标记以及其他打印机的标记。当上载 PDF 文件时，可以从页边裁切这些标记。

上载 PDF 的选项位于“上载”屏幕的“PDF 选项”下。

**处理**

“处理”选项如下所述：

**栅格化** （默认）将翻阅PDF文件中的页面，并将矢量图形转换为位图图像。选择此选项可以创建 eCatalog。

**提取搜** 索词从PDF文件提取词，以便在eCatalog查看器中按关键字搜索文件。

**提取** 链接从PDF文件提取链接，并将其转换为在电子目录查看器中使用的图像映射。

**自动生成包含多页PDF的电子目** 录从PDF文件自动创建电子目录。eCatalog 以您上载的 PDF 文件命名。（只有当上载 PDF 文件时栅格化该文件，才可以使用此选项。）

**分辨率**

确定分辨率设置。该设置确定在 PDF 文件中每英寸显示多少像素。默认值为 150。

**颜色空间**

选择“颜色空间”菜单，并为 PDF 文件选择颜色空间。大多数 PDF 文件既包含 RGB 又包含 CMYK 彩色图像。对于联机查看，首选 RGB 颜色空间。

**自动** 检测保留PDF文件的色彩空间。

**强制作** 为RGBC转换为RGB色彩空间。

**强制为** CMYK转换到CMYK色彩空间。

**强制为灰** 度转换为灰度色彩空间。

**颜色配置文件**

选择“颜色配置文件”选项：

**转换为** sRGBConverts到sRGB（标准红绿蓝）。在网页上显示图像时，推荐使用 sRGB 颜色空间。

**保留原始色彩** 空间保留原始色彩空间。

**“自定”>“** 至打开”菜单，因此您可以选择“从中转换”和“转换为色彩空间”。您可以选择标准Photoshop色彩空间或上传到Dynamic Media Classic的色彩空间。

请参阅[ICC 配置文件](icc-profiles.md#icc_profiles)。

## 从 PDF 文件中裁切空白区域 {#cropping-white-space-from-a-pdf-file}

1. 要在上载 PDF 文件时自动裁切其空白区域像素，请选择“裁切”菜单并选择“修剪”。
1. 指定以下选项：

   **基于修剪移去** 选择是基于颜色还是透明度进行裁剪：

   **颜** 色选择“颜色”选项。然后选择“角”菜单，并选择其颜色最接近于您要裁切的空白区域颜色的 PDF 角。

   **透** 明度选择“透明度”选项。

   **容** 差拖动滑块可指定从0到1的容差：

   **基于颜色** 修剪指定0可仅裁剪与您在PDF角中选择的颜色完全匹配的像素。数字越接近 1，允许的色差越大。

   **基于透明度的** 修剪指定0可仅裁剪完全透明的像素；接近1的数字意味着更加透明。

## 从 PDF 页边裁切 {#cropping-from-the-sides-of-pdf-pages}

当上载 PDF 文件时，可以手动从 PDF 文件中删除页边的打印机标记。

1. 选择“裁切”并选择“手动”。
1. 在“上”、“下”、“左”、“右”文本框中输入像素设置，以便从页面的上、下及两边剪切。

页面被裁切部分的大小取决于您为 PDF 文件输入的“分辨率像素/英寸”选项。例如，如果您输入 150（默认值）作为“分辨率像素/英寸”设置，而从页边裁切 75 像素，则将裁切半英寸，因为对于 150 像素/英寸，75 像素等于半英寸。
