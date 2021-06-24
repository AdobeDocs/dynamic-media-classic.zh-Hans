---
title: 上载模板文件
description: 了解如何上传模板文件。
uuid: e19979b5-3f41-49c5-99aa-107ede3be98c
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: 75658717-5c39-473e-9d32-718d00706310
feature: Dynamic Media Classic
role: Business Practitioner
exl-id: a105c18a-7e06-43cb-938c-a3bcdc3e9d22
source-git-commit: 06bd65c92c88595786b14213944a7cebd0d2590b
workflow-type: tm+mt
source-wordcount: '236'
ht-degree: 48%

---

# 上载模板文件{#uploading-template-files}

在开始构建模板之前，需要将模板的文件上传到Dynamic Media Classic。 可以从 Adobe® Photoshop® PSD 或图像文件构建模板。建议使用 TIFF 和 PNG 图像，因为它们允许设置透明度。

>[!NOTE]
>
>Dynamic Media Classic建议在模板中使用透明TIFF或PSD图像，其大小与您希望在网站上显示的大小完全相同。 发布模板时，调用的图像所带的图像预设大小亦相同。请注意，此大小可确保模板的大小不会调整（重新取样）为大于或小于设计尺寸。

可以使用 Adobe Photoshop PSD 文件或图像文件创建模板。

有关上载文件的详细说明，请参阅[上载文件](uploading-files.md#uploading_files)。上载模板文件时请注意以下事项：

* 如果要上传PSD文件，则可以从中创建模板。 Dynamic Media Classic会为PSD中的每个图层创建一个单独的图像。 在“上传作业选项”对话框中，单击&#x200B;**[!UICONTROL Photoshop选项]**，然后选择&#x200B;**[!UICONTROL 维护层]**&#x200B;和&#x200B;**[!UICONTROL 创建模板]**。 然后，从&#x200B;**[!UICONTROL 图层命名]**下拉列表中选择一个选项，以命名Dynamic Media Classic从PSD中的图层创建的图像。
请参阅[PSD 上载选项](psd-files.md#psd_upload_options)。

<!-- THERE IS NO LONGER AN IMAGE EDITING OPTIONS MENU * If you are uploading images, you can create a mask from its clipping path. This option applies to images created with image-editing applications in which a clipping path was created. In the Upload Job Options dialog box, select Image Editing Options and select the Create Mask From Clipping Path option. 
See [Image editing options at upload](image-editing-options-upload.md#image-editing-options-at-upload). -->

>[!MORELIKETHIS]
>
>* [上载文件](uploading-files.md#uploading_your_files)
* [使用 PSD 文件](psd-files.md#working_with_psd_files)

