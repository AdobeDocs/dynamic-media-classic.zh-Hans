---
title: 锐化图像
description: 了解如何在Adobe Dynamic Media Classic中锐化图像。
uuid: d86af74a-89c5-4f2b-96ba-f2e7da600bca
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 11cd5362-d90a-4c1e-bfbd-46a65a554409
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 4b3e8368-f8f5-46d9-9130-361a8273de2c
source-git-commit: 352b1c383195fa03294ad3501207d63f3cfe3e42
workflow-type: tm+mt
source-wordcount: '2276'
ht-degree: 41%

---

# 锐化图像 {#sharpening-an-image}

锐化是为了让数字图像的轮廓变得更为清晰的图像处理技术。锐化会增加边缘像素之间的对比度，并强调明暗区域的过渡。锐化将增加局部对比度，展现细节。并没有严格的公式可以正确锐化所有图像。锐化过少会使得图像对比度较弱，但过分锐化会增添光晕、伪影和杂波。

Adobe Dynamic Media Classic强烈建议您对所有图像使用图像预设。 它们可确保大小一致，并且会对使用“图像预设”调用的任何图像强制执行锐化。 此外，您还可以轻松编辑和更改图像预设的锐化参数。 下次发布时，将为使用该预设调用的所有图像提供新的值。

Adobe Dynamic Media Classic还建议先对查看器预设添加锐化，然后再使用该预设调用查看器。 这样做可确保查看器内的图像清晰而吸引人。

但是，无论您使用图像预设和查看器预设，还是使用其他锐化方法，总之，您必须锐化图像。 如果不这样做，您的图像（和网站）看起来会很柔和模糊。

>[!NOTE]
>
>“锐化”命令可覆盖图像预设设置，包括锐化效果。图像预设可控制从Dynamic Media图像服务器传送图像的大小和格式。 Adobe Dynamic Media Classic强烈建议使用图像预设传送所有图像，以确保以均匀的大小和锐化传送图像。 不过，在更改单个图像的锐化设置之后，图像预设锐化设置将不再应用于该图像。该图像在传送时将不使用图像预设锐化设置。

通常锐化图像是必须的。Adobe Dynamic Media Classic和图像服务器提供了多个锐化选项。 了解锐化对图像的作用以及您所需的锐化程度很重要。大多数图像都需要进行一定程度的锐化，但是所需的锐化程度取决于图像。

图像锐化可增加像素的对比度，从而达到突出边缘的效果。人们将这种增强的边缘对比度视为锐度。尽管通过对图像使用锐化滤镜可以很轻松地提高图像品质，但是也很容易过度锐化图像。

过度锐化将造成光晕效果，或使边缘线生成条纹。

您可以遵循一些最佳实践，以优化Adobe Dynamic Media Classic和Dynamic Media图像服务器上图像的锐化。

请参阅[在Adobe Dynamic Media Classic和Dynamic Media图像服务器上锐化图像的最佳实践](/help/assets/s7_sharpening_images.pdf)。

另请参阅[锐化](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/547_sharpening1_converted%20renamed_Done-AVS)培训视频。

**锐化图像:**

要锐化图像，请选择其滚动图像&#x200B;**[!UICONTROL 编辑]**&#x200B;按钮，然后选择&#x200B;**[!UICONTROL 锐化]**，或在“详细信息视图”的“浏览面板”中将其打开，然后选择&#x200B;**[!UICONTROL 锐化]**。 “锐化编辑器”页面随即会打开，其中包含锐化命令。 选择命令，然后选择&#x200B;**[!UICONTROL Save]**。

>[!NOTE]
>
>锐化图像之前，您可以选择“应用预设”菜单，然后选择一种图像预设来查看其锐化效果。图像预设的锐化效果适合您的图像。 **[!UICONTROL 应用预设]**&#x200B;菜单位于“锐化编辑器”页面的底部。

**锐化选项**

图像服务器锐化选项如下表所示。

