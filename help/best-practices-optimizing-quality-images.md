---
title: 优化图像质量的最佳做法
description: 了解优化图像质量的最佳实践。
uuid: 102e83fe-ee2a-443b-ba92-6ad5cc3daef0
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 8164466e-2520-482a-88ec-6191fdc77ea3
translation-type: tm+mt
source-git-commit: ca12c96d3a76cfa52fd930d190476cb6fc4f4ac7
workflow-type: tm+mt
source-wordcount: '1517'
ht-degree: 61%

---


# 优化图像质量的最佳做法{#best-practices-for-optimizing-the-quality-of-your-images}

优化图像质量可能是一个需要很长时间的过程，因为很多因素都会影响提供可接受的结果。结果在一定程度上是主观性的，因为个人评价图像质量的标准不尽相同。因此，进行结构化的试验是至关重要的。

Dynamic Media经典包含100多个图像服务命令，用于调整和优化图像以及渲染结果。 以下准则可以帮助您简化流程，并使用一些基本命令和最佳做法快速获得较好的效果。

另请参阅[智能成像](https://helpx.adobe.com/experience-manager/6-3/assets/using/imaging-faq.html)。

## 图像格式的最佳做法 (&amp;fmt=) {#best-practices-for-image-format-fmt}

* 在提供具有较好质量和可控制大小和粗细的图像方面，JPG 或 PNG 是最佳选择。
* 如果URL中未提供任何格式命令，则Dynamic Media图像服务默认为JPG以进行投放。
* JPG 压缩比率为 10:1，通常生成较小的图像文件。PNG的压缩比率约为2:1，但某些情况除外，例如当图像包含空背景时。 通常，PNG 文件比 JPG 文件大。
* JPG 使用有损压缩，这意味着在压缩过程中删除了一些图像元素（像素）；而 PNG 使用无损压缩。
* 通常，JPG 压缩摄影图像的保真度比具有清晰边缘和对比度的合成图像好。
* 如果图像包含透明度，请使用 PNG，因为 JPG 不支持透明度。

作为图像格式的最佳实践，请使用最常见的设置`&fmt=JPG`进行开始。

## 图像大小的最佳做法 {#best-practices-for-image-size}

动态缩小图像大小是Dynamic Media图像服务执行的最常见的任务之一。 这包括指定大小，以及指定用于减小图像的缩减像素采样模式（可选）。

* 对于图像大小调整，最佳且最直接的方法是使用`&wid=<value>`和`&hei=<value>`或仅使用`&hei=<value>`。 这些参数自动根据高宽比设置图像宽度。
* `&resMode=<value>` 控制用于缩减采样的算法。开始`&resMode=sharp2`。 该值提供了最佳的图像质量。虽然使用缩减采样值`=bilin`速度更快，但通常会导致出现锯齿伪像。

作为调整图像大小的最佳实践，请使用`&wid=<value>&hei=<value>&resMode=sharp2`或`&hei=<value>&resMode=sharp2`

## 图像锐化的最佳做法 {#best-practices-for-image-sharpening}

图像锐化是在您的网站上控制图像的最复杂任务，可能会出现很多错误。请花时间参考以下有用资源，进一步了解Dynamic Media经典中锐化和USM锐化的工作原理：

最佳实践白皮书[在Dynamic Media经典Adobe和图像服务器](/help/assets/s7_sharpening_images.pdf)上锐化图像。

另请参阅[使用USM锐化锐化图像](https://helpx.adobe.com/photoshop/atv/cs6-tutorials/sharpening-an-image-with-unsharp-mask.html)。

借助Dynamic Media经典，您可以在摄取、投放或两者时锐化图像。 大多数情况下，只应使用一种方法锐化图像，而不能同时使用两种方法。传送时在 URL 上锐化图像通常可以获得最佳的效果。

可以使用以下两种图像锐化方法：

* 简单锐化(`&op_sharpen`)-简单锐化与在Photoshop使用的锐化滤镜类似，在动态调整大小后，简单锐化将基本锐化应用于图像的最终视图。 不过，用户无法配置这种方法。最佳做法是，除非需要，否则不使用`&op_sharpen`。
* USM锐化(`&op_USM`)- USM锐化是行业标准的锐化滤镜。 最佳做法是按照以下准则使用 USM 锐化功能锐化图像。可以通过 USM 锐化控制以下三个参数：

   * `&op_sharpen=amount,radius,threshold`

      * `amount`（0-5，效果的强度。）
      * `radius`（0-250，在锐化的对象周围绘制的“锐化线条”的宽度，以像素为单位。）

         请记住，`radius` 和 `amount` 参数的作用是相反的。通过增加`amount`可以补偿减少`radius`。 `Radius` 可以进行更精确的控制，因为较低的值仅锐化边缘像素，而较高的值锐化范围更宽的像素。

      * `threshold` （0-255，效果的敏感性。）

         此参数确定锐化的像素与周围区域必须有多大的不同，才会被视为边缘像素，而滤镜会锐化这些像素。 阈值有助于避免出现具有类似颜色的过度锐化区域，如肤色。例如，阈值为12时，会忽略肤色亮度的细微变化，以避免添加“杂色”，同时仍会为高对比度区域添加边缘对比度，如睫毛与皮肤相遇的地方。

         有关如何设置三个参数的详细信息（包括使用滤镜的最佳做法），请参阅以下资源：

         关于[锐化图像](https://help.adobe.com/en_US/scene7/using/WS389B162D-2981-41e5-9253-15D22D2ECBC8.html)的Dynamic Media经典帮助主题。

         最佳实践白皮书[在Adobe Scene7出版系统和图像服务器上锐化图像](/help/assets/s7_sharpening_images.pdf)。

      * Dynamic Media经典还允许您控制第四个参数：monochrome(`0,1`)。 此参数确定是使用值 `0` 将 USM 锐化分别应用于每个颜色分量，还是使用值 `1` 将 USM 锐化应用于图像亮度/强度。

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
* 要优化较小的图像文件大小，但将图像质量保持在可接受的水平，请将`qlt=`值设置为80。 低于 70 到 75 的值将导致图像质量大大下降。
* 作为最佳实践，要保持在中间，请将`qlt=`值设置为85以保持在中间。
* 在 `qlt=` = 中使用色度标记

   * `qlt=`参数有第二个设置，允许您使用正常值`,0`（默认值）打开RGB色度缩减采样，或使用值`,1`关闭它。
   * 要保持其简单性，已关闭RGB色度缩减采样的开始(`,1`)。 此设置通常会获得较好的图像质量，尤其是具有很多清晰边缘和对比度的合成图像。

作为JPG压缩的最佳实践，请使用`&qlt=85,0`。

## JPEG 大小调整的最佳做法 (&amp;jpegSize=) {#best-practices-for-jpeg-sizing-jpegsize}

如果要确保图像不超过特定大小以传送到具有有限内存的设备，`jpegSize` 是一个非常有用的参数。

* 此参数以千字节为单位进行设置(`jpegSize=<size_in_kilobytes>`)。 它定义了图像传送允许的最大大小。
* `&jpegSize=` 与JPG压缩参数交互 `&qlt=`。如果具有指定JPG压缩参数(`&qlt=`)的JPG响应未超过`jpegSize`值，则将按照定义以`&qlt=`返回图像。 否则，`&qlt=`会逐渐减小，直到图像符合允许的最大大小，或直到系统确定它不能适应并返回错误。

作为最佳实践，如果要将JPG图像传送到内存有限的设备，请设置`&jpegSize=`并添加参数`&qlt=`。

## 最佳做法摘要 {#best-practices-summary}

作为最佳做法，要获得较高的图像质量和较小的文件大小，请从以下参数组合入手：

`fmt=jpg&qlt=85,0&resMode=sharp2&op_usm=1.75,0.3,2,0`

大多数情况下，这种设置组合将获得极佳的效果。

如果需要进一步优化图像，请先将 radius 设置为 0.2 或 0.3 以逐步调整锐化（USM 锐化）参数。然后，将 amount 从 1.75 逐渐增加到最多 4（相当于 Photoshop 中的 400%）。检查是否获得了所需的效果。

如果锐化效果仍不令人满意，请按小数点增加 radius 值。每增加一个小数点，请再次将 amount 从 1.75 逐渐增加到 4。重复此过程，直到获得所需的效果。尽管创意工作室已对上面的值进行了验证，但要记住，您最初可以使用其他值和采用其他策略。您对结果是否满意是一个非常主观的问题，因此，进行结构化的试验是至关重要的。

在进行试验时，您还可能会发现以下常规建议对优化工作流程非常有用：

* 实时尝试和测试不同的参数，可以直接在Dynamic Media经典URL上，也可以使用Dynamic Media经典的图像调整功能，该功能为调整操作提供实时预览。
* 作为最佳实践，请记住，您可以将Dynamic Media图像服务命令分组到图像预设中。 图像预设基本上是具有自定义预设名称（如`$thumb_low$`和`&product_high$`）的URL命令宏。 URL 路径中的自定义预设名称将调用这些预设。此功能帮助您针对网站上的图像的不同使用方式管理命令和质量设置，并缩短 URL 的总体长度。
* Dynamic Media经典还提供更高级的图像质量调整方法，如在摄取时应用锐化图像。 对于可以选择使用预设进一步调整和优化图像以及提供相应结果的高级使用案例，Adobe 专业服务部门可以为您提供自定义分析和最佳做法。
