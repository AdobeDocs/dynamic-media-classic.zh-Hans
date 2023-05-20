---
title: 建立迴轉集
description: 瞭解如何在Adobe Dynamic Media Classic中建立迴轉集。
uuid: 697bd78f-5e39-46bf-aa6d-ad8ab99fe40e
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/spin_sets
discoiquuid: 735b5867-e249-4627-a5a5-25c19c2255bf
feature: Dynamic Media Classic,Viewers,Spin Sets
role: User
exl-id: 35e8e7fc-5b3c-441a-959c-df2e39ea0d4b
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '952'
ht-degree: 50%

---

# 建立迴轉集{#creating-a-spin-set}

要创建有效的旋转集，请确保正确拍摄图像。您可以選取「建置」按鈕，然後選擇「迴轉集」，在Adobe Dynamic Media Classic中建立迴轉集。 在“旋转集”屏幕中编辑旋转集。

>[!NOTE]
>
>舊版Adobe Dynamic Media Classic未提供二維迴轉集。 如果您在舊版Adobe Dynamic Media Classic中建立了迴轉集，則必須先以其他名稱儲存一維迴轉集，才能儲存它。 選取 **[!UICONTROL 另存為]** 在「迴轉集」畫面中，輸入新名稱，以便在Adobe Dynamic Media Classic中編輯。

## 旋转集图像拍摄指南 {#guidelines-for-shooting-spin-set-images}

一般而言，迴轉集中的影像越多，影像旋轉效果就越好。 不过，在旋转集中加入许多图像会增加图像的加载时间。Adobe Dynamic Media Classic建議您在拍攝影像以用於「迴轉集」時，遵循下列准則：

* 在一維迴轉集中至少使用8-12個影像，在二維迴轉集中至少使用16-24個影像。
* 请使用无损格式；建议使用 TIFF 和 PNG。
* 为所有图像创建蒙版，这样物品将显示在纯白色或其他高对比度背景上。也可以添加阴影。
* 确保产品细节非常明亮，且位于焦点上。
* 借助人体模型或时装模特儿为流行服饰拍摄旋转图像。通常，人體模型會被遮罩（使用玻璃人體模型），或是樣式化的人體模型/服裝模型會顯示在影像中。 您可以定義角度數來建立模型上的迴轉集。 在地面上用膠帶標籤每個角度，這樣您就可以引導模型步進，並檢視每個拍攝的方向。

## 建立迴轉集 {#create}

在Adobe Dynamic Media Classic中製作或建立迴轉集的順序很重要。 根据将图像拖放到“旋转集”页面上的网格中的顺序，旋转集将按特定的方向旋转。因此，當使用者移動滑鼠指標或移動手指（由左至右）時，資產在產生器中視覺顯示的順序就是資產的旋轉方式。

在创建集时，“**[!UICONTROL 保存后发布]**”选项按以下方式影响集和集成员：

| **[!UICONTROL 儲存後發佈]** 是否已在儲存前選取選項？ | 保存后的集状态 | 保存后的集成员状态 |
| --- | --- | --- |
| 是 | 已发布 | 已发布 |
| 否 | 未发布 | 集成员保持其已发布或未发布状态。 |

另请参阅[手动发布资源](publishing-files.md#manually-publishing-assets)和[手动取消发布资源](publishing-files.md#manually-unpublishing-assets)。

當您建立迴轉集時，Adobe會建議下列最佳作法並強制實行下列限制：

| 迴轉集限制型別 | 最佳实践 | 強制限制 |
| --- | --- | --- |
| 每個2D集的最大列數/欄數 | 每組12-18個影像 | 1000 |

另請參閱 [Dynamic Media限制](/help/limitations.md).

在保存旋转集后，您可以使用“构建：旋转集”页面中的“预览”在默认查看器中查看旋转集的显示效果。

**创建旋转集:**

1. 於 **[!UICONTROL 建置]** 下拉式功能表，選取 **[!UICONTROL 迴轉集]**.
1. 在“旋转集大小”对话框中，设置需要的行数和单元格数。

   要构建一维旋转集，仅选择一行。

   要构建二维旋转集，选择两行或更多行。

1. 選取 **[!UICONTROL 確定]**.
1. 将图像拖放到“旋转集”屏幕上的网格中。
1. 完成后，确保在页面右下角附近选择了“**保存后发布**”（默认）。
1. 選取 **[!UICONTROL 儲存]**.
1. 在“保存”对话框中，选择一个文件夹来存储您的旋转集。在“文件名”字段中，输入旋转集名称。
1. 選取 **[!UICONTROL 儲存]**.

## 編輯迴轉集 {#editing-a-spin-set}

無論您是編輯已發佈集還是未發佈集， **[!UICONTROL 儲存後發佈]** 選項會以下列方式影響設定和設定成員：

| 是否已发布集？ | **[!UICONTROL 儲存後發佈]** 在儲存編輯之前是否已選取選項？ | 保存后的集状态 | 保存后的集成员状态 |
| --- | --- | --- | --- |
| 是 | 是 | 已发布 | 已发布 |
| 是 | 否 | 已发布 | 现有的集成员保持其已发布状态。在编辑期间添加的任何新的集成员保持其已发布或未发布状态。 |
| 否 | 是 | 已发布 | 已发布 |
| 否 | 否 | 未发布 | 现有的集成员以及在编辑期间添加的任何新的集成员保持其已发布或未发布状态。 |

另请参阅[手动发布资源](publishing-files.md#manually-publishing-assets)和[手动取消发布资源](publishing-files.md#manually-unpublishing-assets)。

**编辑旋转集:**

1. 選取迴轉集的變換 **[!UICONTROL 編輯]** 按鈕。
1. 执行任何以下操作：

   * **移除影像**  — 選取影像，然後選取 **[!UICONTROL 刪除]**.

   * **新增影像**  — 將影像拖曳至儲存格。

   * **重新排序列（二維迴轉集）**  — 選取列選擇器方塊（位於列左側），然後選取 **[!UICONTROL 將列下移]** 或 **[!UICONTROL 將列上移]**.

   * **新增列和儲存格**  — 在「列」方塊和「儲存格」方塊中輸入數字，以決定列數和每列中的儲存格數。

1. 在完成编辑后，确保在页面右下角附近选择了“**[!UICONTROL 保存后发布]**”（默认）。
1. 選取 **[!UICONTROL 儲存]**，選取儲存資料夾，輸入集名稱，然後選取 **[!UICONTROL 儲存]**.

## 刪除迴轉集 {#deleting-a-spin-set}

在删除集时，集本身将移到垃圾桶中。不过，集中的成员（或“子项”）不受影响；它们分别保持现有的已发布或未发布状态。

另请参阅[手动发布资源](publishing-files.md#manually-publishing-assets)和[手动取消发布资源](publishing-files.md#manually-unpublishing-assets)。

**删除旋转集:**

1. 在网格视图、列表视图或详细信息视图中，选择一个或多个旋转集。
1. 在全域導覽列上，前往 **[!UICONTROL 檔案]** > **[!UICONTROL 刪除]** > **[!UICONTROL 刪除]**.
