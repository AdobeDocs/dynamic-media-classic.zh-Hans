---
title: 创建混合媒体集
description: 了解如何在Dynamic Media Classic中创建混合媒体集Adobe。
uuid: a0c6e5fa-7a85-4376-b9a3-b72ae63d3d95
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 0ff9e763-897c-4ba5-b606-a95d5e45f35e
feature: Dynamic Media Classic,Viewers,Mixed Media Sets
role: User
exl-id: 18669c65-a1c4-4012-8587-cd5095f4bd4e
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 77%

---

# 创建混合媒体集{#creating-a-mixed-media-set}

如果要将多种类型的查看器合并到一个演示文稿中，需要创建混合媒体集。请确保文件、图像集、样本集以及旋转集已准备就绪可以发布，然后再将这些内容添加到混合媒体集中。

![混合媒体集](/help/assets/mm_mixed_media_set.png)

## 创建混合媒体集 {#create-a-mixed-media-set}

在创建集时，“**保存后发布**”选项按以下方式影响集和集成员：

| 是否在保存之前选择了“保存后发布”选项？ | 保存后的集状态 | 保存后的集成员状态 |
| --- | --- | --- |
| 是 | 已发布 | 已发布 |
| 否 | 未发布 | 集成员保持其已发布或未发布状态。 |

另请参阅[手动发布资源](publishing-files.md#manually_publishing_assets)和[手动取消发布资源](publishing-files.md#manually_unpublishing_assets)。

**创建混合媒体集:**

1. 转到&#x200B;**[!UICONTROL Build]** > **[!UICONTROL 混合媒体集]**。
1. 将视频、图像集、旋转集以及样本从“资源库”拖动到“混合媒体集”屏幕。

   >[!NOTE]
   >
   >混合媒体集不支持文件名包含以下任何字符的资产：`( ) { }`。

1. 执行以下任一操作：

   * 要添加音轨，将音频文件从“资源库”拖动到“音轨”框中。音轨在显示图像时播放，在播放视频时停止。
   * 要更改这些集合的顺序，在“混合媒体集”屏幕上将它们拖动到新位置。在该屏幕上这些集合的顺序决定了用户在“混合媒体集查看器”中从左到右看到这些集合的顺序。
   * （可选）要在查看器中添加代表某个视频的自定义缩略图，请将图像文件从“资源库”拖动到“缩略图”占位符框。

1. 确保在页面右下角附近选择了“**[!UICONTROL 保存后发布]**”（默认）。
1. 选择&#x200B;**[!UICONTROL Save]**。
1. 选择用于存储混合媒体集的文件夹，然后输入该集的名称。
1. 选择&#x200B;**[!UICONTROL Save]**。

   要查看图像集组合查看器中的图像集外观，请选择&#x200B;**[!UICONTROL 预览]**。

## 编辑混合媒体集 {#edit-a-mixed-media-set}

可以编辑混合媒体集。如果要在混合媒体集内编辑某个集合，单独打开该集合进行编辑，然后保存。编辑结果显示在混合媒体集中。

无论您是编辑已发布的集还是未发布的集，**[!UICONTROL 保存后发布]**&#x200B;选项都会通过以下方式影响集和集成员：

| 是否已发布集？ | **[!UICONTROL 在保存您]** 的编辑之前选择保存选项后发布？ | 保存后的集状态 | 保存后的集成员状态 |
| --- |--- |--- |--- |
| 是 | 是 | 已发布 | 已发布 |
| 是 | 否 | 已发布 | 现有的集成员保持其已发布状态。在编辑期间添加的任何新的集成员保持其已发布或未发布状态。 |
| 否 | 是 | 已发布 | 已发布 |
| 否 | 否 | 未发布 | 现有的集成员以及在编辑期间添加的任何新的集成员保持其已发布或未发布状态。 |

另请参阅[手动发布资源](publishing-files.md#manually_publishing_assets)和[手动取消发布资源](publishing-files.md#manually_unpublishing_assets)。

**编辑混合媒体集:**

1. 选择混合媒体集的滚动更新&#x200B;**[!UICONTROL 编辑]**&#x200B;按钮。
1. 执行任何以下操作：

   * 要删除项目，请选择它们，然后选择&#x200B;**[!UICONTROL 删除]**。
   * 要重新对项目进行排序，请将项目拖到新位置。

1. 在编辑完集后，确保在页面右下角附近选择了“**[!UICONTROL 保存后发布]**”（默认）。
1. 选择&#x200B;**[!UICONTROL Save]**&#x200B;或&#x200B;**[!UICONTROL Save As]**。

## 删除混合媒体集 {#deleting-a-mixed-media-set}

在删除集时，集本身将移到垃圾桶中。不过，集中的成员（或“子项”）不受影响；它们分别保持现有的已发布或未发布状态。

另请参阅[手动发布资源](publishing-files.md#manually_publishing_assets)和[手动取消发布资源](publishing-files.md#manually_unpublishing_assets)。

**删除混合媒体集:**

1. 在网格视图、列表视图或详细信息视图中，选择一个或多个混合媒体集。
1. 在全局导航栏上，转到&#x200B;**[!UICONTROL 文件]** > **[!UICONTROL 删除]** > **[!UICONTROL 删除]**。
