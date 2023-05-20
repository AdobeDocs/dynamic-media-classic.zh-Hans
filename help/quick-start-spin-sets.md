---
title: "快速入门：旋转集"
description: 迴轉集的簡介和快速入門，協助您在Adobe Dynamic Media Classic中快速上手並執行。
uuid: d0af9db6-cb6f-48f0-89f6-f3ab2da0659f
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/spin_sets
discoiquuid: 282b8e83-b20f-43f7-b9f8-6eebd5b1c5a7
feature: Dynamic Media Classic,Viewers,Spin Sets
role: User
exl-id: 26e3cd5b-f070-4b92-af36-25631723460e
source-git-commit: cb55e09a997b9d36002c4ac429603576d52fb8bd
workflow-type: tm+mt
source-wordcount: '839'
ht-degree: 22%

---

# 快速入门：旋转集{#quick-start-spin-sets}

旋转集用于模拟转动物品进行查看时的真实动作。利用旋转集能够从任意角度查看物品，从而获得任意角度的重要视觉详细信息。迴轉集可模擬360度的觀賞體驗。 Adobe Dynamic Media Classic提供檢視器可旋轉專案的一維迴轉集，以及檢視器可旋轉及翻轉專案的二維迴轉集。 此外，使用者只要按一下滑鼠幾下，即可「自由變形」縮放及平移任何檢視。 通过这种方式，用户能够以特定的视角，更仔细地查看物品。

![旋转集的图像。](/help/assets/spin_set.png)

旋转集也接受图像映射。图像映射是旋转集内的图像上用于显示含文本的变换面板的区域。当用户单击图像映射时，将触发某种操作。例如，将启动网页，供用户了解产品的更多相关信息。若要指出「迴轉集」中的影像對映，當使用者將滑鼠指標移到「影像對映」上時，就會在「影像對映」本身周圍出現輪廓。

另請參閱 [建立影像地圖](creating-image-maps.md).

另請參閱 [影像和迴轉集：Dynamic Imaging](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/556_Image%20&amp;%20Spin%20Sets_converted%20renamed_Dynamic%20Imaging-AVS) 訓練影片。

當您建立迴轉集時，Adobe會建議下列最佳作法並強制實行下列限制：

| 迴轉集限制型別 | 最佳实践 | 強制限制 |
| --- | --- | --- |
| 每個2D集的最大列數/欄數 | 每組12-18個影像 | 1000 |

另請參閱 [Dynamic Media限制](/help/limitations.md).

此迴轉集快速入門旨在讓您快速上手並執行Adobe Dynamic Media Classic中的迴轉集技術。 按照步骤 1 到 7 操作。在每個步驟結束時，您可以選取主題連結來瞭解更多資訊。

## 1.建立及上傳影像

一維「迴轉集」至少需要8-12個專案快照，二維「迴轉集」至少需要16-24個專案快照。 拍摄照片时必须间隔一定的角度，以便让人感觉物品正在旋转和翻转。例如，如果一維「迴轉集」包含12個鏡頭，則每個鏡頭應將專案旋轉30° (360°/12)。

在全域導覽列上，選取 **[!UICONTROL 上傳]** 將迴轉影像從您的電腦或網路上傳至Adobe Dynamic Media Classic。

请参阅[旋转集图像拍摄指南](creating-spin-set.md#guidelines-for-shooting-spin-set-images)。

## 2.建立迴轉集

若要建立迴轉集，請在全域導覽列上，前往 **[!UICONTROL 建置]** > **[!UICONTROL 迴轉集]**. 在「迴轉集大小」對話方塊中，選擇所需的列數和儲存格數，然後選取 **[!UICONTROL 確定]**. 然後將影像拖曳至「迴轉集」頁面上的格線中。

另請參閱 [建立迴轉集](creating-spin-set.md#creating-a-spin-set).

## 3.編輯迴轉集

若要編輯迴轉集，請在全域導覽列上，前往 **[!UICONTROL 設定]** > **[!UICONTROL 檢視器預設集]**. 選取迴轉集，然後選取 **[!UICONTROL 編輯]**. 添加、删除和更改图像的位置。您可以更改二维旋转集中行的位置。

另請參閱 [編輯迴轉集](creating-spin-set.md#editing-a-spin-set).

## 4.設定迴轉集檢視器預設集

管理员可以创建旋转集查看器预设。这些预设决定了旋转集查看器的外观。若要設定新的「迴轉集檢視器預設集」，請在全域導覽列上，前往 **[!UICONTROL 設定]** > **[!UICONTROL 檢視器預設集]**.

在「檢視器預設集」頁面上，選取 **[!UICONTROL 新增]**，然後選取 **[!UICONTROL 迴轉集檢視器]** 從下拉式清單中，然後選取 **[!UICONTROL 新增]**. 在「設定檢視器」頁面中選擇選項，然後選取 **[!UICONTROL 儲存]**.

另請參閱 [設定迴轉集檢視器預設集](setting-spin-set-viewer-presets.md#setting-up-spin-set-viewer-presets).

## 5.預覽迴轉集

在瀏覽面板中選取您的迴轉集，然後選取 **[!UICONTROL 預覽]**. 在「預覽」頁面上，按住滑鼠鍵並向左或向右拖曳指標，以視覺上「旋轉」專案。

另請參閱 [預覽迴轉集](previewing-spin-set.md#previewing-a-spin-set).

## 6.發佈迴轉集

發佈迴轉集時會將其置於Adobe Dynamic Media Classic伺服器上，以便動態傳送至您的網站或應用程式。 它也會啟用URL字串，從Dynamic Media影像伺服器將迴轉集呼叫至您的網站或應用程式。

若要發佈迴轉集，請選取 **[!UICONTROL 標籤為發佈]** 圖示加以識別。 在全域導覽列上，選取 **[!UICONTROL 發佈]** 以啟動發佈。 在「發佈」畫面上，選取「 」 **[!UICONTROL 提交發佈]**.

另請參閱 [發佈迴轉集](publishing-spin-set.md#publishing-a-spin-set).

## 7.將迴轉集連結至網頁

Adobe Dynamic Media Classic會為迴轉集建立URL圖說文字串，並在您發佈後加以啟用。 您可以從預覽頁面複製這些URL。

選取「迴轉集」，然後選取 **[!UICONTROL 預覽]**. 选择旋转集查看器预设。然後選取 **[!UICONTROL 複製URL]**.

另請參閱 [將迴轉集連結至網頁](linking-spin-set-web-page.md#linking-a-spin-set-to-a-web-page).
