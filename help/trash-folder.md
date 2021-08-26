---
title: 管理垃圾桶文件夹
description: 了解如何管理垃圾桶文件夹。
uuid: 3992a5b8-1919-4924-b07d-7fb25565effd
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: 553c95fc-0a41-4f06-af50-a62bc1438149
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: cffeec19-43fd-4a97-bdcc-df81af108ddd
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '547'
ht-degree: 39%

---

# 管理垃圾桶文件夹{#managing-the-trash-folder}

您从AdobeDynamic Media Classic中删除的项目将移到垃圾桶文件夹。 已删除的内容会在此文件夹中保留七天，直到它们被恢复或永久删除为止。 您可以通过单击资产库底部的&#x200B;**[!UICONTROL 垃圾桶]**&#x200B;图标，并查看垃圾桶文件夹页面中的项目来检查已删除的项目。

所有用户都可以将垃圾桶文件夹中的项目恢复到删除之前所在的文件夹。所有用户也都可以清空垃圾桶文件中的所有内容。

从垃圾桶文件夹删除项目会永久删除Dynamic Media ClassicAdobe中的项目；无法再恢复从垃圾桶文件夹删除的项目。 对于公司管理员，有关在资源将要从垃圾桶自动删除时设置通知的信息，请参阅[应用程序常规设置](application-setup.md#general_settings)。

>[!NOTE]
>
>已移至垃圾桶文件夹的资产仍会在AdobeDynamic Media Classic中注册。 如果您尝试上传的文件与垃圾桶文件夹中已删除的文件同名，则AdobeDynamic Media Classic会将您要上传的资产视为重复资产。 因此，会将一个数字附加到其名称中。

## 关于垃圾桶文件夹 {#about-the-trash-folder}

删除文件夹中的某个项目会将此项目放置在垃圾桶文件夹中。在删除项目并将其移至垃圾桶文件夹时，会发生以下情况：

* 尽管该项目已从您的AdobeDynamic Media Classic文件夹中删除，但是当它保留在垃圾桶文件夹中时，无法将其ID分配给其他资产。 如果您尝试上传的资产与垃圾桶文件夹中的文件同名，则AdobeDynamic Media Classic会将数字附加到资产名称。
* 无法发布该项目。即使在删除项目时将其标记为发布，也不会将其发布。
* 该项目会一直保留在垃圾桶文件夹中，直到它被还原、经过七天，或者有人选择&#x200B;**[!UICONTROL 清空垃圾桶]**&#x200B;命令。 在七天之后，系统会自动执行清除操作永久删除该项目。

## 从垃圾桶文件夹恢复资源 {#restoring-assets-from-the-trash-folder}

被删除资源不必由删除它的人来恢复；任何人都可以恢复垃圾桶文件夹中的资源。恢复的资源会放到被删除时所在的文件夹。如果这些文件夹不再存在，AdobeDynamic Media Classic会重新创建它们，并且还原的资产会放置在重新创建的文件夹中。

要将资产从垃圾桶文件夹还原到从中删除这些资产的文件夹，请执行以下操作：

1. 在“资产库”面板的底部，单击&#x200B;**[!UICONTROL 垃圾桶]**&#x200B;图标以打开垃圾桶文件夹。
1. 选择要恢复的一个或多个资源。
1. 单击&#x200B;**[!UICONTROL 文件]** > **[!UICONTROL 从垃圾桶还原]**。

## 永久删除垃圾桶文件夹中的资源 {#permanently-deleting-assets-in-the-trash-folder}

删除垃圾桶文件夹中的资源时，会永久删除这些资源。资源在七天之后从垃圾桶文件夹被自动删除。

要从垃圾桶文件夹永久删除资产，请单击&#x200B;**[!UICONTROL 垃圾桶]**&#x200B;图标。 在“垃圾桶文件夹”页面上，执行以下任一操作：

* **删除单个资产**  — 选择要永久删除的资产，然后单击 **[!UICONTROL 文件]**  >  **[!UICONTROL 从垃圾桶中清空]**。

* **删除所有资产**  — 单击 **[!UICONTROL 文件]**  >  **[!UICONTROL 空垃圾桶]**。

>[!MORELIKETHIS]
>
>* [删除资源](moving-renaming-deleting-assets.md#delete_assets)