| 名称 | URL 协议 | 值 | 示例 |
| --- | --- | --- | --- |
| 简单锐化 | `op_sharpen` | `0` 或者 `1` | `op_sharpen=1` |
| 重新采样模式 | `resMode` | `bilin`、  `bicub`、  `sharp2`、  `trilin`<br><br>`bilin`:选择标准的双线性插值。最快的重采样方法；通常会出现一些锯齿伪像。<br>`bicub`:选择双三次插值。对 CPU 比 bilin 更敏感，但会产生更清晰且锯齿伪影不太明显的图像。<br><br>`sharp2`:选择修改的Lanczos Windows®函数作为插值算法。在CPU成本较高的情况下，生成比两次立方体更锐利的结果。<br><br>`trilin`：选择改进的三线式插值法，它同时使用更高和更低的分辨率（如果可用）。建议仅当存在锯齿问题时使用。由于减少高频数据而缩小 JPEG 大小。 | `resMode=sharp2` |
| USM 锐化 | `op_usm` | `amount`、  `radius`、  `threshold`、  `monochrome`<br><br>`amount`:滤镜强度因子（实数0...5）<br><br>`radius`:筛选内核半径（以像素为单位，实数为0..250） <br><br>`threshold`:筛选阈值级别（整数0...255）<br><br>`monochrome`:将设置为 `0` 分别对每个颜色组件进行钝化蒙版，将设置为 `1` 对图像亮度（强度）进行钝化蒙版 | `op_usm=1,1,10,0` |

选择&#x200B;**[!UICONTROL 锐化]**&#x200B;菜单，然后选择一个选项：

* **无**  — 禁用锐化。

* **锐化**  — 调整文件大小后，对文件运行简单的锐化传递。它类似于Adobe Photoshop中的“锐化”滤镜，它支持任何用户参数。 通常，您会使用此滤镜或&#x200B;**[!UICONTROL 钝化蒙版]**，但不会同时使用两者。 最佳做法不建议使用此方法，但是它有助于补偿模糊。(URL: `op_sharpen`)

* **钝化蒙版**  — 允许您对最终缩减采样图像微调锐化滤镜效果。您可以控制效果的强度、效果的半径（以像素为单位）以及被忽略的对比度阈值。 此效果使用与 Photoshop 的“钝化蒙蔽”滤镜相同的选项。(URL:`op_usm`)

选择以下选项，以便使用USM锐化对锐化进行微调：

* **数量**  — 控制对边缘像素应用的对比度数量。默认值为 0.0。对于高分辨率图像，可将该值增加到 5.0。数量用于衡量滤镜强度。Adobe Dynamic Media Classic中的&#x200B;**[!UICONTROL Amount]**&#x200B;设置与Adobe Photoshop中的Amount设置不同。 Adobe Photoshop使用的金额范围为1%到500%，而Adobe Dynamic Media Classic则范围为0.0到5.0。 （5.0 大致相当于 Photoshop 中的 500%，0.9 类似于 90%，以此类推。）

* **半径**  — 确定边缘像素周围影响锐化的像素数。此效果应用于图像中的所有像素并向四面八方辐射。

最佳半径值取决于图像的大小。低值仅锐化边缘像素。高值锐化像素的范围更广一些。

例如，要对2000 x 2000像素图像和500 x 500像素图像获得类似的锐化效果，可以在2000 x 2000像素图像上设置两个像素的半径值。 然后，在 500 x 500 像素图像上设置 1 个像素的半径值（具有较多像素的图像具有较大的值）。

* **阈值**  — 确定在应用USM锐化滤镜时要忽略的对比度范围。此选项确定锐化的像素必须与周围区域相差多少，才被滤镜看作边缘像素并被锐化。

阈值使用0到255之间的值，该值是灰度图像中的亮度步骤数。 0=黑色，128=50% 灰色，255=白色。例如，阈值 12 忽略肤色亮度的细微变化以避免增加杂色，但仍会在对比强烈的区域中添加边缘对比度，例如，睫毛与皮肤交接的位置。

