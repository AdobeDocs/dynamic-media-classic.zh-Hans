---
title: 管理垃圾桶文件夹
description: 了解如何管理垃圾桶文件夹。
uuid: 3992a5b8-1919-4924-b07d-7fb25565effd
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: 553c95fc-0a41-4f06-af50-a62bc1438149
feature: Dynamic Media Classic，资产管理
role: 业务从业者
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 60%

---


# 管理垃圾桶文件夹{#managing-the-trash-folder}

从Dynamic Media Classic中删除的项目将移到垃圾桶文件夹。 它们在该文件夹中保留七天，如果不被恢复则被永久删除。您可以通过选择位于资源库底部的“垃圾桶”图标 ，查看垃圾桶文件夹中的项目来检查删除的项目。

所有用户都可以将垃圾桶文件夹中的项目恢复到删除之前所在的文件夹。所有用户也都可以清空垃圾桶文件中的所有内容。

从“废纸篓”文件夹删除项目将永久删除Dynamic Media Classic中的项目；无法再还原从垃圾桶文件夹删除的项目。 对于公司管理员，有关在资源将要从垃圾桶自动删除时设置通知的信息，请参阅[应用程序常规设置](application-setup.md#general_settings)。

>[!NOTE]
>
>已移到垃圾桶文件夹的资源仍在Dynamic Media Classic上注册。 如果您尝试上传的文件与垃圾桶文件夹中的已删除文件同名，Dynamic Media Classic会将要上传的资源视为重复资源。 因此，会将一个数字附加到其名称中。

## 关于垃圾桶文件夹 {#about-the-trash-folder}

删除文件夹中的某个项目会将此项目放置在垃圾桶文件夹中。在删除项目并将其移至垃圾桶文件夹时，会发生以下情况：

* 尽管项目已从您的Dynamic Media经典文件夹中删除，但无法将其ID分配给其他资源，而该资源仍保留在垃圾桶文件夹中。 如果您尝试上传的资源与垃圾桶文件夹中的文件同名，Dynamic Media Classic会将数字附加到该资源的名称中。
* 无法发布该项目。即使在删除项目时将其标记为发布，也不会将其发布。
* 在七天之内，该项目一直停留在垃圾桶文件夹中，直到得到恢复，或有人选择“清空垃圾桶”命令。在七天之后，系统会自动执行清除操作永久删除该项目。

## 从垃圾桶文件夹恢复资源 {#restoring-assets-from-the-trash-folder}

被删除资源不必由删除它的人来恢复；任何人都可以恢复垃圾桶文件夹中的资源。恢复的资源会放到被删除时所在的文件夹。如果这些文件夹不再存在，Dynamic Media Classic会重新创建它们，并且恢复的资产会放置在重新创建的文件夹中。

请执行以下步骤，将资源从垃圾桶文件夹恢复到删除之前所在的文件夹：

1. 单击垃圾桶图标以打开垃圾桶文件夹。
1. 选择要恢复的一个或多个资源。
1. 选择“文件”>“从垃圾桶中还原”。

## 永久删除垃圾桶文件夹中的资源  {#permanently-deleting-assets-in-the-trash-folder}

删除垃圾桶文件夹中的资源时，会永久删除这些资源。资源在七天之后从垃圾桶文件夹被自动删除。

要永久删除垃圾桶文件夹中的资源，请选择“垃圾桶”图标  打开垃圾桶文件夹。然后删除文件夹中的单个资源或所有资源：

* **删除单个** 资源选择要永久删除的资源，然后单击“文 **[!UICONTROL 件”>“从废纸篓清空]**”。

* **删除所有资** 源单 **[!UICONTROL 击“文件”>“清空垃圾桶]**”。

>[!MORELIKETHIS]
>
>* [删除资源](moving-renaming-deleting-assets.md#delete_assets)

