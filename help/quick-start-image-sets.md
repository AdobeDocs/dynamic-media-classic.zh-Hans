---
title: "快速入门：图像集"
description: 影像集簡介和快速入門，可幫助您快速上手並執行Adobe Dynamic Media Classic中的影像集技術。
uuid: daf17d13-9c06-41f0-8fc5-2e56d460d341
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sets
discoiquuid: 612a425f-2840-46c4-8e5a-c0bc5f738f4e
feature: Dynamic Media Classic,Viewers,Image Sets
role: User
exl-id: 280e7201-84d6-46b1-94bb-0499beca2992
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '673'
ht-degree: 21%

---

# 快速入门：图像集{#quick-start-image-sets}

Adobe Dynamic Media Classic影像集為使用者提供整合式檢視體驗。 在动态图像集查看器中，用户单击缩略图图像便可以看到物品的各种不同视图。「影像集」可讓您呈現專案的替代高解析度檢視。

图像集查看器具有缩放工具，可用来仔细查看图像。如果需要，可以将引导式缩放目标和图像映射添加到图像集中。图像集可为用户带来更协调、更详尽的观看体验。

另請參閱 [影像和迴轉集：Dynamic Imaging](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/556_Image%20&amp;%20Spin%20Sets_converted%20renamed_Dynamic%20Imaging-AVS) 訓練影片。

建立影像集時，Adobe會建議下列最佳作法並強制實行下列限制：

| 限制型別 | 最佳实践 | 強制限制 |
| --- | --- | --- |
| 每個集的重複資產數量 | 無重複專案 | 20 |
| 每組影像的最大數量 | 每組5至10個影像 | 1000 |

另請參閱 [Dynamic Media限制](/help/limitations.md).

下列影像集快速入門旨在讓您快速上手，並運用Adobe Dynamic Media Classic中的影像集技術。

## 1.上傳您的主要影像以供多個檢視和色票使用

首先要向图像集上载图像。由於使用者可以在影像集檢視器中放大影像，因此在選擇影像時，請務必說明此功能的重要性。 請確定影像的大小至少為2000畫素。 Adobe Dynamic Media Classic支援許多影像檔案格式，但建議使用不失真TIFF、PNG和EPS影像。

在全域導覽列上，選取 **[!UICONTROL 上傳]** 將檔案從電腦上傳至Adobe Dynamic Media Classic上的資料夾。

另請參閱 [準備影像集資產以供上傳](preparing-image-set-assets-upload.md#preparing-image-set-assets-for-upload) 和 [上傳您的檔案](uploading-files.md#uploading-your-files).

## 2.建立影像集

在「影像集」中，使用者可在「影像集檢視器」中選取縮圖影像，以從不同側面或角度檢視影像。

若要建立影像集，請在全域導覽列上選取 **[!UICONTROL 建置]**，然後選擇 **[!UICONTROL 影像集]**. 在「影像集」視窗上，將影像拖曳至頁面以構成影像集。 根据需要组织、添加和删除图像。

另請參閱 [建立影像集](creating-image-set.md#creating-an-image-set).

另請參閱 [在影像集中包含縮放目標和影像地圖](/help/including-zoom-targets-image-maps-image-sets.md)

## 3.視需要準備影像集檢視器預設集

管理员可以创建或修改图像集查看器预设。Adobe Dynamic Media Classic隨附每個多媒體型別的預設檢視器預設集。 使用縮放檢視器： **[!UICONTROL 自訂]** > **[!UICONTROL 影像]** 或 **[!UICONTROL 影像集]**/**[!UICONTROL 多個檢視]** 用來檢視影像集的預設集。

可在“应用程序设置”屏幕中添加或编辑查看器预设。

另請參閱 [建立和編輯檢視器預設集](application-setup.md#adding-and-editing-viewer-presets).

## 4.預覽影像集

在「瀏覽」面板中選取「影像集」，然後選取 **[!UICONTROL 預覽]**. 在「預覽」頁面中，選取縮圖圖示以在選取的檢視器中檢查影像集。 可以从“预设”菜单中选择不同的查看器。

另請參閱 [預覽資產](previewing-asset.md#previewing-an-asset).

## 5.發佈影像集

發佈影像集時會將其置於Adobe Dynamic Media Classic伺服器上並啟動URL字串。

>[!NOTE]
>
>如果在创建并保存图像集时选择了“**[!UICONTROL 保存后发布]**”（默认），则不需要执行此步骤。

選取 **[!UICONTROL 標籤為發佈]** 圖示加以識別，並加以識別。 然後，選取 **[!UICONTROL 發佈]**. 在發佈頁面上，選取 **[!UICONTROL 提交發佈]**.

另請參閱 [發佈檔案](publishing-files.md#publishing-files).

## 6.將影像集連結至您的網站

Adobe Dynamic Media Classic會為影像集建立URL呼叫，並在您發佈後啟用。 可以从“预览”屏幕复制这些 URL。

選取「影像集」，然後選取 **[!UICONTROL 預覽]**. 現在選取「影像集檢視器預設集」，然後選取 **[!UICONTROL 複製URL]**.

另請參閱 [將影像集連結至網頁](linking-image-set-web-page.md#linking-an-image-set-to-a-web-page).
