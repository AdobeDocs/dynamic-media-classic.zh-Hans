---
title: 创建样本集
description: 了解如何在Adobe Dynamic Media Classic中创建样本集。
uuid: 250b3525-310d-4481-b0bc-f9057e823e0b
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/swatch_sets
discoiquuid: 631d2b2d-9e69-4b96-8392-17e00a1a8de0
feature: Dynamic Media Classic,Viewers
role: User
exl-id: 426b6e6b-daed-4ca6-b095-99bb06604b07
topic: Content Management
level: Intermediate
source-git-commit: a9bd472705bce32f63a5710c3266e51256d17a00
workflow-type: tm+mt
source-wordcount: '708'
ht-degree: 58%

---

# 创建样本集{#creating-a-swatch-set}

样本集允许用户以不同颜色、模式或光泽度查看项目。要使用颜色样本创建样本集，需要具有要提供给用户的每种不同颜色、模式或光泽度的一个图像。还需要每种颜色、模式或光泽度的一种颜色、模式或光泽度样本。

例如，假定要使用不同颜色的标记显示大写字母的图像，标记为红色、绿色和蓝色。在这种情况下，需要同一大写字母的三种快照。一个红色标记快照，一个绿色标记快照，以及一个蓝色标记快照。还需要红色、绿色和蓝色样本。颜色样本用作用户在样本集查看器中选择的缩略图，以查看红色计费、绿色计费或蓝色计费次数上限。

## 创建样本集 {#create}

在创建集时，“**保存后发布**”选项按以下方式影响集和集成员：

| **[!UICONTROL 保存后发布]** 是否保存前已选择选项？ | 保存后的集状态 | 保存后的集成员状态 |
| --- | --- | --- |
| 是 | 已发布 | 已发布 |
| 否 | 未发布 | 集成员保持其已发布或未发布状态。 |

另请参阅[手动发布资源](publishing-files.md#manually_publishing_assets)和[手动取消发布资源](publishing-files.md#manually_unpublishing_assets)。

**要创建样本集，请执行以下操作：**

1. 执行以下任一操作：

   * **首先选择图像**  — 在浏览面板中，选择图像，然后转到 **[!UICONTROL 生成]** > **[!UICONTROL 样本集]**.

   * **从“样本集”屏幕开始**  — 转到 **[!UICONTROL 生成]** > **[!UICONTROL 样本集]**. 从资源库中选择一个文件夹，然后将图像拖到“样本集”页面的“视图”部分中。

1. 将样本颜色、模式或光泽度拖到“样本集”页面上的样本占位符框中。

   确保拖到每个占位符里的颜色、模式或光泽度样本表示相邻图像的颜色、模式或光泽度。

1. 要更改样本集中图像的顺序，请将图像拖到新位置。
1. 确保在页面右下角附近选择了“**[!UICONTROL 保存后发布]**”（默认）。
1. 选择 **[!UICONTROL 保存]**，选择要存储色板集的文件夹，输入色板集的名称，然后选择 **[!UICONTROL 提交]**.
1. 要在样本集查看器中查看您的样本集，请选择 **[!UICONTROL 预览]** 在“样本集”屏幕上。 您可以在样本集查看器中选择样本缩略图以查看其行为。

## 编辑样本集 {#editing-a-swatch-set}

无论是编辑已发布集还是未发布集，您都可以使用 **[!UICONTROL 保存后发布]** 选项会以下列方式影响集和集成员：

| 是否已发布集？ | **[!UICONTROL 发布晚于]** 是否保存您在保存编辑之前选择的选项？ | 保存后的集状态 | 保存后的集成员状态 |
|--- | --- | --- | --- |
| 是 | 是 | 已发布 | 已发布。 |
| 是 | 否 | 已发布 | 现有集成员将保留其已发布状态。 在编辑期间添加的任何新的集成员保持其已发布或未发布状态。 |
| 否 | 是 | 已发布 | 已发布。 |
| 否 | 否 | 未发布 | 现有的集成员以及在编辑期间添加的任何新的集成员保持其已发布或未发布状态。 |

另请参阅[手动发布资源](publishing-files.md#manually_publishing_assets)和[手动取消发布资源](publishing-files.md#manually_unpublishing_assets)。

**要编辑样本集：**

1. 在“网格视图”中，浏览到样本集，然后在图像下方选择 **[!UICONTROL 编辑]**.
1. 执行任何以下操作：

   * 要添加图像（已发布或已取消发布），请将其从添加资产中的文件夹拖动到样本集的 **[!UICONTROL 视图]** 页面。
   * 要删除图像，请选择该图像，然后选择 **[!UICONTROL 删除]** 工具栏上。
   * 要将图像重新排序，请将图像拖到新位置。

1. 在编辑完集后，确保在页面右下角附近选择了“**[!UICONTROL 保存后发布]**”（默认）。
1. 选择 **[!UICONTROL 保存]**，选择一个存储文件夹，输入集的名称，然后选择 **[!UICONTROL 保存]**.

## 删除样本集 {#deleting-a-swatch-set}

在删除集时，集本身将移到垃圾桶中。但是，该集中的成员（或“子项”）不受影响；相反，它们各自保留其现有的已发布或未发布状态。

另请参阅[手动发布资源](publishing-files.md#manually_publishing_assets)和[手动取消发布资源](publishing-files.md#manually_unpublishing_assets)。

**要删除样本集，请执行以下操作：**

1. 在“网格视图”、“列表视图”或“详细信息视图”中，选择一个或多个“样本集”。
1. 在全局导航栏上，转到 **[!UICONTROL 文件]** > **[!UICONTROL 删除]** > **[!UICONTROL 删除]**.
