---
title: 裁切图像
description: 了解如何裁剪图像。
uuid: 84f199de-cbfc-4d06-877f-6e9148e82e15
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 99dfa476-4f11-4569-a27e-a76ed7787674
feature: Dynamic Media Classic，资产管理
role: Business Practitioner
exl-id: aec4c256-f5ed-4307-afec-dec848be95f9
translation-type: tm+mt
source-git-commit: 4e79c98b92dfa4e1a9890ed8a291cdf564126466
workflow-type: tm+mt
source-wordcount: '543'
ht-degree: 51%

---

# 裁切图像{#cropping-an-image}

您可以在Dynamic Media Classic中裁切图像。 系统保留裁切图像的相关信息，以便您将它们恢复到初始状态。您还可以裁切某个图像，然后使用新名称保存裁切的版本。

您可以裁切图像以移除其周围的空白，或裁切图像的某个区域。

>[!NOTE]
>
>裁切后，您可以单击“另存为”按钮，使用其他名称保存图像的裁切版本。在“另存为”窗口中，选择“另存为新的主页”保存图像的另外一个副本。单击&#x200B;**[!UICONTROL 主控]**&#x200B;的“另存为附加视图”，以用其他名称保存原始版本及其裁剪版本。 单击&#x200B;**[!UICONTROL 替换原稿]**&#x200B;以删除您从中裁剪图像的原始文件。 然后输入图像的名称，并单击&#x200B;**[!UICONTROL 提交]**。

## 裁切以删除图像周围的空白区域 {#crop-to-remove-white-space-around-an-image}

您可以将图像边缘的透明或纯色像素区域裁切掉。

1. 要裁剪图像，请单击其翻转&#x200B;**[!UICONTROL 编辑]**&#x200B;按钮并选择&#x200B;**[!UICONTROL 裁剪]**，或在浏览面板中以详细视图显示图像，然后单击&#x200B;**[!UICONTROL 裁剪]**&#x200B;按钮。
1. 在“裁剪编辑器”页面上，执行下列操作之一：

   * 要修剪颜色像素，请单击&#x200B;**[!UICONTROL “修剪]**”>“**[!UICONTROL 颜色]**”。 此时将显示“按颜色自动裁切”对话框。单击&#x200B;**[!UICONTROL Corner]**&#x200B;菜单，并选择一个带有背景色的角以裁切掉。 然后输入从0到1的&#x200B;**[!UICONTROL 容差]**&#x200B;设置。 如果设置为 0，则仅裁切与图像角中选定颜色精确匹配的像素。数字越接近 1，允许的色差越大。单击&#x200B;**[!UICONTROL 裁剪]**&#x200B;按钮。
   * 要裁切透明像素，请选择单击&#x200B;**[!UICONTROL 裁切]** > **[!UICONTROL 透明]**。 此时将显示“根据透明度自动裁切”对话框。输入容差设置，范围为 0 至 1。0设置仅在像素透明时裁剪像素。 数字越接近 1，则裁切透明度越高的像素。单击&#x200B;**[!UICONTROL 裁剪]**。

1. 单击“**[!UICONTROL 保存]**”。

>[!NOTE]
>
>要在裁剪图像后将其恢复到原始状态，请在“裁剪编辑器”屏幕中显示该图像，然后单击&#x200B;**[!UICONTROL 重置]**。

## 选择要裁切的区域 {#select-an-area-to-crop}

1. 要裁剪图像，请单击其翻转&#x200B;**[!UICONTROL 编辑]**&#x200B;按钮，然后选择&#x200B;**[!UICONTROL 裁剪]**，或在“浏览面板”中以详细视图显示图像，然后单击&#x200B;**[!UICONTROL 裁剪]**。

1. 在“裁剪编辑器”窗口中，将不想裁剪的图像部分放在裁剪框中。 框内显示的内容是单击&#x200B;**[!UICONTROL 保存]**&#x200B;并裁剪图像时保留的内容。
1. 要调整裁切区域，请执行以下任一操作：

   * 拖动框的一边或一角。拖动时，按住 Shift 键，以更改大小，但保持裁切框的高宽比（形状）不变。
   * 在“大小”框中输入像素大小。
   * 拖动以移动裁切框。将鼠标指针移动到该框边界内。当指针显示为四向箭头时，将裁切框拖动到图像上的新位置。

1. 单击“**[!UICONTROL 保存]**”。

>[!NOTE]
>
>要在裁剪后将图像恢复到其原始状态，请在“裁剪编辑器”屏幕中显示该图像，然后单击&#x200B;**[!UICONTROL 重置]**。

>[!MORELIKETHIS]
>
>* [上载时的图像编辑选项](image-editing-options-upload.md#image-editing-options-at-upload)
>* [从 PDF 文件中裁切空白区域](pdfs.md#cropping_white_space_from_a_pdf_file)
>* [从 PDF 页边裁切](pdfs.md#cropping_from_the_sides_of_pdf_pages)

