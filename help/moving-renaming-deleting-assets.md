---
title: 移动、重命名和删除资源
description: 了解如何移动、重命名和删除资产。
uuid: deff6521-0ad0-4db9-b4e0-e3211ff97740
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: 1c9e29f0-3083-4d22-a439-2a01faf59683
feature: Dynamic Media Classic,Asset Management
role: Business Practitioner
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '574'
ht-degree: 65%

---


# 移动、重命名和删除资源{#moving-renaming-and-deleting-assets}

可在浏览面板中移动、重命名和删除资源。也可以使用文本文件同时删除许多资源。

## 移动资源 {#move-assets}

可在浏览面板中将资源移至不同文件夹。

1. 在浏览面板中选择一个或多个资源，然后执行以下任一操作：

   * 在资源库中显示要将资源移至的文件夹，然后将资源拖到此文件夹。
   * 选择“文件”>“移动”，在“移动资源”窗口中选择一个文件夹，然后选择“移动”。

## 重命名资源 {#rename-assets}

要重命名资源：

1. 在浏览面板中选择资源，然后执行以下任一操作：

   * 选择名称，键入新名称，然后按下 Enter 或单击名称以外的区域。
   * 选择“文件”>“重命名”。资源的名称被高亮显示。输入一个新名称并按 Enter。

请确保不要输入现有Dynamic Media经典资产的名称。

## 删除资源 {#delete-assets}

可以删除浏览面板中的选定资源，也可以删除整个文件夹。删除的资源和文件夹将移至回收站文件夹，在其中保留七天，之后将被永久删除。

在删除资源时，由此资源派生出的所有资源也会随之删除。例如，删除已为其创建了缩放目标的图像时，缩放目标也会随图像一起删除。

>[!NOTE]
>
>在删除资源时，由资源派生出的缩放目标、图像属性以及历史记录条目会随之永久删除。它们不会随资源一起移至垃圾桶文件夹；因此无法从垃圾桶恢复它们。

1. 执行以下任一操作：

   * 要删除一个或多个资源，请在浏览面板中选择资源，然后按“删除”或选择“文件”>“删除”。
   * 要删除文件夹，请在“资源库”中选择该文件夹，然后单击&#x200B;**删除文件夹**。

      删除文件夹时会删除文件夹、文件夹中的所有资源，以及其子文件夹中的所有资源。

>[!NOTE]
>
>Dynamic Media Classic建议，如果删除资产文件的原因是要用同名的其他文件替换它，则应覆盖资产文件，而不是删除它们。

## 使用文本文件删除多个资源 {#delete-multiple-assets-with-a-text-file}

要在整个资源库中同时删除多个资源，您可以在文本文件中列表要删除的资源，然后将列表提交到Dynamic Media Classic。

创建Dynamic Media Classic ID的列表，并将其另存为文本(.txt)文件。 每个Dynamic Media Classic ID都必须在其自己的行上（后跟硬返回）。

在创建列表之后，请执行以下步骤，以使用列表来删除资源：

1. 选择“文件”>“删除资源列表”。
1. 在“删除资源列表”对话框中，浏览或键入包含要删除的资源列表的文本文件路径。
1. 单击“删除”按钮。

当您使用文本文件删除资产时，如果Dynamic Media中没有任何Dynamic Media经典ID，则会显示一条消息，告知您列表经典“无法在您的列表中验证这些条目：”以及条目的列表。 但是，Dynamic Media Classic不会在“作业”屏幕上生成错误。

>[!MORELIKETHIS]
>
>* [在浏览面板中选择资源](selecting-assets-browse-panel.md#selecting_assets_in_the_browse_panel)
>* [准备将上载的资源和文件夹](uploading-files.md#preparing_your_assets_and_folders_for_uploading)
>* [从垃圾桶文件夹恢复资源](trash-folder.md#restoring_assets_from_the_trash_folder)

