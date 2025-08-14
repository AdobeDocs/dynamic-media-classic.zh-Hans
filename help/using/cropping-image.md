---
title: 裁切图像
description: 了解如何在Adobe Dynamic Media Classic中裁切图像。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: aec4c256-f5ed-4307-afec-dec848be95f9
topic: Content Management
level: Intermediate
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '557'
ht-degree: 31%

---

# 裁切图像{#cropping-an-image}

您可以在Adobe Dynamic Media Classic中裁切图像。 系统保留裁切图像的相关信息，以便您将它们恢复到初始状态。您还可以裁切某个图像，然后使用新名称保存裁切的版本。

您可以裁切图像以移除其周围的空白，或裁切图像的某个区域。

>[!NOTE]
>
>裁剪后，您可以选择&#x200B;**[!UICONTROL 另存为]**&#x200B;并以其他名称保存该图像的裁剪版本。 在“另存为”窗口中，选择&#x200B;**[!UICONTROL 另存为新主映像]**&#x200B;以保存该映像的第二个副本。 选择&#x200B;**[!UICONTROL 另存为主]**&#x200B;的添加视图，以便使用其他名称保存原始版本及其裁切版本。 选择&#x200B;**[!UICONTROL 替换原始]**&#x200B;以删除从中裁剪图像的原始文件。 然后输入映像的名称，并选择&#x200B;**[!UICONTROL 提交]**。

## 裁切以删除图像周围的空白区域 {#crop-to-remove-white-space-around-an-image}

您可以将图像边缘的透明或纯色像素区域裁切掉。

1. 要裁切图像，请选择图像的变换图像&#x200B;**[!UICONTROL 编辑]**&#x200B;按钮，然后选择&#x200B;**[!UICONTROL 裁切]**，或在“详细信息”视图的“浏览”面板中显示该图像，然后选择&#x200B;**[!UICONTROL 裁切]**&#x200B;按钮。
1. 在裁切编辑器页面上，执行以下操作之一：

   * 若要修剪颜色像素，请转到&#x200B;**[!UICONTROL 修剪]** > **[!UICONTROL 颜色]**。 在&#x200B;**[!UICONTROL 按颜色自动裁切]**&#x200B;对话框中，选择&#x200B;**[!UICONTROL 角点]**&#x200B;菜单，然后选择要裁切掉的具有背景颜色的角点。 然后输入从0到1的&#x200B;**[!UICONTROL 容差]**&#x200B;设置。 如果设置为 0，则仅裁切与图像角中选定颜色精确匹配的像素。数字越接近 1，允许的色差越大。选择&#x200B;**[!UICONTROL 裁切]**。
   * 若要修剪透明像素，请转到&#x200B;**[!UICONTROL 修剪]** > **[!UICONTROL 透明]**。 在&#x200B;**[!UICONTROL 按透明度自动裁切]**&#x200B;对话框中，输入从0到1的容差设置。 0设置仅在像素为透明时才裁剪像素。 数字越接近 1，则裁切透明度越高的像素。选择&#x200B;**[!UICONTROL 裁切]**。

1. 选择&#x200B;**[!UICONTROL 保存]**。

>[!NOTE]
>
>要在裁切图像后将其恢复到原始状态，请在“裁切编辑器”屏幕中显示该图像，然后选择&#x200B;**[!UICONTROL 重置]**。

## 选择要裁切的区域 {#select-an-area-to-crop}

1. 要裁切图像，请选择图像的变换图像&#x200B;**[!UICONTROL 编辑]**&#x200B;按钮，然后选择&#x200B;**[!UICONTROL 裁切]**，或在“详细信息”视图的“浏览”面板中显示该图像，然后选择&#x200B;**[!UICONTROL 裁切]**。

1. 在“裁切编辑器”窗口中，将您不希望裁切的图像部分放入裁切框中。 选择保存&#x200B;**[!UICONTROL 并裁切图像后，框内显示的内容将保持不变。]**
1. 要调整裁切区域，请执行以下任一操作：

   * 拖动框的一边或一角。拖动时按住Shift键可更改裁切框的大小，但保持其长宽比（形状）。
   * 在“大小”框中输入像素大小。
   * 拖动以移动裁切框。将鼠标指针移动到该框边界内。当指针显示为四向箭头时，将裁切框拖动到图像上的新位置。

1. 选择&#x200B;**[!UICONTROL 保存]**。

>[!NOTE]
>
>要在裁切图像后将其恢复到原始状态，请在“裁切编辑器”屏幕中显示该图像，然后选择&#x200B;**[!UICONTROL 重置]**。

>[!MORELIKETHIS]
>
>* 在上传时进行[图像编辑的选项](image-editing-options-upload.md#image-editing-options-at-upload)
>* [从PDF文件裁切空格](pdfs.md#cropping_white_space_from_a_pdf_file)
>* [从PDF页面侧面裁切](pdfs.md#cropping_from_the_sides_of_pdf_pages)
