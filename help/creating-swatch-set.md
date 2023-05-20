---
title: 创建样本集
description: 瞭解如何在Adobe Dynamic Media Classic中建立色票集。
uuid: 250b3525-310d-4481-b0bc-f9057e823e0b
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/swatch_sets
discoiquuid: 631d2b2d-9e69-4b96-8392-17e00a1a8de0
feature: Dynamic Media Classic,Viewers
role: User
exl-id: 426b6e6b-daed-4ca6-b095-99bb06604b07
source-git-commit: cb55e09a997b9d36002c4ac429603576d52fb8bd
workflow-type: tm+mt
source-wordcount: '708'
ht-degree: 67%

---

# 创建样本集{#creating-a-swatch-set}

样本集允许用户以不同颜色、模式或光泽度查看项目。要使用颜色样本创建样本集，需要具有要提供给用户的每种不同颜色、模式或光泽度的一个图像。还需要每种颜色、模式或光泽度的一种颜色、模式或光泽度样本。

例如，假定要使用不同颜色的标记显示大写字母的图像，标记为红色、绿色和蓝色。在这种情况下，需要同一大写字母的三种快照。一个红色标记快照，一个绿色标记快照，以及一个蓝色标记快照。还需要红色、绿色和蓝色样本。顏色色票可作為縮圖，供使用者在色票集檢視器中選取，以檢視紅色計費、綠色計費或藍色計費上限。

## 创建样本集 {#create}

在创建集时，“**保存后发布**”选项按以下方式影响集和集成员：

| **[!UICONTROL 儲存後發佈]** 是否已在儲存前選取選項？ | 保存后的集状态 | 保存后的集成员状态 |
| --- | --- | --- |
| 是 | 已发布 | 已发布 |
| 否 | 未发布 | 集成员保持其已发布或未发布状态。 |

另请参阅[手动发布资源](publishing-files.md#manually_publishing_assets)和[手动取消发布资源](publishing-files.md#manually_unpublishing_assets)。

**创建样本集:**

1. 执行以下任一操作：

   * **請先選取影像**  — 在「瀏覽」面板中，選取影像，然後前往 **[!UICONTROL 建置]** > **[!UICONTROL 色票集]**.

   * **從「色票集」畫面開始**  — 前往 **[!UICONTROL 建置]** > **[!UICONTROL 色票集]**. 从资源库中选择一个文件夹，然后将图像拖到“样本集”页面的“视图”部分中。

1. 将样本颜色、模式或光泽度拖到“样本集”页面上的样本占位符框中。

   确保拖到每个占位符里的颜色、模式或光泽度样本表示相邻图像的颜色、模式或光泽度。

1. 要更改样本集中图像的顺序，请将图像拖到新位置。
1. 确保在页面右下角附近选择了“**[!UICONTROL 保存后发布]**”（默认）。
1. 選取 **[!UICONTROL 儲存]**，選取儲存色票集資料夾，輸入色票集名稱，然後選取 **[!UICONTROL 提交]**.
1. 若要在色票集檢視器中檢視您的色票集，請選取 **[!UICONTROL 預覽]** 在「色票集」畫面上。 您可以在「色票集檢視器」中選取色票縮圖，以檢視其行為。

## 编辑样本集 {#editing-a-swatch-set}

無論您是編輯已發佈集還是未發佈集， **[!UICONTROL 儲存後發佈]** 選項會以下列方式影響設定和設定成員：

| 是否已发布集？ | **[!UICONTROL 發佈晚於]** 儲存編輯之前是否已選取儲存選項？ | 保存后的集状态 | 保存后的集成员状态 |
|--- |--- |--- |--- |
| 是 | 是 | 已发布 | 已发布 |
| 是 | 否 | 已发布 | 现有的集成员保持其已发布状态。在编辑期间添加的任何新的集成员保持其已发布或未发布状态。 |
| 否 | 是 | 已发布 | 已发布 |
| 否 | 否 | 未发布 | 现有的集成员以及在编辑期间添加的任何新的集成员保持其已发布或未发布状态。 |

另请参阅[手动发布资源](publishing-files.md#manually_publishing_assets)和[手动取消发布资源](publishing-files.md#manually_unpublishing_assets)。

**编辑样本集:**

1. 在「格點檢視」中，瀏覽至「色票集」，然後在影像下方選取 **[!UICONTROL 編輯]**.
1. 执行任何以下操作：

   * 要添加图像（已发布或未发布），请在“添加资源”中将其从文件夹拖到样本集的“**[!UICONTROL 视图]**”页面上。
   * 若要移除影像，請選取該影像，然後選取 **[!UICONTROL 刪除]** （在工具列上）。
   * 要将图像重新排序，请将图像拖到新位置。

1. 在编辑完集后，确保在页面右下角附近选择了“**[!UICONTROL 保存后发布]**”（默认）。
1. 選取 **[!UICONTROL 儲存]**，選取儲存資料夾，輸入集名稱，然後選取 **[!UICONTROL 儲存]**.

## 刪除色票集 {#deleting-a-swatch-set}

在删除集时，集本身将移到垃圾桶中。不过，集中的成员（或“子项”）不受影响；它们分别保持现有的已发布或未发布状态。

另请参阅[手动发布资源](publishing-files.md#manually_publishing_assets)和[手动取消发布资源](publishing-files.md#manually_unpublishing_assets)。

**删除样本集:**

1. 在「格點檢視」、「清單檢視」或「詳細資訊檢視」中，選取一個或多個「色票集」。
1. 在全域導覽列上，前往 **[!UICONTROL 檔案]** > **[!UICONTROL 刪除]** > **[!UICONTROL 刪除]**.
