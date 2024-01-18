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
source-git-commit: ae7d0c6d3047d68ed3da4187ef516dc51c95de30
workflow-type: tm+mt
source-wordcount: '557'
ht-degree: 35%

---

# 裁切图像{#cropping-an-image}

您可以在Adobe Dynamic Media Classic中裁切图像。 系统保留裁切图像的相关信息，以便您将它们恢复到初始状态。您还可以裁切某个图像，然后使用新名称保存裁切的版本。

您可以裁切图像以移除其周围的空白，或裁切图像的某个区域。

>[!NOTE]
>
>裁切后，您可以选择 **[!UICONTROL 另存为]** 并使用其他名称保存该图像的裁剪版本。 在“另存为”窗口中，选择 **[!UICONTROL 另存为新的主要播放器]** 以保存图像的第二个副本。 选择 **[!UICONTROL 另存为主要播放器的添加视图]** 因此，您可以使用其他名称保存原始版本及其裁切版本。 选择 **[!UICONTROL 替换原始]** 删除从中裁切图像的原始文件。 然后输入图像的名称，并选择 **[!UICONTROL 提交]**.

## 裁切以删除图像周围的空白区域 {#crop-to-remove-white-space-around-an-image}

您可以将图像边缘的透明或纯色像素区域裁切掉。

1. 要裁切图像，请选择其变换图像 **[!UICONTROL 编辑]** 按钮，然后选择 **[!UICONTROL 裁切]**，或在“浏览”面板的“详细信息”视图中显示它，然后选择 **[!UICONTROL 裁切]** 按钮。
1. 在裁切编辑器页面上，执行以下操作之一：

   * 要修剪颜色像素，请转到 **[!UICONTROL Trim]** > **[!UICONTROL 颜色]**. 在 **[!UICONTROL 按颜色自动裁切]** 对话框中，选择 **[!UICONTROL 角]** 菜单，然后选择要裁切掉的具有背景颜色的角。 然后输入 **[!UICONTROL 容差]** 从0到1的设置。 如果设置为 0，则仅裁切与图像角中选定颜色精确匹配的像素。数字越接近 1，允许的色差越大。选择 **[!UICONTROL 裁切]**.
   * 要修剪透明像素，请转到 **[!UICONTROL Trim]** > **[!UICONTROL 透明]**. 在 **[!UICONTROL 按透明度自动裁切]** 对话框中，输入从0到1的公差设置。 0设置仅在像素为透明时才裁剪像素。 数字越接近 1，则裁切透明度越高的像素。选择 **[!UICONTROL 裁切]**.

1. 选择 **[!UICONTROL 保存]**.

>[!NOTE]
>
>要在裁切图像后将其恢复到原始状态，请在裁切编辑器屏幕中显示该图像，然后选择 **[!UICONTROL 重置]**.

## 选择要裁切的区域 {#select-an-area-to-crop}

1. 要裁切图像，请选择其变换图像 **[!UICONTROL 编辑]** 按钮，然后选择 **[!UICONTROL 裁切]**，或在“浏览”面板的“详细信息”视图中显示它，然后选择 **[!UICONTROL 裁切]**.

1. 在“裁切编辑器”窗口中，将您不希望裁切的图像部分放入裁切框中。 框内显示的任何内容都是选择后要保留的内容 **[!UICONTROL 保存]** 并裁切图像。
1. 要调整裁切区域，请执行以下任一操作：

   * 拖动框的一边或一角。拖动时，按住 Shift 键，以更改大小，但保持裁切框的高宽比（形状）不变。
   * 在“大小”框中输入像素大小。
   * 拖动以移动裁切框。将鼠标指针移动到该框边界内。当指针显示为四向箭头时，将裁切框拖动到图像上的新位置。

1. 选择 **[!UICONTROL 保存]**.

>[!NOTE]
>
>要在裁切图像后将其恢复到原始状态，请在裁切编辑器屏幕中显示该图像，然后选择 **[!UICONTROL 重置]**.

>[!MORELIKETHIS]
>
>* [上传时图像编辑的选项](image-editing-options-upload.md#image-editing-options-at-upload)
>* [裁剪PDF文件中的空格](pdfs.md#cropping_white_space_from_a_pdf_file)
>* [从PDF页侧面裁切](pdfs.md#cropping_from_the_sides_of_pdf_pages)
