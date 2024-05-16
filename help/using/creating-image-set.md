---
title: 创建图像集
description: 了解如何在Adobe Dynamic Media Classic中创建图像集。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sets
feature: Dynamic Media Classic,Viewers,Image Sets,Spin Sets
role: User
exl-id: c18bb98c-b087-45d0-a4c9-44f58a3b514f
topic: Content Management
level: Intermediate
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '676'
ht-degree: 38%

---

# 创建图像集{#creating-an-image-set}

要创建多视图图像集，您需要从不同视角显示物品或显示同一物品不同侧面的图像。这是为了向观看者展示物品的图像，使其对物品的外观或功能有充分的认识。

## 创建图像集 {#create}

创建集合时， **[!UICONTROL 保存后发布]** 选项会以下列方式影响集和集成员：

| **[!UICONTROL `Publish after a save`]** 是否保存前已选择选项？ | 保存后的集状态 | 保存后的集成员状态 |
| --- | --- | --- |
| 是 | 已发布 | 已发布 |
| 否 | 未发布 | 集成员保持其已发布或未发布状态。 |

另请参阅[手动发布资源](publishing-files.md#manually_publishing_assets)和[手动取消发布资源](publishing-files.md#manually_unpublishing_assets)。

在创建图像集时，Adobe建议以下最佳实践并强制实施以下限制：

| 限制类型 | 最佳实践 | 施加的限制 |
| --- | --- | --- |
| 每集的重复资产数 | 无重复项 | 20‡ |
| 每组的最大图像数 | 每组5至10个图像 | 1000 |

‡最佳做法是不要在一个集中拥有重复的资产。 单个资产的限制为20个重复项。 如果在集中为该资源添加另一个重复项，则请求会给出错误或忽略该重复项。

另请参阅 [Dynamic Media限制](/help/using/limitations.md).

**创建图像集：**

1. 执行以下任一操作：

   * **首先选择图像**：在“浏览”面板中，选择所需的图像集图像，转到 **[!UICONTROL 生成]** > **[!UICONTROL 图像集]**.

   * **从“图像集”屏幕开始**：转到 **[!UICONTROL 生成]** > **[!UICONTROL 图像集]**. “图像集”屏幕随即打开。在资源库中选择一个文件夹，然后将要用于图像集的图像拖到“图像集”屏幕中。

1. 要更改图像顺序，将图像拖到新位置即可。
1. 在页面的右下角附近，确保 **[!UICONTROL 保存后发布]** 处于选中状态（默认）。
1. 选择 **[!UICONTROL 保存]**，选择要存储图像集的文件夹，输入图像集的名称，然后选择 **[!UICONTROL 保存]**.
1. 要在图像集查看器中查看图像集，请选择 **[!UICONTROL 预览]** 在“Image Set（图像集）”屏幕上。 您可以在图像集查看器中选择样本缩略图以查看它们的行为。

## 编辑图像集 {#editing-an-image-set}

无论是编辑已发布集还是未发布集，您都可以使用 **[!UICONTROL 保存后发布]** 选项会以下列方式影响集和集成员：

| 是否已发布集？ | **[!UICONTROL `Publish after a save`]** 在保存编辑之前是否选择了选项？ | 保存后的集状态 | 保存后的集成员状态 |
| --- | --- | --- | --- |
| 是 | 是 | 已发布 | 已发布 |
| 是 | 否 | 已发布 | 现有集成员将保留其已发布状态。 在编辑期间添加的任何新的集成员保持其已发布或未发布状态。 |
| 否 | 是 | 已发布 | 已发布 |
| 否 | 否 | 未发布 | 现有的集成员以及在编辑期间添加的任何新的集成员保持其已发布或未发布状态。 |

另请参阅[手动发布资源](publishing-files.md#manually_publishing_assets)和[手动取消发布资源](publishing-files.md#manually_unpublishing_assets)。

**要编辑图像集：**

1. 在“网格视图”中，浏览到图像集，然后在图像下方选择 **[!UICONTROL 编辑]**.
1. 执行任何以下操作：

   * 要添加图像（已发布或已取消发布），请将其从添加资产中的文件夹拖动到图像集的 **[!UICONTROL 视图]** 页面。
   * 要删除图像，请选择该图像，然后选择 **[!UICONTROL 删除]** 工具栏上。
   * 要将图像重新排序，请将图像拖到新位置。

1. 编辑完页面右下角附近的集后，请确保 **[!UICONTROL 保存后发布]** 处于选中状态（默认）。
1. 选择 **[!UICONTROL 保存]**，为您的集选择存储文件夹，输入集的名称，然后选择 **[!UICONTROL 保存]**.

## 删除图像集

在删除集时，集本身将移到垃圾桶中。但是，该集中的成员（或“子项”）不受影响；相反，它们各自保留其现有的已发布或未发布状态。

另请参阅[手动发布资源](publishing-files.md#manually_publishing_assets)和[手动取消发布资源](publishing-files.md#manually_unpublishing_assets)。

**要删除图像集，请执行以下操作：**

1. 在“网格视图”、“列表视图”或“详细信息视图”中，选择一个或多个图像集。
1. 在全局导航栏上，转到 **[!UICONTROL 文件]** > **[!UICONTROL 删除]** > **[!UICONTROL 删除]**.
