---
title: 创建样本集
description: 了解如何在AdobeDynamic Media Classic中创建色板集。
uuid: 250b3525-310d-4481-b0bc-f9057e823e0b
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/swatch_sets
discoiquuid: 631d2b2d-9e69-4b96-8392-17e00a1a8de0
feature: Dynamic Media Classic,Viewers
role: User
exl-id: 426b6e6b-daed-4ca6-b095-99bb06604b07
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '708'
ht-degree: 61%

---

# 创建样本集{#creating-a-swatch-set}

样本集允许用户以不同颜色、模式或光泽度查看项目。要使用颜色样本创建样本集，需要具有要提供给用户的每种不同颜色、模式或光泽度的一个图像。还需要每种颜色、模式或光泽度的一种颜色、模式或光泽度样本。

例如，假定要使用不同颜色的标记显示大写字母的图像，标记为红色、绿色和蓝色。在这种情况下，需要同一大写字母的三种快照。一个红色标记快照，一个绿色标记快照，以及一个蓝色标记快照。还需要红色、绿色和蓝色样本。颜色色板用作用户在色板集查看器中选择的缩略图，以查看红色、绿色或蓝色的帽子。

## 创建样本集 {#create}

创建集时，**保存后发布**选项会通过以下方式影响集和设置成员：
| **[!UICONTROL 在保存前选择保存后发布]**选项？ |保存后设置的状态 |保存后集成员的状态 |
| — | — | — |
|是 |已发布 |已发布 |
|否 |未发布 |设置成员将保留其已发布或未发布状态。 |

另请参阅[手动发布资源](publishing-files.md#manually_publishing_assets)和[手动取消发布资源](publishing-files.md#manually_unpublishing_assets)。

**创建样本集:**

1. 执行以下任一操作：

   * **首先选择图像**  — 在“浏览”面板中，选择图像，然后转到 **[!UICONTROL 生成]**  >  **[!UICONTROL 色板集]**。

   * **从“色板集”屏幕开始**  — 转到“ **[!UICONTROL 生成]** ”>“ **[!UICONTROL 色板集]**”。从资源库中选择一个文件夹，然后将图像拖到“样本集”页面的“视图”部分中。

1. 将样本颜色、模式或光泽度拖到“样本集”页面上的样本占位符框中。

   确保拖到每个占位符里的颜色、模式或光泽度样本表示相邻图像的颜色、模式或光泽度。

1. 要更改样本集中图像的顺序，请将图像拖到新位置。
1. 确保在页面右下角附近选择了“**[!UICONTROL 保存后发布]**”（默认）。
1. 选择&#x200B;**[!UICONTROL Save]**，选择用于存储色板样本集的文件夹，输入色板集的名称，然后选择&#x200B;**[!UICONTROL Submit]**。
1. 要在样本集查看器中查看样本集，请在“样本集”屏幕上选择&#x200B;**[!UICONTROL 预览]**。 您可以在样本集查看器中选择样本缩略图，以查看其行为方式。

## 编辑样本集 {#editing-a-swatch-set}

无论您是编辑已发布的集还是未发布的集，**[!UICONTROL 保存后发布]**&#x200B;选项都会通过以下方式影响集和集成员：

| 是否已发布集？ | **[!UICONTROL 在保]** 存编辑之前选择保存后发布选项？ | 保存后的集状态 | 保存后的集成员状态 |
|--- |--- |--- |--- |
| 是 | 是 | 已发布 | 已发布 |
| 是 | 否 | 已发布 | 现有的集成员保持其已发布状态。在编辑期间添加的任何新的集成员保持其已发布或未发布状态。 |
| 否 | 是 | 已发布 | 已发布 |
| 否 | 否 | 未发布 | 现有的集成员以及在编辑期间添加的任何新的集成员保持其已发布或未发布状态。 |

另请参阅[手动发布资源](publishing-files.md#manually_publishing_assets)和[手动取消发布资源](publishing-files.md#manually_unpublishing_assets)。

**编辑样本集:**

1. 在“网格视图”中，浏览到一个色板集，然后在图像下方选择&#x200B;**[!UICONTROL 编辑]**。
1. 执行任何以下操作：

   * 要添加图像（已发布或未发布），请在“添加资源”中将其从文件夹拖到样本集的“**[!UICONTROL 视图]**”页面上。
   * 要删除图像，请选择它，然后选择工具栏上的&#x200B;**[!UICONTROL 删除]**。
   * 要将图像重新排序，请将图像拖到新位置。

1. 在编辑完集后，确保在页面右下角附近选择了“**[!UICONTROL 保存后发布]**”（默认）。
1. 选择&#x200B;**[!UICONTROL Save]**，选择存储文件夹，输入集的名称，然后选择&#x200B;**[!UICONTROL Save]**。

## 删除色板集 {#deleting-a-swatch-set}

在删除集时，集本身将移到垃圾桶中。不过，集中的成员（或“子项”）不受影响；它们分别保持现有的已发布或未发布状态。

另请参阅[手动发布资源](publishing-files.md#manually_publishing_assets)和[手动取消发布资源](publishing-files.md#manually_unpublishing_assets)。

**删除样本集:**

1. 在“网格视图”、“列表视图”或“详细信息视图”中，选择一个或多个样本集。
1. 在全局导航栏上，转到&#x200B;**[!UICONTROL 文件]** > **[!UICONTROL 删除]** > **[!UICONTROL 删除]**。
