---
title: 优化图像质量的最佳做法
description: 了解优化图像质量的最佳实践。
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
feature: Dynamic Media Classic，Asset Management
role: User
exl-id: 3c50e706-b9ed-49db-8c08-f179de52b9cf
source-git-commit: 1c7900b2807e6b67e9802e6361e42cce893b0217
workflow-type: tm+mt
source-wordcount: '1465'
ht-degree: 55%

---

# 优化图像质量的最佳做法{#best-practices-for-optimizing-the-quality-of-your-images}

优化图像质量可能是一个需要很长时间的过程，因为很多因素都会影响提供可接受的结果。结果在一定程度上是主观性的，因为个人评价图像质量的标准不尽相同。因此，进行结构化的试验是至关重要的。

Dynamic Media Classic包含100多个图像服务命令，用于调整和优化图像以及渲染结果。 以下准则可以帮助您简化流程，并使用一些基本命令和最佳做法快速获得较好的效果。

另请参阅[智能成像](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/imaging-faq.html#dynamic)。

## 图像格式的最佳做法 (&amp;fmt=) {#best-practices-for-image-format-fmt}

* 在提供具有较好质量和可控制大小和粗细的图像方面，JPG 或 PNG 是最佳选择。
* 如果URL中未提供format命令，则Dynamic Media图像提供默认为JPG以进行交付。
* JPG 压缩比率为 10:1，通常生成较小的图像文件。PNG的压缩比率约为2:1，但有时包含空背景的图像除外。 通常，PNG 文件比 JPG 文件大。
* JPG 使用有损压缩，这意味着在压缩过程中删除了一些图像元素（像素）；而 PNG 使用无损压缩。
* 通常，JPG 压缩摄影图像的保真度比具有清晰边缘和对比度的合成图像好。
* 如果图像包含透明度，请使用 PNG，因为 JPG 不支持透明度。

作为图像格式的最佳实践，请首先使用最常见的设置`&fmt=JPG`。

## 图像大小的最佳做法 {#best-practices-for-image-size}

动态减小图像大小是Dynamic Media图像服务执行的最常见任务之一。 这包括指定大小，以及指定用于减小图像的缩减像素采样模式（可选）。

* 对于图像大小调整，最好且最直接的方法是使用`&wid=<value>`和`&hei=<value>`，或者只使用`&hei=<value>`。 这些参数自动根据高宽比设置图像宽度。
* `&resMode=<value>` 控制用于缩减采样的算法。从`&resMode=sharp2`开始。 该值提供了最佳的图像质量。虽然使用缩减采样值`=bilin`的速度更快，但通常会导致出现锯齿伪像。

作为图像大小调整的最佳实践，请使用`&wid=<value>&hei=<value>&resMode=sharp2`或`&hei=<value>&resMode=sharp2`

## 图像锐化的最佳做法 {#best-practices-for-image-sharpening}

图像锐化是在您的网站上控制图像的最复杂任务，可能会出现很多错误。请花些时间，通过参考以下有用资源，详细了解Dynamic Media Classic中锐化和USM锐化的工作原理：

最佳实践白皮书[在AdobeDynamic Media Classic和图像服务器上锐化图像](/help/assets/s7_sharpening_images.pdf)。

<!-- Give a 404 See also [Sharpening an image with unsharp mask](https://helpx.adobe.com/photoshop/atv/cs6-tutorials/sharpening-an-image-with-unsharp-mask.html). -->

借助Dynamic Media Classic，您可以在摄取、交付或同时在两者中锐化图像。 但是，通常只使用一种方法锐化图像，而不使用两种方法锐化图像。 传送时在 URL 上锐化图像通常可以获得最佳的效果。

可以使用以下两种图像锐化方法：

* 简单锐化(`&op_sharpen`) — 简单锐化与Photoshop中使用的锐化滤镜类似，它会在动态调整大小后对图像的最终视图应用基本锐化。 不过，用户无法配置这种方法。最佳实践是除非有必要，否则不使用`&op_sharpen`。
* USM锐化(`&op_USM`)- USM锐化是行业标准的锐化滤镜。 最佳做法是按照以下准则使用 USM 锐化功能锐化图像。可以通过 USM 锐化控制以下三个参数：

   * `&op_sharpen=amount,radius,threshold`

      * `amount`（0-5，效果的强度。）
      * `radius`（0-250，在锐化的对象周围绘制的“锐化线条”的宽度，以像素为单位。）

         请记住，`radius` 和 `amount` 参数的作用是相反的。通过增加`amount`可以补偿`radius`的减少。 `Radius` 可以进行更精确的控制，因为较低的值仅锐化边缘像素，而较高的值锐化范围更宽的像素。

      * `threshold` （0-255，效果的敏感性。）

         此参数确定锐化的像素与周围区域必须有多大的不同，才会被视为边缘像素，而滤镜会锐化这些像素。 阈值有助于避免出现具有类似颜色的过度锐化区域，如肤色。例如，阈值为12时，会忽略肤色亮度的细微变化，以避免添加“杂色”，同时仍会为高对比度区域添加边缘对比度，如睫毛与皮肤相遇的地方。

         有关如何设置这三个参数的更多信息（包括与滤镜一起使用的最佳实践），请参阅[在Dynamic Media ClassicAdobe和图像服务器](/help/assets/s7_sharpening_images.pdf)上锐化图像。

      * Dynamic Media Classic还允许您控制第四个参数：单色(`0,1`)。 此参数确定是使用值 `0` 将 USM 锐化分别应用于每个颜色分量，还是使用值 `1` 将 USM 锐化应用于图像亮度/强度。

作为最佳做法，请从 USM 锐化 radius 参数入手。可以最初使用以下 radius 设置：

* 网站：0.2-0.3 像素
* 摄影打印 (250-300 ppi)：0.3-0.5 像素
* 胶印胶印 (266-300 ppi)：0.7-1.0 像素
* 画布打印 (150 ppi)：1.5-2.0 像素

将 amount 从 1.75 逐渐增加到 4。如果锐化仍达不到所需的效果，请按小数点增加 radius 值，然后再次将 amount 从 1.75 增加到 4。根据需要，重复此步骤。

将 monochrome 参数设置保留为 0。

## JPEG 压缩的最佳做法 (&amp;qlt=) {#best-practices-for-jpeg-compression-qlt}

* 此参数控制 JPG 编码质量。较高的值表示图像质量较高，但文件较大；而较低的值表示图像质量较低，但文件较小。此参数的范围是 0-100。
* 要优化质量，不要将参数值设置为 100。几乎感觉不到设置 90 或 95 与 100 之间的差异，但 100 会不必要地增加图像文件的大小。因此，要优化质量，同时避免图像文件过大，请将`qlt=`值设置为90或95。
* 要优化较小的图像文件大小，但将图像质量保持在可接受的级别，请将`qlt=`值设置为80。 低于 70 到 75 的值将导致图像质量大大下降。
* 最佳做法是：要保持居中，请将`qlt=`值设置为85以保持居中。
* 在 `qlt=` = 中使用色度标记

   * `qlt=`参数有第二个设置，允许您使用正常值`,0`（默认）打开RGB色度缩减采样，或使用值`,1`关闭。
   * 要保持简单，请首先关闭RGB色度缩减采样(`,1`)。 此设置通常会获得较好的图像质量，尤其是具有很多清晰边缘和对比度的合成图像。

作为JPG压缩的最佳实践，请使用`&qlt=85,0`。

## JPEG 大小调整的最佳做法 (&amp;jpegSize=) {#best-practices-for-jpeg-sizing-jpegsize}

如果要确保图像不会超过某个大小，以便传送到内存有限的设备，则参数`jpegSize`非常有用。

* 此参数以千字节为单位进行设置(`jpegSize=<size_in_kilobytes>`)。 它定义了图像传送允许的最大大小。
* `&jpegSize=` 与JPG压缩参数交互 `&qlt=`。如果具有指定JPG压缩参数(`&qlt=`)的JPG响应没有超过`jpegSize`值，则返回图像时会按照定义的`&qlt=`。 否则，`&qlt=`会逐渐减小，直到图像符合允许的最大大小，或直到系统确定它不能满足并返回错误为止。

如果要将JPG图像传送到内存有限的设备，请设置`&jpegSize=`并添加参数`&qlt=`，这是最佳做法。

## 最佳做法摘要 {#best-practices-summary}

作为最佳做法，要获得较高的图像质量和较小的文件大小，请从以下参数组合入手：

`fmt=jpg&qlt=85,0&resMode=sharp2&op_usm=1.75,0.3,2,0`

大多数情况下，这种设置组合将获得极佳的效果。

如果需要进一步优化图像，请先将 radius 设置为 0.2 或 0.3 以逐步调整锐化（USM 锐化）参数。然后，将 amount 从 1.75 逐渐增加到最多 4（相当于 Photoshop 中的 400%）。检查是否获得了所需的效果。

如果锐化效果仍不令人满意，请按小数点增加 radius 值。每增加一个小数点，请再次将 amount 从 1.75 逐渐增加到 4。重复此过程，直到获得所需的效果。尽管创意工作室已对上面的值进行了验证，但要记住，您最初可以使用其他值和采用其他策略。您对结果是否满意是一个非常主观的问题，因此，进行结构化的试验是至关重要的。

在您进行实验时，以下常规建议有助于优化工作流：

* 可以直接在Dynamic Media Classic URL上或使用Dynamic Media Classic的图像调整功能，实时尝试和测试不同的参数。 后者提供调整操作的实时预览。
* 作为最佳实践，请记住，可以将Dynamic Media图像提供命令分组到图像预设中。 图像预设基本上就是具有自定义预设名称（如`$thumb_low$`和`&product_high$`）的URL命令宏。 URL路径中的自定义预设名称会调用这些预设。 此功能帮助您针对网站上的图像的不同使用方式管理命令和质量设置，并缩短 URL 的总体长度。
* Dynamic Media Classic还提供了更高级的图像质量调整方法，例如在摄取时应用图像锐化。 对于高级用例，如果可以进一步调整和优化渲染的结果，Adobe Professional Services可以帮助您获得自定义的洞察信息和最佳实践。
