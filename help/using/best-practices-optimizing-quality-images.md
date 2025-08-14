---
title: 优化图像质量的最佳做法
description: 了解优化图像质量的最佳实践。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 3c50e706-b9ed-49db-8c08-f179de52b9cf
topic: Content Management
level: Intermediate
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '1602'
ht-degree: 39%

---

# 优化图像质量的最佳做法{#best-practices-for-optimizing-the-quality-of-your-images}

优化图像质量需要花费大量时间。 许多因素有助于得到可接受的结果。 结果在一定程度上是主观性的，因为个人评价图像质量的标准不尽相同。因此，进行结构化的试验是至关重要的。

Adobe Dynamic Media Classic包括100多个图像服务命令，用于调整和优化图像和渲染结果。 以下准则可以帮助您简化流程，并使用一些基本命令和最佳做法快速获得较好的效果。

另请参阅[智能成像](https://experienceleague.adobe.com/zh-hans/docs/experience-manager-65/content/assets/dynamic/imaging-faq)。

>[!TIP]
>
>尝试使用Dynamic Media [_快照_](https://snapshot.scene7.com/)来发现Dynamic Media图像修饰符和智能成像的好处。
>
> Snapshot是一种可视化演示工具，旨在说明Dynamic Media在优化和动态图像投放方面的强大功能。 尝试使用测试图像或Dynamic Media URL，以便直观地观察各种Dynamic Media图像修饰符的输出，并优化以下各项的智能成像：
>
>* 文件大小（使用WebP和AVIF交付）
>* 网络带宽
>* DPR（设备像素比率）
>
>要了解使用快照的容易程度，请播放[快照培训视频](https://experienceleague.adobe.com/zh-hans/docs/experience-manager-learn/assets/dynamic-media/images/dynamic-media-snapshot)（3分17秒）。


## 图像格式的最佳做法 (&amp;fmt=) {#best-practices-for-image-format-fmt}

* 在提供具有较好质量和可控制大小和粗细的图像方面，JPG 或 PNG 是最佳选择。
* 如果URL中未提供任何格式命令，则Dynamic Media图像服务将默认使用JPG进行交付。
* JPG压缩的比率为10:1，通常生成的图像文件较小。 PNG压缩的比例约为2:1，除非图像包含空背景。 通常，PNG 文件比 JPG 文件大。
* JPG 使用有损压缩，这意味着在压缩过程中删除了一些图像元素（像素）；而 PNG 使用无损压缩。
* 通常，JPG 压缩摄影图像的保真度比具有清晰边缘和对比度的合成图像好。
* 如果图像包含透明度，请使用 PNG，因为 JPG 不支持透明度。

作为图像格式的最佳实践，请从最常见的设置`&fmt=JPG`开始。

## 图像大小的最佳做法 {#best-practices-for-image-size}

动态减小图像大小是Dynamic Media图像服务执行的最常见任务之一。 这包括指定大小，以及指定用于减小图像的缩减像素采样模式（可选）。

* 对于图像大小调整，最佳且最直接的方法是使用`&wid=<value>`和`&hei=<value>`，或者只使用`&hei=<value>`。 这些参数自动根据高宽比设置图像宽度。
* `&resMode=<value>`控制用于缩减像素采样的算法。 从`&resMode=sharp2`开始。 该值提供了最佳的图像质量。使用缩减像素取样值`=bilin`的速度较快，但通常会导致工件出现锯齿。

作为调整图像大小的最佳实践，请使用`&wid=<value>&hei=<value>&resMode=sharp2`或`&hei=<value>&resMode=sharp2`

## 图像锐化的最佳做法 {#best-practices-for-image-sharpening}

图像锐化是在您的网站上控制图像的最复杂任务，可能会出现很多错误。请查看以下有用资源，详细了解Adobe Dynamic Media Classic中锐化和USM的工作原理：

最佳实践白皮书[在Adobe Dynamic Media Classic和图像服务器上锐化图像](/help/using/assets/s7_sharpening_images.pdf)。

<!-- Give a 404 See also [Sharpening an image with unsharp mask](https://helpx.adobe.com/photoshop/atv/cs6-tutorials/sharpening-an-image-with-unsharp-mask.html). -->

借助Adobe Dynamic Media Classic，您可以在摄取和/或交付时锐化图像。 但是，通常您只使用一种方法或另一种方法来锐化图像，但不能同时使用这两种方法来锐化。 传送时在 URL 上锐化图像通常可以获得最佳的效果。

可以使用两种图像锐化方法：

* 简单锐化(`&op_sharpen`)：与Photoshop中使用的锐化滤镜类似，简单锐化会在动态调整大小后对图像的最终视图应用基本锐化。 不过，用户无法配置这种方法。最佳做法是避免使用`&op_sharpen`（如果需要）。
* USM锐化( `&op_USM`)：USM锐化是用于锐化的行业标准滤镜。 最佳做法是按照以下准则使用 USM 锐化功能锐化图像。可以通过 USM 锐化控制以下三个参数：

   * `&op_sharpen=amount,radius,threshold`

      * `amount` （0-5，效果的强度。）
      * `radius` （0-250，围绕锐化对象绘制的“锐化线”的宽度，以像素为单位。）

        请记住，参数`radius`和`amount`相互对应。 通过增加`radius`可以补偿减少`amount`。 `Radius`允许更细的控制，因为较低的值仅锐化边缘像素，而较高的值锐化较宽的像素范围。

      * `threshold` （0-255，效果敏感度。）

        此参数确定锐化的像素与周围区域相差多少，滤镜才会将它们视为边缘像素并进行锐化。阈值有助于避免出现具有类似颜色的过度锐化区域，如肤色。例如，阈值为12会忽略肤色亮度的细微变化，以避免添加“杂色”，同时仍会为高对比度区域添加边缘对比度，如睫毛与皮肤相遇的地方。

        有关如何设置这三个参数的更多信息，包括要用于滤镜的最佳实践，请参阅[在Adobe Dynamic Media Classic和图像服务器上锐化图像](/help/using/assets/s7_sharpening_images.pdf)。

      * Adobe Dynamic Media Classic还允许您控制第四个参数：单色(`0,1`)。 此参数确定是使用值`0`分别将钝化蒙版应用于每个颜色组件，还是使用值`1`将钝化蒙版应用于图像亮度/强度。

作为最佳做法，请从 USM 锐化 radius 参数入手。可以最初使用以下 radius 设置：

* 网站：0.2-0.3 像素
* 摄影打印 (250-300 ppi)：0.3-0.5 像素
* 胶印胶印 (266-300 ppi)：0.7-1.0 像素
* 画布打印 (150 ppi)：1.5-2.0 像素

将 amount 从 1.75 逐渐增加到 4。如果锐化仍达不到所需的效果，请按小数点增加 radius 值，然后再次将 amount 从 1.75 增加到 4。根据需要，重复此步骤。

将 monochrome 参数设置保留为 0。

## JPEG压缩的最佳实践(`&qlt=`) {#best-practices-for-jpeg-compression-qlt}

* 此参数控制 JPG 编码质量。较高的值表示图像质量较高，但文件较大；而较低的值表示图像质量较低，但文件较小。此参数的范围是 0-100。
* 要优化质量，不要将参数值设置为 100。将90或95设置为100几乎可以察觉到差异。 而100则毫无必要地增大了图像文件的大小。 因此，要优化质量但避免图像文件过大，请将`qlt=`值设置为90或95。
* 若要针对较小的图像文件大小进行优化，但使图像质量保持在可接受的级别，请将`qlt=`值设置为80。 低于 70 到 75 的值将导致图像质量大大下降。
* 作为最佳实践，要停留在中间，请将`qlt=`值设置为85以停留在中间。
* 在`qlt=`中使用色度标志

   * `qlt=`参数具有第二个设置，通过该设置，您可以使用正常值`,0`打开RGB色度缩减像素采样（默认值），或使用值`,1`关闭它。
   * 要保持简单，请从关闭RGB色度缩减像素采样(`,1`)开始。 此设置通常会获得较好的图像质量，尤其是具有很多清晰边缘和对比度的合成图像。

作为JPG压缩的最佳实践，请使用`&qlt=85,0`。

## JPEG 大小调整的最佳做法 (&amp;jpegSize=) {#best-practices-for-jpeg-sizing-jpegsize}

如果要保证图像不超过特定大小，以便传递到内存有限的设备，则参数`jpegSize`非常有用。

* 此参数设置为千字节(`jpegSize=<size_in_kilobytes>`)。 它定义了图像传送允许的最大大小。
* `&jpegSize=`与JPG压缩参数`&qlt=`交互。 如果具有指定JPG压缩参数(`&qlt=`)的JPG响应未超过`jpegSize`值，则按定义返回带有`&qlt=`的图像。 否则，`&qlt=`将逐渐减小，直到图像符合允许的最大尺寸。 或者，直到系统确定它不合适并返回错误为止。

如果您要将JPG图像传送到内存有限的设备，最佳做法是设置`&jpegSize=`并添加参数`&qlt=`。

## 最佳做法摘要 {#best-practices-summary}

为了达到较高的图像质量和较小的文件大小，最好从以下参数组合开始：

`fmt=jpg&qlt=85,0&resMode=sharp2&op_usm=1.75,0.3,2,0`

在大多数情况下，这种设置组合会产生卓越的结果。

如果需要进一步优化图像，请先将 radius 设置为 0.2 或 0.3 以逐步调整锐化（USM 锐化）参数。然后，将 amount 从 1.75 逐渐增加到最多 4（相当于 Photoshop 中的 400%）。检查是否获得了所需的效果。

如果锐化效果仍不令人满意，请按小数点增加 radius 值。每增加一个小数点，请再次将 amount 从 1.75 逐渐增加到 4。重复此过程，直到获得所需的效果。尽管创意工作室已对上面的值进行了验证，但要记住，您最初可以使用其他值和采用其他策略。您对结果是否满意是一个非常主观的问题，因此，进行结构化的试验是至关重要的。

在实验过程中，以下一般建议有助于优化您的工作流：

* 尝试直接在URL上或使用Adobe Dynamic Media Classic的图像调整功能实时测试和测试各种参数。 后者为调整操作提供实时预览。
* 作为最佳实践，请记住，您可以将Dynamic Media图像服务命令分组到图像预设中。 图像预设基本上是带有自定义预设名称（如`$thumb_low$`和`&product_high$`）的URL命令宏。 URL路径中的自定义预设名称将调用这些预设。 此功能帮助您针对网站上的图像的不同使用方式管理命令和质量设置，并缩短 URL 的总体长度。
* Adobe Dynamic Media Classic还提供了更高级的方法来调整图像质量，例如在摄取时应用图像锐化。 对于可以选择进一步调整和优化渲染结果的高级用例，Adobe Professional Services可以帮助您使用自定义的insight和最佳实践。
