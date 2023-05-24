---
title: 创建和启用图像预设
description: 了解如何在Adobe Dynamic Media Classic中创建和启用图像预设。
uuid: 62cfc6fa-da91-4c42-a3ed-10956384d633
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
discoiquuid: 84257b2a-681c-4fe9-a6e5-3633c1d61d8c
feature: Dynamic Media Classic,Collaboration,Image Presets,Asset Management
role: Admin,User
exl-id: 94c6c388-226b-4172-a6c7-a8dcf9c0f0cf
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '258'
ht-degree: 72%

---

# 创建和启用图像预设{#creating-and-enabling-image-presets}

当用户使用 Media Portal 导出图像资源时，他们可以在“导出所选资源”对话框中选择一种“图像预设”。图像预设是一组预定义的设置，用于更改图像在导出时的外观大小、图像质量、格式、分辨率以及其他方面。

Media Portal 管理员可以创建图像预设，以便控制导出时如何重设它们的格式。当用户从Adobe Dynamic Media Classic导出图像时，图像预设会根据公司的规范重新设置图像的格式。 用户按照“图像预设”的精确规范导出图像，而非自已重设图像的格式。

导出图像资源时，有下列限制：

* 每张图像的宽 x 高必须小于或等于 100 MB。例如，图像不能超过 10K x 10K，或以下任意宽高比变体（如 8K x 12K）。
* 每个导出作业的最大总文件大小为1 GB。
* 每个导出作业最多可以有 500 个总资源。

>[!NOTE]
>
>这些限制仅适用于导出派生的图像资产，而不适用于导出主文件。

要创建图像预设，请参阅[图像预设](application-setup.md#image_presets)。

要使用户能够在导出文件时选择“图像预设”，请参阅[指定 Media Portal 用户可以使用的导出选项](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users)。

要选择某个组的成员可以使用的图像预设，请参阅[为组选择图像预设访问权限](creating-media-portal-groups.md#choosing_image_preset_access_permissions_for_a_group)。
