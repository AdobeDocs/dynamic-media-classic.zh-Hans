---
title: 使用PSD文件
description: 了解如何在Adobe Dynamic Media Classic中处理PSD文件。
uuid: 5836b660-6bca-46e7-ab39-1a31d1e0cff2
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 4086e3db-5aca-41a0-8f15-302afbf67ddb
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: e3b8c4b9-e9c4-4d7f-84de-2efb456755a1
source-git-commit: dc1ec666b208cec8fffe836d64ed501f6ccf4e7b
workflow-type: tm+mt
source-wordcount: '1003'
ht-degree: 25%

---

# 使用PSD文件{#working-with-psd-files}

<!--   USED TO BE AN OPTION UNDER COLOR PROFILE OPTIONS * **Convert To sRGB (default)** - Converts to sRGB (Standard Red Green Blue). sRGB is the recommended color space for displaying images on web pages. -->

PSD(Photoshop文档文件)在Adobe Dynamic Media Classic中最常用于创建模板。 上传PSD文件时，可以从文件自动创建Adobe Dynamic Media Classic模板（在“上传”屏幕上选择“创建模板”选项）。

如果使用文件创建模板，则Adobe Dynamic Media Classic会从带有层的PSD文件创建多个图像；它会为每个图层创建一个图像。

## PSD 上载选项 {#psd-upload-options}

上传PSD文件的选项位于“上传作业选项”对话框的Photoshop选项下。 您可以裁切文件、为其选择颜色配置文件、使用该文件创建模板，以及选择锚点。

以下选项在上载 PSD 文件时可用：

* **裁剪选项**  — 位于 **[!UICONTROL 裁剪选项]**. 选择 **[!UICONTROL 裁切]** 自动从PSD文件的边缘裁剪空格；选择 **[!UICONTROL 手动]** 要裁剪PSD文件的侧边，请执行以下操作：

   * **[!UICONTROL 裁切]**  — 选择 **[!UICONTROL 根据]** ，然后选择 **[!UICONTROL 颜色]** 或 **[!UICONTROL 透明度]**.
   如果您选择 **[!UICONTROL 颜色]** 选项，选择“角”菜单，然后选择PSD的角，其颜色最能代表要裁剪的空格颜色。

   拖动滑块以指定从0到1的公差。 基于颜色修剪时，如果指定为 0，则仅裁切与 PSD 角中选定颜色精确匹配的像素。数字越接近 1，允许的色差越大。要根据透明度进行裁切，请指定0，以仅在像素透明时裁剪像素；接近1的数字使透明度更高。

   * **[!UICONTROL 手动]**  — 输入要从图像的任何一侧或每一侧裁剪的像素数。 图像被裁切部分的大小取决于图像文件中的 ppi（像素/英寸）设置。例如，如果图像显示150 ppi，而您在“顶部”、“右”、“底部”和“左”文本框中输入75，则输入0.5英寸。 会从图像的每一侧裁剪。


* **颜色配置文件选项**  — 位于 **[!UICONTROL 颜色配置文件选项]**.

   * **[!UICONTROL 默认护色]**

   * **[!UICONTROL 保留原始色彩空间]**  — 保留图像的原始颜色空间。

   * **[!UICONTROL 自定义自]** > **[!UICONTROL 至]**  — 打开菜单，以便您选择“从中转换”和“转换到”色彩空间。 您可以选择标准的Photoshop色彩空间或上传到Adobe Dynamic Media Classic的色彩空间。 请参阅[ICC 配置文件](/help/icc-profiles.md)。

