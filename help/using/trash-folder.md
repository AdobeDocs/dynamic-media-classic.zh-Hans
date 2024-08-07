---
title: 管理垃圾桶文件夹
description: 了解如何管理垃圾桶文件夹。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: cffeec19-43fd-4a97-bdcc-df81af108ddd
topic: Content Management
level: Intermediate
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '560'
ht-degree: 28%

---

# 管理垃圾桶文件夹{#managing-the-trash-folder}

从Adobe Dynamic Media Classic中删除的项目将移至垃圾桶文件夹。 这些已删除的项目将在此文件夹中保留七天，直到它们被恢复或永久删除。 通过选择资源库底部的&#x200B;**[!UICONTROL 垃圾桶]**&#x200B;图标，并查看“垃圾桶”文件夹页面中的项目，可以检查已删除的项目。

所有用户都可以将垃圾桶文件夹中的项目恢复到删除之前所在的文件夹。所有用户也都可以清空垃圾桶文件中的所有内容。

从垃圾桶文件夹中删除项目会永久删除Adobe Dynamic Media Classic中的项目；无法再还原从垃圾桶文件夹中删除的项目。 对于公司管理员，有关在资源将要从垃圾桶自动删除时设置通知的信息，请参阅[应用程序常规设置](application-setup.md#general_settings)。

>[!NOTE]
>
>已移至垃圾桶文件夹的Assets仍在Adobe Dynamic Media Classic中注册。 例如，假设您尝试上载一个与垃圾桶文件夹中已删除文件同名的文件。 Adobe Dynamic Media Classic会将您要上传的资产视为重复资产。 在这种情况下，会在名称后附加一个数字。

## 关于垃圾桶文件夹 {#about-the-trash-folder}

删除文件夹中的某个项目会将此项目放置在垃圾桶文件夹中。在删除项目并将其移至垃圾桶文件夹时，会发生以下情况：

* 虽然该项已从Adobe Dynamic Media Classic文件夹中删除，但如果其ID仍保留在垃圾桶文件夹中，则无法将其分配给其他资源。 如果尝试上载与垃圾桶文件夹中文件同名的资源，Adobe Dynamic Media Classic会在资源的名称后附加一个数字。
* 无法发布该项目。即使在删除项目时将其标记为发布，也不会将其发布。
* 该项将保留在垃圾桶文件夹中，直到它恢复、7天过去或者有人选择&#x200B;**[!UICONTROL 清空垃圾桶]**&#x200B;命令为止。 在七天之后，系统会自动执行清除操作永久删除该项目。

## 从垃圾桶文件夹中还原资源 {#restoring-assets-from-the-trash-folder}

删除资源的人员无需恢复资源；任何人都可以从垃圾桶文件夹恢复资源。 恢复的资源会放到被删除时所在的文件夹。如果这些文件夹不再存在，Adobe Dynamic Media Classic将重新创建它们，并且还原的资源将放置在重新创建的文件夹中。

要将资源从“垃圾桶”文件夹还原到从中删除资源的文件夹，请执行以下操作：

1. 在“资源库”面板底部，选择&#x200B;**[!UICONTROL 垃圾桶]**&#x200B;图标以打开垃圾桶文件夹。
1. 选择要还原的一个或多个资源。
1. 转到&#x200B;**[!UICONTROL 文件]** > **[!UICONTROL 从垃圾桶还原]**。

## 永久删除垃圾桶文件夹中的资源 {#permanently-deleting-assets-in-the-trash-folder}

删除垃圾桶文件夹中的资源时，会永久删除这些资源。资源在七天之后从垃圾桶文件夹被自动删除。

您可以通过选择&#x200B;**[!UICONTROL 垃圾桶]**&#x200B;图标，从垃圾桶文件夹中永久删除资源。 在“垃圾桶”文件夹页面上，执行以下任一操作：

* **删除单个资源**：您可以永久删除资源。 选择所需的资源，然后单击&#x200B;**[!UICONTROL 文件]** > **[!UICONTROL 从垃圾桶中删除]**。

* **正在删除所有资源**：转到&#x200B;**[!UICONTROL 文件]** > **[!UICONTROL 清空垃圾桶]**。

>[!MORELIKETHIS]
>
>* [删除资源](moving-renaming-deleting-assets.md#delete_assets)
