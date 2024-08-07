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
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '963'
ht-degree: 32%

---

# 创建旋转集{#creating-a-spin-set}

要创建有效的旋转集，请确保正确拍摄图像。您可以通过选择“构建”按钮并选择旋转集在Adobe Dynamic Media Classic中创建旋转集。 在“旋转集”屏幕中编辑旋转集。

>[!NOTE]
>
>Adobe Dynamic Media Classic的早期版本不提供二维旋转集。 如果在以前版本的Adobe Dynamic Media Classic中创建了旋转集，请用其他名称保存它，然后可以保存一维旋转集。 在“旋转集”屏幕中选择&#x200B;**[!UICONTROL 另存为]**&#x200B;并输入新名称，以便在Adobe Dynamic Media Classic中对其进行编辑。

## 旋转集图像拍摄指南 {#guidelines-for-shooting-spin-set-images}

通常，旋转集中拥有的图像越多，图像旋转效果就越好。 不过，在旋转集中加入许多图像会增加图像的加载时间。Adobe Dynamic Media Classic建议在拍摄要用于旋转集的图像时遵循以下准则：

* 至少，在一维旋转集中使用8-12个图像，在二维旋转集中使用16-24个图像。
* 请使用无损格式；建议使用 TIFF 和 PNG。
* 为所有图像创建蒙版，这样物品将显示在纯白色或其他高对比度背景上。也可以添加阴影。
* 确保产品细节非常明亮，且位于焦点上。
* 借助人体模型或时装模特儿为流行服饰拍摄旋转图像。通常，人体模型会被遮蔽（使用玻璃人体模型），或者图像中显示风格化的人体模型/服装。 通过定义角度数，可在模型旋转集上创建。 使用地板上的胶带标记每个角度，以便引导模型步进，并查看每个拍摄的方向。

## 创建旋转集 {#create}

在Adobe Dynamic Media Classic中创作或创建旋转集的顺序很重要。 在将图像拖放到旋转集页面的网格中时，旋转集会按特定方向旋转，具体取决于您对资源的排序方式。 因此，资产在生成器中可视化显示的顺序是，当用户从左到右移动鼠标指针或手指时，资产是如何旋转的。

创建集时，**[!UICONTROL 保存]**&#x200B;后的Publish选项会以下列方式影响该集和设置成员：

| 保存前是否选择了保存后的&#x200B;**[!UICONTROL Publish]**&#x200B;选项？ | 保存后的集状态 | 保存后的集成员状态 |
| --- | --- | --- |
| 是 | 已发布 | 已发布 |
| 否 | 未发布 | 集成员保持其已发布或未发布状态。 |

另请参阅[手动发布资源](publishing-files.md#manually-publishing-assets)和[手动取消发布资源](publishing-files.md#manually-unpublishing-assets)。

在创建旋转集时，Adobe建议采用以下最佳实践并强制实施以下限制：

| 旋转集限制类型 | 最佳实践 | 施加的限制 |
| --- | --- | --- |
| 每个2D集的最大行/列数 | 每组12-18个图像 | 1000 |

另请参阅[Dynamic Media限制](/help/using/limitations.md)。

在保存旋转集后，您可以使用“构建：旋转集”页面中的“预览”在默认查看器中查看旋转集的显示效果。

**创建旋转集：**

1. 在&#x200B;**[!UICONTROL 生成]**&#x200B;下拉菜单中，选择&#x200B;**[!UICONTROL 旋转集]**。
1. 在“旋转集大小”对话框中，设置需要的行数和单元格数。

   要生成一维旋转集，请仅选择一行。

   要构建二维旋转集，选择两行或更多行。

1. 选择&#x200B;**[!UICONTROL 确定]**。
1. 将图像拖放到“旋转集”屏幕上的网格中。
1. 完成后，在页面的右下角附近，确保选中了&#x200B;**保存Publish**（默认）。
1. 选择&#x200B;**[!UICONTROL 保存]**。
1. 在“保存”对话框中，选择一个用于存储旋转集的文件夹。 在“文件名”字段中，输入旋转集名称。
1. 选择&#x200B;**[!UICONTROL 保存]**。

## 编辑旋转集 {#editing-a-spin-set}

无论您是编辑已发布的集还是未发布的集，**[!UICONTROL 保存]**&#x200B;后的Publish选项都将通过以下方式影响该集和集成员：

| 是否已发布集？ | 在保存编辑之前，是否选择了保存&#x200B;**[!UICONTROL Publish]**&#x200B;选项？ | 保存后的集状态 | 保存后的集成员状态 |
| --- | --- | --- | --- |
| 是 | 是 | 已发布 | 已发布 |
| 是 | 否 | 已发布 | 现有集成员将保留其已发布状态。 在编辑期间添加的任何新的集成员保持其已发布或未发布状态。 |
| 否 | 是 | 已发布 | 已发布 |
| 否 | 否 | 未发布 | 现有的集成员以及在编辑期间添加的任何新的集成员保持其已发布或未发布状态。 |

另请参阅[手动发布资源](publishing-files.md#manually-publishing-assets)和[手动取消发布资源](publishing-files.md#manually-unpublishing-assets)。

**要编辑旋转集：**

1. 选择旋转集的变换&#x200B;**[!UICONTROL 编辑]**&#x200B;按钮。
1. 执行任何以下操作：

   * **正在删除映像**：选择映像，然后选择&#x200B;**[!UICONTROL 删除]**。

   * **添加图像**：将图像拖动到单元格中。

   * **重新排列行（二维旋转集）**：选择行选择器框（行左侧），然后选择&#x200B;**[!UICONTROL 向下移动行]**&#x200B;或&#x200B;**[!UICONTROL 向上移动行]**。

   * **添加行和单元格**：在“行”框和“单元格”框中输入一个数字，以确定每行的行数和单元格数。

1. 完成编辑后，在页面的右下角附近，请确保选中了&#x200B;**[!UICONTROL 保存]**&#x200B;后的Publish（默认）。
1. 选择&#x200B;**[!UICONTROL 保存]**，选择一个存储文件夹，输入该集的名称，然后选择&#x200B;**[!UICONTROL 保存]**。

## 删除旋转集

在删除集时，集本身将移到垃圾桶中。但是，该集中的成员（或“子项”）不受影响；相反，它们各自保留其现有的已发布或未发布状态。

另请参阅[手动发布资源](publishing-files.md#manually-publishing-assets)和[手动取消发布资源](publishing-files.md#manually-unpublishing-assets)。

**要删除旋转集：**

1. 在网格视图、列表视图或详细信息视图中，选择一个或多个旋转集。
1. 在全局导航栏上，转到&#x200B;**[!UICONTROL 文件]** > **[!UICONTROL 删除]** > **[!UICONTROL 删除]**。
