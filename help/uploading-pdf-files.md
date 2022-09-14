---
title: 上传PDF文件
description: 了解如何在Adobe Dynamic Media Classic中上传与eCatalog关联的PDF文件。
uuid: 9e178bb2-ac09-427a-b61a-aad4e87a5837
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 0097cba5-c886-4115-bc35-7ae7a500202f
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: a787d6b5-48c8-4cf7-b136-60ba3d3eb2f2
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '831'
ht-degree: 36%

---

# 上传PDF文件{#uploading-the-pdf-files}

通常，Adobe PDF文件是eCatalog的源。 这些文件包含所有图像信息、字体和矢量图形。 也可以利用图像来构建 eCatalog。准备好上传PDF文件后，在全局导航栏上，选择 **[!UICONTROL 上传]** 开始上传PDF。

在上传PDF以进行页面提取时，Adobe强制实施以下限制：

| PDF限制类型 | 规定的限制 | 2022年12月31日的上限变更 |
| --- | --- | --- |
| 要考虑提取的PDF的最大页面数 | 5000（用于新上传） | 100(适用于所有PDF) |

另请参阅 [Dynamic Media限制](/help/limitations.md).

## 准备PDF文件 {#preparing-your-pdf-files}

在将PDF文件上传到Adobe Dynamic Media Classic之前，请准备文件：

* 为了更便于上传文件，请将所有文件放置在您计算机或网络上的同一文件夹中。
* 按照页面的字母数字顺序命名文件。如果对页面进行排序，则在文件上载之后，更容易按正确顺序放置页面。
* 要查看PDF页面是包含裁剪标记、注册目标还是颜色条，请检查页面。 这些标记决定了印刷文档时的切纸位置，将 eCatalog 放到网络中之前，必须删除这些标记。Adobe Dynamic Media Classic在您上传PDF文件时提供了用于裁剪标记的选项。
* 如果希望观众按关键字搜索 eCatalog，应确认您的 PDF 文件是否已“平面化”。从平面化的 PDF 文件中无法提取搜索词。要确认 PDF 是否平面化，尝试选择其中的文本。如果无法选择文本，则对PDF进行扁平化处理，并且查看器无法在eCatalog中按关键字进行搜索。
* 由于 PDF 文件要用于印刷，因此通常包含 CMYK 图像。默认情况下，Adobe Dynamic Media Classic可以智能地检测这些CMYK图像，并使用内部CMYK颜色配置文件进行转换。 但如果需要，也可以使用自定颜色配置文件来转换 CMYK 图像。

   请参阅 [ICC（国际颜色联盟）配置文件](icc-profiles.md#icc_profiles).

## 最佳实践 PDF 上载选项 {#best-practice-pdf-upload-options}

有关不同上载方法的详细信息，请参阅[上载文件](uploading-files.md#uploading_your_files)。

选择要上传的文件，然后选择这些文件 *最佳实践* PDF选项：

* **裁剪选项**  — 在上传作业选项对话框中，选择 **[!UICONTROL 裁剪选项]**. 如果PDF页面在 **[!UICONTROL 裁切]** 下拉列表中，选择 **[!UICONTROL 手动]**. 输入要从页面的上侧、右侧、下侧及左侧裁切的像素数。裁切标记通常设置为半英寸边距。 假设您选择 **[!UICONTROL 150]** （推荐）作为每英寸像素分辨率，并在“顶部”、“右”、“底部”和“左”文本框中输入75、75、75、75。 在这种情况下，它会从边距裁剪半英寸（150 ppi，1的半数等于75像素）。

* **处理**  — 在上传作业选项对话框中，选择 **[!UICONTROL PDF选项]**. 在 **[!UICONTROL 处理]** 下拉列表中，选择 **[!UICONTROL 光栅化]**. PDF 文件必须经过栅格化才能在 eCatalog 中显示所有页面和图像。

* **提取搜索词（可选）**  — 在上传作业选项对话框中，选择 **[!UICONTROL PDF选项]**. 在提取下拉列表中，选择 **[!UICONTROL 搜索词]** 如果您希望查看者能够在eCatalog中按关键词搜索。

* **从多个页面PDF自动生成eCatalog（可选）**  — 在上传作业选项对话框中，选择 **[!UICONTROL PDF选项]**. 选择 **[!UICONTROL 从多个页面自动生成eCatalogPDF]** 以在您上传时自动创建eCatalog。 可以直接进入 eCatalog 屏幕，并开始使用 eCatalog，无需先选择 PDF 文件及选择“构建”命令。eCatalog 用 PDF 文件的名称命名。

* **分辨率**  — 在上传作业选项对话框中，选择 **[!UICONTROL PDF选项]**. 在 **[!UICONTROL 分辨率]** 文本字段中输入一个值。 Adobe Dynamic Media Classic建议每英寸150像素。

* **Colorspace**  — 在上传作业选项对话框中，选择 **[!UICONTROL PDF选项]**. 在Colorspace下拉列表中，选择 **[!UICONTROL 自动检测]**. 通常，为印刷输出创建的 PDF 采用 CMYK；而用于在线查看的 PDF 则采用 RGB。如果 PDF 使用两个颜色空间，可以选择“强制渲染为 RGB”或“强制渲染为 CMYK”来选择特定颜色空间。例如，当页面图形使用 CMYK 颜色空间，但图片使用 RGB 时，PDF 使用这两个颜色空间。如果上载了 ICC 配置文件，则其名称显示在“颜色空间”菜单上，您可以在其中选择该名称。

   请参阅 [ICC（国际颜色联盟）配置文件](/help/icc-profiles.md).

* **颜色配置文件选项**  — 在上传作业选项对话框中，选择 **[!UICONTROL 颜色配置文件选项]**，然后选择“颜色配置文件”选项：

   * **保留原始色彩空间**  — 保留原始色彩空间。

   * **自定义从>到**  — 打开子菜单，以便您选择 **[!UICONTROL 转换自]** 和 **[!UICONTROL 转换为]** 色彩空间。 您可以选择标准的Photoshop色彩空间或上传到Adobe Dynamic Media Classic的色彩空间。

<!-- * **Convert To SRGB** - Converts to SRGB (Standard Red Green Blue). SRGB is the recommended color space for displaying images on web pages. -->

请参阅 [ICC（国际颜色联盟）配置文件](icc-profiles.md#icc_profiles).

>[!NOTE]
>
>有关所有 PDF 选项的详细信息，请参阅[PDF 上载选项](pdfs.md#pdf_upload_options)。
