---
title: 設定eCatalog檢視器預設集
description: 瞭解如何在Adobe Dynamic Media Classic中設定eCatalog檢視器預設集。
uuid: aca66bc5-8491-4d81-9a06-1d3531860a14
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 6c123f85-3bc4-4392-a7fb-55618127c65e
feature: Dynamic Media Classic,Viewers,Viewer Presets,eCatalog
role: User
exl-id: 4357e6b8-fbc5-4e93-9476-db92a7dc7464
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '489'
ht-degree: 34%

---

# 設定eCatalog檢視器預設集{#setting-up-ecatalog-viewer-presets}

eCatalog 查看器预设决定了 eCatalog 查看器的样式、行为和外观。Adobe Dynamic Media Classic提供eCatalog檢視器預設集，如果您是管理員，也可以建立自己的eCatalog檢視器預設集。

若要建立預設集，您可以從頭開始，或從Adobe Dynamic Media Classic提供的eCatalog檢視器預設集開始，然後以新名稱儲存。 可以创建自己的 eCatalog 查看器预设，以使用公司颜色来显示印刷材料并设置色调。

eCatalog 查看器预设提供很多设置，包括页间跳转、缩放、搜索及选择“外观”。這些控制項的外觀和檢視器的顯示方式取決於您選擇的eCatalog檢視器預設集。

請依照下列步驟進行，以便建立eCatalog檢視器預設集（您必須是管理員）：

1. 在全域導覽列上，前往 **[!UICONTROL 設定]** > **[!UICONTROL 檢視器預設集]**.
1. 在“查看器预设”屏幕上，重新开始或从现有的 eCatalog 查看器预设开始创建 eCatalog 查看器预设：

   * **建立eCatalog檢視器預設集**  — 選取 **[!UICONTROL 新增]**. 在「新增檢視器預設集」對話方塊中，選擇平台，選擇「eCatalog檢視器」，然後選取 **[!UICONTROL 新增]**.

   * **編輯eCatalog檢視器預設集**  — 選取eCatalog檢視器預設集，然後選取 **[!UICONTROL 編輯]**. 選取 **[!UICONTROL 另存為]** 完成建立預設集之後。

1. 在“配置查看器”屏幕上，输入 eCatalog 查看器预设的名称。
1. 在“配置查看器”屏幕上，设置所需选项。

   選取 **[!UICONTROL 資訊提示]** 圖示（位於選項旁）。

   當您更新和變更設定時，「預覽」頁面會顯示檢視器。

1. （選用）在 **[!UICONTROL 資訊面板設定]**，則 **[!UICONTROL 資訊伺服器URL]** 選項可包含下列特殊代號，由檢視器加以替代：

   | 令牌 | 代替为 | 说明 |
   | --- | --- | --- |
   | `$1$` | rollover_key 值 | 來自以下專案的專案識別碼： `<area>` 地圖元素。 |
   | `$2$` | frame | 图像集中当前显示的帧的序号。 |
   | `$3$` | 影像根 | 在图像命令中指定的第一个物品的第一个路径元素（通常为指定图像集的目录条目的图像目录 ID）。 |

1. （選用）在 **[!UICONTROL 資訊面板設定]**，在 **[!UICONTROL 回應範本]** 方塊中，輸入您要在Adobe Dynamic Media Classic擷取影像地圖資訊時發生錯誤，顯示的文字。 例如，如果系统收到公司名称和 eCatalog 名称，但是没有变换标识符，则将为用户显示该消息。

>[!NOTE]
>
>若要使用此回應範本，而非eCatalog本身所定義的範本，請新增 `fmt=1` 到資訊伺服器URL的結尾。 示例: `https://.../$3$/$4$/$1$/?FMT=1`.

1. 選取 **[!UICONTROL 儲存]**.
1. 選取 **[!UICONTROL 預設]** 如果您希望您所建立的eCatalog檢視器預設集是在網頁上顯示eCatalog時所使用的檢視器預設集。

若要刪除eCatalog檢視器預設集，請在「檢視器預設集」畫面上選取該預設集，然後選取 **[!UICONTROL 刪除]**.

>[!MORELIKETHIS]
>
>* [Viewer Presets](application-setup.md#viewer_presets)

