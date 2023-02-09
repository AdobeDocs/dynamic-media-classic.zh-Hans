---
title: 移动、重命名和删除资产
description: 了解如何在Adobe Dynamic Media Classic中移动、重命名和删除资产。
uuid: deff6521-0ad0-4db9-b4e0-e3211ff97740
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: 1c9e29f0-3083-4d22-a439-2a01faf59683
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 391eb7ce-ed89-47a8-a6c6-5adb3e95bf78
source-git-commit: 13d9199e0613c7b1eb664ffee859a79dd3f9faca
workflow-type: tm+mt
source-wordcount: '618'
ht-degree: 0%

---

# 移动、重命名和删除资产{#moving-renaming-and-deleting-assets}

可在浏览面板中移动、重命名和删除资源。也可以使用文本文件同时删除许多资源。

## 移动资源 {#move-assets}

可在浏览面板中将资源移至不同文件夹。

**要移动资产，请执行以下操作：**

1. 在浏览面板中选择一个或多个资源，然后执行以下任一操作：

   * 在资产库中显示要将资产移动到的文件夹，然后将资产拖到该文件夹中。
   * 转到 **[!UICONTROL 文件]** > **[!UICONTROL 移动]**，在移动资产窗口中选择一个文件夹，然后选择 **[!UICONTROL 移动]**.

## 重命名资源 {#rename-assets}

1. 在浏览面板中选择资产，然后执行下列操作之一：

   * 选择名称，键入新名称，然后按 **[!UICONTROL 输入]** 或从名称中选择。
   * 转到 **[!UICONTROL 文件]** > **[!UICONTROL 重命名]**. 资源的名称被高亮显示。输入新名称并按 **[!UICONTROL 输入]**. 请确保未输入现有Adobe Dynamic Media Classic资产的名称。

## 删除资源 {#delete-assets}

您可以在浏览面板中删除选定资产，并删除整个文件夹。 删除的资源和文件夹将移至回收站文件夹，在其中保留七天，之后将被永久删除。

在删除资源时，由此资源派生出的所有资源也会随之删除。例如，删除已为其创建了缩放目标的图像时，缩放目标也会随图像一起删除。

在删除资源时，由资源派生出的缩放目标、图像属性以及历史记录条目会随之永久删除。它们不会随资源一起移至垃圾桶文件夹；因此无法从垃圾桶恢复它们。

>[!IMPORTANT]
>
>批量删除是一项密集操作。 请确保按顺序执行批量删除操作，而不是作为并发的大量删除操作。 Adobe建议您将删除操作限制为每小时删除资产的次数不超过5000次。 超过每小时5000的数字可能导致速率限制。

**要删除资产，请执行以下操作：**

1. 执行任何以下操作：

   * 要删除一个或多个资产，请在“浏览”面板中选择资产，然后按 **[!UICONTROL 删除]** 或转到 **[!UICONTROL 文件]** > **[!UICONTROL 删除]**.
   * 要删除文件夹，请在资产库中选择该文件夹，然后选择 **[!UICONTROL 删除文件夹]**.

      删除文件夹会删除文件夹、文件夹中的所有资产及其子文件夹中的所有资产。

如果您删除资产文件的原因是使用同名的其他资产文件替换它，则Adobe Dynamic Media Classic建议覆盖资产文件，而不是删除它们。

## 使用文本文件删除多个资源 {#delete-multiple-assets-with-a-text-file}

要在整个资产库中同时删除多个资产，您可以在文本文件中列出要删除的资产，然后将该列表提交到Adobe Dynamic Media Classic。

创建Adobe Dynamic Media Classic ID列表，并将其另存为文本(.txt)文件。 每个Adobe Dynamic Media Classic ID必须位于其自己的行上（后跟硬返回）。

在创建列表之后，请执行以下步骤，以使用列表来删除资源：

1. 转到 **[!UICONTROL 文件]** > **[!UICONTROL 删除资产列表]**.
1. 在删除资产列表对话框中，浏览或键入包含要删除的资产列表的文本文件路径。
1. 选择 **[!UICONTROL 删除]**.

当您使用文本文件删除资产时，如果列表上没有任何Adobe Dynamic Media Classic ID，则会显示消息“无法在您的列表中验证这些条目：”。 此时还会显示条目列表。 但是，Adobe Dynamic Media Classic在“作业”页面上不生成错误。

>[!MORELIKETHIS]
>
>* [在浏览面板中选择资产](selecting-assets-browse-panel.md#selecting_assets_in_the_browse_panel)
>* [准备要上传的资产和文件夹](uploading-files.md#preparing_your_assets_and_folders_for_uploading)
>* [从垃圾桶文件夹恢复资产](trash-folder.md#restoring_assets_from_the_trash_folder)

