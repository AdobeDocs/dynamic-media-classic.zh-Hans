---
title: 裁切图像
description: 了解如何在AdobeDynamic Media Classic中裁剪图像。
uuid: 84f199de-cbfc-4d06-877f-6e9148e82e15
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 99dfa476-4f11-4569-a27e-a76ed7787674
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: aec4c256-f5ed-4307-afec-dec848be95f9
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '550'
ht-degree: 35%

---

# 裁切图像{#cropping-an-image}

您可以在AdobeDynamic Media Classic中裁剪图像。 系统保留裁切图像的相关信息，以便您将它们恢复到初始状态。您还可以裁切某个图像，然后使用新名称保存裁切的版本。

您可以裁切图像以移除其周围的空白，或裁切图像的某个区域。

>[!NOTE]
>
>裁剪后，您可以选择&#x200B;**[!UICONTROL 另存为]**，然后使用其他名称保存图像的裁剪版本。 在“另存为”窗口中，选择&#x200B;**[!UICONTROL 另存为新主控]**&#x200B;以保存图像的第二个副本。 选择&#x200B;**[!UICONTROL Save As Addition View Of 主控]**，以便您可以使用其他名称保存原始版本及其裁剪版本。 选择&#x200B;**[!UICONTROL 替换原始文件]**&#x200B;以删除您从中裁剪图像的原始文件。 然后输入图像的名称，并选择&#x200B;**[!UICONTROL Submit]**。

## 裁切以删除图像周围的空白区域 {#crop-to-remove-white-space-around-an-image}

您可以将图像边缘的透明或纯色像素区域裁切掉。

1. 要裁剪图像，请选择其滚动图像&#x200B;**[!UICONTROL 编辑]**&#x200B;按钮，然后选择&#x200B;**[!UICONTROL 裁剪]**，或在“详细信息视图”的“浏览面板”中显示该图像，然后选择&#x200B;**[!UICONTROL 裁剪]**&#x200B;按钮。
1. 在“裁剪编辑器”页面上，执行以下操作之一：

   * 要裁切颜色像素，请转到&#x200B;**[!UICONTROL Trim]** > **[!UICONTROL Color]**。 在&#x200B;**[!UICONTROL 自动按颜色裁剪]**&#x200B;对话框中，选择&#x200B;**[!UICONTROL 角]**&#x200B;菜单，然后选择背景颜色要裁剪掉的角。 然后输入从0到1的&#x200B;**[!UICONTROL 容差]**&#x200B;设置。 如果设置为 0，则仅裁切与图像角中选定颜色精确匹配的像素。数字越接近 1，允许的色差越大。选择&#x200B;**[!UICONTROL 裁剪]**。
   * 要裁切透明像素，请转到&#x200B;**[!UICONTROL Trim]** > **[!UICONTROL Transparent]**。 在&#x200B;**[!UICONTROL 透明度自动裁剪]**&#x200B;对话框中，输入从0到1的公差设置。 0设置仅会在像素透明时裁剪像素。 数字越接近 1，则裁切透明度越高的像素。选择&#x200B;**[!UICONTROL 裁剪]**。

1. 选择&#x200B;**[!UICONTROL Save]**。

>[!NOTE]
>
>要在裁剪图像后将其恢复为原始状态，请在“裁剪编辑器”屏幕中显示该图像，然后选择&#x200B;**[!UICONTROL 重置]**。

## 选择要裁切的区域 {#select-an-area-to-crop}

1. 要裁剪图像，请选择其滚动图像&#x200B;**[!UICONTROL 编辑]**&#x200B;按钮，然后选择&#x200B;**[!UICONTROL 裁剪]**，或在“详细信息视图”的“浏览面板”中显示图像，然后选择&#x200B;**[!UICONTROL 裁剪]**。

1. 在“裁剪编辑器”窗口中，将不想裁剪的图像部分放入裁剪框中。 选择&#x200B;**[!UICONTROL 保存]**&#x200B;并裁剪图像后，框内显示的内容将保留。
1. 要调整裁切区域，请执行以下任一操作：

   * 拖动框的一边或一角。拖动时，按住 Shift 键，以更改大小，但保持裁切框的高宽比（形状）不变。
   * 在“大小”框中输入像素大小。
   * 拖动以移动裁切框。将鼠标指针移动到该框边界内。当指针显示为四向箭头时，将裁切框拖动到图像上的新位置。

1. 选择&#x200B;**[!UICONTROL Save]**。

>[!NOTE]
>
>要在裁剪图像后将其恢复为原始状态，请在“裁剪编辑器”屏幕中显示该图像，然后选择&#x200B;**[!UICONTROL 重置]**。

>[!MORELIKETHIS]
>
>* [上传时用于图像编辑的选项](image-editing-options-upload.md#image-editing-options-at-upload)
>* [从PDF文件裁剪空格](pdfs.md#cropping_white_space_from_a_pdf_file)
>* [从PDF页面的侧边裁剪](pdfs.md#cropping_from_the_sides_of_pdf_pages)

