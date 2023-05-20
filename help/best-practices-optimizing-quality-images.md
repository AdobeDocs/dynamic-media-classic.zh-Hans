---
title: 优化图像质量的最佳做法
description: 瞭解影像品質最佳化的最佳實務。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 3c50e706-b9ed-49db-8c08-f179de52b9cf
source-git-commit: f3082fc6b66cf0903bf6cb1907a8615a12399fdc
workflow-type: tm+mt
source-wordcount: '1569'
ht-degree: 50%

---

# 优化图像质量的最佳做法{#best-practices-for-optimizing-the-quality-of-your-images}

优化图像质量可能是一个需要很长时间的过程，因为很多因素都会影响提供可接受的结果。结果在一定程度上是主观性的，因为个人评价图像质量的标准不尽相同。因此，进行结构化的试验是至关重要的。

Adobe Dynamic Media Classic包含100多個影像伺服命令，可用於調整和最佳化影像及演算結果。 以下准则可以帮助您简化流程，并使用一些基本命令和最佳做法快速获得较好的效果。

另請參閱 [智慧型影像](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/imaging-faq.html#dynamic).

>[!TIP]
>
>嘗試使用Dynamic Media來探索Dynamic Media影像修飾元和智慧型影像處理的優點 [_快照_](https://snapshot.scene7.com/).
>
> Snapshot是視覺化展示工具，旨在說明Dynamic Media在最佳化及動態影像傳送方面的強大功能。 實驗測試影像或Dynamic Media URL，以視覺化方式觀察各種Dynamic Media影像修飾元的輸出，以及針對下列專案的智慧型影像最佳化：
>* 檔案大小（含WebP和AVIF傳送）
>* 網路頻寬
>* DPR （裝置畫素比率）
>
>若要瞭解使用快照的簡單程度，請播放 [快照訓練影片](https://experienceleague.adobe.com/docs/experience-manager-learn/assets/dynamic-media/images/dynamic-media-snapshot.html?lang=en) （3分17秒）。


## 图像格式的最佳做法 (&amp;fmt=) {#best-practices-for-image-format-fmt}

* 在提供具有较好质量和可控制大小和粗细的图像方面，JPG 或 PNG 是最佳选择。
* 如果URL中未提供任何格式命令，Dynamic Media Image Serving會預設為傳送JPG。
* JPG 压缩比率为 10:1，通常生成较小的图像文件。PNG會以大約2:1的比率壓縮，除非有時影像包含空白背景。 通常，PNG 文件比 JPG 文件大。
* JPG 使用有损压缩，这意味着在压缩过程中删除了一些图像元素（像素）；而 PNG 使用无损压缩。
* 通常，JPG 压缩摄影图像的保真度比具有清晰边缘和对比度的合成图像好。
* 如果图像包含透明度，请使用 PNG，因为 JPG 不支持透明度。

影像格式的最佳作法是從最常見的設定開始 `&fmt=JPG`.

## 图像大小的最佳做法 {#best-practices-for-image-size}

動態縮減影像大小是Dynamic Media Image Serving最常執行的工作之一。 这包括指定大小，以及指定用于减小图像的缩减像素采样模式（可选）。

* 調整影像大小時，最好且最直接的方法是使用 `&wid=<value>` 和 `&hei=<value>` 或只是 `&hei=<value>`. 这些参数自动根据高宽比设置图像宽度。
* `&resMode=<value>` 控制縮減取樣所使用的演演算法。 開始於 `&resMode=sharp2`. 该值提供了最佳的图像质量。使用縮減取樣值時 `=bilin` 速度較快，通常會導致鋸齒狀不自然感。

如需調整影像大小的最佳作法，請使用 `&wid=<value>&hei=<value>&resMode=sharp2` 或 `&hei=<value>&resMode=sharp2`

## 图像锐化的最佳做法 {#best-practices-for-image-sharpening}

图像锐化是在您的网站上控制图像的最复杂任务，可能会出现很多错误。請參考下列實用資源，以進一步瞭解銳利化和非銳利化遮色片在Adobe Dynamic Media Classic中的運作方式：

最佳實務白皮書 [在Adobe Dynamic Media Classic和影像伺服器上銳利化影像](/help/assets/s7_sharpening_images.pdf).

<!-- Give a 404 See also [Sharpening an image with unsharp mask](https://helpx.adobe.com/photoshop/atv/cs6-tutorials/sharpening-an-image-with-unsharp-mask.html). -->

透過Adobe Dynamic Media Classic，您可以在內嵌和/或傳送時銳利化影像。 不過，通常您只會使用其中一種方法來銳利化影像，但不會同時使用這兩種方法來銳利化。 传送时在 URL 上锐化图像通常可以获得最佳的效果。

有兩種影像銳利化方法可供您使用：

* 簡單銳利化( `&op_sharpen`) — 類似於Photoshop中使用的銳利化濾鏡，簡單銳利化會在動態調整大小後，將基本銳利化套用至影像的最終檢視。 不过，用户无法配置这种方法。最佳實務是不使用 `&op_sharpen` 除非有需要。
* 不銳利化遮色片( `&op_USM`) — 不銳利化遮色片是業界標準的銳利化濾鏡。 最佳做法是按照以下准则使用 USM 锐化功能锐化图像。可以通过 USM 锐化控制以下三个参数：

   * `&op_sharpen=amount,radius,threshold`

      * `amount`（0-5，效果的强度。）
      * `radius`（0-250，在锐化的对象周围绘制的“锐化线条”的宽度，以像素为单位。）

         请记住，`radius` 和 `amount` 参数的作用是相反的。減少 `radius` 可以通過增加來補償 `amount`. `Radius` 可以进行更精确的控制，因为较低的值仅锐化边缘像素，而较高的值锐化范围更宽的像素。

      * `threshold` （0-255，效果敏感度。）

         此参数确定锐化的像素与周围区域相差多少，滤镜才会将它们视为边缘像素并进行锐化。阈值有助于避免出现具有类似颜色的过度锐化区域，如肤色。例如，阈值 12 忽略肤色亮度的细微变化以避免产生杂色，但仍会在对比强烈的区域中添加边缘对比度，例如，睫毛与皮肤交接的位置。

         如需如何設定這三個引數的詳細資訊，包括篩選使用的最佳實務，請參閱 [在Adobe Dynamic Media Classic和影像伺服器上銳利化影像](/help/assets/s7_sharpening_images.pdf).

      * Adobe Dynamic Media Classic也可讓您控制第四個引數：單色( `0,1`)。 此参数确定是使用值 `0` 将 USM 锐化分别应用于每个颜色分量，还是使用值 `1` 将 USM 锐化应用于图像亮度/强度。

作为最佳做法，请从 USM 锐化 radius 参数入手。可以最初使用以下 radius 设置：

* 网站：0.2-0.3 像素
* 摄影打印 (250-300 ppi)：0.3-0.5 像素
* 胶印胶印 (266-300 ppi)：0.7-1.0 像素
* 画布打印 (150 ppi)：1.5-2.0 像素

将 amount 从 1.75 逐渐增加到 4。如果锐化仍达不到所需的效果，请按小数点增加 radius 值，然后再次将 amount 从 1.75 增加到 4。根据需要，重复此步骤。

将 monochrome 参数设置保留为 0。

## JPEG 压缩的最佳做法 (&amp;qlt=) {#best-practices-for-jpeg-compression-qlt}

* 此参数控制 JPG 编码质量。较高的值表示图像质量较高，但文件较大；而较低的值表示图像质量较低，但文件较小。此参数的范围是 0-100。
* 要优化质量，不要将参数值设置为 100。几乎感觉不到设置 90 或 95 与 100 之间的差异，但 100 会不必要地增加图像文件的大小。因此，若要最佳化影像品質，但避免影像檔案過大，請設定 `qlt=` 值為90或95。
* 若要針對較小的影像檔案大小進行最佳化，但將影像品質維持在可接受的等級，請設定 `qlt=` 值為80。 低于 70 到 75 的值将导致图像质量大大下降。
* 最佳做法是居於中間，將 `qlt=` 值設為85，則維持在中間位置。
* 在 `qlt=` = 中使用色度标记

   * 此 `qlt=` 引數有第二個設定，可讓您使用一般值開啟RGB色度縮減取樣 `,0` （預設），或使用值將其關閉 `,1`.
   * 若要保持簡單，請從RGB色度縮減取樣關閉( `,1`)。 此设置通常会获得较好的图像质量，尤其是具有很多清晰边缘和对比度的合成图像。

使用JPG壓縮當作最佳實務 `&qlt=85,0`.

## JPEG 大小调整的最佳做法 (&amp;jpegSize=) {#best-practices-for-jpeg-sizing-jpegsize}

引數 `jpegSize` 如果您想要保證影像不會超過傳送至記憶體有限之裝置的特定大小，這個選項就十分實用。

* 此引數是以千位元組( `jpegSize=<size_in_kilobytes>`)。 它定义了图像传送允许的最大大小。
* `&jpegSize=` 與JPG壓縮引數互動 `&qlt=`. 如果JPG回應具有指定的JPG壓縮引數( `&qlt=`)不可超過 `jpegSize` 值，則影像會以 `&qlt=` 依定義。 否則， `&qlt=` 會逐漸減少，直到影像符合允許的大小上限，或直到系統判斷它無法符合併傳回錯誤為止。

最佳實務是 `&jpegSize=` 並新增引數 `&qlt=` 如果您要將JPG影像傳送至記憶體有限的裝置。

## 最佳做法摘要 {#best-practices-summary}

作为最佳做法，要获得较高的图像质量和较小的文件大小，请从以下参数组合入手：

`fmt=jpg&qlt=85,0&resMode=sharp2&op_usm=1.75,0.3,2,0`

大多数情况下，这种设置组合将获得极佳的效果。

如果需要进一步优化图像，请先将 radius 设置为 0.2 或 0.3 以逐步调整锐化（USM 锐化）参数。然后，将 amount 从 1.75 逐渐增加到最多 4（相当于 Photoshop 中的 400%）。检查是否获得了所需的效果。

如果锐化效果仍不令人满意，请按小数点增加 radius 值。每增加一个小数点，请再次将 amount 从 1.75 逐渐增加到 4。重复此过程，直到获得所需的效果。尽管创意工作室已对上面的值进行了验证，但要记住，您最初可以使用其他值和采用其他策略。您对结果是否满意是一个非常主观的问题，因此，进行结构化的试验是至关重要的。

實驗時，以下一般建議有助於最佳化您的工作流程：

* 請直接在URL上或使用Adobe Dynamic Media Classic的影像調整功能，即時嘗試並測試不同的引數。 後者提供調整作業的即時預覽。
* 如需參考最佳做法，請記住，您可以將「Dynamic Media影像伺服」命令群組至影像預設集。 影像預設集基本上是含有自訂預設集名稱的URL命令巨集，例如 `$thumb_low$` 和 `&product_high$`. URL路徑中的自訂預設集名稱會呼叫這些預設集。 此功能帮助您针对网站上的图像的不同使用方式管理命令和质量设置，并缩短 URL 的总体长度。
* Adobe Dynamic Media Classic也提供更進階的影像品質調整方式，例如在擷取時套用影像銳利化。 針對可選擇進一步調整及最佳化呈現結果的進階使用案例，Adobe Professional Services可協助您提供自訂的深入分析和最佳作法。
