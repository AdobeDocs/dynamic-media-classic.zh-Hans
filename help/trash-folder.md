---
title: 管理垃圾桶資料夾
description: 瞭解如何管理垃圾桶資料夾。
uuid: 3992a5b8-1919-4924-b07d-7fb25565effd
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: 553c95fc-0a41-4f06-af50-a62bc1438149
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: cffeec19-43fd-4a97-bdcc-df81af108ddd
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '553'
ht-degree: 31%

---

# 管理垃圾桶資料夾{#managing-the-trash-folder}

您從Adobe Dynamic Media Classic刪除的專案會移至垃圾桶資料夾。 已刪除的檔案會在此資料夾中保留七天，直到恢復或永久刪除為止。 您可以按一下 **[!UICONTROL 垃圾桶]** 圖示並檢視「垃圾桶」資料夾頁面中的專案。

所有用户都可以将垃圾桶文件夹中的项目恢复到删除之前所在的文件夹。所有用户也都可以清空垃圾桶文件中的所有内容。

若從垃圾桶資料夾刪除專案，將會從Adobe Dynamic Media Classic中永久刪除專案；從垃圾桶資料夾刪除的專案將無法再還原。 对于公司管理员，有关在资源将要从垃圾桶自动删除时设置通知的信息，请参阅[应用程序常规设置](application-setup.md#general_settings)。

>[!NOTE]
>
>已移至垃圾桶資料夾的資產仍會在Adobe Dynamic Media Classic上註冊。 如果您嘗試上傳的檔案名稱與垃圾桶資料夾中已刪除的檔案名稱相同，Adobe Dynamic Media Classic會將您要上傳的資產視為重複資產。 因此，会将一个数字附加到其名称中。

## 关于垃圾桶文件夹 {#about-the-trash-folder}

删除文件夹中的某个项目会将此项目放置在垃圾桶文件夹中。在删除项目并将其移至垃圾桶文件夹时，会发生以下情况：

* 雖然專案已從您的Adobe Dynamic Media Classic資料夾中移除，但其ID無法指派給另一個資產，因其仍保留在垃圾桶資料夾中。 如果您嘗試上傳與「垃圾桶」資料夾中檔案同名的資產，Adobe Dynamic Media Classic會在資產名稱后附加一個數字。
* 无法发布该项目。即使在删除项目时将其标记为发布，也不会将其发布。
* 專案會保留在垃圾桶資料夾中，直到還原完成、過了七天或有人選擇 **[!UICONTROL 清空垃圾桶]** 命令。 在七天之后，系统会自动执行清除操作永久删除该项目。

## 從垃圾桶資料夾還原資產 {#restoring-assets-from-the-trash-folder}

刪除資產的人不需要還原資產；任何人都可以從垃圾桶資料夾中還原資產。 恢复的资源会放到被删除时所在的文件夹。如果這些資料夾已不存在，Adobe Dynamic Media Classic會重新建立它們，而還原的資產會放在重新建立的資料夾中。

若要將資產從垃圾桶資料夾還原至刪除它們的資料夾，請執行下列動作：

1. 在「資產庫」面板底部，選取 **[!UICONTROL 垃圾桶]** 圖示以開啟垃圾桶資料夾。
1. 選取您要還原的一個或多個資產。
1. 前往 **[!UICONTROL 檔案]** > **[!UICONTROL 從垃圾桶還原]**.

## 永久删除垃圾桶文件夹中的资源 {#permanently-deleting-assets-in-the-trash-folder}

删除垃圾桶文件夹中的资源时，会永久删除这些资源。资源在七天之后从垃圾桶文件夹被自动删除。

若要從垃圾桶資料夾中永久刪除資產，請選取 **[!UICONTROL 垃圾桶]** 圖示。 在「垃圾桶」資料夾頁面上，執行下列任一項作業：

* **刪除個別資產**  — 選取您要永久刪除的資產，然後前往 **[!UICONTROL 檔案]** > **[!UICONTROL 從垃圾桶清空]**.

* **刪除所有資產**  — 前往 **[!UICONTROL 檔案]** > **[!UICONTROL 清空垃圾桶]**.

>[!MORELIKETHIS]
>
>* [删除资源](moving-renaming-deleting-assets.md#delete_assets)

