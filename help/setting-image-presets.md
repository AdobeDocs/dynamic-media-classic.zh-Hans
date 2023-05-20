---
title: 設定影像預設集
description: 瞭解如何在Adobe Dynamic Media Classic中設定影像預設集。
uuid: 90530948-dee9-41bd-b39e-684140446abc
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
discoiquuid: 1ec39fe5-7b2a-4034-9570-6b5595f97052
feature: Dynamic Media Classic,Image Presets
role: User
exl-id: 336802cc-b032-49b2-b2e6-d699bc997ee5
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '659'
ht-degree: 50%

---

# 設定影像預設集{#setting-up-image-presets}

像宏一样，图像预设是用某个名称保存的一组预定义大小和格式命令。若要瞭解影像預設集如何運作，假設您的網站要求每個產品影像以兩種不同的大小顯示：500 x 500畫素和150 x 150畫素。 您创建了两个图像预设，一个称为“放大”，以 500 x 500 像素显示图像，另一个称为“缩略图”，以 150 x 150 像素显示图像。為了以「放大」和「縮圖」大小傳送影像，Dynamic Media影像伺服器會查詢放大影像預設集和縮圖影像預設集的定義。 然后，服务器按每个图像预设的大小和格式规范动态生成图像。

Adobe Dynamic Media Classic隨附數個「最佳實務」影像預設集，這些預設集已設定好供您使用。 管理員也可以建立影像預設集。 要创建图像预设，您可以从头开始，也可以使用现有的图像预设进行创建，然后用新名称进行保存。

从服务器动态传送图像时，对于大小有所缩减的图像，其清晰度和细节可能会有些损失。因此，每个图像预设都包含格式控制，用于优化以特定大小进行传送的图像。这些控制可确保传送至网站或应用程序的图像清晰可辨。

## 建立影像預設集 {#creating-an-image-preset}

如果您是公司的管理员，则可以创建自己的图像预设。您可以建立影像預設集或從Adobe Dynamic Media Classic提供的預設影像預設集開始、編輯預設集，然後以新名稱儲存預設集。

**创建图像预设:**

1. 前往 **[!UICONTROL 設定]** > **[!UICONTROL 影像預設集]**.

   可以在该屏幕上浏览至一个图像预设名称来预览现有的图像预设。在选择图像预设名称时，预览窗口中示例图像的大小和外观会发生更改。

1. 执行以下任一操作：

   * **建立影像預設集**  — 選取 **[!UICONTROL 新增]**.
   * **編輯影像預設集**  — 瀏覽至與您要建立的最相似的影像預設集，然後選取 **[!UICONTROL 編輯]**.

1. 输入图像预设的名称。
1. 输入宽和高的像素数。这些数字确定了所传送图像的大小。
1. 填写“添加预设”或“编辑预设”屏幕。有关详细信息，请参阅[图像预设选项](application-setup.md#image_preset_options)。

   Adobe Dynamic Media Classic建議從下列「最佳實務」選項選擇開始：

   * **[!UICONTROL 格式]**  — 選擇JPEG或其他符合您需求的格式。 所有 Web 浏览器都支持 JPEG 图像格式；这种格式在小文件大小与图像质量之间取得了良好平衡。然而，JPEG 格式图像使用了有损压缩模式，如果压缩设置过低，可能会产生多余的图像伪影。因此，Adobe Dynamic Media Classic建議將壓縮品質（在滑杆上）設為75。 该设置在图像质量与小文件大小之间取得了良好平衡。

   * **[!UICONTROL 銳利化]**  — 請勿選取「銳利化」 (此銳利化濾鏡提供的控制項少於 **[!UICONTROL 不銳利化遮色片]** 設定)。

   * **[!UICONTROL 重新取樣模式]**  — 選擇 **[!UICONTROL 雙立方式]**.

   * **[!UICONTROL 不銳利化遮色片]** (USM) — 輸入下列設定：

   | 预设类型 | 大小 | USM：数量 | USM：半径 | USM：阈值 |
   | --- | --- | --- | --- | --- |
   | 交叉销售（微型缩略图） | 75 x 75 | 1.5 | 0.8 | 5 |
   | 缩略图 | 150 x 150 | 1.1 | 1 | 5 |
   | 主图像 | 350 x 350 | 1 | 1 | 6 |
   | 放大 | 500 x 500 | 1.2 | 1.2 | 5 |

1. 選取 **[!UICONTROL 儲存]**.

用來建立影像預設集的Adobe Dynamic Media Classic「最佳實務」選項列於此處，這些是一般建議；銳利化是高度主觀的。 這些「最佳實務」設定是以2000 x 2000主要影像為基礎；大型或小型主要檔案的設定可能不同。 如果要調整「不銳利化遮色片」設定，Adobe Dynamic Media Classic建議使用下列範圍：

* **[!UICONTROL 數量]**  — 介於。8和1.5之間。

* **[!UICONTROL 半徑]**  — 介於。6和2之間。

* **[!UICONTROL 臨界值]**  — 從1到6。

若要刪除影像預設集，請在「影像預設集」畫面上選取它，然後選取 **[!UICONTROL 刪除]**.

>[!MORELIKETHIS]
>
>* [创建并编辑图像预设](application-setup.md#creating_and_editing_image_presets)
>* [图像预设选项](application-setup.md#image_preset_options)
>* [根據影像預設集預覽影像資產](previewing-asset.md#previewing_an_image_asset_based_on_its_image_preset)

