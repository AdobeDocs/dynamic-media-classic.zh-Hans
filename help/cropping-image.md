---
title: 裁切图像
description: 瞭解如何在Adobe Dynamic Media Classic中裁切影像。
uuid: 84f199de-cbfc-4d06-877f-6e9148e82e15
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 99dfa476-4f11-4569-a27e-a76ed7787674
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: aec4c256-f5ed-4307-afec-dec848be95f9
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '550'
ht-degree: 35%

---

# 裁切图像{#cropping-an-image}

您可以在Adobe Dynamic Media Classic中裁切影像。 系统保留裁切图像的相关信息，以便您将它们恢复到初始状态。您还可以裁切某个图像，然后使用新名称保存裁切的版本。

您可以裁切图像以移除其周围的空白，或裁切图像的某个区域。

>[!NOTE]
>
>裁切之後，您可以選取 **[!UICONTROL 另存為]** 並使用不同的名稱儲存影像的裁切版本。 在「另存新檔」視窗中，選取 **[!UICONTROL 另存為新主版]** 以儲存影像的第二個復本。 選取 **[!UICONTROL 另存為主版的新增檢視]** 因此您可以使用不同的名稱來儲存原始版本及其裁切版本。 選取 **[!UICONTROL 取代原始檔案]** 刪除您從中裁切影像的原始檔案。 然後輸入影像的名稱，並選取 **[!UICONTROL 提交]**.

## 裁切以删除图像周围的空白区域 {#crop-to-remove-white-space-around-an-image}

您可以将图像边缘的透明或纯色像素区域裁切掉。

1. 若要裁切影像，請選取其滑鼠指向效果 **[!UICONTROL 編輯]** 按鈕，然後選取 **[!UICONTROL 裁切]**，或在「詳細資料檢視」的「瀏覽」面板中顯示，然後選取 **[!UICONTROL 裁切]** 按鈕。
1. 在「裁切編輯器」頁面上，執行下列任一項作業：

   * 若要修剪顏色畫素，請前往 **[!UICONTROL Trim]** > **[!UICONTROL 顏色]**. 在 **[!UICONTROL 依色彩自動裁切]** 對話方塊中，選取 **[!UICONTROL 轉角]** 選單，並選擇要裁切掉背景顏色的轉角。 然後輸入 **[!UICONTROL 容許度]** 從0到1的設定。 如果设置为 0，则仅裁切与图像角中选定颜色精确匹配的像素。数字越接近 1，允许的色差越大。選取 **[!UICONTROL 裁切]**.
   * 若要裁剪透明畫素，請移至 **[!UICONTROL Trim]** > **[!UICONTROL 透明]**. 在 **[!UICONTROL 依透明度自動裁切]** 對話方塊中，輸入從0到1的公差設定。 0設定只有在畫素為透明時，才會裁切畫素。 数字越接近 1，则裁切透明度越高的像素。選取 **[!UICONTROL 裁切]**.

1. 選取 **[!UICONTROL 儲存]**.

>[!NOTE]
>
>若要在裁切影像後將其還原為原始狀態，請在「裁切編輯器」畫面中顯示該影像，然後選取 **[!UICONTROL 重設]**.

## 选择要裁切的区域 {#select-an-area-to-crop}

1. 若要裁切影像，請選取其滑鼠指向效果 **[!UICONTROL 編輯]** 按鈕，然後選擇 **[!UICONTROL 裁切]**，或在「詳細資訊」檢視的「瀏覽」面板中顯示它，然後選取 **[!UICONTROL 裁切]**.

1. 在「裁切編輯器」視窗中，將您不想裁切的影像部分放置在裁切方塊中。 方塊內顯示的內容即為選取後所保留的內容 **[!UICONTROL 儲存]** 並裁切影像。
1. 要调整裁切区域，请执行以下任一操作：

   * 拖动框的一边或一角。拖动时，按住 Shift 键，以更改大小，但保持裁切框的高宽比（形状）不变。
   * 在“大小”框中输入像素大小。
   * 拖动以移动裁切框。将鼠标指针移动到该框边界内。当指针显示为四向箭头时，将裁切框拖动到图像上的新位置。

1. 選取 **[!UICONTROL 儲存]**.

>[!NOTE]
>
>若要在裁切影像後將其還原為原始狀態，請在「裁切編輯器」畫面中顯示該影像，然後選取 **[!UICONTROL 重設]**.

>[!MORELIKETHIS]
>
>* [上傳時影像編輯的選項](image-editing-options-upload.md#image-editing-options-at-upload)
>* [從PDF檔案裁切空白字元](pdfs.md#cropping_white_space_from_a_pdf_file)
>* [從PDF頁面側面裁切](pdfs.md#cropping_from_the_sides_of_pdf_pages)

