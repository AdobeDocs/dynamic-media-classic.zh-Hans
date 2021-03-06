---
title: 上传主控图像
description: 了解如何将主控图像上传到AdobeDynamic Media Classic。
uuid: 50bcf2e2-852b-48f1-a7c7-5063a87ce9c1
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
discoiquuid: 8c94bafc-94cc-496f-a394-a945cd7b02cf
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 410ba80c-7f01-4cd0-9ab3-db9658757ba7
source-git-commit: 8bc49ae3704f0551c70d68a0ddd63725bdcc645c
workflow-type: tm+mt
source-wordcount: '259'
ht-degree: 2%

---

# 上传主控图像{#uploading-master-images}

在将图像上传到AdobeDynamic Media Classic之前，请确保这些图像具有最高质量的大小和格式。 AdobeDynamic Media Classic建议上传具有足够像素计数的高质量图像（从1500到2000像素的长像素）。 此大小调整允许进行任何所需的Dynamic Imaging。

有关上传图像的详细信息，请参阅[上传文件](uploading-files.md#uploading_files)。

**准备主控图像以上传：**

在将主控图像文件上传到AdobeDynamic Media Classic之前，请准备这些文件：

* **图像大小**  — 创建您预期使用的最大大小图像。典型图像大小介于1500到2500像素之间，最长为1500像素。 如果您打算使用缩放功能，请AdobeDynamic Media Classic，建议使用最大大小至少为2000像素的图像，以优化缩放详细信息。 AdobeDynamic Media Classic可以每幅渲染多达2500万像素的图像。 例如，您可以使用5000 x 5000 MP的图像，或任何其他大小组合，最多25 MP。

* **文件格式**  -AdobeDynamic Media Classic支持所有标准图像文件格式，包括TIFF、BMP、JPEG、PSD、GIF和EPS。建议使用无损图像格式（TIFF 和 PNG）。如果您使用的是JPEG图像，请使用最高质量设置。

* **色彩空间** - RGB是Web图像演示的色彩空间；在上传时，通常用于打印的CMYK图像会自动转换为RGB。建议上载具有嵌入ICC（国际颜色联盟）颜色配置文件的CMYK图像，以便转换为RGB。 另请参阅[ICC（国际颜色联盟）配置文件](/help/icc-profiles.md)。
