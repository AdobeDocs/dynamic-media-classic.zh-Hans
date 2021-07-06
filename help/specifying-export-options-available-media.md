---
title: 指定 Media Portal 用户可以使用的导出选项
description: 了解如何指定Media Portal用户可用的导出选项。
uuid: 5258b8a4-0704-43cd-97d1-c9af2e4e298b
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 9bfd95da-3714-4e38-98af-331a04c685f5
feature: Dynamic Media Classic，协作，资产管理
role: Admin,User
exl-id: c27df6c2-76f4-441c-bd26-cee98203291e
source-git-commit: df689ff5a127bfbc400ca5331168d1ff7bb0b42e
workflow-type: tm+mt
source-wordcount: '380'
ht-degree: 71%

---

# 指定 Media Portal 用户可以使用的导出选项 {#specifying-export-options-available-to-media-portal-users}

如果管理员为他们授予权限，Media Portal 用户可以在导出图像时重设图像的格式。例如，他们可以更改大小、文件格式和图像质量。导出时自动重设图像的格式无需单独重设图像的格式，从而节省了时间。此外，管理员可以创建预设，即预先建立图像格式设置选区。当导出图像来根据您公司的规范重设图像的格式时，您可以采用预设。

通过用户定义的转换导出图像资源，或导出原始主图像时，将应用以下两种限制：

* 可用于导出作业的 Zip 压缩导出文件的最大文件大小为 1 GB。
* 每个导出作业最多可以有 500 个总资源。

另请参阅[从Dynamic Media Classic](exporting-assets-from-dmc.md#exporting-assets-from_dmc)导出资产。

**指定 Media Portal 用户可以使用的导出选项:**

1. 在全局导航栏上，单击&#x200B;**[!UICONTROL 设置]** > **[!UICONTROL 图像预设]**。
1. 在“图像预设”窗口中，选择下列任一选项：

   * **启用用户定义的转化**  — 选中此选项后，用户可以从“导出选定的资 **** 产”窗口的“缩放”下拉列表中选择其他。然后用户可以选择度量单位（如像素或厘米），并指定所需的宽度和高度。当他们导出或下载这些文件时，图像文件将重新格式化。

      从“**[!UICONTROL 大小]**”下拉列表中选择“**[!UICONTROL 像素]**”时，生成的图像宽度 x 高度不得超过 1 亿像素。此大小相当于正方形图像的 10,000 x 10,000 像素，或大约为 2x3 宽高比图像的 8,000 x 12,000 像素。如果导出原始主图像，则不会应用此大小限制。

      如果您希望用户下载文件，而不在下载时重设文件的格式，请取消选择该选项。

   * **启用导出原始图像**  — 用于导出原始主控图像。在&#x200B;**[!UICONTROL 导出选定资产]**&#x200B;面板中，用户可以打开&#x200B;**[!UICONTROL 转化]**&#x200B;下拉菜单，然后选择&#x200B;**[!UICONTROL 导出原始]**&#x200B;以导出原始文件。 如果要强制用户在导出图像时选择图像预设或选择转换选项，请取消选择此选项。

>[!MORELIKETHIS]
>
>* [图像预设](application-setup.md#image_presets)
* [为组选择图像预设访问权限](creating-media-portal-groups.md#choosing_image_preset_access_permissions_for_a_group)

