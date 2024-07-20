---
title: 使用PDF
description: 了解如何在Adobe Dynamic Media Classic中使用PDF。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 02892514-61fe-48ba-a2e3-eeb30580a1e4
topic: Integrations, Development
level: Experienced
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '726'
ht-degree: 25%

---

# 使用PDF{#working-with-pdfs}

PDF（可移植文档格式）文件在Adobe Dynamic Media Classic中用于创建eCatalog的频率最高。 默认情况下，上传PDF文件时，Adobe Dynamic Media Classic会栅格化或rip页面，以便使用这些页面构建富媒体。

在上传用于页面提取的PDF时，Adobe会强制实施以下限制：

| 限制类型 | 施加的限制 | 2022年12月31日更改为限制 |
| --- | --- | --- |
| 考虑进行提取的PDF的最大页数 | 5000（用于新上传） | 100(适用于所有PDF) |

另请参阅[Dynamic Media限制](/help/using/limitations.md)。

## PDF 上载选项 {#pdf-upload-options}

当上载 PDF 文件时，您能够以多种方法设置其格式。可以裁切其页面、提取搜索词、输入像素/英寸分辨率以及选择颜色空间。PDF文件通常包含修剪边距、裁切标记、注册标记和其他打印机标记。 当上载 PDF 文件时，可以从页边裁切这些标记。

上传PDF文件的选项位于“上传”页面的“PDF选项”下。

### 处理选项

**[!UICONTROL 栅格化]**： （默认）断开PDF文件中的页面，并将矢量图形转换为位图图像。 要创建eCatalog，请选择此选项。

**[!UICONTROL 提取搜索词]**：从PDF文件中提取搜索词，以便在eCatalog查看器中搜索文件中的关键字。

**[!UICONTROL 提取链接]**：从PDF文件中提取链接，并将其转换为在eCatalog查看器中使用的图像映射。

**[!UICONTROL 使用多页PDF自动生成eCatalog]**：自动从PDF文件创建eCatalog。 eCatalog 以您上载的 PDF 文件命名。（只有当上载 PDF 文件时栅格化该文件，才可以使用此选项。）

### 分辨率

确定分辨率设置。该设置确定在 PDF 文件中每英寸显示多少像素。默认值为 150。

### 色彩空间选项

选择“颜色空间”菜单，并为 PDF 文件选择颜色空间。大多数 PDF 文件既包含 RGB 又包含 CMYK 彩色图像。对于联机查看，首选 RGB 颜色空间。

* **[!UICONTROL 自动检测]**：保留PDF文件的色彩空间。

* **[!UICONTROL 强制作为RGB]**：转换为RGB色彩空间。

* **[!UICONTROL 强制为CMYK]**：转换为CMYK颜色空间。

* **[!UICONTROL 强制为灰度]**：转换为灰度颜色空间。

### 颜色配置文件选项

* **[!UICONTROL 转换为sRGB]**：转换为sRGB（标准红绿蓝）。 sRGB是在网页上显示图像的推荐颜色空间。

* **[!UICONTROL 保留原始颜色空间]**：保留原始颜色空间。

* **[!UICONTROL 自定义从]** > **[!UICONTROL 到]**：打开菜单，以便选择“转换自”和“转换为颜色空间”。 您可以选择标准的Photoshop色彩空间，也可以选择上传到Adobe Dynamic Media Classic的色彩空间。

另请参阅[ ICC 配置文件](/help/using/icc-profiles.md#icc_profiles)。

## 裁剪PDF文件中的空格 {#cropping-white-space-from-a-pdf-file}

上传内容文件时，您可以自动裁剪PDF文件中的空白像素。

1. 选择“裁切”菜单，然后选择“裁剪”。
1. 指定以下选项：

   * **[!UICONTROL 裁切依据]**：选择根据颜色还是透明度裁切：

      * **[!UICONTROL 颜色]**：选择“颜色”选项。 然后选择&#x200B;**[!UICONTROL 角]**&#x200B;菜单并选择该PDF的角，该角最能代表您要裁切的空白颜色。

      * **[!UICONTROL 透明度]**：选择透明度选项。

   * **[!UICONTROL 容差]**：拖动滑块以指定从0到1的容差。

   * **[!UICONTROL 基于颜色的修剪]**：指定0表示仅在像素与在PDF角选择的颜色完全匹配时才裁剪像素。 数字越接近 1，允许的色差越大。

   * **[!UICONTROL 基于透明度的修剪]**：指定0以仅裁切透明像素；数字越接近1则透明度越高。

## 从PDF页侧面裁切 {#cropping-from-the-sides-of-pdf-pages}

上传打印文件时，可以手动从PDF文件的页面两侧删除打印机标记。

1. 从“裁切”菜单中，选择&#x200B;**[!UICONTROL 手动]**。
1. 在“上”、“下”、“左”、“右”文本框中输入像素设置，以便从页面的上、下及两边剪切。

页面被裁切部分的大小取决于您为 PDF 文件输入的“分辨率像素/英寸”选项。例如，假设您输入150（缺省值）作为“分辨率PX/英寸”设置。 然后裁切页面两侧75像素。 在这种情况下，0.5英寸 被裁剪了。 以每英寸150像素计算，75像素等于半英寸。
