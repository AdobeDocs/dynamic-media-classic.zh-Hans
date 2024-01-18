---
title: 指定Media Portal用户可用的导出选项
description: 了解如何在Adobe Dynamic Media Classic中指定Media Portal用户可用的导出选项。
uuid: 5258b8a4-0704-43cd-97d1-c9af2e4e298b
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 9bfd95da-3714-4e38-98af-331a04c685f5
feature: Dynamic Media Classic,Collaboration,Asset Management
role: Admin,User
exl-id: c27df6c2-76f4-441c-bd26-cee98203291e
topic: Collaboration, Content Management
level: Intermediate
source-git-commit: ae7d0c6d3047d68ed3da4187ef516dc51c95de30
workflow-type: tm+mt
source-wordcount: '385'
ht-degree: 37%

---

# 指定Media Portal用户可用的导出选项 {#specifying-export-options-available-to-media-portal-users}

如果管理员为他们授予权限，Media Portal 用户可以在导出图像时重设图像的格式。例如，他们可以更改大小、文件格式和图像质量。导出时自动重设图像的格式无需单独重设图像的格式，从而节省了时间。此外，管理员可以创建预设，即预先建立图像格式设置选区。当导出图像来根据您公司的规范重设图像的格式时，您可以采用预设。

如果通过用户定义的转换导出图像资产，或者导出原始主图像，则以下两个限制适用：

* 可用于导出作业的 Zip 压缩导出文件的最大文件大小为 1 GB。
* 每个导出作业最多可以有 500 个总资源。

另请参阅 [从Adobe Dynamic Media Classic导出资源](exporting-assets-from-dmc.md#exporting-assets-from_dmc).

**要指定可供Media Portal用户使用的导出选项，请执行以下操作：**

1. 在全局导航栏上，转到 **[!UICONTROL 设置]** > **[!UICONTROL 图像预设]**.
1. 在“图像预设”窗口中，选择下列任一选项：

   * **启用用户定义的转换**  — 选中此选项后，用户可以从 **[!UICONTROL 大小]** 导出选定资源窗口中的下拉列表。 然后，用户可以选择一个度量单位，如像素或厘米，然后指定所需的宽度和高度。 当他们导出或下载这些文件时，图像文件将重新格式化。

     时间 **[!UICONTROL 像素]** 是从 **[!UICONTROL 大小]** 下拉列表中，生成的图像宽度×高度不能超过1亿像素。 此大小等于方形图像的10,000 × 10,000像素，或长宽比为2x3的图像的大约8,000 × 12,000像素。 如果导出原始主图像，则此大小限制不适用。

     如果您希望用户下载文件，而不在下载时重设文件的格式，请取消选择该选项。

   * **启用导出原始**  — 用于导出原始主图像。 在 **[!UICONTROL 导出所选资源]** 面板，用户可以打开 **[!UICONTROL 转化]** 下拉菜单并选择 **[!UICONTROL 导出原始]** 以导出原始文件。 如果要强制用户在导出图像时选择图像预设或选择转换选项，请取消选择此选项。

>[!MORELIKETHIS]
>
>* [Image Presets](application-setup.md#image_presets)
>* [选择群组的图像预设访问权限](creating-media-portal-groups.md#choosing_image_preset_access_permissions_for_a_group)
