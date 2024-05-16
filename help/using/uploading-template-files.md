---
title: 上载模板文件
description: 了解如何在Adobe Dynamic Media Classic中上传模板文件。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
feature: Dynamic Media Classic
role: User
exl-id: a105c18a-7e06-43cb-938c-a3bcdc3e9d22
topic: Content Management
level: Experienced
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '244'
ht-degree: 32%

---

# 上载模板文件{#uploading-template-files}

在开始构建模板之前，将模板所需的文件上传到Adobe Dynamic Media Classic中。 您可以从Adobe®Photoshop®PSD或图像文件构建模板。 建议使用 TIFF 和 PNG 图像，因为它们允许设置透明度。

>[!NOTE]
>
>Adobe Dynamic Media Classic建议在模板中使用透明TIFF或PSD图像，且模板大小应与在网站上显示的图像完全相同。 发布模板时，调用的图像所带的图像预设大小亦相同。请注意，此大小可确保模板的大小不会调整（重新取样）为大于或小于设计尺寸。

可以使用 Adobe Photoshop PSD 文件或图像文件创建模板。

有关上传文件的详细说明，请参阅 [上载文件](uploading-files.md#uploading_files). 上载模板文件时请注意以下事项：

* 如果要上传PSD文件，您可以从中创建模板。 Adobe Dynamic Media Classic会为PSD中的每个图层创建单独的图像。 在“上载作业选项”对话框中，选择 **[!UICONTROL Photoshop选项]**，并选择 **[!UICONTROL 保留图层]** 和 **[!UICONTROL 创建模板]**. 然后，从 **[!UICONTROL 图层命名]** 下拉列表，用于命名Adobe Dynamic Media Classic从PSD中的图层创建的图像。
请参阅[PSD 上载选项](psd-files.md#psd_upload_options)。
<!-- THERE IS NO LONGER AN IMAGE EDITING OPTIONS MENU * If you are uploading images, you can create a mask from its clipping path. This option applies to images created with image-editing applications in which a clipping path was created. In the Upload Job Options dialog box, select Image Editing Options and select the Create Mask From Clipping Path option. 
See [Image editing options at upload](image-editing-options-upload.md#image-editing-options-at-upload). -->

>[!MORELIKETHIS]
>
>* [上传文件](uploading-files.md#uploading_your_files)
>* [使用PSD文件](psd-files.md#working_with_psd_files)
