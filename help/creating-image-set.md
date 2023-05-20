---
title: 创建图像集
description: 瞭解如何在Adobe Dynamic Media Classic中建立影像集。
uuid: 689fdc14-4f51-4c94-8515-cd8551e101d8
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sets
discoiquuid: 3f356410-b30e-4870-ad95-6e5a9dc126c8
feature: Dynamic Media Classic,Viewers,Image Sets,Spin Sets
role: User
exl-id: c18bb98c-b087-45d0-a4c9-44f58a3b514f
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '635'
ht-degree: 59%

---

# 创建图像集{#creating-an-image-set}

要创建多视图图像集，您需要从不同视角显示物品或显示同一物品不同侧面的图像。这是为了向观看者展示物品的图像，使其对物品的外观或功能有充分的认识。

## 创建图像集 {#create}

在创建集时，“**[!UICONTROL 保存后发布]**”选项按以下方式影响集和集成员：

| **[!UICONTROL 儲存後發佈]** 是否已在儲存前選取選項？ | 保存后的集状态 | 保存后的集成员状态 |
| --- | --- | --- |
| 是 | 已发布 | 已发布 |
| 否 | 未发布 | 集成员保持其已发布或未发布状态。 |

另请参阅[手动发布资源](publishing-files.md#manually_publishing_assets)和[手动取消发布资源](publishing-files.md#manually_unpublishing_assets)。

建立影像集時，Adobe會建議下列最佳作法並強制實行下列限制：

| 限制型別 | 最佳实践 | 強制限制 |
| --- | --- | --- |
| 每個集的重複資產數量 | 無重複專案 | 20 |
| 每組影像的最大數量 | 每組5至10個影像 | 1000 |

另請參閱 [Dynamic Media限制](/help/limitations.md).

**创建图像集:**

1. 执行以下任一操作：

   * **請先選取影像**  — 在「瀏覽」面板中，選取您想用於影像集的影像，前往 **[!UICONTROL 建置]** > **[!UICONTROL 影像集]**.

   * **從「影像集」畫面開始**  — 前往 **[!UICONTROL 建置]** > **[!UICONTROL 影像集]**. “图像集”屏幕随即打开。在资源库中选择一个文件夹，然后将要用于图像集的图像拖到“图像集”屏幕中。

1. 要更改图像顺序，将图像拖到新位置即可。
1. 确保在页面右下角附近选择了“**[!UICONTROL 保存后发布]**”（默认）。
1. 選取 **[!UICONTROL 儲存]**，選取儲存影像集的資料夾，輸入影像集名稱，然後選取 **[!UICONTROL 儲存]**.
1. 若要在影像集檢視器中檢視您的影像集，請選取 **[!UICONTROL 預覽]** 在「影像集」畫面上。 您可以在「影像集檢視器」中選取色票縮圖，以檢視其行為。

## 编辑图像集 {#editing-an-image-set}

無論您是編輯已發佈集還是未發佈集， **[!UICONTROL 儲存後發佈]** 選項會以下列方式影響設定和設定成員：

| 是否已发布集？ | **[!UICONTROL 儲存後發佈]** 在儲存編輯之前是否已選取選項？ | 保存后的集状态 | 保存后的集成员状态 |
| --- | --- | --- | --- |
| 是 | 是 | 已发布 | 已发布 |
| 是 | 否 | 已发布 | 现有的集成员保持其已发布状态。在编辑期间添加的任何新的集成员保持其已发布或未发布状态。 |
| 否 | 是 | 已发布 | 已发布 |
| 否 | 否 | 未发布 | 现有的集成员以及在编辑期间添加的任何新的集成员保持其已发布或未发布状态。 |

另请参阅[手动发布资源](publishing-files.md#manually_publishing_assets)和[手动取消发布资源](publishing-files.md#manually_unpublishing_assets)。

**编辑图像集:**

1. 在「格點檢視」中，瀏覽至影像集，然後在影像下方選取 **[!UICONTROL 編輯]**.
1. 执行任何以下操作：

   * 要添加图像（已发布或未发布），请在“添加资源”中将其从文件夹拖到图像集的“**[!UICONTROL 视图]**”页面上。
   * 若要移除影像，請選取該影像，然後選取 **[!UICONTROL 刪除]** （在工具列上）。
   * 要将图像重新排序，请将图像拖到新位置。

1. 在编辑完集后，确保在页面右下角附近选择了“**[!UICONTROL 保存后发布]**”（默认）。
1. 選取 **[!UICONTROL 儲存]**，為您的集選取儲存資料夾，輸入集名稱，然後選取 **[!UICONTROL 儲存]**.

## 刪除影像集 {#deleting-an-image-set}

在删除集时，集本身将移到垃圾桶中。不过，集中的成员（或“子项”）不受影响；它们分别保持现有的已发布或未发布状态。

另请参阅[手动发布资源](publishing-files.md#manually_publishing_assets)和[手动取消发布资源](publishing-files.md#manually_unpublishing_assets)。

**删除图像集:**

1. 在「格點檢視」、「清單檢視」或「詳細資訊檢視」中，選取一個或多個「影像集」。
1. 在全域導覽列上，前往 **[!UICONTROL 檔案]** > **[!UICONTROL 刪除]** > **[!UICONTROL 刪除]**.
