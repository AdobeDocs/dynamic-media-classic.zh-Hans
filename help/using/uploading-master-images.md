---
title: 上传主图像
description: 了解如何将主图像上传到Adobe Dynamic Media Classic。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 410ba80c-7f01-4cd0-9ab3-db9658757ba7
topic: Content Management
level: Intermediate
autotag-review: '2026-05-13T20:17:09.649Z'
TQID: 'https://experienceleague.adobe.com/xi8ZvTLYacPSL7P2uqo142VpXY6SOOU7cZvA7tT0zOQ'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
source-git-commit: 81e92d0e8963cccb5b058328cb7601925f7ace4f
workflow-type: tm+mt
source-wordcount: 275
ht-degree: 0%

---

# 上传主图像{#uploading-master-images}

在将图像上传到Adobe Dynamic Media Classic之前，请确保它们是最高质量的大小和格式。 Adobe Dynamic Media Classic建议上载像素数足够的高质量图像（长像素从1500到2000像素）。 此大小调整允许使用所需的任何Dynamic Imaging。

有关上传图像的详细信息，请参阅[上传文件](uploading-files.md#uploading_files)。

**准备要上载的主映像：**

在将主图像文件上传到Adobe Dynamic Media Classic之前，请对其进行准备：

* **图像大小**：创建您预期使用的最大大小的图像。 通常情况下，图像的最长大小在1500到2500像素之间。 如果您打算使用缩放功能，Adobe Dynamic Media Classic建议使用大小最大会至少为2000像素的图像以获得最佳缩放详细信息。 Adobe Dynamic Media Classic可渲染每个图像高达2500万像素。 例如，可以使用5000 × 5000 MP的图像或任何其他大小组合，最大可达25 MP。

* **文件格式**： Adobe Dynamic Media Classic支持所有标准图像文件格式。 这些格式包括TIFF、BMP、JPEG、PSD、GIF和EPS。 推荐无损图像格式 — TIFF和PNG。 如果您使用的是JPEG图像，请使用最高质量的设置。

* **色彩空间**： RGB是Web图像演示文稿的色彩空间；通常用于打印的CMYK图像在上传时自动转换为RGB。 建议上传具有嵌入式ICC（国际颜色联盟）颜色配置文件的CMYK图像以转换为RGB。 另请参阅[ICC（国际彩色联盟）配置文件](/help/using/icc-profiles.md)。
