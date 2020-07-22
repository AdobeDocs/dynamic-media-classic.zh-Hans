---
title: 上载 PDF 文件
seo-title: 上载 PDF 文件
description: 'null'
seo-description: 了解如何上传与电子目录相关的PDF文件。
uuid: 9e178bb2-ac09-427a-b61a-aad4e87a5837
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 0097cba5-c886-4115-bc35-7ae7a500202f
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '701'
ht-degree: 71%

---


# 上载 PDF 文件{#uploading-the-pdf-files}

通常，eCatalog 由 Adobe PDF 文件创建；这些文件包含所有图像信息以及字体和矢量图。也可以利用图像来构建 eCatalog。准备好要上载的 PDF 文件之后，选择全局导航栏上的“上载”按钮开始上载 PDF。

## 准备 PDF 文件 {#preparing-your-pdf-files}

在将PDF文件上传到Dynamic Media经典之前，请准备这些文件：

* 将所有文件放入您的计算机或网络上的同一文件夹中，以便于上载文件。
* 按照页面的字母数字顺序命名文件。如果对页面进行排序，则在文件上载之后，更容易按正确顺序放置页面。
* 检查 PDF 页，以查看这些页面中是否包含裁切标记、对齐目标或颜色条。这些标记决定了印刷文档时的切纸位置，将 eCatalog 放到网络中之前，必须删除这些标记。Dynamic Media经典在您上传PDF文件时提供用于裁剪标记的选项。
* 如果希望观众按关键字搜索 eCatalog，应确认您的 PDF 文件是否已“平面化”。从平面化的 PDF 文件中无法提取搜索词。要确认 PDF 是否平面化，尝试选择其中的文本。如果无法选择文本，则表明 PDF 已平面化，观众无法在 eCatalog 中按关键字进行搜索。
* 由于 PDF 文件要用于印刷，因此通常包含 CMYK 图像。默认情况下，Dynamic Media经典可以智能检测这些CMYK图像，并使用内部CMYK颜色用户档案进行转换。 但如果需要，也可以使用自定颜色配置文件来转换 CMYK 图像。

   请参阅[ICC 配置文件](icc-profiles.md#icc_profiles)。

## 最佳实践 PDF 上载选项 {#best-practice-pdf-upload-options}

有关不同上载方法的详细信息，请参阅[上载文件](uploading-files.md#uploading_your_files)。

选择要上载的文件，然后选择以下&#x200B;*最佳实践* PDF 选项：

* **裁剪**&#x200B;如果页面包含裁剪标记、套版色标记或其他标记，请选择“裁剪”菜单并选择“手动”。 输入要从页面的上侧、右侧、下侧及左侧裁切的像素数。裁切标记通常设置为半英寸边距。假定选择 150 PPI 的分辨率（推荐设置），则若分别在“上”、“右”、“下”和“左”文本框中输入 75、75、75、75，则将从边距中裁切半英寸（150 PPI 时，半英寸等于 75 像素）。

* **处理**&#x200B;选择“处理”菜单，然后选择“栅格化”。 PDF 文件必须经过栅格化才能在 eCatalog 中显示所有页面和图像。

* **提取搜索词（可选）**&#x200B;如果希望查看者能够在电子目录中按关键字进行搜索，请选择此选项。

* **自动从多页PDF生成电子目录（可选）选**&#x200B;择此选项，在上传时自动创建电子目录。 可以直接进入 eCatalog 屏幕，并开始使用 eCatalog，无需先选择 PDF 文件及选择“构建”命令。eCatalog 用 PDF 文件的名称命名。

* **分辨率** Dynamic Media经典建议每英寸150像素。

* **ColorspaceDynamic Media**&#x200B;经典建议选择“自动检测”。 通常，为印刷输出创建的 PDF 采用 CMYK；而用于在线查看的 PDF 则采用 RGB。如果 PDF 使用两个颜色空间，可以选择“强制渲染为 RGB”或“强制渲染为 CMYK”来选择特定颜色空间。例如，当页面图形使用 CMYK 颜色空间，但图片使用 RGB 时，PDF 使用这两个颜色空间。如果上载了 ICC 配置文件，则其名称显示在“颜色空间”菜单上，您可以在其中选择该名称。

   请参阅[ICC 配置文件](icc-profiles.md#icc_profiles)。

* **颜色用户档案**&#x200B;选择颜色用户档案选项：

* **转换为** SRGB（标准红绿蓝）。 在网页上显示图像时，推荐使用 SRGB 颜色空间。

* **保留原始色彩空**&#x200B;间保留原始色彩空间。

* **“自定义自”>“**&#x200B;至”打开菜单，因此您可以选择“转换自”和“转换至色彩空间”。 您可以选择标准Photoshop色彩空间或上传到Dynamic Media经典的色彩空间。

请参阅[ICC 配置文件](icc-profiles.md#icc_profiles)。

>[!NOTE]
>
>有关所有 PDF 选项的详细信息，请参阅[PDF 上载选项](pdfs.md#pdf_upload_options)。

