---
title: 创建和启用图像预设
seo-title: 创建和启用图像预设
description: 'null'
seo-description: 了解如何创建和启用图像预设。
uuid: 62cfc fa-da91-4c42-a3 ed-10956384d633
contentOwner: admin
content-type: 引用
products: SG_ EXPERIENCE MANAGER/Dynamic-Media-Scene-7
geptopics: SG_ SCENESELEFERENDER_ PK/categories/media_ Portal
discoiquuid: 84257b2a-681c-4fe9e5-3633c1d61d8c
translation-type: tm+mt
source-git-commit: 75f006fd81b0fe2dad5479cdd98e45eaada46b2a

---


# 创建和启用图像预设{#creating-and-enabling-image-presets}

当用户使用 Media Portal 导出图像资源时，他们可以在“导出所选资源”对话框中选择一种“图像预设”。图像预设是一组预定义的设置，用于更改图像在导出时的外观大小、图像质量、格式、分辨率以及其他方面。

Media Portal 管理员可以创建图像预设，以便控制导出时如何重设它们的格式。当用户从 Scene7 Publishing System 导出图像时，“图像预设”会根据您公司的规范重设图像的格式。用户按照“图像预设”的精确规范导出图像，而非自已重设图像的格式。

导出图像资源时，有下列限制：

* 每张图像的宽 x 高必须小于或等于 100 MB。例如，图像不能超过 10K x 10K，或以下任意宽高比变体（如 8K x 12K）。
* 每个导出作业的总文件大小最大为 1 GB。
* 每个导出作业最多可以有 500 个总资源。

>[!NOTE]
>
>这些限制仅适用于导出派生的图像资源，而不适用于导出主文件。

要创建图像预设，请参阅[图像预设](application-setup.md#image_presets)。

要使用户能够在导出文件时选择“图像预设”，请参阅[指定 Media Portal 用户可以使用的导出选项](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users)。

要选择某个组的成员可以使用的图像预设，请参阅[为组选择图像预设访问权限](creating-media-portal-groups.md#choosing_image_preset_access_permissions_for_a_group)。