例如，假定有一张某人脸部的照片。USM 锐化影响具有最大对比度的图像部分和光滑皮肤本身。甚至最平滑的皮肤也会展现亮度值的细微更改。如果您不使用阈值，滤镜将强调皮肤像素的这些细微更改，从而创建杂色效果（很可能不需要此效果），同时还将增加睫毛的对比度，增强锐度（很可能需要此效果）。为了避免出现该问题，请使用此类阈值：可使滤镜忽略未显著更改对比度的像素（如平滑的皮肤）。为避免引入含有肉色色调的噪声或后验图像，例如尝试使用&#x200B;**[!UICONTROL Threshold]**&#x200B;值2到20。 默认的&#x200B;**[!UICONTROL Threshold]**&#x200B;值为0会锐化图像中的所有像素。

* **应用到**  — 如果要 **[!UICONTROL 分别]** 对每种颜色组件应用锐化，请选择每种颜色；如果 **** 要对图像亮度区域应用锐化，请选择Brightness。

**重新取样**

选择&#x200B;**[!UICONTROL 重新取样]**&#x200B;菜单，然后选择一个选项。 当图像缩减像素取样时，以下选项锐化该图像：

* **[!UICONTROL 无]**  — 关闭重新取样。

* **[!UICONTROL 双线性]**  — 最快速的重新取样方法；会出现一些锯齿伪像。

* **[!UICONTROL 双立方]**  — 提高图像服务器的CPU使用率，但会生成较锐利的图像，出现的锯齿伪像较少。

* **[!UICONTROL 锐化2]**  — 生成的结果比双立方 **[!UICONTROL 法]**&#x200B;更锐利，但图像服务器的CPU成本更高。

* **[!UICONTROL 三线性]**  — 如果可用，则同时使用较高和较低分辨率；仅当出现锯齿问题时，才建议使用。由于减少了高频数据，此方法会减小 JPEG 的大小。

**锐化预设和图像预设**

您可以整合所有三种锐化效果，以获得最终效果。 但是，不建议使用此方法。 Adobe Dynamic Media Classic建议您将锐化效果另存为图像预设的一部分。 通过图像预设，您可以打包最常用的图像修饰符，以便以小文本字符串的形式创建动态调整大小的图像。 图像预设包含文件格式(通常为WebJPEG)、像素计数和图像锐化的值。 您无需在附加每个图像修饰符（必须使用这些修饰符来创建特定类型的图像大小）的同时，创建一个命名的图像预设，如“缩略图”。 然后，使用相应的大小、文件格式和锐化选项配置缩略图图像预设。 使用图像预设名称调用图像。 图像预设可缩短整个URL的长度。 这两个URL会生成相同的350x350JPEG图像，且具有锐化功能：

* `https://sample.scene7.com/is/image/S7train/Backpack_A?wid=350&hei=350&fmt=jpeg&qlt=85,0&resMode=sharp2&op_usm=0.9,1.0,8,0`
* `https://sample.scene7.com/is/image/S7train/Backpack_A?$!_s7product$`

图像预设随时都可以更改和更新。在发布后和清除URL的缓存后，您会看到对图像预设进行更改的结果。

如果您为一个大小类别中的每个图像使用一个预设，则任何公司管理员都可以更新该图像预设的定义、重新发布，并影响使用该格式的每个图像，而无需更改任何 Web 代码。作为最佳做法，请在您的网站针对每个特定大小使用一个图像预设。要添加图像预设，请在全局导航栏中，转到&#x200B;**[!UICONTROL 设置]** > **[!UICONTROL 应用程序设置]** > **[!UICONTROL 图像预设]**。 然后，选择&#x200B;**[!UICONTROL 添加]**&#x200B;或选择&#x200B;**[!UICONTROL 编辑]**&#x200B;以更改现有预设。 唯一的必填字段是预设自身的名称。但是，最好在每个预设中包含一定程度的锐化。

