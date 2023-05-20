---
title: 移動、重新命名和刪除資產
description: 瞭解如何在Adobe Dynamic Media Classic中移動、重新命名和刪除資產。
uuid: deff6521-0ad0-4db9-b4e0-e3211ff97740
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: 1c9e29f0-3083-4d22-a439-2a01faf59683
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 391eb7ce-ed89-47a8-a6c6-5adb3e95bf78
source-git-commit: 741e31e64125a2dfe3f801480837ffbaf81767aa
workflow-type: tm+mt
source-wordcount: '618'
ht-degree: 31%

---

# 移動、重新命名和刪除資產{#moving-renaming-and-deleting-assets}

可在浏览面板中移动、重命名和删除资源。也可以使用文本文件同时删除许多资源。

## 移动资源 {#move-assets}

可在浏览面板中将资源移至不同文件夹。

**若要移動資產：**

1. 在浏览面板中选择一个或多个资源，然后执行以下任一操作：

   * 在「資產庫」中顯示您要移動資產的資料夾，並將資產拖曳至資料夾。
   * 前往 **[!UICONTROL 檔案]** > **[!UICONTROL 移動]**，請在「移動資產」視窗中選取資料夾，然後選取 **[!UICONTROL 移動]**.

## 重命名资源 {#rename-assets}

1. 在浏览面板中选择资源，然后执行以下任一操作：

   * 選取名稱，輸入新名稱，然後按下 **[!UICONTROL 輸入]** 或從名稱中選取「離開」。
   * 前往 **[!UICONTROL 檔案]** > **[!UICONTROL 重新命名]**. 资源的名称被高亮显示。輸入新名稱，然後按 **[!UICONTROL 輸入]**. 請勿輸入現有Adobe Dynamic Media Classic資產的名稱。

## 删除资源 {#delete-assets}

您可以刪除「瀏覽」面板中選取的資產並刪除整個資料夾。 删除的资源和文件夹将移至回收站文件夹，在其中保留七天，之后将被永久删除。

在删除资源时，由此资源派生出的所有资源也会随之删除。例如，删除已为其创建了缩放目标的图像时，缩放目标也会随图像一起删除。

在删除资源时，由资源派生出的缩放目标、图像属性以及历史记录条目会随之永久删除。它们不会随资源一起移至垃圾桶文件夹；因此无法从垃圾桶恢复它们。

>[!IMPORTANT]
>
>大量刪除是一項密集的作業。 請確定您是依序執行大量刪除，而非同時執行大量刪除作業。 Adobe建議您將刪除操作限製為每小時5000個或更少的資產刪除。 任何大於每小時5000的數字都可能導致速率限制。

**若要刪除資產：**

1. 执行任何以下操作：

   * 若要刪除一個或多個資產，請在「瀏覽」面板中選取資產，然後按下 **[!UICONTROL 刪除]** 或前往 **[!UICONTROL 檔案]** > **[!UICONTROL 刪除]**.
   * 若要刪除資料夾，請選取資產資料庫中的資料夾，然後選取 **[!UICONTROL 移除資料夾]**.

      刪除資料夾會刪除該資料夾、該資料夾中的所有資產及其子資料夾中的所有資產。

如果您刪除資產檔案的原因是要以相同名稱取代另一個資產檔案，Adobe Dynamic Media Classic建議覆寫資產檔案，而非刪除資產檔案。

## 使用文本文件删除多个资源 {#delete-multiple-assets-with-a-text-file}

若要在整個資產庫中一次刪除許多資產，您可以在文字檔中列出您要刪除的資產，並將清單提交至Adobe Dynamic Media Classic。

建立Adobe Dynamic Media Classic ID清單，並將其儲存為文字(.txt)檔案。 每個Adobe Dynamic Media Classic ID都必須有自己的行（後面接著硬式傳回）。

在创建列表之后，请执行以下步骤，以使用列表来删除资源：

1. 前往 **[!UICONTROL 檔案]** > **[!UICONTROL 刪除資產清單]**.
1. 在「刪除資產清單」對話方塊中，瀏覽或輸入包含您要刪除之資產清單的文字檔路徑。
1. 選取 **[!UICONTROL 刪除]**.

當您刪除含有文字檔的資產時，如果清單中沒有任何Adobe Dynamic Media Classic ID，則會顯示「無法驗證清單中的這些專案：」訊息。 也會顯示專案清單。 不過，Adobe Dynamic Media Classic不會在作業頁面上產生錯誤。

>[!MORELIKETHIS]
>
>* [在瀏覽面板中選取資產](selecting-assets-browse-panel.md#selecting_assets_in_the_browse_panel)
>* [準備資產和資料夾以進行上傳](uploading-files.md#preparing_your_assets_and_folders_for_uploading)
>* [從垃圾桶資料夾還原資產](trash-folder.md#restoring_assets_from_the_trash_folder)

