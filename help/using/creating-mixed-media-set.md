---
title: 创建混合媒体集
description: 了解如何在Adobe Dynamic Media Classic中创建混合媒体集。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic,Viewers,Mixed Media Sets
role: User
exl-id: 18669c65-a1c4-4012-8587-cd5095f4bd4e
topic: Content Management
level: Intermediate
source-git-commit: b2a6aeb1aab420803a8b7dafb0fdeda495e2a69b
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 68%

---

# 创建混合媒体集{#creating-a-mixed-media-set}

如果要将多种类型的查看器合并到一个演示文稿中，需要创建混合媒体集。请确保文件、图像集、样本集以及旋转集已准备就绪可以发布，然后再将这些内容添加到混合媒体集中。

![混合媒体集](/help/using/assets/mm_mixed_media_set.png)

## 创建混合媒体集 {#create-a-mixed-media-set}

在创建集时，“**保存后发布**”选项按以下方式影响集和集成员：

| 在保存前是否选择了“保存后发布”选项？ | 保存后的集状态 | 保存后的集成员状态 |
| --- | --- | --- |
| 是 | 已发布 | 已发布 |
| 否 | 未发布 | 集成员保持其已发布或未发布状态。 |

另请参阅[手动发布资源](publishing-files.md#manually_publishing_assets)和[手动取消发布资源](publishing-files.md#manually_unpublishing_assets)。

**创建混合媒体集：**

1. 转到 **[!UICONTROL 生成]** > **[!UICONTROL 混合媒体集]**.
1. 将视频、图像集、旋转集以及样本从“资源库”拖动到“混合媒体集”屏幕。

   >[!NOTE]
   >
   >混合媒体集不支持文件名包含以下任意字符的资产： `( ) { }`.

1. 执行以下任一操作：

   * 要添加音轨，将音频文件从“资源库”拖动到“音轨”框中。音轨在显示图像时播放，在播放视频时停止。
   * 要更改这些集合的顺序，在“混合媒体集”屏幕上将它们拖动到新位置。在该屏幕上这些集合的顺序决定了用户在“混合媒体集查看器”中从左到右看到这些集合的顺序。
   * （可选）要在查看器中添加代表某个视频的自定义缩略图，请将图像文件从“资源库”拖动到“缩略图”占位符框。

1. 确保在页面右下角附近选择了“**[!UICONTROL 保存后发布]**”（默认）。
1. 选择 **[!UICONTROL 保存]**.
1. 选择用于存储混合媒体集的文件夹，然后输入该集的名称。
1. 选择 **[!UICONTROL 保存]**.

   要查看您的组合图像集在图像集查看器中是什么样的，请选择 **[!UICONTROL 预览]**.

## 编辑混合媒体集 {#edit-a-mixed-media-set}

可以编辑混合媒体集。如果要在混合媒体集内编辑某个集合，单独打开该集合进行编辑，然后保存。编辑结果显示在混合媒体集中。

无论是编辑已发布集还是未发布集，您都可以使用 **[!UICONTROL 保存后发布]** 选项会以下列方式影响集和集成员：

| 是否已发布集？ | **[!UICONTROL 保存后发布]** 在保存编辑之前是否选择了选项？ | 保存后的集状态 | 保存后的集成员状态 |
| --- |--- |--- |--- |
| 是 | 是 | 已发布 | 已发布 |
| 是 | 否 | 已发布 | 现有集成员将保留其已发布状态。 在编辑期间添加的任何新的集成员保持其已发布或未发布状态。 |
| 否 | 是 | 已发布 | 已发布 |
| 否 | 否 | 未发布 | 现有的集成员以及在编辑期间添加的任何新的集成员保持其已发布或未发布状态。 |

另请参阅[手动发布资源](publishing-files.md#manually_publishing_assets)和[手动取消发布资源](publishing-files.md#manually_unpublishing_assets)。

**要编辑混合媒体集：**

1. 选择混合媒体集的变换 **[!UICONTROL 编辑]** 按钮。
1. 执行任何以下操作：

   * 要删除项目，请选择这些项目并选择 **[!UICONTROL 删除]**.
   * 要重新对项目进行排序，请将项目拖到新位置。

1. 在编辑完集后，确保在页面右下角附近选择了“**[!UICONTROL 保存后发布]**”（默认）。
1. 选择 **[!UICONTROL 保存]** 或 **[!UICONTROL 另存为]**.

## 删除混合媒体集

在删除集时，集本身将移到垃圾桶中。但是，该集中的成员（或“子项”）不受影响；相反，它们各自保留其现有的已发布或未发布状态。

另请参阅[手动发布资源](publishing-files.md#manually_publishing_assets)和[手动取消发布资源](publishing-files.md#manually_unpublishing_assets)。

**要删除混合媒体集，请执行以下操作：**

1. 在网格视图、列表视图或详细信息视图中，选择一个或多个混合媒体集。
1. 在全局导航栏上，转到 **[!UICONTROL 文件]** > **[!UICONTROL 删除]** > **[!UICONTROL 删除]**.
