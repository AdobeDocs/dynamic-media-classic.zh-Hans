---
title: 上传PDF文件
description: 了解如何在Adobe Dynamic Media Classic中上传与eCatalog关联的PDF文件。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: a787d6b5-48c8-4cf7-b136-60ba3d3eb2f2
topic: Integrations, Development
level: Experienced
source-git-commit: 29752cf9eca0fc9bb760c721e1c3dc8e4ef912c3
workflow-type: tm+mt
source-wordcount: '847'
ht-degree: 30%

---

# 上传PDF文件{#uploading-the-pdf-files}

通常，Adobe PDF文件是eCatalog的源。 这些文件包含所有图像信息、字体和矢量图形。 也可以利用图像来构建 eCatalog。准备好要上载的PDF文件后，在全局导航栏上，选择 **[!UICONTROL 上传]** 开始上传PDF。

在上传用于页面提取的PDF时，Adobe会强制实施以下限制：

| PDF限制类型 | 施加的限制 | 2022年12月31日更改为限制 |
| --- | --- | --- |
| 考虑进行提取的PDF的最大页数 | 5000（用于新上传） | 100(适用于所有PDF) |

另请参阅 [Dynamic Media限制](/help/using/limitations.md).

## 准备PDF文件

在将PDF文件上传到Adobe Dynamic Media Classic之前对其进行准备：

* 为了更轻松地上传文件，请将所有文件放在计算机或网络上的同一文件夹中。
* 按照页面的字母数字顺序命名文件。如果对页面进行排序，则在文件上载之后，更容易按正确顺序放置页面。
* 要查看PDF页是否包含裁切标记、注册目标或颜色条，请检查页面。 这些标记决定了印刷文档时的切纸位置，将 eCatalog 放到网络中之前，必须删除这些标记。Adobe Dynamic Media Classic提供了用于在上传PDF文件时裁切标记的选项。
* 如果您希望查看者按关键字搜索eCatalog，请了解PDF文件是否为“拼合”。 从平面化的 PDF 文件中无法提取搜索词。要确定PDF是否被拼合，请尝试选择内容中的文本。 如果无法选择文本，则PDF将被拼合，并且查看器无法按eCatalog中的关键字进行搜索。
* 由于 PDF 文件要用于印刷，因此通常包含 CMYK 图像。默认情况下，Adobe Dynamic Media Classic可以智能地检测这些CMYK图像，并使用内部CMYK颜色配置文件转换它们。 但如果需要，也可以使用自定颜色配置文件来转换 CMYK 图像。

  请参阅 [ICC（国际颜色联盟）配置文件](icc-profiles.md#icc_profiles).

## 最佳实践 PDF 上载选项 {#best-practice-pdf-upload-options}

有关不同上载方法的详细信息，请参阅[上载文件](uploading-files.md#uploading_your_files)。

选择要上载的文件，然后选择这些文件 *最佳实践* PDF选项：

* **裁切选项**：在上载作业选项对话框中，选择 **[!UICONTROL 裁切选项]**. 如果PDF页包含裁切标记、注册标记或其他标记，则在 **[!UICONTROL 裁切]** 下拉列表，选择 **[!UICONTROL 手动]**. 输入要从页面的顶部、右侧、底部以及左侧裁切的像素数。 裁切标记通常设置为半英寸边距。 假设您选择 **[!UICONTROL 150]** （推荐）作为像素/英寸分辨率。 然后在“顶部”、“右侧”、“底部”和“左侧”文本框中输入75、75、75、75。 在这种情况下，它会从边距裁切半英寸（150 ppi，1的一半等于75像素）。

* **正在处理**：在上载作业选项对话框中，选择 **[!UICONTROL PDF选项]**. 在 **[!UICONTROL 正在处理]** 下拉列表，选择 **[!UICONTROL 栅格化]**. PDF 文件必须经过栅格化才能在 eCatalog 中显示所有页面和图像。

* **提取搜索词（可选）**：在上载作业选项对话框中，选择 **[!UICONTROL PDF选项]**. 在提取下拉列表中，选择 **[!UICONTROL 搜索词]** 如果您希望查看者能够在eCatalog中按关键字进行搜索。

* **从多页PDF自动生成eCatalog（可选）**：在上载作业选项对话框中，选择 **[!UICONTROL PDF选项]**. 单击 **[!UICONTROL 从多页PDF自动生成eCatalog]** 以便在上传时自动创建eCatalog。 可以直接进入 eCatalog 屏幕，并开始使用 eCatalog，无需先选择 PDF 文件及选择“构建”命令。eCatalog 用 PDF 文件的名称命名。

* **分辨率**：在上载作业选项对话框中，选择 **[!UICONTROL PDF选项]**. 在 **[!UICONTROL 分辨率]** 文本字段，输入值。 Adobe Dynamic Media Classic建议每英寸150像素。

* **颜色空间**：在上载作业选项对话框中，选择 **[!UICONTROL PDF选项]**. 在“颜色空间”下拉列表中，选择 **[!UICONTROL 自动检测]**. 通常，为印刷输出创建的 PDF 采用 CMYK；而用于在线查看的 PDF 则采用 RGB。如果 PDF 使用两个颜色空间，可以选择“强制渲染为 RGB”或“强制渲染为 CMYK”来选择特定颜色空间。例如，当页面图形使用 CMYK 颜色空间，但图片使用 RGB 时，PDF 使用这两个颜色空间。如果上载了 ICC 配置文件，则其名称显示在“颜色空间”菜单上，您可以在其中选择该名称。

  请参阅 [ICC（国际颜色联盟）配置文件](/help/using/icc-profiles.md).

* **颜色配置文件选项**：在上载作业选项对话框中，选择 **[!UICONTROL 颜色配置文件选项]**，然后选择颜色配置文件选项：

   * **保留原始颜色空间**：保留原始颜色空间。

   * **自定义从>到**：打开子菜单，以便您选择 **[!UICONTROL 转换自]** 和 **[!UICONTROL 转换为]** 颜色空间。 您可以选择标准的Photoshop色彩空间，也可以选择上传到Adobe Dynamic Media Classic的色彩空间。

<!-- * **Convert To SRGB**: Converts to SRGB (Standard Red Green Blue). SRGB is the recommended color space for displaying images on Web pages. -->

请参阅 [ICC（国际颜色联盟）配置文件](icc-profiles.md#icc_profiles).

>[!NOTE]
>
>有关所有 PDF 选项的详细信息，请参阅[PDF 上载选项](pdfs.md#pdf_upload_options)。
