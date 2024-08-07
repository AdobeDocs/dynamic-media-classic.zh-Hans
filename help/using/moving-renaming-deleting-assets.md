---
title: 移动、重命名和删除资源
description: 了解如何在Adobe Dynamic Media Classic中移动、重命名和删除资源。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 391eb7ce-ed89-47a8-a6c6-5adb3e95bf78
topic: Content Management
level: Intermediate
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '617'
ht-degree: 17%

---

# 移动、重命名和删除资源{#moving-renaming-and-deleting-assets}

您可以从“浏览”面板移动、重命名和删除资源。 也可以使用文本文件同时删除许多资源。

## 移动资源 {#move-assets}

您可以在“浏览”面板中将资产移动到不同的文件夹。

**要移动资产：**

1. 在“浏览”面板中选择一个或多个资源，然后执行以下操作之一：

   * 在资产库中显示要将资产移动到的文件夹，然后将资产拖到该文件夹。
   * 转到&#x200B;**[!UICONTROL 文件]** > **[!UICONTROL 移动]**，在“移动Assets”窗口中选择一个文件夹，然后选择&#x200B;**[!UICONTROL 移动]**。

## 重命名资源 {#rename-assets}

1. 在“浏览”面板中选择资产，然后执行以下操作之一：

   * 选择名称，键入新名称，然后按&#x200B;**[!UICONTROL Enter]**&#x200B;或选择退出名称。
   * 转到&#x200B;**[!UICONTROL 文件]** > **[!UICONTROL 重命名]**。 资源的名称被高亮显示。输入新名称，然后按&#x200B;**[!UICONTROL Enter]**。 确保不输入现有Adobe Dynamic Media Classic资源的名称。

## 删除资源 {#delete-assets}

您可以在“浏览”面板中删除所选资源并删除整个文件夹。 删除的资源和文件夹将移至回收站文件夹，在其中保留七天，之后将被永久删除。

当您删除某个资源时，源自该资源的所有资源也会被删除。 例如，删除已为其创建缩放目标的图像会同时删除缩放目标和图像。

在删除资源时，由资源派生出的缩放目标、图像属性以及历史记录条目会随之永久删除。它们不会随资源一起移至垃圾桶文件夹；因此无法从垃圾桶恢复它们。

>[!IMPORTANT]
>
>批量删除是一项密集的操作。 请确保按顺序运行批量删除，而不是按并发大量删除操作运行。 Adobe建议您将删除操作限制为每小时5000个或更少的资源删除。 任何大于每小时5000的数字都可能导致速率限制。

**要删除资源：**

1. 执行任何以下操作：

   * 要删除一个或多个资源，请在“浏览”面板中选择资源，然后按&#x200B;**[!UICONTROL 删除]**&#x200B;或转到&#x200B;**[!UICONTROL 文件]** > **[!UICONTROL 删除]**。
   * 要删除文件夹，请在资产库中选择该文件夹，然后选择&#x200B;**[!UICONTROL 删除文件夹]**。

     删除文件夹会删除该文件夹、该文件夹中的所有资源及其子文件夹中的所有资源。

如果您删除某个资源文件的原因是要用另一个同名资源文件替换它，则Adobe Dynamic Media Classic建议覆盖而不是删除资源文件。

## 使用文本文件删除多个资源 {#delete-multiple-assets-with-a-text-file}

要在整个资源库中同时删除许多资源，您可以在文本文件中列出要删除的资源，并将该列表提交到Adobe Dynamic Media Classic。

创建Adobe Dynamic Media Classic ID列表并将其另存为文本(.txt)文件。 每个Adobe Dynamic Media Classic ID必须位于其自身的行中（后跟一个硬返回）。

在创建列表之后，请执行以下步骤，以使用列表来删除资源：

1. 转到&#x200B;**[!UICONTROL 文件]** > **[!UICONTROL 删除资源列表]**。
1. 在&#x200B;**[!UICONTROL 已删除的资源列表]**&#x200B;对话框中，键入包含要删除的资源列表的文本文件的路径。
1. 选择&#x200B;**[!UICONTROL 删除]**。

使用文本文件删除资源时，如果列表中未列出任何Adobe Dynamic Media Classic ID，则会显示消息“无法验证列表中的这些条目：”。 还会显示条目列表。 但是，Adobe Dynamic Media Classic不会在“作业”页面上生成错误。

>[!MORELIKETHIS]
>
>* [在浏览面板中选择资源](selecting-assets-browse-panel.md#selecting_assets_in_the_browse_panel)
>* [准备要上载的资产和文件夹](uploading-files.md#preparing_your_assets_and_folders_for_uploading)
>* [从垃圾桶文件夹中还原资源](trash-folder.md#restoring_assets_from_the_trash_folder)
