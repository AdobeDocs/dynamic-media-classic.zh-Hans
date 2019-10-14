---
title: 管理垃圾桶文件夹
seo-title: 管理垃圾桶文件夹
description: 'null'
seo-description: 了解如何管理垃圾桶文件夹。
uuid: 3992a5b8-1919-4924-b07d-7fb25565effd
contentOwner: admin
content-type: 引用
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEEVENTONDEMAND_PK/categories/managing_assets
discoiquuid: 553c95fc-0a41-4f06-af50-a62bc1438149
translation-type: tm+mt
source-git-commit: 6fff3699f8a08af433df3f3a7790a11bf9d05b00

---


# 管理垃圾桶文件夹{#managing-the-trash-folder}

您从 Scene7 Publishing System 删除的项目会移到垃圾桶文件夹。它们在该文件夹中保留七天，如果不被恢复则被永久删除。您可以通过选择位于资源库底部的“垃圾桶”图标 ，查看垃圾桶文件夹中的项目来检查删除的项目。

所有用户都可以将垃圾桶文件夹中的项目恢复到删除之前所在的文件夹。所有用户也都可以清空垃圾桶文件中的所有内容。

删除垃圾桶文件夹中的项目会从 Scene7 Publishing System 永久删除此项目；从垃圾桶文件夹删除的项目将无法恢复。对于公司管理员，有关在资源将要从垃圾桶自动删除时设置通知的信息，请参阅[应用程序常规设置](application-setup.md#general_settings)。

>[!NOTE]
>
>已移到垃圾桶文件夹的资源仍会在 Scene7 Publishing System 上注册。如果您尝试上传的文件与垃圾桶文件夹中已删除的文件同名，Dynamic Media Classic会将要上传的资产视为重复的资产。 因此，会将一个数字附加到其名称中。

## 关于垃圾桶文件夹 {#about-the-trash-folder}

删除文件夹中的某个项目会将此项目放置在垃圾桶文件夹中。在删除项目并将其移至垃圾桶文件夹时，会发生以下情况：

* 虽然已从 Scene7 Publishing System 文件夹删除了项目，但此项目仍位于垃圾桶文件夹中，其 ID 无法分配给其他资源。如果您尝试上传的资产名称与垃圾桶文件夹中的文件相同，Dynamic Media Classic会在资产名称中附加一个数字。
* 无法发布该项目。即使在删除项目时将其标记为发布，也不会将其发布。
* 在七天之内，该项目一直停留在垃圾桶文件夹中，直到得到恢复，或有人选择“清空垃圾桶”命令。在七天之后，系统会自动执行清除操作永久删除该项目。

## 从垃圾桶文件夹恢复资源 {#restoring-assets-from-the-trash-folder}

被删除资源不必由删除它的人来恢复；任何人都可以恢复垃圾桶文件夹中的资源。恢复的资源会放到被删除时所在的文件夹。如果这些文件夹不再存在，Scene7 Publishing System 会重新创建，恢复的资源会放入重新创建的文件夹。

请执行以下步骤，将资源从垃圾桶文件夹恢复到删除之前所在的文件夹：

1. 单击垃圾桶图标以打开垃圾桶文件夹。
1. 选择要恢复的一个或多个资源。
1. 选择“文件”&gt;“从垃圾桶中还原”。

## 永久删除垃圾桶文件夹中的资源 {#permanently-deleting-assets-in-the-trash-folder}

删除垃圾桶文件夹中的资源时，会永久删除这些资源。资源在七天之后从垃圾桶文件夹被自动删除。

要永久删除垃圾桶文件夹中的资源，请选择“垃圾桶”图标  打开垃圾桶文件夹。然后删除文件夹中的单个资源或所有资源：

* **删除单个资产** ，选择要永久删除的资产，然后单击文 **[!UICONTROL 件&gt;从垃圾桶中清空]**。

* **删除所有资产** ，单击 **[!UICONTROL 文件&gt;清空垃圾桶]**。

>[!MORELIKETHIS]
>
>* [删除资源](moving-renaming-deleting-assets.md#delete_assets)

