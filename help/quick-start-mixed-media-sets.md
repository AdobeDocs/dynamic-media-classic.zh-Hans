---
title: 「快速入門：混合媒體集」
description: 介紹和快速入門混合媒體集，協助您在Adobe Dynamic Media Classic中快速上手並執行。
uuid: 0ef033d5-b053-4d7c-b1e1-1980f899fd88
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/mixed_media_sets
discoiquuid: 2708d077-94fc-4045-8992-ad3589ed9cfd
feature: Dynamic Media Classic,Viewers,Mixed Media Sets
role: User
exl-id: 757893ae-7507-42a0-a67b-f6542e7231c7
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '701'
ht-degree: 34%

---

# 快速入门：混合媒体集{#quick-start-mixed-media-sets}

 混合媒体集为用户提供了集成的查看体验。混合媒体集可以包括图像、图像集、样本集、旋转集和视频。使用者可以在混合媒體檢視器中選取不同的標籤，以檢視不同檢視器中的專案。 如果未指定选项卡，所有资源都将一起显示在样本行中。

“混合媒体集查看器预设”包括最终用户用来嵌入代码、复制 URL 以及链接到主网站的社区选项。用户可以使用这些选项在其个人网站或社交网站上共享有关产品的信息。

此混合媒體集快速入門旨在讓您快速上手，並運用Adobe Dynamic Media Classic中的混合媒體集技術。

## 1.上傳影像、色票檔案和影片

首先为混合媒体集上载图像、样本文件和视频。由於使用者可以在混合媒體集檢視器中放大影像，因此選擇影像時，請務必說明此功能的重要性。 請確定影像的大小至少為2000畫素。

在全域導覽列上，選取 **[!UICONTROL 上傳]** 將檔案從電腦上傳至Adobe Dynamic Media Classic上的資料夾。

另請參閱 [上傳您的檔案](uploading-files.md#uploading-your-files).

## 2.建立媒體集，以便在混合媒體集中使用

可以将图像、图像集、样本集、旋转集和视频添加到混合媒体集中。先准备好媒体集，然后再将其添加到混合媒体集中。

另請參閱 [建立影像集](creating-image-set.md#creating-an-image-set)， [建立色票集](creating-swatch-set.md#creating-a-swatch-set)、和 [建立迴轉集](creating-spin-set.md#creating-a-spin-set).

## 3.建立混合媒體集

在全域導覽列上，前往 **[!UICONTROL 建置]** > **[!UICONTROL 混合媒體集]**. 將影像、色票集、影像集和視訊拖曳至「混合媒體集」頁面。 要添加音轨，将音频文件拖动到“音轨”框中。

另請參閱 [建立混合媒體集](creating-mixed-media-set.md#creating-a-mixed-media-set).

## 4.設定混合媒體檢視器預設集

Adobe Dynamic Media Classic隨附混合媒體集的預設檢視器預設集。 管理员可以创建或修改混合媒体集查看器预设。

設定混合媒體集檢視器預設集時，請為檢視器集中的所有其他資產新增檢視器預設集。 例如，如果混合媒体集包括视频，则在混合媒体查看器预设中添加视频查看器预设。也可以将音轨添加到查看器中。该音轨在查看器打开时播放，但在视频处于活动状态时不播放。

另請參閱 [設定混合媒體集檢視器預設集](setting-mixed-media-set-viewer.md#setting-up-a-mixed-media-set-viewer-preset) 和 [建立和編輯檢視器預設集](application-setup.md#adding-and-editing-viewer-presets).

另請參閱 [檢視器預設集](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/550_viewer-presets_converted%20renamed_Done-AVS) 訓練影片。

## 5.預覽混合媒體集

選取混合媒體集的 **[!UICONTROL 預覽]** 按鈕。 您可以選取縮圖和色票圖示，在混合媒體集檢視器中檢查混合媒體集。 可以从“预设”菜单中选择不同的查看器。

另請參閱 [預覽資產](previewing-asset.md#previewing-an-asset).

## 6.發佈混合媒體集

發佈混合媒體集時會將其置於Adobe Dynamic Media Classic伺服器上並啟動URL字串。

混合媒体集要求同时发布到&#x200B;**视频服务器**&#x200B;和&#x200B;**图像服务器**。使用&#x200B;**视频服务器**&#x200B;发布已标记为发布的实际视频。而且，您會使用 **影像伺服器** 以發佈相關資產（例如視訊縮圖），並為任何最適化視訊集設定資訊。

另請參閱 [發佈混合媒體集](publishing-mixed-media-set.md#publishing-a-mixed-media-set).

## 7.將混合媒體集連結至網頁

Adobe Dynamic Media Classic會在您發佈混合媒體集後為其啟用URL呼叫。 您可以從預覽頁面複製這些URL。

選取混合媒體集，然後選取 **[!UICONTROL 預覽]**. 在「預覽」頁面中，選取「混合媒體集檢視器預設集」，然後選取 **[!UICONTROL 複製URL]**. 请参阅[将混合媒体集与网页链接](linking-mixed-media-set-web.md#linking-a-mixed-media-set-to-a-web-page)。
