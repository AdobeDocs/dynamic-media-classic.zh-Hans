---
title: 移动、重命名和删除资产
description: 了解如何在Dynamic Media Classic中移动、重命名和删除Adobe。
uuid: deff6521-0ad0-4db9-b4e0-e3211ff97740
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: 1c9e29f0-3083-4d22-a439-2a01faf59683
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 391eb7ce-ed89-47a8-a6c6-5adb3e95bf78
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '564'
ht-degree: 37%

---

# 移动、重命名和删除资产{#moving-renaming-and-deleting-assets}

可在浏览面板中移动、重命名和删除资源。也可以使用文本文件同时删除许多资源。

## 移动资源 {#move-assets}

可在浏览面板中将资源移至不同文件夹。

1. 在浏览面板中选择一个或多个资源，然后执行以下任一操作：

   * 在资源库中显示要将资源移至的文件夹，然后将资源拖到此文件夹。
   * 转到&#x200B;**[!UICONTROL 文件]** > **[!UICONTROL 移动]**，在“移动资产”窗口中选择文件夹，然后选择&#x200B;**[!UICONTROL 移动]**。

## 重命名资源 {#rename-assets}

1. 在浏览面板中选择资源，然后执行以下任一操作：

   * 选择名称，键入新名称，然后按&#x200B;**[!UICONTROL Enter]**&#x200B;或选择离开该名称。
   * 转到&#x200B;**[!UICONTROL File]** > **[!UICONTROL Rename]**。 资源的名称被高亮显示。输入新名称，然后按&#x200B;**[!UICONTROL Enter]**。

请确保不要输入现有AdobeDynamic Media Classic资产的名称。

## 删除资源 {#delete-assets}

您可以在浏览面板中删除选定资产，并删除整个文件夹。 删除的资源和文件夹将移至回收站文件夹，在其中保留七天，之后将被永久删除。

在删除资源时，由此资源派生出的所有资源也会随之删除。例如，删除已为其创建了缩放目标的图像时，缩放目标也会随图像一起删除。

>[!NOTE]
>
>在删除资源时，由资源派生出的缩放目标、图像属性以及历史记录条目会随之永久删除。它们不会随资源一起移至垃圾桶文件夹；因此无法从垃圾桶恢复它们。

1. 执行以下任一操作：

   * 要删除一个或多个资产，请在浏览面板中选择资产，然后按&#x200B;**[!UICONTROL Delete]**&#x200B;或转到&#x200B;**[!UICONTROL File]** > **[!UICONTROL Delete]**。
   * 要删除文件夹，请在资产库中选择该文件夹，然后选择&#x200B;**[!UICONTROL 删除文件夹]**。

      删除文件夹会删除文件夹、文件夹中的所有资产及其子文件夹中的所有资产。

>[!NOTE]
>
>AdobeDynamic Media Classic建议覆盖资产文件，而不是删除它们，前提是您删除资产文件的原因是要用同名的资产文件替换它。

## 使用文本文件删除多个资源 {#delete-multiple-assets-with-a-text-file}

要在整个资产库中同时删除多个资产，您可以在文本文件中列出要删除的资产，并提交该列表以AdobeDynamic Media Classic。

创建AdobeDynamic Media Classic ID列表，并将其另存为文本(.txt)文件。 每个AdobeDynamic Media Classic ID必须位于其自己的行上（后跟硬返回）。

在创建列表之后，请执行以下步骤，以使用列表来删除资源：

1. 转到&#x200B;**[!UICONTROL 文件]** > **[!UICONTROL 删除资产列表]**。
1. 在删除资产列表对话框中，浏览或键入包含要删除的资产列表的文本文件路径。
1. 选择&#x200B;**[!UICONTROL Delete]**。

在删除包含文本文件的Adobe时，如果列表上没有任何资产Dynamic Media Classic ID，则会显示消息“无法在列表中验证这些条目：”以及条目列表。 但是，AdobeDynamic Media Classic不会在“作业”页面上生成错误。

>[!MORELIKETHIS]
>
>* [在浏览面板中选择资产](selecting-assets-browse-panel.md#selecting_assets_in_the_browse_panel)
>* [准备要上传的资产和文件夹](uploading-files.md#preparing_your_assets_and_folders_for_uploading)
>* [从垃圾桶文件夹恢复资产](trash-folder.md#restoring_assets_from_the_trash_folder)

