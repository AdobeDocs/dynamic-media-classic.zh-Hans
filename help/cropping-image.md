---
title: 裁切图像
seo-title: 裁切图像
description: 'null'
seo-description: 了解如何裁剪图像。
uuid: 84f199de-cbfc-4d06-877f-6e9148e82e15
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 99dfa476-4f11-4569-a27e-a76ed7787674
translation-type: tm+mt
source-git-commit: b8d245bfc8375966af314ed95e81a519c5ee6c24

---


# 裁切图像{#cropping-an-image}

您可以在 Scene7 Publishing System 中裁切图像。系统保留裁切图像的相关信息，以便您将它们恢复到初始状态。您还可以裁切某个图像，然后使用新名称保存裁切的版本。

您可以裁切图像以移除其周围的空白，或裁切图像的某个区域。

>[!NOTE]
>
>裁切后，您可以单击“另存为”按钮，使用其他名称保存图像的裁切版本。在“另存为”窗口中，选择“另存为新的主页”保存图像的另外一个副本。选择“另存为主页的其他视图”保存原始版本同时使用其他名称保存裁切版本。选择“替换原始”删除裁切图像所用的原始文件。然后输入图像的名称并选择“提交”按钮。

## 裁切以删除图像周围的空白区域 {#crop-to-remove-white-space-around-an-image}

您可以将图像边缘的透明或纯色像素区域裁切掉。

1. 要裁切图像，请单击其变换“编辑”按钮，并选择“裁切”，或者在浏览面板的详细信息视图中显示图像，并单击“裁切”按钮 。将打开“裁切编辑器”屏幕。
1. 执行以下任一操作：

   * 要修剪颜色像素，请选择“修剪”菜单并选择“颜色”。此时将显示“按颜色自动裁切”对话框。选择“角”菜单，并选择具有要裁切掉的背景颜色的角。然后输入容差设置，范围为 0 至 1。如果设置为 0，则仅裁切与图像角中选定颜色精确匹配的像素。数字越接近 1，允许的色差越大。选择“裁切”按钮。
   * 要修剪透明像素，请选择“修剪”菜单并选择“透明”。此时将显示“根据透明度自动裁切”对话框。输入容差设置，范围为 0 至 1。如果设置为 0，则仅裁切完全透明的像素。数字越接近 1，则裁切透明度越高的像素。选择“裁切”按钮。

1. 单击“**保存**”。

>[!NOTE]
>
>在裁切图像之后，如果要将其恢复为原始状态，请在“裁切编辑器”屏幕中显示该图像并选择“重置”按钮。

## 选择要裁切的区域 {#select-an-area-to-crop}

1. To crop an image, click its rollover Edit button and choose **Crop**, or display it in the Browse Panel in Detail view and click **Crop**.

1. 在“裁剪编辑器”窗口中，将不想裁剪的图像部分放在裁剪框中。 What appears inside the box remains when you click **Save** and crop the image.
1. 要调整裁切区域，请执行以下任一操作：

   * 拖动框的一边或一角。拖动时，按住 Shift 键，以更改大小，但保持裁切框的高宽比（形状）不变。
   * 在“大小”框中输入像素大小。
   * 拖动以移动裁切框。将鼠标指针移动到该框边界内。当指针显示为四向箭头时，将裁切框拖动到图像上的新位置。

1. 单击“**保存**”。

>[!NOTE]
>
>在裁切图像之后，如果要将其恢复为原始状态，请在“裁切编辑器”屏幕中显示该图像并选择“重置”按钮。

>[!MORELIKETHIS]
>
>* [上载时的图像编辑选项](image-editing-options-upload.md#image-editing-options-at-upload)
>* [从 PDF 文件中裁切空白区域](pdfs.md#cropping_white_space_from_a_pdf_file)
>* [从 PDF 页边裁切](pdfs.md#cropping_from_the_sides_of_pdf_pages)

