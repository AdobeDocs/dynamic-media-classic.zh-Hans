---
title: 上传主图像
description: 了解如何将主图像上传到Adobe Dynamic Media Classic。
uuid: 50bcf2e2-852b-48f1-a7c7-5063a87ce9c1
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
discoiquuid: 8c94bafc-94cc-496f-a394-a945cd7b02cf
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 410ba80c-7f01-4cd0-9ab3-db9658757ba7
topic: Content Management
level: Intermediate
source-git-commit: 51c05c62448b39a75facb2e90cc9da5d0f26ab45
workflow-type: tm+mt
source-wordcount: '259'
ht-degree: 2%

---

# 上传主图像{#uploading-master-images}

在将图像上传到Adobe Dynamic Media Classic之前，请确保它们是最高质量的大小和格式。 Adobe Dynamic Media Classic建议上载像素数足够的高质量图像（长像素从1500到2000像素）。 此大小调整允许所需的任何Dynamic Imaging。

有关上传图像的详细信息，请参阅 [上载文件](uploading-files.md#uploading_files).

**准备要上载的主映像：**

在将主图像文件上传到Adobe Dynamic Media Classic之前，请对其进行准备：

* **图像大小**  — 创建您预期使用的最大大小的图像。 通常情况下，图像的最长大小在1500到2500像素之间。 如果您打算使用缩放功能，Adobe Dynamic Media Classic建议使用大小最大会至少为2000像素的图像以获得最佳缩放详细信息。 Adobe Dynamic Media Classic可渲染每个图像高达2500万像素。 例如，可以使用5000 × 5000 MP的图像或任何其他大小组合，最大可达25 MP。

* **文件格式** - Adobe Dynamic Media Classic支持所有标准图像文件格式，包括TIFF、BMP、JPEG、PSD、GIF和EPS。 建议使用无损图像格式（TIFF 和 PNG）。如果您使用的是JPEG图像，请使用最高质量的设置。

* **颜色空间** -RGB是Web图像演示文稿的颜色空间；通常用于打印的CMYK图像在上传时自动转换为RGB。 建议上传具有嵌入式ICC（国际颜色联盟）颜色配置文件的CMYK图像以转换为RGB。 另请参阅 [ICC（国际颜色联盟）配置文件](/help/using/icc-profiles.md).
