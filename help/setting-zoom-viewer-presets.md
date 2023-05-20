---
title: 設定縮放檢視器預設集
description: 瞭解如何在Adobe Dynamic Media Classic中設定縮放檢視器預設集。
uuid: 202d80cb-8282-45d4-89e8-942c8677aa93
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/zoom
discoiquuid: 5023a933-e229-4d3c-8e91-3ac5e9f4970b
feature: Dynamic Media Classic,Viewers,Zoom
role: User
exl-id: ddaaff6c-5447-408e-9c92-bcdfd1a0e72e
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '613'
ht-degree: 47%

---

# 設定縮放檢視器預設集{#setting-up-zoom-viewer-presets}

缩放查看器预设可确定缩放查看器的样式、行为和外观。Adobe Dynamic Media Classic提供許多自訂檢視器及為其設定外觀的選項。 Adobe Dynamic Media Classic隨附預設基本（快速）、彈出和自訂縮放檢視器預設集。 如果您是管理員，可以建立公司「縮放檢視器預設集」或編輯預設集，並使用新名稱儲存它。

所有缩放查看器都带有用于放大、缩小、平移并在缩放后将图像重置为原始状态的按钮。這些按鈕的外觀和視窗本身的顯示方式取決於您選擇的縮放檢視器預設集。 您可以使用不同的颜色、边框、字体及图像设置来配置缩放查看器预设。配置引导式缩放查看器时，还可以选择缩放目标的放置位置。缩放目标指的是用户单击后可缩放到指定区域的缩略图。

## 关于缩放查看器预设 {#about-zoom-viewer-presets}

Adobe Dynamic Media Classic提供下列縮放檢視器預設集：

* **縮放檢視器：基本**  — 提供原始影像的基本縮放。

* **縮放檢視器：彈出**  — 在原始影像旁顯示縮放區域的第二個影像。 没有控件可以使用，用户只需将选取范围移动到他们要查看的区域上即可。

在确定此查看器的完整带宽使用量时，请考虑在查看器中有主图像和弹出图像。弹出图像大小取决于主图像大小（舞台宽度和高度）和缩放因子。为防止弹出文件大小变得太大，需对这两个值进行平衡：如果您的主图像大小很大，请降低缩放系数值。（弹出宽度和弹出高度决定了弹出窗口的大小，但不决定提供给查看器的弹出图像的大小。）

例如，如果您的主图像大小是 350 X 350 像素，缩放系数为 3，则生成的弹出图像是 1050 X 1050 像素。如果您的主图像大小是 300 X 300 像素，缩放系数为 4，则弹出图像是 1200 X 1200 像素。根据 JPEG 品质设置（推荐的设置介于 80-90），您可以显著地减少文件大小。建议的缩放系数为 2.5 至 4，取决于您的主图像的大小。

Adobe Dynamic Media Classic建議您將下列引數用於彈出式縮放檢視器預設集：

* **放大的影像大小**  — 大約1500 x 1500畫素，不超過2000 x 2000畫素。

* **影像大小** - 100 KB以下，不得超過150 KB （壓縮檔案使其低於150 KB）。

* **縮放檢視器：自訂**  — 提供具有影像、具有多個檢視的影像集或色票集的引導式或無引導式縮放。

## 建立和編輯縮放檢視器預設集 {#creating-and-editing-zoom-viewer-presets}

1. 在全域導覽列上，前往 **[!UICONTROL 設定]** > **[!UICONTROL 檢視器預設集]**.
1. 执行以下任一操作：

   * **建立預設集**  — 選取 **[!UICONTROL 新增]**. 在「新增檢視器預設集」對話方塊中，選擇平台、縮放檢視器，然後選取 **[!UICONTROL 新增]**. 在「預設集名稱」方塊中輸入預設集名稱。

   * **編輯預設集**  — 選取縮放檢視器預設集，然後選取「 」 **[!UICONTROL 編輯]**.

1. 根据需要指定设置。

   若要檢視選項的說明，請選取 **[!UICONTROL 資訊提示]** 圖示加以存取。

   當您更新和變更設定時，「預覽」頁面會顯示檢視器。

1. 選取 **[!UICONTROL 儲存]** 或 **[!UICONTROL 另存為]**.
1. 在「檢視器預設集」頁面上，檢查您建立的縮放檢視器預設集或引導式縮放檢視器預設集。 如果需要調整，請選取 **[!UICONTROL 編輯]**，變更「設定檢視器」頁面上的設定，然後選取 **[!UICONTROL 儲存]**.

有关在“查看器预设”屏幕上管理查看器预设的信息，请参阅[查看器预设](application-setup.md#viewer_presets)。

>[!MORELIKETHIS]
>
>* [建立和編輯檢視器預設集](application-setup.md#adding_and_editing_viewer_presets)

