---
title: 指定Media Portal使用者可用的匯出選項
description: 瞭解如何在Adobe Dynamic Media Classic中指定Media Portal使用者可用的匯出選項。
uuid: 5258b8a4-0704-43cd-97d1-c9af2e4e298b
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 9bfd95da-3714-4e38-98af-331a04c685f5
feature: Dynamic Media Classic,Collaboration,Asset Management
role: Admin,User
exl-id: c27df6c2-76f4-441c-bd26-cee98203291e
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '381'
ht-degree: 57%

---

# 指定Media Portal使用者可用的匯出選項 {#specifying-export-options-available-to-media-portal-users}

如果管理员为他们授予权限，Media Portal 用户可以在导出图像时重设图像的格式。例如，他们可以更改大小、文件格式和图像质量。导出时自动重设图像的格式无需单独重设图像的格式，从而节省了时间。此外，管理员可以创建预设，即预先建立图像格式设置选区。当导出图像来根据您公司的规范重设图像的格式时，您可以采用预设。

如果您透過使用者定義的轉換來匯出影像資產，或匯出原始主要影像，則以下兩個限制適用：

* 可用于导出作业的 Zip 压缩导出文件的最大文件大小为 1 GB。
* 每个导出作业最多可以有 500 个总资源。

另請參閱 [從Adobe Dynamic Media Classic匯出資產](exporting-assets-from-dmc.md#exporting-assets-from_dmc).

**指定 Media Portal 用户可以使用的导出选项:**

1. 在全域導覽列上，前往 **[!UICONTROL 設定]** > **[!UICONTROL 影像預設集]**.
1. 在“图像预设”窗口中，选择下列任一选项：

   * **啟用使用者定義的轉換**  — 選取後，此選項可讓使用者從 **[!UICONTROL 大小]** 「匯出選取的資產」視窗中的下拉式清單。 然后用户可以选择度量单位（如像素或厘米），并指定所需的宽度和高度。当他们导出或下载这些文件时，图像文件将重新格式化。

      从“**[!UICONTROL 大小]**”下拉列表中选择“**[!UICONTROL 像素]**”时，生成的图像宽度 x 高度不得超过 1 亿像素。此大小相当于正方形图像的 10,000 x 10,000 像素，或大约为 2x3 宽高比图像的 8,000 x 12,000 像素。如果您匯出原始主要影像，則大小限制不適用。

      如果您希望用户下载文件，而不在下载时重设文件的格式，请取消选择该选项。

   * **啟用匯出原始檔案**  — 可讓您匯出原始主要影像。 在 **[!UICONTROL 匯出選取的資產]** 面板，使用者可開啟 **[!UICONTROL 轉換]** 下拉式功能表，然後選擇 **[!UICONTROL 匯出原始檔案]** 以匯出原始檔案。 如果您要強制使用者選擇影像預設集，或在匯出影像時選擇轉換選項，請取消選取此選項。

>[!MORELIKETHIS]
>
>* [Image Presets](application-setup.md#image_presets)
>* [为组选择图像预设访问权限](creating-media-portal-groups.md#choosing_image_preset_access_permissions_for_a_group)