**JPG 品质**

JPG 品质选项控制 JPG 压缩等级：

* **JPG质量**  — 如果要控制压缩级别和色度缩减采样，请选择此选项。

* **滑块**  — 确定JPG压缩级别。此设置既影响文件大小，又影响图像质量。JPG质量比例尺为1-100。

* **启用JPG色度缩减采样**  — 由于眼睛对高频颜色信息的敏感程度低于高频亮度，因此JPEG图像会将图像信息分为亮度和颜色分量。压缩 JPEG 图像时，通过将各组像素放到一起平均，亮度分量为全分辨率，颜色分量为缩减像素取样。缩减像素采样会将数据量减少二分之一或三分之一，而对于用户所能感知到的质量而言却几乎没有任何影响。缩减像素采样不适用于灰度图像。这种方法会减少对于高对比度图像有用的压缩的数量（例如，包含覆盖文本的图像）。

**设置公司范围的锐化选项**

如果您不使用图像预设，或未通过 URL 字符串传送特定的图像服务器锐化协议，在缩减像素采样时，不会对您的图像进行锐化。但是，如果出现这种缺少锐化的情况，您可以设置默认锐化值，然后任何图像都始终会有一些锐化。

要设置公司的默认锐化选项，请转到&#x200B;**[!UICONTROL 设置]** > **[!UICONTROL 应用程序设置]** > **[!UICONTROL 发布设置]** > **[!UICONTROL 图像服务器]**。 如果将默认的重新取样模式设置为&#x200B;**[!UICONTROL Sharp2]**，则在缩减像素采样时会始终锐化图像。

**为查看器预设添加锐化**

除非您将锐化图像修饰符添加到预设，否则较小的初始加载图像会看起来对比度较柔和，因为它在未进行锐化的情况下被缩减像素采样以适合查看器窗口。

查看器预设（与图像预设类似）允许您将多个选项集中到一个位置，包括选择外观和查看器选项（例如，包括“打印”按钮或控制缩放动画的速度）。 查看器预设位于与图像预设相同的部分中，位于&#x200B;**[!UICONTROL 设置]** > **[!UICONTROL 应用程序设置]** > **[!UICONTROL 查看器预设]**&#x200B;下。

请参阅[查看器预设](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/550_viewer-presets_converted%20renamed_Done-AVS)培训视频。

可在所有“eCatalog”、“旋转”和“自定义缩放查看器预设”的“核心设置”部分下找到“修饰符”选项。通过将 URL 锐化命令添加到“修饰符”框中，每次使用该查看器预设调用该查看器时，您都可以添加锐化。

要调用查看器预设，请使用查看器URL上的`config=`命令。 以下是使用查看器预设(`FantasticoZoom2022`)调用图像集（鞋）的示例：

`https://s7d9.scene7.com/s7viewers/html5/ZoomViewer.html?asset=Scene7SharedAssets/ImageSet-Views-Sample&config=S7train/FantasticoZoom2022`

此处的预设将锐化并更改查看器的默认外观。

**创建特定于图像的覆盖**

最后一个最不推荐的锐化方法是在基于图像创建锐化覆盖。此方法会使用其自身的特定值覆盖图像预设中的锐化。 但是，此方法也会覆盖所有其他任何大小的锐化方法。 此方法最好用于以下情况：如果您的某些图像分辨率不高，而图像预设的值对于这些小图像而言太高。在这种情况下，可能需要按图像锐化一些。

在Adobe Dynamic Media Classic中，选择任意图像，转到“详细信息视图”（通过双击或按&#x200B;**[!UICONTROL 详细信息视图]**&#x200B;按钮），然后选择“锐化&#x200B;]**”。**[!UICONTROL &#x200B;更改任何参数，然后选择&#x200B;**[!UICONTROL Save]**。 此过程会告知图像服务器使用这些锐化参数，而不是您在URL中调用的任何命令，如锐化修饰符或图像预设。 请确保发布以查看更改是否生效。
