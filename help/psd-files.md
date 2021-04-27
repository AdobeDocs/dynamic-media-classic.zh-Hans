---
title: 使用 PSD 文件
description: 了解如何使用PSD文件。
uuid: 5836b660-6bca-46e7-ab39-1a31d1e0cff2
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 4086e3db-5aca-41a0-8f15-302afbf67ddb
feature: Dynamic Media Classic，资产管理
role: Business Practitioner
exl-id: e3b8c4b9-e9c4-4d7f-84de-2efb456755a1
translation-type: tm+mt
source-git-commit: c4e2b8b42b56420269087d0d4f262490464270c0
workflow-type: tm+mt
source-wordcount: '989'
ht-degree: 45%

---

# 使用 PSD 文件{#working-with-psd-files}

<!--   USED TO BE AN OPTION UNDER COLOR PROFILE OPTIONS * **Convert To sRGB (default)** - Converts to sRGB (Standard Red Green Blue). sRGB is the recommended color space for displaying images on web pages. -->

Dynamic Media Classic中最常使用PSD(Photoshop 文档文件)创建模板。 在上传PSD文件时，可以自动从该文件创建Dynamic Media Classic模板（在“上传”屏幕上选择“创建模板”选项）。

Dynamic Media Classic使用PSD文件创建模板时，会使用图层从PSD文件创建多个图像；它为每个图层创建一个图像。

## PSD 上载选项 {#psd-upload-options}

用于上传PSD文件的选项位于“上传作业选项”对话框的“Photoshop选项”下。 您可以裁切文件、为其选择颜色配置文件、使用该文件创建模板，以及选择锚点。

以下选项在上载 PSD 文件时可用：

* **裁剪选项**  — 位于“裁剪 **[!UICONTROL 选项”下]**。选择“裁切”以自动裁切PSD文件边缘的空白；单击&#x200B;**[!UICONTROL 手动]**&#x200B;可裁剪PSD文件的两侧：

   * **裁切**  — 选择“基于 **[!UICONTROL 裁切的上]** 菜单”，然后选 **** 择“颜色 **[!UICONTROL ”或“透]**&#x200B;明度”。

      如果选择“颜色”选项，请选择“角”菜单，并选择其颜色最接近于您要裁切的空白区域颜色的 PSD 角。

      拖动滑块可指定从0到1的公差。 基于颜色修剪时，如果指定为 0，则仅裁切与 PSD 角中选定颜色精确匹配的像素。数字越接近 1，允许的色差越大。要根据透明度进行裁切，请指定0，以仅裁剪透明像素；接近1的数字意味着更加透明。

   * **手动**  — 输入要从图像的任何一侧或每一侧裁剪的像素数。图像被裁切部分的大小取决于图像文件中的 ppi（像素/英寸）设置。例如，如果图像显示 150 ppi，您在“上”、“下”、“左”、“右”文本框中输入 75，则将从图像各边裁切半英寸。

* **颜色用户档案选项**  — 位于“颜色 **[!UICONTROL 用户档案选项”下]**。

   * **默认护色**

   * **保留原始色彩空间**  — 保留图像的原始色彩空间。

   * **“自定”>“至** ” — 打开菜单，以便您可以选择“转换自”和“转换至”色彩空间。您可以选择标准Photoshop色彩空间或上传到Dynamic Media Classic的色彩空间。 请参阅[ICC 配置文件](/help/icc-profiles.md)。

* **Photoshop 选项**

   * **维护图层**  — 将PSD中的图层（如果有）拆分为单个资源。资源图层仍然与 PSD 关联。查看方法是，在详细信息视图中打开 PSD 文件，然后选择图层面板。请参阅查看和编辑 PSD 文件中的图层。

   * **创建模板**  — 从PSD文件中的图层创建模板。

   * **提取文本**  — 提取文本，以便用户可以在查看器中搜索文本。

   * **将图层扩展到背景大小**  — 将已撕开的图像图层的大小扩展到背景图层的大小。

   * **图层命名** - PSD文件中的图层作为单独的图像上传。要在Dynamic Media Classic中命名这些图像，请从以下选项中进行选择：

      * **图层名称**  — 在PSD文件中的图层名称之后命名图像。例如，原始 PSD 文件中名为“Price Tag”的图层将成为名为“Price Tag”的图像。但是，如果 PSD 文件中的图层名称是默认 Photoshop 图层名称（“Background”、“Layer 1”、“Layer 2”等等），将以该文件中的图层编号而不是默认图层名称为图像命名。

      * **Photoshop和图层编号**  — 在PSD文件中将图像命名为图层编号之后的图像，而忽略原始图层名称。使用 Photoshop 文件名和附加的图层编号为图像命名。例如，名为`Spring Ad.psd`的文件的第二个层名为`Spring Ad_2`，即使它在Photoshop中具有非默认名称。

      * **Photoshop和图层名称**  — 在PSD文件之后命名图像，后跟图层名称或图层编号。如果 PSD 文件中的图层名称是默认的 Photoshop 图层名称，则将使用图层编号。例如，名为`SpringAd`的PSD文件中名为`Price Tag`的图层名为`Spring Ad_Price Tag`。 名为“Layer 2”的默认图层称为`Spring Ad_2`。
   * **锚点**  — 指定如何在从PSD文件生成的分层合成生成的模板中定位图像。默认情况下，锚点是中心。中心锚点允许替换图像尽可能占据相同的空间，无论替换图像的高宽比是多少。当引用模板并使用参数替换时，替换该图像的高宽比不同的图像有效地占据相同的空间。如果应用程序要求替换图像占据模板中分配的空间，请更改为其他设置。


## 查看和编辑 PSD 文件中的图层 {#viewing-and-editing-layers-in-a-psd-file}

如果您在上传PSD时选择了“维护图层”选项，Dynamic Media Classic会将各个图层翻录到资产中。 您可以在浏览面板的详细信息视图中打开 PSD 文件，以查看和编辑属于该文件的资源图层。

1. 多次在“浏览”面板中单击完整的PSD文件。 文件将以“详细信息”视图打开。

   >[!NOTE]
   >
   >请确保您打开的是完整资源，而不是某一个 PSD 图层。

1. 单击&#x200B;**[!UICONTROL Layers]**。 在“图层”面板中将以单独的图像显示所有各图层。
1. 多次单击图层并执行下列任一操作：

   * 要在图层上创建图像映射，请单击&#x200B;**[!UICONTROL 图像映射]**&#x200B;图标。 （请参阅[创建图像映射](creating-image-maps.md#creating_image_maps)。）
   * 要在图层上创建缩放目标，请单击&#x200B;**[!UICONTROL 缩放目标]**&#x200B;图标。 （请参阅[为引导式缩放创建缩放目标](creating-zoom-targets-guided-zoom.md#creating_zoom_targets_for_guided_zoom)。）
   * 要裁剪图层，请单击&#x200B;**[!UICONTROL 裁剪]**&#x200B;图标。 （请参阅[裁切图像](cropping-image.md#cropping_an_image)。）
   * 要锐化图层，请单击&#x200B;**[!UICONTROL 锐化]**。 （请参阅[锐化图像](sharpening-image.md#sharpening_an_image)。）
   * 要调整图层，请单击&#x200B;**[!UICONTROL 调整]**。 （请参阅[调整图像](adjusting-image.md#adjusting_an_image)。）

1. 单击“**[!UICONTROL 保存]**”或“**[!UICONTROL 另存为]**”。
1. 要查看或编辑其他图层，请单击图层预览底部的箭头。
1. 要退出图层Detail视图，请单击&#x200B;**[!UICONTROL Grid视图]**&#x200B;图标。
