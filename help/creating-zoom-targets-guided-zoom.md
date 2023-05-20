---
title: 建立引導式縮放的縮放目標
description: 瞭解如何為Adobe Dynamic Media Classic中的引導式縮放建立縮放目標。
uuid: 501ea37b-adc5-4290-87eb-52a3501e5d26
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/zoom
discoiquuid: e7b4673c-8681-4741-912e-9a31cf106449
feature: Dynamic Media Classic,Viewers,Zoom
role: User
exl-id: ffb799ba-1cf1-48e0-91a8-dea758139140
source-git-commit: cb55e09a997b9d36002c4ac429603576d52fb8bd
workflow-type: tm+mt
source-wordcount: '729'
ht-degree: 41%

---

# 建立引導式縮放的縮放目標{#creating-zoom-targets-for-guided-zoom}

缩放目标会将查看者引导到图像的特定部分。除了自由格式縮放以外，檢視者還可以選取縮放目標縮圖，並縮放至您要其聚焦的影像部分。 通过缩放目标，可突出显示图像的有趣或诱人之处。

![建立引導式縮放的縮放目標](/help/assets/zo_guided_zoom.png)

## 关于缩放目标 {#about-zoom-targets}

缩放目标的最大缩放百分比是 100%。根据查看器大小和图像大小的不同组合，最小缩放百分比也会有所不同，如下表所示：

| 图像大小 | 查看器大小 | 缩放百分比 |
| --- | --- | --- |
| 大 | 较小 | 最小缩放百分比较小 |
| 小 | 较大 | 最小缩放百分比较大 |

您可以更改缩放查看器大小，使之与网页上使用的大小相匹配。要永久更改此设置，可以在“设置”屏幕上更改查看器大小（如果您是管理员）。另請參閱 [設定縮放檢視器預設集](setting-zoom-viewer-presets.md#setting_up_zoom_viewer_presets).

## 建立和編輯縮放目標 {#creating-and-editing-zoom-targets}

在“缩放目标编辑器”屏幕上创建并编辑缩放目标。要打开该屏幕，请选择一个图像并执行以下任一操作：

* 選取滑鼠指向效果 **[!UICONTROL 編輯]** 按鈕，然後選擇「縮放目標」。
* 在「瀏覽」面板中，將影像顯示於 **[!UICONTROL 詳細資料檢視]**，然後選取 **[!UICONTROL 縮放目標]**.

在「縮放目標編輯器」畫面上，選取 **[!UICONTROL 選取目標]** 按鈕（箭頭），在變更目標大小或位置之前選取目標。 若要在影像上建立縮放目標，請選取 **[!UICONTROL 新增目標]** （矩形）。 「縮放目標編輯器」頁面也提供刪除、複製和命名縮放目標的工具。

### 建立縮放目標 {#creating-a-zoom-target}

若要建立縮放目標，請開啟「縮放目標編輯器」頁面，並執行下列動作：

1. 選取 **[!UICONTROL 新增目標]** （矩形），將指標移到影像上，然後選取縮放目標的位置。

   缩放目标的缩略图图像显示在屏幕右侧的面板中。

1. 選取 **[!UICONTROL 選取目標]** （箭頭），然後選取您建立的縮放目標，並調整目標的大小和位置。

   * **調整大小**  — 將指標移到縮放目標的一個角落上，然後拖曳以放大或縮小目標。

   * **位置**  — 將指標移到縮放目標上方，並將其拖曳至其他位置。

1. 在“名称”框中输入缩放目标名称。

   >[!NOTE]
   >
   >在“名称”框中输入的不仅仅是名称。用户在缩放目标上移动指针时，将会看到您在“名称”框中输入的内容。在“名称”框中输入对缩放目标的简要描述，以便用户了解其可以缩放的内容。

1. 可以视情况在“用户数据”字段中输入用户数据。该字段可供网站设计人员向缩放目标中添加信息。
1. 選取 **[!UICONTROL 儲存]**.

   即可保存缩放目标的坐标和缩放级别。带有您输入的名称的缩放目标缩略图显示在屏幕右侧。

>[!NOTE]
>
>若要在縮放檢視器中檢視您的縮放目標外觀，請選取 **[!UICONTROL 預覽]** 「縮放目標編輯器」畫面中的按鈕，並在「預覽」畫面中選擇「縮放檢視器」。 如需有關此熒幕的資訊，請參閱 [使用不同的縮放檢視器預覽影像](previewing-image-assets-different-zoom.md#previewing_image_assets_with_different_zoom_viewers).

### 編輯縮放目標 {#editing-zoom-targets}

若要編輯縮放目標，請在「縮放目標編輯器」頁面上使用下列技術：

* **重新定位**  — 使用「選取目標」按鈕（箭頭），選取目標。 然后，将目标拖动到其他位置。

* **調整大小**  — 使用「選取目標」按鈕（箭頭），選取目標。 若要放大或縮小目標，請將指標移至縮放目標的一個角落並拖曳。

* **刪除**  — 選取畫面右側的目標縮圖影像。 然後選取 **[!UICONTROL 刪除目標]**.

* **重新命名**  — 選取畫面右側的目標縮圖影像。 然後，在 **[!UICONTROL 名稱]** 文字欄位並選取 **[!UICONTROL 儲存]**.

### 複製縮放目標 {#copying-zoom-targets}

可以将缩放目标从一个图像复制到另一个图像。如果两个图像的内容相似且缩放目标位于同一位置，则可复制目标。若要將縮放目標複製到另一個影像，請執行下列動作：

1. 在「縮放目標編輯器」畫面中，開啟含有您要複製的縮放目標的影像。
1. 選取 **[!UICONTROL 將目標複製到]**.
1. 在「選取影像」對話方塊中，選取影像並擇取 **[!UICONTROL 選取]**.
