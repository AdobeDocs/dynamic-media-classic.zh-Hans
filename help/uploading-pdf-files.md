---
title: 上载 PDF 文件
description: 了解如何上传与电子目录关联的PDF文件。
uuid: 9e178bb2-ac09-427a-b61a-aad4e87a5837
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 0097cba5-c886-4115-bc35-7ae7a500202f
feature: Dynamic Media Classic，查看器，电子目录
role: Business Practitioner
exl-id: a787d6b5-48c8-4cf7-b136-60ba3d3eb2f2
translation-type: tm+mt
source-git-commit: 06bd65c92c88595786b14213944a7cebd0d2590b
workflow-type: tm+mt
source-wordcount: '769'
ht-degree: 44%

---

# 上载 PDF 文件{#uploading-the-pdf-files}

通常，Adobe PDF文件是eCatalog的源。 这些文件包含所有图像信息、字体和矢量图形。 也可以利用图像来构建 eCatalog。准备好要上传的PDF文件后，在全局导航栏上，单击&#x200B;**[!UICONTROL 上传]**&#x200B;开始上传PDF。

## 准备 PDF 文件 {#preparing-your-pdf-files}

在将PDF文件上传到Dynamic Media Classic之前，请准备这些文件：

* 要使上传文件更简单，请将所有文件放在您的计算机或网络上的同一文件夹中。
* 按照页面的字母数字顺序命名文件。如果对页面进行排序，则在文件上载之后，更容易按正确顺序放置页面。
* 要查看PDF页面是否包含裁剪标记、套版色目标或颜色条，请检查页面。 这些标记决定了印刷文档时的切纸位置，将 eCatalog 放到网络中之前，必须删除这些标记。Dynamic Media Classic提供了在您上传PDF文件时裁剪标记的选项。
* 如果希望观众按关键字搜索 eCatalog，应确认您的 PDF 文件是否已“平面化”。从平面化的 PDF 文件中无法提取搜索词。要确认 PDF 是否平面化，尝试选择其中的文本。如果无法选择文本，则拼合PDF，并且查看器无法在eCatalog中按关键字搜索。
* 由于 PDF 文件要用于印刷，因此通常包含 CMYK 图像。默认情况下，Dynamic Media Classic可以智能检测这些CMYK图像，并使用内部CMYK颜色用户档案转换它们。 但如果需要，也可以使用自定颜色配置文件来转换 CMYK 图像。

   请参阅[ICC 配置文件](icc-profiles.md#icc_profiles)。

## 最佳实践 PDF 上载选项 {#best-practice-pdf-upload-options}

有关不同上载方法的详细信息，请参阅[上载文件](uploading-files.md#uploading_your_files)。

选择要上载的文件，然后选择以下&#x200B;*最佳实践* PDF 选项：

* **裁剪选项**  — 在“上传作业选项”对话框中，单击“ **[!UICONTROL 裁剪选项]**”。如果PDF页面包含裁剪标记、套版色标记或其他标记，请在&#x200B;**[!UICONTROL “裁剪]**”下拉列表中选择&#x200B;**[!UICONTROL “手动]**”。 输入要从页面的上侧、右侧、下侧及左侧裁切的像素数。裁剪标记通常设置为半英寸边距。 假设您选择&#x200B;**[!UICONTROL 150]**（推荐）作为每英寸像素分辨率，并在“顶部”、“右”、“底部”和“左”文本框中输入75、75、75、75。 在这种情况下，它会裁切半英寸（以150 ppi，1的半数等于75像素）。

* **处理**  — 在“上载作业选项”对话框中，单击“ **[!UICONTROL PDF选项”]**。在&#x200B;**[!UICONTROL 处理]**&#x200B;下拉列表中，选择&#x200B;**[!UICONTROL 栅格化]**。 PDF 文件必须经过栅格化才能在 eCatalog 中显示所有页面和图像。

* **提取搜索词（可选）**  — 在“上载作业选项”对话框中，单击“ **[!UICONTROL PDF选项”]**。在“提取”下拉列表中，如果希望查看者能够在eCatalog中按关键字搜索，请选择&#x200B;**[!UICONTROL 搜索词]**。

* **从多页PDF（可选）自动生成电子目录**  — 在“上载作业选项”对话框中，单击“ **[!UICONTROL PDF选项”]**。选择&#x200B;**[!UICONTROL 从多页PDF]**&#x200B;自动生成eCatalog，以在您上传时自动创建eCatalog。 可以直接进入 eCatalog 屏幕，并开始使用 eCatalog，无需先选择 PDF 文件及选择“构建”命令。eCatalog 用 PDF 文件的名称命名。

* **分辨率**  — 在“上载作业选项”对话框中，单击“ **[!UICONTROL PDF选项”]**。在&#x200B;**[!UICONTROL Resolution]**&#x200B;文本字段中，输入一个值。 Dynamic Media Classic建议每英寸150像素。

* **Colorspace**  — 在“上载作业选项”对话框中，单击“ **[!UICONTROL PDF选项]**”。在“色彩空间”下拉列表中，选择&#x200B;**[!UICONTROL 自动检测]**。 通常，为印刷输出创建的 PDF 采用 CMYK；而用于在线查看的 PDF 则采用 RGB。如果 PDF 使用两个颜色空间，可以选择“强制渲染为 RGB”或“强制渲染为 CMYK”来选择特定颜色空间。例如，当页面图形使用 CMYK 颜色空间，但图片使用 RGB 时，PDF 使用这两个颜色空间。如果上载了 ICC 配置文件，则其名称显示在“颜色空间”菜单上，您可以在其中选择该名称。

   请参阅[ICC 配置文件](/help/icc-profiles.md)。

* **颜色用户档案选项**  — 在“上传作业选项”对话框中，单击“ **[!UICONTROL 颜色用户档案选项]**”，然后选择“颜色用户档案”选项：

   * **保留原始色彩空间**  — 保留原始色彩空间。

   * **“自定”>“至** ” — 打开子菜单，以便您可以选择“转 **[!UICONTROL 换]** 格式” **[!UICONTROL “转]** 换为颜色”空间。您可以选择标准Photoshop色彩空间或上传到Dynamic Media Classic的色彩空间。

<!-- * **Convert To SRGB** - Converts to SRGB (Standard Red Green Blue). SRGB is the recommended color space for displaying images on web pages. -->

请参阅[ICC 配置文件](icc-profiles.md#icc_profiles)。

>[!NOTE]
>
>有关所有 PDF 选项的详细信息，请参阅[PDF 上载选项](pdfs.md#pdf_upload_options)。
