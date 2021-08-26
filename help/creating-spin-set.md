---
title: 创建旋转集
description: 了解如何在AdobeDynamic Media Classic中创建旋转集。
uuid: 697bd78f-5e39-46bf-aa6d-ad8ab99fe40e
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/spin_sets
discoiquuid: 735b5867-e249-4627-a5a5-25c19c2255bf
feature: Dynamic Media Classic,Viewers,Spin Sets
role: User
exl-id: 35e8e7fc-5b3c-441a-959c-df2e39ea0d4b
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '910'
ht-degree: 55%

---

# 创建旋转集{#creating-a-spin-set}

要创建有效的旋转集，请确保正确拍摄图像。您可以在AdobeDynamic Media Classic中创建旋转集，方法是选择生成按钮并选择旋转集。 在“旋转集”屏幕中编辑旋转集。

>[!NOTE]
>
>AdobeDynamic Media Classic的早期版本不提供二维旋转集。 如果您是在以前版本的AdobeDynamic Media Classic中创建的旋转集，则要先以其他名称保存一维旋转集，然后再保存它。 在旋转集屏幕中选择&#x200B;**[!UICONTROL 另存为]**&#x200B;并输入新名称，以便在AdobeDynamic Media Classic中对其进行编辑。

## 旋转集图像拍摄指南 {#guidelines-for-shooting-spin-set-images}

通常，旋转集中的图像越多，图像的旋转效果越好。不过，在旋转集中加入许多图像会增加图像的加载时间。AdobeDynamic Media Classic建议遵循以下准则来拍摄图像以在旋转集中使用：

* 在一维旋转集中至少使用8-12幅图像，在二维旋转集中至少使用16-24幅图像。
* 请使用无损格式；建议使用 TIFF 和 PNG。
* 为所有图像创建蒙版，这样物品将显示在纯白色或其他高对比度背景上。也可以添加阴影。
* 确保产品细节非常明亮，且位于焦点上。
* 借助人体模型或时装模特儿为流行服饰拍摄旋转图像。通常，模特人道模型会被蒙版（使用玻璃材质的模特人道模型），或者图像中会显示风格化的模特人道模型/裁缝。 通过定义角度的数目，可以创建模特儿旋转集。用胶带在地板上标出每个角度，以便引导模型步进并查看每个拍摄方向。

## 创建旋转集 {#create}

在Dynamic Media Classic中创作或创建Adobe集的顺序很重要。 根据将图像拖放到“旋转集”页面上的网格中的顺序，旋转集将按特定的方向旋转。因此，在生成器中以可视方式显示资产的顺序是，当用户移动鼠标指针或移动手指时，资产的旋转方式。

在创建集时，“**[!UICONTROL 保存后发布]**”选项按以下方式影响集和集成员：

| **[!UICONTROL 在保存前]** 选择保存后发布选项？ | 保存后的集状态 | 保存后的集成员状态 |
| --- | --- | --- |
| 是 | 已发布 | 已发布 |
| 否 | 未发布 | 集成员保持其已发布或未发布状态。 |

另请参阅[手动发布资源](publishing-files.md#manually-publishing-assets)和[手动取消发布资源](publishing-files.md#manually-unpublishing-assets)。

在保存旋转集后，您可以使用“构建：旋转集”页面中的“预览”在默认查看器中查看旋转集的显示效果。

**创建旋转集:**

1. 在&#x200B;**[!UICONTROL Build]**&#x200B;下拉菜单中，选择&#x200B;**[!UICONTROL 旋转集]**。
1. 在“旋转集大小”对话框中，设置需要的行数和单元格数。

   要构建一维旋转集，仅选择一行。

   要构建二维旋转集，选择两行或更多行。

1. 选择&#x200B;**[!UICONTROL 确定]**。
1. 将图像拖放到“旋转集”屏幕上的网格中。
1. 完成后，确保在页面右下角附近选择了“**保存后发布**”（默认）。
1. 选择&#x200B;**[!UICONTROL Save]**。
1. 在“保存”对话框中，选择一个文件夹来存储您的旋转集。在“文件名”字段中，输入旋转集名称。
1. 选择&#x200B;**[!UICONTROL Save]**。

## 编辑旋转集 {#editing-a-spin-set}

无论您是编辑已发布的集还是未发布的集，**[!UICONTROL 保存后发布]**&#x200B;选项都会通过以下方式影响集和集成员：

| 是否已发布集？ | **[!UICONTROL 在保存您]** 的编辑之前选择保存选项后发布？ | 保存后的集状态 | 保存后的集成员状态 |
| --- | --- | --- | --- |
| 是 | 是 | 已发布 | 已发布 |
| 是 | 否 | 已发布 | 现有的集成员保持其已发布状态。在编辑期间添加的任何新的集成员保持其已发布或未发布状态。 |
| 否 | 是 | 已发布 | 已发布 |
| 否 | 否 | 未发布 | 现有的集成员以及在编辑期间添加的任何新的集成员保持其已发布或未发布状态。 |

另请参阅[手动发布资源](publishing-files.md#manually-publishing-assets)和[手动取消发布资源](publishing-files.md#manually-unpublishing-assets)。

**编辑旋转集:**

1. 选择旋转集的滚动更新&#x200B;**[!UICONTROL 编辑]**&#x200B;按钮。
1. 执行任何以下操作：

   * **删除图像**  — 选择图像，然后选择“删 **[!UICONTROL 除”]**。

   * **添加图像**  — 将图像拖入单元格中。

   * **重新排序行（二维旋转集）**  — 选择一个行选择器框（位于行的左侧），然后选择 **[!UICONTROL 下移]** 行或 **[!UICONTROL 上移行]**。

   * **添加行和单元格**  — 在“行”框和“单元格”框中输入一个数字，以确定每行的行数和单元格数。

1. 在完成编辑后，确保在页面右下角附近选择了“**[!UICONTROL 保存后发布]**”（默认）。
1. 选择&#x200B;**[!UICONTROL Save]**，选择存储文件夹，输入集的名称，然后选择&#x200B;**[!UICONTROL Save]**。

## 删除旋转集 {#deleting-a-spin-set}

在删除集时，集本身将移到垃圾桶中。不过，集中的成员（或“子项”）不受影响；它们分别保持现有的已发布或未发布状态。

另请参阅[手动发布资源](publishing-files.md#manually-publishing-assets)和[手动取消发布资源](publishing-files.md#manually-unpublishing-assets)。

**删除旋转集:**

1. 在网格视图、列表视图或详细信息视图中，选择一个或多个旋转集。
1. 在全局导航栏上，转到&#x200B;**[!UICONTROL 文件]** > **[!UICONTROL 删除]** > **[!UICONTROL 删除]**。
