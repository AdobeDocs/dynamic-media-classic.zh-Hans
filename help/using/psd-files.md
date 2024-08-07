---
title: 使用PSD文件
description: 了解如何在Adobe Dynamic Media Classic中使用PSD文件。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: e3b8c4b9-e9c4-4d7f-84de-2efb456755a1
topic: Integrations, Development
level: Experienced
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '1023'
ht-degree: 21%

---

# 使用PSD文件{#working-with-psd-files}

<!--   USED TO BE AN OPTION UNDER COLOR PROFILE OPTIONS * **Convert To sRGB (default)**: Converts to sRGB (Standard Red Green Blue). sRGB is the recommended color space for displaying images on Web pages. -->

PSD(Photoshop文档文件)在Adobe Dynamic Media Classic中最常用于创建模板。 上传PSD文件时，您可以使用该文件自动创建Adobe Dynamic Media Classic模板（在“上传”屏幕上选择“创建模板”选项）。

如果使用包含图层的PSD文件创建模板，则Adobe Dynamic Media Classic会从包含图层的模板文件创建多个图像；它为每个图层创建一个图像。

## PSD 上载选项 {#psd-upload-options}

用于上传PSD文件的选项位于“上载作业选项”对话框中的Photoshop选项下。 您可以裁切文件、为其选择颜色配置文件、使用该文件创建模板，以及选择锚点。

以下选项在上载 PSD 文件时可用：

* **裁切选项**：位于&#x200B;**[!UICONTROL 裁切选项]**&#x200B;下。 选择&#x200B;**[!UICONTROL 裁剪]**，以便自动裁剪来自PSD文件边缘的空格。 选择&#x200B;**[!UICONTROL 手动]**&#x200B;裁切PSD文件两侧：

   * **[!UICONTROL 修剪]**：选择&#x200B;**[!UICONTROL 基于]**&#x200B;菜单修剪掉，然后选择&#x200B;**[!UICONTROL 颜色]**&#x200B;或&#x200B;**[!UICONTROL 透明度]**。

  如果选择&#x200B;**[!UICONTROL 颜色]**&#x200B;选项，请选择“边角”菜单，然后选择最能代表要裁切的空格颜色的PSD边角。

  拖动滑块以指定从0到1的公差。 基于颜色修剪时，如果指定为 0，则仅裁切与 PSD 角中选定颜色精确匹配的像素。数字越接近 1，允许的色差越大。要根据透明度进行裁剪，请指定0以仅裁切透明像素；数字越接近1则透明度越高。

   * **[!UICONTROL 手动]**：输入要从图像任何一侧或每侧裁切的像素数。 图像被裁切部分的大小取决于图像文件中的 ppi（像素/英寸）设置。例如，假设图像显示150 ppi。 然后在“顶部”、“右侧”、“底部”和“左侧”文本框中输入75。 图像的每一边都将被裁剪，0.5英寸。

* **颜色配置文件选项**：位于&#x200B;**[!UICONTROL 颜色配置文件选项]**&#x200B;下。

   * **[!UICONTROL 默认保色]**

   * **[!UICONTROL 保留原始颜色空间]**：保留图像的原始颜色空间。

   * **[!UICONTROL 自定义从]** > **[!UICONTROL 到]**：打开菜单，以便选择“转换自”和“转换为颜色空间”。 您可以选择标准的Photoshop色彩空间，也可以选择上传到Adobe Dynamic Media Classic的色彩空间。 请参阅[ICC 配置文件](/help/using/icc-profiles.md)。

