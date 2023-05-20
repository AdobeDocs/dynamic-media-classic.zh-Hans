---
title: 建立優惠方案集
description: 瞭解如何在Adobe Dynamic Media Classic中建立優惠方案集。
uuid: 6d6a4af9-70c0-4cfa-9a8f-855d6adfcc8f
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
discoiquuid: 59b6437d-c21e-4929-9291-3032dbb34565
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 05f2cce0-72bf-4933-87ab-c9003c848e35
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '1294'
ht-degree: 35%

---

# 建立優惠方案集 {#creating-an-offer-set}

您可以创建以下任意类型的优惠套餐：

* 视频
* 参数化模板
* 图像

對於範本，請選取 **[!UICONTROL 新增並預覽]**，然後設定您選擇的引數。 其他選件集型別不包含引數，但您仍可以透過選取來自訂引數 **[!UICONTROL 預覽]** 以及變更可用的預設集。

Adobe Dynamic Media Classic提供編輯和建立優惠方案集的工具。

>[!NOTE]
>
>建立優惠方案集之前，請務必先發佈您打算用於優惠方案集的所有資產，並設為Adobe Dynamic Media Classic。 请参阅[手动发布资源](publishing-files.md#manually_publishing_assets)和[手动取消发布资源](publishing-files.md#manually_unpublishing_assets)。

## 优惠套餐的类型 {#types-of-offer-sets}

从以下类型的优惠套餐创建一种优惠套餐：

* **影像**  — 您可以組合優惠方案集的影像。 每個影像在集中包含不同的選件。

* **影像範本**  — 您可以在Adobe Dynamic Media Classic中使用將影像範本引數化 **[!UICONTROL 建置]** >範本基本概念指令。 通过参数，可换出及自定义模板的各组成部分（文本框架中的文本、不同的图像）。对于优惠套餐，举例来说，您可以使用模板参数在优惠套餐中的同一图像上创建变型。如需建立及引數化影像範本的相關資訊，請參閱 [建立範本引數](creating-template-parameters.md#creating_template_parameters).

另請參閱 [範本基本需知](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/553_Template%20Basics_converted%20renamed_Dynamic%20Banners-AVS) 訓練影片。

* **視訊**  — 您可以為選件集組合視訊。 每个视频是套餐中的一个不同优惠。

## 使用引數化範本建立優惠方案集 {#creating-an-offer-set-with-a-parameterized-template}

在创建优惠套餐时，“**[!UICONTROL 保存后发布]**”选项按以下方式影响集和集成员：

| **[!UICONTROL 儲存後發佈]** 是否已在儲存前選取選項？ | 保存后的集状态 | 保存后的集成员状态 |
| --- | --- | --- |
| 是 | 已发布 | 已发布 |
| 否 | 未发布 | 集成员保持其已发布或未发布状态。 |

另请参阅[手动发布资源](publishing-files.md#manually_publishing_assets)和[手动取消发布资源](publishing-files.md#manually_unpublishing_assets)。

**使用引數化範本建立優惠方案集：**

1. 選取範本或橫幅。
1. 前往 **[!UICONTROL 建置]** > **[!UICONTROL Test&amp;Target選件集]**.

   Test&amp;Target選件集頁面會列出選件集中的選件。 列表中的第一项是对象。

1. 選取物件並選取 **[!UICONTROL 新增並預覽]**.

   此页面的左侧将列出模板中的参数和参数值。

1. 更改参数值以创建优惠。例如，在文本字段中输入不同文本、更改图层大小、用一个图像交换另一个图像或者选择不同的查看器预设。
1. 選取 **[!UICONTROL 儲存]** 或 **[!UICONTROL 另存新檔**]** 將優惠儲存為優惠方案集的一部分。

   「Test&amp;Target選件集」頁面會列出您建立的選件。

1. 重复步骤 3 到 5 为套餐创建更多优惠。
1. 完成時（在頁面的右下角附近），請確定 **[!UICONTROL 儲存後發佈*]** 已選取（預設）。
1. 選取 **[!UICONTROL 關閉]**，輸入優惠方案集的名稱，然後選取 **[!UICONTROL 儲存]**.

在關閉Test&amp;Target選件集頁面之前，請將選件集推送至Adobe Target Standard/Premium。 另請參閱 [將優惠方案集推送到Test&amp;Target](pushing-offer-sets-target.md#pushing_offer_sets_to_target).

## 使用影像或影片建立優惠方案集 {#creating-an-offer-set-with-images-or-videos}

在创建优惠套餐时，“**[!UICONTROL 保存后发布]**”选项按以下方式影响集和集成员：

| **[!UICONTROL 儲存後發佈]** 是否已在儲存前選取選項？ | 保存后的集状态 | 保存后的集成员状态 |
| --- | --- | --- |
| 是 | 已发布 | 已发布 |
| 否 | 未发布 | 集成员保持其已发布或未发布状态。 |

另请参阅[手动发布资源](publishing-files.md#manually_publishing_assets)和[手动取消发布资源](publishing-files.md#manually_unpublishing_assets)。

**使用图像或视频创建优惠套餐:**

1. 組合優惠方案集的影像或影片。 在「Test&amp;Target選件集」畫面或「格線檢視」或「清單檢視」中啟動，然後使用下列其中一種方法：

   * **Test&amp;Target選件集畫面**  — 前往 **[!UICONTROL 建置]** > **[!UICONTROL Test&amp;Target選件集]**. 将图像或视频拖到屏幕上。要创建大小不同的视频或图像，请拖入图像或视频的多个副本，然后逐个设置每个大小。

   * **格點檢視或清單檢視**  — 選取影像或影片，然後前往 **[!UICONTROL 建置]** > **[!UICONTROL Test&amp;Target選件集]**.

1. 或者，選取影像或視訊，然後選取 **[!UICONTROL 預覽]**. 在「預覽選件」頁面上，您可以變更所選影像或視訊的大小和外觀。 或者，您也可以變更選件集中的所有影像或影片。

   * 选择预设以更改图像或视频的外观和大小。
   * 若要將您選擇的預設集套用至選件集中的所有選件，請選取 **[!UICONTROL 選取預設集至全部]** 核取方塊。

   選取 **[!UICONTROL 儲存]** 以儲存您對影像或視訊選件所做的變更。 然後選取 **[!UICONTROL 關閉]** 返回Test&amp;Target選件集頁面。

1. 完成建立選件集的選件並選擇不同影像的影像預設集後，請確定 **[!UICONTROL 儲存後發佈]** 已選取（預設）。
1. 選取 **[!UICONTROL 儲存]** 並輸入優惠方案集的名稱，然後選取 **[!UICONTROL 儲存]**.

在關閉Test&amp;Target選件集頁面之前，請將選件集推送至Adobe Target Standard/Premium。 另請參閱 [將優惠方案集推送到Test&amp;Target](pushing-offer-sets-target.md#pushing_offer_sets_to_target).

## 編輯優惠方案集 {#editing-an-offer-set}

無論您是編輯已發佈集還是未發佈集， **[!UICONTROL 儲存後發佈]** 選項會以下列方式影響設定和設定成員：

| 是否已发布集？ | **[!UICONTROL 儲存後發佈]** 在儲存編輯之前是否已選取選項？ | 保存后的集状态 | 保存后的集成员状态 |
| --- | --- | --- | --- |
| 是 | 是 | 已发布 | 已发布 |
| 是 | 否 | 已发布 | 现有的集成员保持其已发布状态。在编辑期间添加的任何新的集成员保持其已发布或未发布状态。 |
| 否 | 是 | 已发布 | 已发布 |
| 否 | 否 | 未发布 | 现有的集成员以及在编辑期间添加的任何新的集成员保持其已发布或未发布状态。 |

另请参阅[手动发布资源](publishing-files.md#manually_publishing_assets)和[手动取消发布资源](publishing-files.md#manually_unpublishing_assets)。

**若要編輯優惠方案集：**

1. 若要編輯選件集，請在「網格檢視」或「清單檢視」中顯示選件集，然後選取其 **[!UICONTROL 編輯]** 滑鼠指向效果按鈕。
1. 在「Test&amp;Target選件集」頁面中，執行下列任一項作業：

   * **移除優惠方案**  — 選取選件，然後選取 **[!UICONTROL 刪除]** 以從選件集移除選件。
   * **新增優惠方案**  — 新增優惠的方式取決於您使用的優惠方案集型別：
      * **範本**  — 選取 **[!UICONTROL 新增並預覽]**，並在新增和預覽選件頁面上，建立其他選件。
      * **影像和影片**  — 將影像或視訊拖曳至Test&amp;Target選件集頁面。

   >[!NOTE]
   >
   >您无法删除与某个活动相关联的优惠套餐。若要刪除與行銷活動相關聯的優惠方案集，請先登入Adobe Target Standard/Premium並移除行銷活動關聯。 即使在與行銷活動解除關聯後，資產也只能從Adobe Dynamic Media Classic中刪除，這要求登入Adobe Target Standard/Premium，而不是從Adobe Target Standard/Premium中登入。

1. 當您完成編輯時（在頁面的右下角附近），請確定 **[!UICONTROL 儲存後發佈]** 已選取（預設）。
1. 選取 **[!UICONTROL 儲存]**，選取儲存資料夾，輸入集名稱，然後選取 **[!UICONTROL 儲存]**.

## 刪除優惠方案集 {#deleting-an-offer-set}

在删除优惠套餐时，套餐本身将移到垃圾桶中。不过，集中的成员（或“子项”）不受影响；它们分别保持现有的已发布或未发布状态。

另请参阅[手动发布资源](publishing-files.md#manually_publishing_assets)和[手动取消发布资源](publishing-files.md#manually_unpublishing_assets)。

**若要刪除優惠方案集：**

1. 在「網格檢視」、「清單檢視」或「詳細資料檢視」中，選取一個或多個選件集。
1. 在全域導覽列上，前往 **[!UICONTROL 檔案]** > **[!UICONTROL 刪除]** > **刪除**.

>[!MORELIKETHIS]
>
>* [创建模板参数](creating-template-parameters.md#creating_template_parameters)

