---
title: 建立和管理Media Portal群組
description: 瞭解如何在Adobe Dynamic Media Classic中建立和管理Media Portal群組。
uuid: 23f360e1-ddcb-491b-ab9f-428f3ac9c316
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
discoiquuid: 91524d36-b77a-4dc4-acba-a7bd85297e98
feature: Dynamic Media Classic,Collaboration,Asset Management
role: Admin,User
exl-id: 0deb7133-b895-4c3f-8e5e-8604a6f2d16b
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '839'
ht-degree: 56%

---

# 建立和管理Media Portal群組{#creating-and-managing-media-portal-groups}

*组*&#x200B;旨在帮助您管理 Media Portal 用户。要访问某个资源，用户必须至少是一个具有该资源访问权限的组的成员。添加用户时，将该用户指定给一个或多个组。从而赋予该用户指定给该组的文件夹访问权限。您还可以选择某个组可以使用的图像预设。

## 使用群組來限制對資料夾、資產和影像預設集的存取 {#using-groups-to-restrict-access-to-folders-assets-and-image-presets}

要在不同级别授予访问权限，请创建组。为每个组指定对不同文件夹和文件夹中资源的读取、写入和删除权限。此外，您还要决定该组可以使用的图像预设。然后，向组指定用户。一个用户可以是多个组的成员。使用组可以灵活地指定对所有内容中有限的一部分内容的访问权限。

如果您未明確授予群組對資產或檔案夾的許可權，則該資產或檔案夾會繼承您指派給其父檔案夾（檔案夾階層中位於其上方的檔案夾）的許可權。 如果您想确保父文件夹的所有子文件夹继承相同的权限，请为父文件夹授予权限。

>[!NOTE]
>
>用户可以属于多个组。当一个用户属于两个对某个文件夹具有不同访问权限的组时，该用户将被授予最高访问权限。

## 添加组 {#adding-a-group}

1. 前往 **[!UICONTROL 設定]** > **[!UICONTROL Media Portal設定]** > **[!UICONTROL 群組]**.
1. 選取 **[!UICONTROL 新增]**.
1. 在「新增群組」對話方塊的「群組名稱」方塊中，輸入群組的名稱，然後選取 **[!UICONTROL 新增群組]**.
1. 根据需要选中用户名称旁的方框，以便将用户添加到新组。
1. 如果您想要立即指定存取許可權，請選取 **[!UICONTROL 資產存取許可權]** 標籤，然後指定您想要的選項。

   请参阅[建立组的资源访问权限](creating-media-portal-groups.md#establishing_asset_access_permissions_for_a_group)。

1. 如果要選擇群組可用的影像預設集，請選取 **[!UICONTROL 影像預設集存取許可權]** 標籤，並選取群組可以使用的影像預設集。

   请参阅[为组选择图像预设访问权限](creating-media-portal-groups.md#choosing_image_preset_access_permissions_for_a_group)。

1. 選取 **[!UICONTROL 關閉]**.

## 建立组的资源访问权限 {#establishing-asset-access-permissions-for-a-group}

1. 前往 **[!UICONTROL 設定]** > **[!UICONTROL Media Portal設定]** > **[!UICONTROL 群組]**.
1. 在“组列表”页面上，执行下列操作之一：

   * 若要新增群組並指定許可權，請選取 **[!UICONTROL 新增]**. 在「新增群組」對話方塊中，輸入群組的名稱，選取 **[!UICONTROL 新增群組]**，並將使用者新增至群組。
   * 若要編輯群組的許可權，請選取群組，然後選取 **[!UICONTROL 編輯]**.

1. 在「新增群組」或「編輯群組」對話方塊中，選取 **[!UICONTROL 資產存取許可權]** 標籤。 该选项卡的右侧提供了用于建立文件夹和资源读取、写入和删除权限的方框。您可以在左窗格中展开和折叠文件夹和子文件夹。
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

1. 選取 **[!UICONTROL 關閉]**.

>[!NOTE]
>
>选中一个框后，即可设置访问权限。向某个文件夹指定权限时，其所含的子文件夹和所有文件将被授予与父文件夹相同的权限。但是，您可以为单个子文件夹和资源文件指定不同的权限。

## 为组选择图像预设访问权限 {#choosing-image-preset-access-permissions-for-a-group}

如果您要指定组成员在使用 Media Portal 导出资源时可以使用的图像预设，请为组选择图像预设访问权限。

另請參閱 [指定Media Portal使用者可用的匯出選項](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users).

**若要選擇群組的影像預設集存取許可權：**

1. 前往 **[!UICONTROL 設定]** > **[!UICONTROL Media Portal設定]** > **[!UICONTROL 群組]**.
1. 在“组列表”页面上，执行下列操作之一：

   * 若要新增群組並指定哪些影像預設集可供使用，請選取 **[!UICONTROL 新增]**. 在「新增群組」對話方塊中，輸入群組的名稱，選取 **[!UICONTROL 新增群組]**，並將使用者新增至群組。
   * 若要編輯群組的「影像預設集」選項，請選取該群組，然後選取 **[!UICONTROL 編輯]**.

1. 在「新增群組」或「編輯群組」對話方塊中，選取 **[!UICONTROL 影像預設集存取許可權]** 標籤。
1. 若要指定Media Portal使用者匯出資產時可以使用哪些預設集，請選取或取消選取影像預設集。
1. 選取 **[!UICONTROL 關閉]**.

## 编辑和删除组 {#edit-and-delete-groups}

1. 前往 **[!UICONTROL 設定]** > **[!UICONTROL Media Portal設定]** > **[!UICONTROL 群組]**.
1. 在“组列表”页面上，选择一个组，然后进行编辑或删除。

   **編輯群組**  — 選取 **[!UICONTROL 編輯]**，然後在「編輯群組」對話方塊中選擇選項。

   **刪除群組**  — 選取 **[!UICONTROL 刪除]**.