* **Photoshop 选项**

   * **[!UICONTROL 维护图层]**  — 将PSD中的层（如果有）拆分为单个资产。 资源图层仍然与 PSD 关联。可通过在“详细信息视图”中打开PSD文件并选择层面板来查看它们。 请参阅查看和编辑 PSD 文件中的图层。

   * **[!UICONTROL 创建模板]**  — 从PSD文件的层创建模板。

   * **[!UICONTROL 提取文本]**  — 提取文本，以便用户在查看器中搜索文本。

   * **[!UICONTROL 将图层扩展到背景大小]**  — 将已撕裂图像层的大小扩展到背景层的大小。

   * **[!UICONTROL 层命名]** -PSD文件中的图层将作为单独的图像上传。 要在Adobe Dynamic Media Classic中命名这些图像，请从以下选项中进行选择：

      * **[!UICONTROL 层名称]**  — 将图像命名为PSD文件中图层名称之后的图像。 例如，原始 PSD 文件中名为“Price Tag”的图层将成为名为“Price Tag”的图像。但是，如果PSD文件中的层名称是默认的Photoshop层名称（背景、层1、层2等），则图像将以其在PSD文件中的层编号命名。 <!-- not their default layer names -->

      * **[!UICONTROL Photoshop和图层编号]**  — 在PSD文件中将图像命名为图层编号之后，而忽略原始图层名称。 使用 Photoshop 文件名和附加的图层编号为图像命名。例如，文件的第二层，名为 `Spring Ad.psd` 已命名 `Spring Ad_2` 即使它在Photoshop中具有非默认名称。

      * **[!UICONTROL Photoshop和层名称]**  — 在PSD文件后面命名图像，后跟层名或层号。 如果 PSD 文件中的图层名称是默认的 Photoshop 图层名称，则将使用图层编号。例如，名为 `Price Tag` 在名为的PSD文件中 `SpringAd` 已命名 `Spring Ad_Price Tag`. 将调用缺省名称为Layer 2的层 `Spring Ad_2`.
   * **[!UICONTROL 锚点]**  — 指定如何在模板中锚定图像，这些模板是从PSD文件生成的分层组合生成的。 默认情况下，锚点是中心。中心锚点允许替换图像尽可能占据相同的空间，无论替换图像的高宽比是多少。当引用模板并使用参数替换时，替换该图像的高宽比不同的图像有效地占据相同的空间。如果应用程序要求替换图像占据模板中分配的空间，请更改为其他设置。


## 在PSD文件中查看和编辑图层 {#viewing-and-editing-layers-in-a-psd-file}

如果您在上传PSD时选择了维护层选项，Adobe Dynamic Media Classic会将各个层拆分为资产。 您可以通过在详细信息视图的浏览面板中打开属于PSD文件的资产层来查看和编辑该文件。

>[!NOTE]
>
>Adobe Dynamic Media Classic在嵌套图层组中最多支持五个级别。

1. 双击“Browse（浏览）”面板中的完整PSD文件。 文件将在“详细信息视图”中打开。

   >[!NOTE]
   >
   >请确保您打开的是完整资源，而不是某一个 PSD 图层。

1. 选择 **[!UICONTROL 图层]**. 在“图层”面板中将以单独的图像显示所有各图层。
1. 双击图层并执行下列任一操作：

   * 要在图层上创建图像映射，请选择 **[!UICONTROL 图像映射]** 图标。 (请参阅 [创建图像映射](creating-image-maps.md#creating_image_maps).)
   * 要在图层上创建缩放目标，请选择 **[!UICONTROL 缩放目标]** 图标。 (请参阅 [为引导式缩放创建缩放目标](creating-zoom-targets-guided-zoom.md#creating_zoom_targets_for_guided_zoom).)
   * 要裁剪图层，请选择 **[!UICONTROL 裁切]** 图标。 (请参阅 [裁剪图像](cropping-image.md#cropping_an_image).)
   * 要锐化图层，请选择 **[!UICONTROL 锐化]**. (请参阅 [锐化图像](sharpening-image.md#sharpening_an_image).)
   * 要调整图层，请选择 **[!UICONTROL 调整]**. (请参阅 [调整图像](adjusting-image.md#adjusting_an_image).)

1. 选择 **[!UICONTROL 保存]** 或 **[!UICONTROL 另存为]**.
1. 要查看或编辑其他图层，请在图层预览的底部选择一个箭头。
1. 要退出层“细节视图”(Detail View)，请选择 **[!UICONTROL 网格视图]** 图标。