* **Photoshop选项**

   * **[!UICONTROL 保留图层]**：将PSD中的图层（如果有）拆分为单独的资源。 资源图层仍然与 PSD 关联。可通过在“详细PSD”中打开视图文件并选取图层面板来查看它们。 请参阅在PSD文件中查看和编辑图层。

   * **[!UICONTROL 创建模板]**：从PSD文件中的图层创建模板。

   * **[!UICONTROL 提取文本]**：提取文本，以便用户在查看器中搜索文本。

   * **[!UICONTROL 将图层扩展到背景大小]**：将翻录的图像图层的大小扩展到背景图层的大小。

   * **[!UICONTROL 图层命名]**：PSD文件中的图层作为单独的图像上传。 要在Adobe Dynamic Media Classic中命名这些图像，请选择以下选项：

      * **[!UICONTROL 图层名称]**：将图像命名为PSD文件中的图层名称。 例如，原始 PSD 文件中名为“Price Tag”的图层将成为名为“Price Tag”的图像。但是，如果PSD文件中的图层名称是默认的Photoshop图层名称（“背景”、“图层1”、“图层2”等），则图像将根据PSD文件中的图层编号进行命名。<!-- not their default layer names -->

      * **[!UICONTROL Photoshop和图层编号]**：将图像命名为PSD文件中的图层编号，而不考虑原始图层名称。 使用 Photoshop 文件名和附加的图层编号为图像命名。例如，名为`Spring Ad.psd`的文件的第二层名为`Spring Ad_2`，即使它在Photoshop中具有非默认名称。

      * **[!UICONTROL Photoshop和图层名称]**：将图像命名为PSD文件后跟图层名称或图层编号。 如果 PSD 文件中的图层名称是默认的 Photoshop 图层名称，则将使用图层编号。例如，名为`SpringAd`的PSD文件中名为`Price Tag`的图层名为`Spring Ad_Price Tag`。 默认名称为Layer 2的层称为`Spring Ad_2`。

   * **[!UICONTROL 锚点]**：指定如何在模板中锚定图像，该模板是根据PSD文件生成的分层组合生成的。 默认情况下，锚点是中心。中心锚点允许以最佳方式填充相同空间的替换图像，而不管替换图像的长宽比如何。 当引用模板并使用参数替换时，替换该图像的高宽比不同的图像有效地占据相同的空间。如果应用程序要求替换图像占据模板中分配的空间，请更改为其他设置。

## 在PSD文件中查看和编辑图层 {#viewing-and-editing-layers-in-a-psd-file}

如果您在上传PSD时选择了&#x200B;**[!UICONTROL 保留图层]**&#x200B;选项，Adobe Dynamic Media Classic会将各个图层翻录到资源中。 通过在“详细视图”的“浏览”面板中打开文件，可以查看和编辑属于PSD文件的资源图层。

>[!NOTE]
>
>Adobe Dynamic Media Classic在嵌套图层组中最多支持五个级别。

1. 在“浏览”面板中双击完整的PSD文件。 文件将在“详细视图”中打开。

   >[!NOTE]
   >
   >请确保您打开的是完整资源，而不是某一个 PSD 图层。

1. 选择&#x200B;**[!UICONTROL 层]**。 在“图层”面板中将以单独的图像显示所有各图层。
1. 双击一个图层并执行以下任一操作：

   * 要在图层上创建图像映射，请选择&#x200B;**[!UICONTROL 图像映射]**&#x200B;图标。 （请参阅[创建图像映射](creating-image-maps.md#creating_image_maps)。）
   * 要在图层上创建缩放目标，请选择&#x200B;**[!UICONTROL 缩放目标]**&#x200B;图标。 （请参阅[创建引导缩放的缩放目标](creating-zoom-targets-guided-zoom.md#creating_zoom_targets_for_guided_zoom)。）
   * 要裁切图层，请选择&#x200B;**[!UICONTROL 裁切]**&#x200B;图标。 （请参阅[裁切图像](cropping-image.md#cropping_an_image)。）
   * 若要锐化图层，请选择&#x200B;**[!UICONTROL 锐化]**。 （请参阅[锐化图像](sharpening-image.md#sharpening_an_image)。）
   * 要调整图层，请选择&#x200B;**[!UICONTROL 调整]**。 （请参阅[调整图像](adjusting-image.md#adjusting_an_image)。）

1. 选择&#x200B;**[!UICONTROL 保存]**&#x200B;或&#x200B;**[!UICONTROL 另存为]**。
1. 要查看或编辑其他图层，请选择图层预览底部的箭头。
1. 要退出图层详细信息视图，请选择&#x200B;**[!UICONTROL 网格视图]**&#x200B;图标。
