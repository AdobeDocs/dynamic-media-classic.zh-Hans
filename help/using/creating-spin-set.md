---
title: 创建旋转集
description: 了解如何在Adobe Dynamic Media Classic中创建旋转集。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/spin_sets
feature: Dynamic Media Classic,Viewers,Spin Sets
role: User
exl-id: 35e8e7fc-5b3c-441a-959c-df2e39ea0d4b
topic: Content Management
level: Intermediate
source-git-commit: b2a6aeb1aab420803a8b7dafb0fdeda495e2a69b
workflow-type: tm+mt
source-wordcount: '958'
ht-degree: 44%

---

# 创建旋转集{#creating-a-spin-set}

要创建有效的旋转集，请确保正确拍摄图像。您可以通过选择“构建”按钮并选择旋转集在Adobe Dynamic Media Classic中创建旋转集。 在“旋转集”屏幕中编辑旋转集。

>[!NOTE]
>
>Adobe Dynamic Media Classic的早期版本不提供二维旋转集。 如果在以前版本的Adobe Dynamic Media Classic中创建了旋转集，则不能在不以其他名称首先保存一维旋转集的情况下保存它。 选择 **[!UICONTROL 另存为]** 在旋转集屏幕中输入新名称，以便在Adobe Dynamic Media Classic中对其进行编辑。

## 旋转集图像拍摄指南 {#guidelines-for-shooting-spin-set-images}

通常，旋转集中拥有的图像越多，图像旋转效果就越好。 不过，在旋转集中加入许多图像会增加图像的加载时间。Adobe Dynamic Media Classic建议在拍摄要用于旋转集的图像时遵循以下准则：

* 在一维旋转集中最少使用 8 到 12 张图像，在二维旋转集中最少使用 16 到 24 张图像。
* 请使用无损格式；建议使用 TIFF 和 PNG。
* 为所有图像创建蒙版，这样物品将显示在纯白色或其他高对比度背景上。也可以添加阴影。
* 确保产品细节非常明亮，且位于焦点上。
* 借助人体模型或时装模特儿为流行服饰拍摄旋转图像。通常，人体模型会被遮蔽（使用玻璃人体模型），或者图像中显示风格化的人体模型/服装。 可通过定义角度数来创建模型上的旋转集。 使用地板上的胶带标记每个角度，以便引导模型步进，并查看每个拍摄的方向。

## 创建旋转集 {#create}

在Adobe Dynamic Media Classic中创作或创建旋转集的顺序很重要。 在将图像拖放到旋转集页面的网格中时，旋转集会按特定方向旋转，具体取决于您对资源的排序方式。 因此，资产在生成器中可视化显示的顺序是，当用户从左到右移动鼠标指针或手指时，资产是如何旋转的。

在创建集时，“**[!UICONTROL 保存后发布]**”选项按以下方式影响集和集成员：

| **[!UICONTROL 保存后发布]** 是否保存前已选择选项？ | 保存后的集状态 | 保存后的集成员状态 |
| --- | --- | --- |
| 是 | 已发布 | 已发布 |
| 否 | 未发布 | 集成员保持其已发布或未发布状态。 |

另请参阅[手动发布资源](publishing-files.md#manually-publishing-assets)和[手动取消发布资源](publishing-files.md#manually-unpublishing-assets)。

在创建旋转集时，Adobe建议采用以下最佳实践并强制实施以下限制：

| 旋转集限制类型 | 最佳实践 | 施加的限制 |
| --- | --- | --- |
| 每个2D集的最大行/列数 | 每组12-18个图像 | 1000 |

另请参阅 [Dynamic Media限制](/help/using/limitations.md).

在保存旋转集后，您可以使用“构建：旋转集”页面中的“预览”在默认查看器中查看旋转集的显示效果。

**要创建旋转集，请执行以下操作：**

1. 在 **[!UICONTROL 生成]** 下拉菜单，选择 **[!UICONTROL 旋转集]**.
1. 在“旋转集大小”对话框中，设置需要的行数和单元格数。

   要构建一维旋转集，仅选择一行。

   要构建二维旋转集，选择两行或更多行。

1. 选择 **[!UICONTROL 确定]**.
1. 将图像拖放到“旋转集”屏幕上的网格中。
1. 完成后，确保在页面右下角附近选择了“**保存后发布**”（默认）。
1. 选择 **[!UICONTROL 保存]**.
1. 在“保存”对话框中，选择一个文件夹来存储您的旋转集。在“文件名”字段中，输入旋转集名称。
1. 选择 **[!UICONTROL 保存]**.

## 编辑旋转集 {#editing-a-spin-set}

无论您编辑的是已发布的集还是未发布的集，您都可以 **[!UICONTROL 保存后发布]** 选项会以下列方式影响集和集成员：

| 是否已发布集？ | **[!UICONTROL 保存后发布]** 在保存编辑之前是否选择了选项？ | 保存后的集状态 | 保存后的集成员状态 |
| --- | --- | --- | --- |
| 是 | 是 | 已发布 | 已发布 |
| 是 | 否 | 已发布 | 现有集成员将保留其已发布状态。 在编辑期间添加的任何新的集成员保持其已发布或未发布状态。 |
| 否 | 是 | 已发布 | 已发布 |
| 否 | 否 | 未发布 | 现有的集成员以及在编辑期间添加的任何新的集成员保持其已发布或未发布状态。 |

另请参阅[手动发布资源](publishing-files.md#manually-publishing-assets)和[手动取消发布资源](publishing-files.md#manually-unpublishing-assets)。

**要编辑旋转集，请执行以下操作：**

1. 选择旋转集的变换图像 **[!UICONTROL 编辑]** 按钮。
1. 执行任何以下操作：

   * **删除图像**  — 选择图像，然后选择 **[!UICONTROL 删除]**.

   * **添加图像**  — 将图像拖动到单元格中。

   * **重新排列行（二维旋转集）**  — 选择一个行选择器框（位于行的左侧），然后选择 **[!UICONTROL 下移行]** 或 **[!UICONTROL 上移行]**.

   * **添加行和单元格**  — 在“行”框和“单元格”框中输入一个数字，以确定每行的行数和单元格数。

1. 在完成编辑后，确保在页面右下角附近选择了“**[!UICONTROL 保存后发布]**”（默认）。
1. 选择 **[!UICONTROL 保存]**，选择一个存储文件夹，输入集的名称，然后选择 **[!UICONTROL 保存]**.

## 删除旋转集

在删除集时，集本身将移到垃圾桶中。但是，该集中的成员（或“子项”）不受影响；相反，它们各自保留其现有的已发布或未发布状态。

另请参阅[手动发布资源](publishing-files.md#manually-publishing-assets)和[手动取消发布资源](publishing-files.md#manually-unpublishing-assets)。

**要删除旋转集，请执行以下操作：**

1. 在网格视图、列表视图或详细信息视图中，选择一个或多个旋转集。
1. 在全局导航栏上，转到 **[!UICONTROL 文件]** > **[!UICONTROL 删除]** > **[!UICONTROL 删除]**.
