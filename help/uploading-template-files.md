---
title: 上载模板文件
seo-title: 上载模板文件
description: 'null'
seo-description: 了解如何上传模板文件。
uuid: e19979b5-3f41-49c5-99aa-107eDE3be98c
contentOwner: admin
content-type: 引用
products: SG_ EXPERIENCE MANAGER/Dynamic-Media-Scene-7
geptopics: SG_ SCENESELEFERENDER_ PK/categories/template_ basics
discoiquuid: 75658717-5c39-473e-9d32-718d00706310
translation-type: tm+mt
source-git-commit: a1722c15d3c049f05959d895e85297d47d730872

---


# 上载模板文件{#uploading-template-files}

将模板所需的文件上载到 Scene7 Publishing System，然后开始构建模板。可以从 Adobe® Photoshop® PSD 或图像文件构建模板。建议使用 TIFF 和 PNG 图像，因为它们允许设置透明度。

>[!NOTE]
>
>Dynamic Media Classic建议您按照模板中的透明TIFF或PSD图像，以精确的大小在您的网站上显示它们。发布模板时，调用的图像所带的图像预设大小亦相同。请注意，此大小可确保模板的大小不会调整（重新取样）为大于或小于设计尺寸。

可以使用 Adobe Photoshop PSD 文件或图像文件创建模板。

有关上载文件的详细说明，请参阅[上载文件](uploading-files.md#uploading_files)。上载模板文件时请注意以下事项：

* 如果上载的是 PSD 文件，则可以从该文件创建模板。动态媒体经典为PSD中的每个图层创建一个单独的图像。在“上载作业选项”对话框中，选择“Photoshop 选项”，选择“保持图层”选项，然后选择“创建模板”选项。然后在“图层命名”菜单上选择一个选项，用于命名Dynamic Media经典从PSD中的图层创建的图像。请参阅[PSD 上载选项](psd-files.md#psd_upload_options)。
* 如果上载的是图像，则可以从其剪贴路径创建蒙版。该选项适用于使用创建了剪切路径的图像编辑应用程序所创建的图像。在“上载作业选项”对话框中，选择“图像编辑选项”，然后选择“从剪切路径创建蒙版”选项。请参阅[上载时的图像编辑选项](image-editing-options-upload.md#image-editing-options-at-upload)。

>[!MORELIKETHIS]
>
>* [上载文件](uploading-files.md#uploading_your_files)
>* [Working with PSD files](psd-files.md#working_with_psd_files)

