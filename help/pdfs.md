---
title: 使用PDF
description: 了解如何在Adobe Dynamic Media Classic中使用PDF。
uuid: 26d70d28-9393-49b1-9051-d70456deca67
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 5a073de3-6b1d-4c3e-8c03-9182f9f3874a
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 02892514-61fe-48ba-a2e3-eeb30580a1e4
source-git-commit: d5293a2983e1105c65005634e7eb4147e17e8328
workflow-type: tm+mt
source-wordcount: '699'
ht-degree: 36%

---

# 使用PDF{#working-with-pdfs}

PDF（可移植文档格式）文件在Adobe Dynamic Media Classic中最常用于创建eCatalog。 在上传PDF文件、Adobe Dynamic Media Classic栅格化或翻页时，默认情况下会显示页面，以便页面可用于构建富媒体。

在上传PDF以进行页面提取时，Adobe强制实施以下限制：

| PDF限制类型 | 已实施的限制 | 对2022年12月31日上限的更改 |
| --- | --- | --- |
| 要考虑提取的PDF的最大页面数 | 5000（用于新上传） | 100 |

## PDF 上载选项 {#pdf-upload-options}

当上载 PDF 文件时，您能够以多种方法设置其格式。可以裁切其页面、提取搜索词、输入像素/英寸分辨率以及选择颜色空间。PDF 文件中常常包含修剪边距、裁切标记、对齐标记以及其他打印机的标记。当上载 PDF 文件时，可以从页边裁切这些标记。

上传PDF文件的选项位于“上传”页面上的PDF选项下方。

### 处理选项

**[!UICONTROL 光栅化]**  — （默认）拆除PDF文件中的页面，并将矢量图形转换为位图图像。 要创建eCatalog，请选择此选项。

**[!UICONTROL 提取搜索词]**  — 从PDF文件中提取词语，以便在eCatalog查看器中按关键字搜索文件。

**[!UICONTROL 提取链接]**  — 从PDF文件中提取链接，并将其转换为在eCatalog查看器中使用的图像映射。

**[!UICONTROL 具有多页面PDF的自动生成电子目录]**  — 自动从PDF文件创建eCatalog。 eCatalog 以您上载的 PDF 文件命名。（只有当上载 PDF 文件时栅格化该文件，才可以使用此选项。）

### 分辨率

确定分辨率设置。该设置确定在 PDF 文件中每英寸显示多少像素。默认值为 150。

### 颜色空间选项

选择“颜色空间”菜单，并为 PDF 文件选择颜色空间。大多数 PDF 文件既包含 RGB 又包含 CMYK 彩色图像。对于联机查看，首选 RGB 颜色空间。

* **[!UICONTROL 自动检测]**  — 保留PDF文件的色彩空间。

* **[!UICONTROL 强制作为RGB]**  — 转换为RGB色彩空间。

* **[!UICONTROL 强制为CMYK]**  — 转换为CMYK色彩空间。

* **[!UICONTROL 强制作为灰度]**  — 转换为灰度色彩空间。

### 颜色配置文件选项

* **[!UICONTROL 转换为sRGB]**  — 转换为sRGB（标准红绿蓝）。 在网页上显示图像时，推荐使用 sRGB 颜色空间。

* **[!UICONTROL 保留原始色彩空间]**  — 保留原始色彩空间。

* **[!UICONTROL 自定义自]** > **[!UICONTROL 至]**  — 打开菜单，以便您选择“从中转换”和“转换到”色彩空间。 您可以选择标准的Photoshop色彩空间或上传到Adobe Dynamic Media Classic的色彩空间。

另请参阅[ ICC 配置文件](/help/icc-profiles.md#icc_profiles)。

## 从PDF文件裁剪空格 {#cropping-white-space-from-a-pdf-file}

1. 要在上载 PDF 文件时自动裁切其空白区域像素，请选择“裁切”菜单并选择“修剪”。
1. 指定以下选项：

   * **[!UICONTROL 根据]**  — 选择是根据颜色还是透明度进行裁剪：

      * **[!UICONTROL 颜色]**  — 选择颜色选项。 然后，选择 **[!UICONTROL 角]** 菜单中，选择PDF的角，其颜色最能代表要裁剪的空格颜色。

      * **[!UICONTROL 透明度]**  — 选择“透明度”选项。
   * **[!UICONTROL 容差]**  — 拖动滑块以指定从0到1的公差。

   * **[!UICONTROL 基于颜色的修剪]**  — 仅当像素与您在PDF角选择的颜色完全匹配时，才指定0来裁剪像素。 数字越接近 1，允许的色差越大。

   * **[!UICONTROL 基于透明度的修剪]**  — 指定0，以仅在像素透明时裁剪像素；接近1的数字使透明度更高。


## 从PDF页面的侧边裁剪 {#cropping-from-the-sides-of-pdf-pages}

当上载 PDF 文件时，可以手动从 PDF 文件中删除页边的打印机标记。

1. 从“裁剪”菜单中，选择 **[!UICONTROL 手动]**.
1. 在“上”、“下”、“左”、“右”文本框中输入像素设置，以便从页面的上、下及两边剪切。

页面被裁切部分的大小取决于您为 PDF 文件输入的“分辨率像素/英寸”选项。例如，如果输入150（默认值）作为“分辨率PX/英寸”设置，并从页面侧边裁剪75像素，则会裁剪半英寸；每英寸150像素，75像素等于半英寸。
