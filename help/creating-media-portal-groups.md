---
title: 创建和管理媒体门户组
description: 了解如何在AdobeDynamic Media Classic中创建和管理媒体门户组。
uuid: 23f360e1-ddcb-491b-ab9f-428f3ac9c316
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
discoiquuid: 91524d36-b77a-4dc4-acba-a7bd85297e98
feature: Dynamic Media Classic,Collaboration,Asset Management
role: Admin,User
exl-id: 0deb7133-b895-4c3f-8e5e-8604a6f2d16b
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '839'
ht-degree: 56%

---

# 创建和管理媒体门户组{#creating-and-managing-media-portal-groups}

*组*&#x200B;旨在帮助您管理 Media Portal 用户。要访问某个资源，用户必须至少是一个具有该资源访问权限的组的成员。添加用户时，将该用户指定给一个或多个组。从而赋予该用户指定给该组的文件夹访问权限。您还可以选择某个组可以使用的图像预设。

## 使用群组可限制对文件夹、资产和图像预设的访问 {#using-groups-to-restrict-access-to-folders-assets-and-image-presets}

要在不同级别授予访问权限，请创建组。为每个组指定对不同文件夹和文件夹中资源的读取、写入和删除权限。此外，您还要决定该组可以使用的图像预设。然后，向组指定用户。一个用户可以是多个组的成员。使用组可以灵活地指定对所有内容中有限的一部分内容的访问权限。

如果您没有专门为资产或文件夹授予群组权限，则该资产或文件夹会继承您分配给其父文件夹（文件夹层次结构中该文件夹的上方文件夹）的权限。 如果您想确保父文件夹的所有子文件夹继承相同的权限，请为父文件夹授予权限。

>[!NOTE]
>
>用户可以属于多个组。当一个用户属于两个对某个文件夹具有不同访问权限的组时，该用户将被授予最高访问权限。

## 添加组 {#adding-a-group}

1. 转到&#x200B;**[!UICONTROL 设置]** > **[!UICONTROL 媒体门户设置]** > **[!UICONTROL 组]**。
1. 选择&#x200B;**[!UICONTROL Add]**。
1. 在“添加组”对话框的“组名称”框中输入组的名称，然后选择“添加组”]**。**[!UICONTROL 
1. 根据需要选中用户名称旁的方框，以便将用户添加到新组。
1. 如果您现在想要指定访问权限，请选择&#x200B;**[!UICONTROL 资产访问权限]**&#x200B;选项卡，然后指定所需的选项。

   请参阅[建立组的资源访问权限](creating-media-portal-groups.md#establishing_asset_access_permissions_for_a_group)。

1. 如果要选择可用于组的图像预设，请选择&#x200B;**[!UICONTROL 图像预设访问权限]**&#x200B;选项卡，然后选择组可以使用的图像预设。

   请参阅[为组选择图像预设访问权限](creating-media-portal-groups.md#choosing_image_preset_access_permissions_for_a_group)。

1. 选择&#x200B;**[!UICONTROL 关闭]**。

## 建立组的资源访问权限 {#establishing-asset-access-permissions-for-a-group}

1. 转到&#x200B;**[!UICONTROL 设置]** > **[!UICONTROL 媒体门户设置]** > **[!UICONTROL 组]**。
1. 在“组列表”页面上，执行下列操作之一：

   * 要添加群组并指定权限，请选择&#x200B;**[!UICONTROL Add]**。 在“添加组”对话框中，输入组的名称，选择&#x200B;**[!UICONTROL 添加组]**，然后将用户添加到组。
   * 要编辑群组的权限，请选择群组，然后选择&#x200B;**[!UICONTROL 编辑]**。

1. 在添加组或编辑组对话框中，选择&#x200B;**[!UICONTROL 资产访问权限]**&#x200B;选项卡。 该选项卡的右侧提供了用于建立文件夹和资源读取、写入和删除权限的方框。您可以在左窗格中展开和折叠文件夹和子文件夹。
1. 要向文件夹或单个资源指定权限，请在左窗格中选择该文件夹。文件夹内容便会显示在右窗格中。然后，在右窗格中选中相应文件或文件夹的方框，为该组指定权限。

   下表显示了不同任务所对应的读取、写入和删除权限。

   | 任务 | 读取 | 写入 | 删除 |
   | --- | --- | --- | --- |
   | 浏览文件夹和文件 | X |  |  |
   | 编辑文件（剪切、锐化、调整） |  | X |  |
   | 更改文件名 |  | X |  |
   | 将文件移动到其他文件夹 |  | X |  |
   | 重命名文件 |  | X |  |
   | 删除文件 |  |  | X |

1. 选择&#x200B;**[!UICONTROL 关闭]**。

>[!NOTE]
>
>选中一个框后，即可设置访问权限。向某个文件夹指定权限时，其所含的子文件夹和所有文件将被授予与父文件夹相同的权限。但是，您可以为单个子文件夹和资源文件指定不同的权限。

## 为组选择图像预设访问权限 {#choosing-image-preset-access-permissions-for-a-group}

如果您要指定组成员在使用 Media Portal 导出资源时可以使用的图像预设，请为组选择图像预设访问权限。

另请参阅[指定Media Portal用户可用的导出选项](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users)。

**要为群组选择“图像预设”访问权限，请执行以下操作：**

1. 转到&#x200B;**[!UICONTROL 设置]** > **[!UICONTROL 媒体门户设置]** > **[!UICONTROL 组]**。
1. 在“组列表”页面上，执行下列操作之一：

   * 要添加组并指定可用的图像预设，请选择&#x200B;**[!UICONTROL 添加]**。 在“添加组”对话框中，输入组的名称，选择&#x200B;**[!UICONTROL 添加组]**，然后将用户添加到组。
   * 要编辑组的“图像预设”选项，请选择该组，然后选择&#x200B;**[!UICONTROL 编辑]**。

1. 在添加组或编辑组对话框中，选择&#x200B;**[!UICONTROL 图像预设访问权限]**&#x200B;选项卡。
1. 要指定Media Portal用户在导出资产时可以使用的预设，请选择或取消选择图像预设。
1. 选择&#x200B;**[!UICONTROL 关闭]**。

## 编辑和删除组 {#edit-and-delete-groups}

1. 转到&#x200B;**[!UICONTROL 设置]** > **[!UICONTROL 媒体门户设置]** > **[!UICONTROL 组]**。
1. 在“组列表”页面上，选择一个组，然后进行编辑或删除。

   **编辑群组**  — 选择 **[!UICONTROL 编辑]**，然后在“编辑群组”对话框中选择选项。

   **删除群组**  — 选择 **[!UICONTROL 删除]**。
