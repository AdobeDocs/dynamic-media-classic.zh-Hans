---
title: 使用 PDF
description: 了解如何在Dynamic Media Classic中使用PDFAdobe。
uuid: 26d70d28-9393-49b1-9051-d70456deca67
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 5a073de3-6b1d-4c3e-8c03-9182f9f3874a
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 02892514-61fe-48ba-a2e3-eeb30580a1e4
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '662'
ht-degree: 45%

---

# 使用 PDF{#working-with-pdfs}

PDF（可移植文档格式）文件最常用于AdobeDynamic Media Classic以创建电子目录。 在上传PDF文件、AdobeDynamic Media Classic时，默认情况下会对页面进行栅格化或锐化，以便这些页面可用于构建富媒体。

## PDF 上载选项 {#pdf-upload-options}

当上载 PDF 文件时，您能够以多种方法设置其格式。可以裁切其页面、提取搜索词、输入像素/英寸分辨率以及选择颜色空间。PDF 文件中常常包含修剪边距、裁切标记、对齐标记以及其他打印机的标记。当上载 PDF 文件时，可以从页边裁切这些标记。

上传PDF文件的选项位于“PDF选项”下的“上传”页面上。

### 处理选项

**栅格化**  — （默认）去除PDF文件中的页面，并将矢量图形转换为位图图像。要创建eCatalog，请选择此选项。

**提取搜索词**  — 从PDF文件中提取词语，以便在eCatalog查看器中按关键字搜索文件。

**提取链接**  — 从PDF文件中提取链接，并将其转换为在eCatalog查看器中使用的图像映射。

**自动生成包含多页面PDF的eCatalog**  — 从PDF文件自动创建eCatalog。eCatalog 以您上载的 PDF 文件命名。（只有当上载 PDF 文件时栅格化该文件，才可以使用此选项。）

### 分辨率

确定分辨率设置。该设置确定在 PDF 文件中每英寸显示多少像素。默认值为 150。

### 颜色空间选项

选择“颜色空间”菜单，并为 PDF 文件选择颜色空间。大多数 PDF 文件既包含 RGB 又包含 CMYK 彩色图像。对于联机查看，首选 RGB 颜色空间。

* **自动检测**  — 保留PDF文件的色彩空间。

* **强制设置为RGB**  — 转换为RGB颜色空间。

* **强制作为CMYK**  — 转换为CMYK色彩空间。

* **强制作为灰度**  — 转换为灰度色彩空间。

### 颜色配置文件选项

* **转换为sRGB**  — 转换为sRGB（标准红绿蓝）。在网页上显示图像时，推荐使用 sRGB 颜色空间。

* **保留原始色彩空间**  — 保留原始色彩空间。

* **自定义从>自定义到**  — 打开菜单，以便您可以选择“从中转换”和“转换为色彩空间”。您可以选择标准的Photoshop色彩空间或上传到AdobeDynamic Media Classic的色彩空间。

另请参阅[ ICC 配置文件](/help/icc-profiles.md#icc_profiles)。

## 从 PDF 文件中裁切空白区域 {#cropping-white-space-from-a-pdf-file}

1. 要在上载 PDF 文件时自动裁切其空白区域像素，请选择“裁切”菜单并选择“修剪”。
1. 指定以下选项：

   * **根据** 裁切掉 — 选择是根据颜色还是透明度进行裁剪：

   * **颜色**  — 选择“颜色”选项。然后选择“角”菜单，并选择其颜色最接近于您要裁切的空白区域颜色的 PDF 角。

   * **透明度**  — 选择“透明度”选项。

   * **容差**  — 拖动滑块以指定从0到1的容差。

   * **基于颜色进行修剪**  — 仅当像素与您在PDF角部选择的颜色完全匹配时，才指定0来裁剪像素。数字越接近 1，允许的色差越大。

   * **基于透明度进行裁切**  — 指定0，以仅在像素透明时裁剪像素；接近1的数字使透明度更高。

## 从 PDF 页边裁切 {#cropping-from-the-sides-of-pdf-pages}

当上载 PDF 文件时，可以手动从 PDF 文件中删除页边的打印机标记。

1. 在“裁剪”菜单中，单击&#x200B;**[!UICONTROL 手动]**。
1. 在“上”、“下”、“左”、“右”文本框中输入像素设置，以便从页面的上、下及两边剪切。

页面被裁切部分的大小取决于您为 PDF 文件输入的“分辨率像素/英寸”选项。例如，如果输入150（默认值）作为“分辨率PX/英寸”设置，并从页面侧边裁剪75像素，则会裁剪半英寸；每英寸150像素，75像素等于半英寸。
