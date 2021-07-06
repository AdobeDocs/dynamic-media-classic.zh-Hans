---
title: 创建图像集
description: 了解如何创建图像集。
uuid: 689fdc14-4f51-4c94-8515-cd8551e101d8
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sets
discoiquuid: 3f356410-b30e-4870-ad95-6e5a9dc126c8
feature: Dynamic Media Classic，查看器，图像集
role: User
exl-id: c18bb98c-b087-45d0-a4c9-44f58a3b514f
source-git-commit: df689ff5a127bfbc400ca5331168d1ff7bb0b42e
workflow-type: tm+mt
source-wordcount: '586'
ht-degree: 86%

---

# 创建图像集{#creating-an-image-set}

要创建多视图图像集，您需要从不同视角显示物品或显示同一物品不同侧面的图像。这是为了向观看者展示物品的图像，使其对物品的外观或功能有充分的认识。

## 创建图像集 {#create}

在创建集时，“**保存后发布**”选项按以下方式影响集和集成员：

| 是否在保存之前选择了“保存后发布”选项？ | 保存后的集状态 | 保存后的集成员状态 |
|:--- |:--- |:--- |
| 是 | 已发布 | 已发布 |
| 否 | 未发布 | 集成员保持其已发布或未发布状态。 |

另请参阅[手动发布资源](publishing-files.md#manually_publishing_assets)和[手动取消发布资源](publishing-files.md#manually_unpublishing_assets)。

**创建图像集:**

1. 执行以下任一操作：

   * **首先选择图像**  — 在“浏览”面板中，选择您想要用于图像集的图像，单击 **[!UICONTROL 生成]**  >  **[!UICONTROL 图像集]**。

   * **从“图像集”屏幕开始**  — 单击 **[!UICONTROL 生成]**  >  **[!UICONTROL 图像集]**。“图像集”屏幕随即打开。在资源库中选择一个文件夹，然后将要用于图像集的图像拖到“图像集”屏幕中。

1. 要更改图像顺序，将图像拖到新位置即可。
1. 确保在页面右下角附近选择了“**[!UICONTROL 保存后发布]**”（默认）。
1. 单击“**[!UICONTROL 保存]**”，选择一个文件夹以存储图像集，输入该集的名称，然后单击“**[!UICONTROL 保存]**”。
1. 要在图像集查看器中查看图像集，请单击“图像集”屏幕上的“**[!UICONTROL 预览]**”。可以单击图像集查看器中的样本缩略图来观看它们的显示效果。

## 编辑图像集 {#editing-an-image-set}

无论您是编辑已发布的集还是未发布的集，**[!UICONTROL 保存后发布]**&#x200B;选项都会通过以下方式影响集和集成员：

| 是否已发布集？ | **[!UICONTROL 在保存您]** 的编辑之前选择保存选项后发布？ | 保存后的集状态 | 保存后的集成员状态 |
|--- |--- |--- |--- |
| 是 | 是 | 已发布 | 已发布 |
| 是 | 否 | 已发布 | 现有的集成员保持其已发布状态。在编辑期间添加的任何新的集成员保持其已发布或未发布状态。 |
| 否 | 是 | 已发布 | 已发布 |
| 否 | 否 | 未发布 | 现有的集成员以及在编辑期间添加的任何新的集成员保持其已发布或未发布状态。 |

另请参阅[手动发布资源](publishing-files.md#manually_publishing_assets)和[手动取消发布资源](publishing-files.md#manually_unpublishing_assets)。

**编辑图像集:**

1. 在网格视图中，浏览到一个图像集，然后单击图像下面的“**[!UICONTROL 编辑]**”。
1. 执行任何以下操作：

   * 要添加图像（已发布或未发布），请在“添加资源”中将其从文件夹拖到图像集的“**[!UICONTROL 视图]**”页面上。
   * 要删除图像，请选择该图像，然后单击工具栏上的“**[!UICONTROL 删除]**”。
   * 要将图像重新排序，请将图像拖到新位置。

1. 在编辑完集后，确保在页面右下角附近选择了“**[!UICONTROL 保存后发布]**”（默认）。
1. 单击“**[!UICONTROL 保存]**”，选择一个文件夹以存储集，输入该集的名称，然后单击“**[!UICONTROL 保存]**”。

## 删除图像集 {#deleting-an-image-set}

在删除集时，集本身将移到垃圾桶中。不过，集中的成员（或“子项”）不受影响；它们分别保持现有的已发布或未发布状态。

另请参阅[手动发布资源](publishing-files.md#manually_publishing_assets)和[手动取消发布资源](publishing-files.md#manually_unpublishing_assets)。

**删除图像集:**

1. 在网格视图、列表视图或详细信息视图中，选择一个或多个图像集。
1. 在全局导航栏上，单击“**[!UICONTROL 文件]**”>“**[!UICONTROL 删除]**”>“**[!UICONTROL 删除]**”。
