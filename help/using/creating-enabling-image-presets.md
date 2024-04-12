---
title: 创建和启用图像预设
description: 了解如何在Adobe Dynamic Media Classic中创建和启用图像预设。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
feature: Dynamic Media Classic,Collaboration,Image Presets,Asset Management
role: Admin,User
exl-id: 94c6c388-226b-4172-a6c7-a8dcf9c0f0cf
topic: Content Management
level: Intermediate
source-git-commit: b2a6aeb1aab420803a8b7dafb0fdeda495e2a69b
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 49%

---

# 创建和启用图像预设{#creating-and-enabling-image-presets}

当用户使用 Media Portal 导出图像资源时，他们可以在“导出所选资源”对话框中选择一种“图像预设”。图像预设是预定义设置的集合，这些设置可在导出图像时更改图像的大小、图像质量、格式、分辨率及其他外观方面。

Media Portal 管理员可以创建图像预设，以便控制导出时如何重设它们的格式。当用户从Adobe Dynamic Media Classic导出图像时，图像预设会根据贵公司的规范重新设置图像的格式。 用户按照“图像预设”的精确规范导出图像，而非自已重设图像的格式。

导出图像资源时，有下列限制：

* 每个图像的宽度×高度必须小于或等于100 MB。 例如，图像不能超过10 K×10 K，或者下面的任何外观变化，如8 K×12 K。
* 每个导出作业的总文件大小最多为1 GB。
* 每个导出作业最多可以有 500 个总资源。

>[!NOTE]
>
>这些限制仅适用于导出派生的图像资产，而不适用于导出主文件。

要创建图像预设，请参阅[图像预设](application-setup.md#image_presets)。

要使用户能够在导出文件时选择“图像预设”，请参阅[指定 Media Portal 用户可以使用的导出选项](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users)。

要选择某个组的成员可以使用的图像预设，请参阅[为组选择图像预设访问权限](creating-media-portal-groups.md#choosing_image_preset_access_permissions_for_a_group)。
