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
role: Business Practitioner
exl-id: cffeec19-43fd-4a97-bdcc-df81af108ddd
translation-type: tm+mt
source-git-commit: 1beb30b9eda4487dcd549034906079dee0b3149a
workflow-type: tm+mt
source-wordcount: '545'
ht-degree: 39%

---

# 管理垃圾桶文件夹{#managing-the-trash-folder}

从Dynamic Media Classic中删除的项目将移到垃圾桶文件夹。 已删除的内容将保留在此文件夹中七天，直到它们被恢复或永久删除。 可以通过单击资源库底部的&#x200B;**[!UICONTROL 垃圾桶]**&#x200B;图标，并查看垃圾桶文件夹页面中的项目来检查已删除的项目。

所有用户都可以将垃圾桶文件夹中的项目恢复到删除之前所在的文件夹。所有用户也都可以清空垃圾桶文件中的所有内容。

从“废纸篓”文件夹删除项目将永久删除Dynamic Media Classic中的项目；无法再还原从垃圾桶文件夹删除的项目。 对于公司管理员，有关在资源将要从垃圾桶自动删除时设置通知的信息，请参阅[应用程序常规设置](application-setup.md#general_settings)。

>[!NOTE]
>
>已移到垃圾桶文件夹的资源仍在Dynamic Media Classic上注册。 如果您尝试上传的文件与垃圾桶文件夹中的已删除文件同名，Dynamic Media Classic会将要上传的资源视为重复资源。 因此，会将一个数字附加到其名称中。

## 关于垃圾桶文件夹 {#about-the-trash-folder}

删除文件夹中的某个项目会将此项目放置在垃圾桶文件夹中。在删除项目并将其移至垃圾桶文件夹时，会发生以下情况：

* 尽管项目已从您的Dynamic Media经典文件夹中删除，但无法将其ID分配给其他资源，而该资源仍保留在垃圾桶文件夹中。 如果您尝试上传的资源与垃圾桶文件夹中的文件同名，Dynamic Media Classic会将数字附加到该资源的名称中。
* 无法发布该项目。即使在删除项目时将其标记为发布，也不会将其发布。
* 项目将保留在“废纸篓”文件夹中，直到恢复、七天过去，或者有人选择&#x200B;**[!UICONTROL 清空“废纸篓”]**&#x200B;命令。 在七天之后，系统会自动执行清除操作永久删除该项目。

## 从垃圾桶文件夹恢复资源 {#restoring-assets-from-the-trash-folder}

被删除资源不必由删除它的人来恢复；任何人都可以恢复垃圾桶文件夹中的资源。恢复的资源会放到被删除时所在的文件夹。如果这些文件夹不再存在，Dynamic Media Classic会重新创建它们，并且恢复的资产会放置在重新创建的文件夹中。

要将资源从垃圾桶文件夹恢复到删除它们的文件夹，请执行以下操作：

1. 在“资源库”面板底部，单击&#x200B;**[!UICONTROL 垃圾桶]**&#x200B;图标以打开垃圾桶文件夹。
1. 选择要恢复的一个或多个资源。
1. 单击&#x200B;**[!UICONTROL 文件]** > **[!UICONTROL 从垃圾桶]**&#x200B;恢复。

## 永久删除垃圾桶文件夹中的资源 {#permanently-deleting-assets-in-the-trash-folder}

删除垃圾桶文件夹中的资源时，会永久删除这些资源。资源在七天之后从垃圾桶文件夹被自动删除。

要从垃圾桶文件夹中永久删除资源，请单击&#x200B;**[!UICONTROL 垃圾桶]**&#x200B;图标。 在“废纸篓”文件夹中，执行下列任一操作：

* **删除单个资源**  — 选择要永久删除的资源，然后单击“文件”>“从废纸篓 **[!UICONTROL 中清空”]**  ****。

* **删除所有资源**  — 单击 **[!UICONTROL 文件]** >清 **[!UICONTROL 空垃圾桶]**。

>[!MORELIKETHIS]
>
>* [删除资源](moving-renaming-deleting-assets.md#delete_assets)

