---
title: 使用PDF
description: 了解如何在Adobe Dynamic Media Classic中使用PDF。
uuid: 26d70d28-9393-49b1-9051-d70456deca67
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 5a073de3-6b1d-4c3e-8c03-9182f9f3874a
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 02892514-61fe-48ba-a2e3-eeb30580a1e4
source-git-commit: 38d7f8d6e5888e1c5ba9260ada45b79fb16b338f
workflow-type: tm+mt
source-wordcount: '710'
ht-degree: 36%

---

# 使用PDF{#working-with-pdfs}

PDF（可移植文档格式）文件在Adobe Dynamic Media Classic中用于创建eCatalog的频率最高。 在上传PDF文件时，默认情况下，Adobe Dynamic Media Classic会栅格化或rip页面，以便使用这些页面构建富媒体。

在上传用于页面提取的PDF时，Adobe会强制实施以下限制：

| 限制类型 | 施加的限制 | 2022年12月31日更改为限额 |
| --- | --- | --- |
| 考虑进行提取的PDF的最大页数 | 5000（用于新上传） | 100(适用于所有PDF) |

另请参阅 [Dynamic Media限制](/help/using/limitations.md).

## PDF 上载选项 {#pdf-upload-options}

当上载 PDF 文件时，您能够以多种方法设置其格式。可以裁切其页面、提取搜索词、输入像素/英寸分辨率以及选择颜色空间。PDF 文件中常常包含修剪边距、裁切标记、对齐标记以及其他打印机的标记。当上载 PDF 文件时，可以从页边裁切这些标记。

上传PDF文件的选项位于“上传”页面的“PDF选项”下。

### 处理选项

**[!UICONTROL 栅格化]**  — （默认）翻录PDF文件中的页面，并将矢量图形转换为位图图像。 要创建eCatalog，请选择此选项。

**[!UICONTROL 提取搜索词]**  — 从PDF文件中提取单词，以便在eCatalog查看器中按关键字搜索该文件。

**[!UICONTROL 提取链接]**  — 从PDF文件中提取链接，并将其转换为eCatalog查看器中使用的图像映射。

**[!UICONTROL 使用多页PDF自动生成eCatalog]**  — 自动从PDF文件创建eCatalog。 eCatalog 以您上载的 PDF 文件命名。（只有当上载 PDF 文件时栅格化该文件，才可以使用此选项。）

### 分辨率

确定分辨率设置。该设置确定在 PDF 文件中每英寸显示多少像素。默认值为 150。

### 颜色空间选项

选择“颜色空间”菜单，并为 PDF 文件选择颜色空间。大多数 PDF 文件既包含 RGB 又包含 CMYK 彩色图像。对于联机查看，首选 RGB 颜色空间。

* **[!UICONTROL 自动检测]**  — 保留PDF文件的色彩空间。

* **[!UICONTROL 强制作为RGB]**  — 转换为RGB色彩空间。

* **[!UICONTROL 强制为CMYK]**  — 转换为CMYK颜色空间。

* **[!UICONTROL 强制为灰度]**  — 转换为灰度颜色空间。

### 颜色配置文件选项

* **[!UICONTROL 转换为sRGB]**  — 转换为sRGB（标准红绿蓝）。 在网页上显示图像时，推荐使用 sRGB 颜色空间。

* **[!UICONTROL 保留原始颜色空间]**  — 保留原始颜色空间。

* **[!UICONTROL 自定义自]** > **[!UICONTROL 至]**  — 打开菜单，以便选择“转换自”和“转换至”色彩空间。 您可以选择标准的Photoshop色彩空间，也可以选择上传到Adobe Dynamic Media Classic的色彩空间。

另请参阅[ ICC 配置文件](/help/using/icc-profiles.md#icc_profiles)。

## 裁切PDF文件中的空格 {#cropping-white-space-from-a-pdf-file}

1. 要在上载 PDF 文件时自动裁切其空白区域像素，请选择“裁切”菜单并选择“修剪”。
1. 指定以下选项：

   * **[!UICONTROL 裁切依据]**  — 选择根据颜色或透明度裁切：

      * **[!UICONTROL 颜色]**  — 选择颜色选项。 然后选择 **[!UICONTROL 角]** 菜单，然后选择最能代表要裁切的空白区域PDF的颜色作为颜色的角。

      * **[!UICONTROL 透明度]**  — 选择透明度选项。
   * **[!UICONTROL 容差]**  — 拖动滑块以指定从0到1的公差。

   * **[!UICONTROL 根据颜色进行修剪]**  — 指定0表示仅在像素与在PDF角选择的颜色完全匹配时裁切像素。 数字越接近 1，允许的色差越大。

   * **[!UICONTROL 基于透明度的修剪]**  — 指定0可仅在像素为透明时裁切像素；数字越接近1则透明度越高。


## 从PDF页侧面裁切 {#cropping-from-the-sides-of-pdf-pages}

当上载 PDF 文件时，可以手动从 PDF 文件中删除页边的打印机标记。

1. 从裁切菜单中，选择 **[!UICONTROL 手动]**.
1. 在“上”、“下”、“左”、“右”文本框中输入像素设置，以便从页面的上、下及两边剪切。

页面被裁切部分的大小取决于您为 PDF 文件输入的“分辨率像素/英寸”选项。例如，假设您输入150（缺省值）作为“分辨率像素/英寸”设置。 然后裁切页面两侧75个像素。 在这种情况下，0.5英寸 已裁切。 在150像素/英寸处，75像素等于半英寸。
