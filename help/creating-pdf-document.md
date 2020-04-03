---
title: 创建 PDF 文档
seo-title: 创建 PDF 文档
description: 'null'
seo-description: 了解如何在Dynamic Media Classic中使用Web到打印流程创建PDF文档。
uuid: 274fb06b-320b-40fa-8b61-c224d8aceaa1
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template-publishing
discoiquuid: 87e91e8e-10a2-4fba-87c7-aad2bd798146
translation-type: tm+mt
source-git-commit: 6fff3699f8a08af433df3f3a7790a11bf9d05b00

---


# 创建 PDF 文档 {#creating-a-pdf-document}

Web-to-Print 过程的最后一步是生成自定义的 PDF。在最终用户使用您创建的 Web 应用程序创建个性化的模板之后，他们便将创建最终 PDF 文档。这一最终 PDF 通常将发送给印刷服务提供商，以实现专业级印刷水平。要确保按预期印刷最终的 PDF，开发人员应使用正确的作业选项文件并正确设置字体、印刷标记及颜色。

## 设置 PDF 预设 {#setting-up-pdf-presets}

通过创建PDF作业选项文件并将其上传到Dynamic Media Classic Server来指定PDF兼容性级别和打印机设置。 例如，您可以选择符合 PDF/X-4 的 PDF 输出（建议用于 PDF 打印发布工作流程）。您可以在创作软件（如 Adobe Illustrator）或 Acrobat 中创建作业选项文件。请务必咨询您的印刷商，以便针对您的打印作业的作业选项设置给出建议。

有关创建作业选项文件的更多信息以及有关在 Acrobat 中创建作业选项文件的信息，请参阅 Adobe Acrobat 帮助。

要在 Illustrator 中创建作业选项文件：

1. 选择“编辑”>“Adobe PDF 预设”。
1. 在此对话框中，选择要使用的预设。

   Dynamic Media Classic支持以下作业选项设置：

   | 作业选项 | 说明 |
   |--- |--- |
   | 常规 | <ul><li>兼容性 </li><li>对象级压缩</li><li>嵌入缩略图</li><li>优化快速 Web 查看</li></ul> |
   | 图像 | <ul><li>缩减像素取样</li><li>分辨率</li><li>阈值</li><li>颜色、灰度和单色压缩</li></ul> |
   | 字体 | <ul><li>嵌入所有字体（默认情况下，嵌入字体）</li><li>嵌入 OpenType 字体</li><li>子集化嵌入的字体，若被使用的字符百分比低于:</li><li>始终嵌入列表</li><li>永不嵌入列表</li></ul> |
   | 颜色 | <ul><li>颜色策略（仅标记图像被视为标记所有内容）</li><li>文档渲染方法</li><li>4.2.5 仅支持下列工作空间。4.3 将允许您使用已上载到 IPS 的客户提供的配置文件。</li><li>作为一种解决方法，您可以使用公司的默认颜色配置文件为要转换到的插图指定目标颜色空间。</li></ul> |
   | RGB | <ul><li>e-sRGB </li><li>scRGB with encoding range [-4.0, 4.0]</li><li>Lab D50</li><li>PCS XYZ</li><li>平面 XYZ</li><li>线性 ROMM-RGB</li><li>ROMM-RGB</li><li>sYCC 8 位</li><li>e-sYCC 8 位</li></ul> |
   | 灰度 | <ul><li>灰度系数 1.8</li><li>灰度系数 2.2</li><li>网点增大 10%</li><li>网点增大 15%</li><li>网点增大 20%</li><li>网点增大 25%</li><li>网点增大 30%</li><li>sGray</li></ul> |
   | 保留 CMYK 值用于校准的 CMYK 色彩空间 |  |
   | 高级 | 保留 OPI 注释始终处于打开状态 |
   | 标准 | 规范标准 |

   >[!NOTE]
   >
   >Dynamic Media Classic会忽略作业选项文件中的打印机标记设置。 而是通过使用Dynamic Media Classic URL命令配置打印机标记。

1. 单击“导出”，然后指定名称和位置并单击“保存”。
1. 将作业选项文件作为一种资源上载到 Scene7 Publishing System。

   在 URL 中引用该文件，便可在您发布的模板中使用它。例如：

   `https://yourpublishserver.scene7.com/is/agm/SiliconPublishing/PetNews?&fmt=pdf,cmyk&joboption=SPSfilenameid`

## 准备 PDF 进行打印 {#preparing-the-pdf-for-print}

在最终完成 PDF 进行打印之前，请确保您遵循本节中的准则。

**图像**

确保发布作业中的所有图像已上传到Dynamic Media Classic Server并已发布。

**Fonts**

确保发布作业中的所有字体已上传到Dynamic Media Classic Server并已发布。 如果您打算允许最终用户更改字体，请确定您具有托管这些字体的合法权限。

**图像分辨率（每英寸像素）**

Dynamic Media Classic服务器在生成的可打印的PDF中保留位图图像的分辨率。 Dynamic Media Classic会根据需要提高图像分辨率。 为获得最佳效果，请在 Web 上预览时保留默认分辨率值（通常为 72 dpi）。请在“发布设置/图像服务器”窗口的“默认打印分辨率”部分中设置您公司的所有图像的默认分辨率。较高的分辨率（如 300 dpi）可能会导致处理时间更长，仅适用于准备打印的 PDF。在 URL 中使用 imageRes= 命令手动覆盖 PDF 作业的默认分辨率。

**颜色管理**

您的文档和图像可以使用灰度、CMYK、已命名专色、RGB 或 Lab 颜色模型。每一项都可通过采用 ICC 颜色配置文件来进行校色或取消校色。为获得最佳效果，请将该配置文件嵌入生成的准备打印的 PDF 中。默认情况下，Dynamic Media Classic Server会执行此操作。 确保所有必需的颜色用户档案已上传到Dynamic Media Classic平台。 最好确保在设计应用程序中设置的颜色管理选项与在Dynamic Media Classic Server中设置的颜色管理选项相匹配：

* **设计应用程序色彩管理设置：**&#x200B;在您的创作应用程序（如 Adobe Illustrator）的“颜色设置”中，请在“工作空间”部分中指定 RGB 和 CMYK 颜色配置文件。

* **Dynamic Media Classic颜色管理设置：** 通常，设计应用程序中的颜色管理设置应与Dynamic Media Classic服务器中的默认颜色用户档案相匹配。 您可以在“发布设置/图像服务器”窗口中找到这些设置。

## 显示印刷标记 {#displaying-printer-marks}

在以下任一情形中，您可能需要创建 PDF：

* 最终文档
* 中间文档（如胶片或印版），这可能发送给打印机用于制作

中间文档可能包含其他制作内容，如出血边距、印刷标记等等。该内容通常显示在最终页面边界外。

Acrobat“添加印刷标记”屏幕中的所有标记均受支持。印刷标记使用 `printerMark` 参数进行控制。The syntax is `&printerMark=trim marks, bleed marks, registration marks, color bars, page information, style, line weight, layer embed`.

* trim marks = 0|1
* bleed marks = 0|1
* registration marks = 0|1
* color bars = 0|1
* page information = 0|1
* style = Illustrator | IllustratorJ | QuarkXPress
* line weight = 0.125 | 0.25 | 0.50
* layer embed = 0|1

准备文档进行印刷制作时，需要添加一些印刷标记以帮助印刷服务在生成样稿时对齐分色胶片、为获取正确校准数据测量胶片和油墨密度、裁切胶片大小等等。印刷标记表示文档框（如裁切框和出血框）的边界。与制作相关的内容可能包括：

* **介质**&#x200B;盒打印页面的物理介质的边界。 可以安全地放弃媒体框之外的内容，而不会影响文件的内容。

* **出血框**&#x200B;在生产环境中输出时，页面内容被剪切到的区域。 出血框可能包括满足剪切、折叠和裁切设备的固有限制所需的区域。默认值为页面的裁剪框。

* **裁切框**&#x200B;裁切后已完成页面的预期尺寸。 裁切框可能小于媒体框，以便使用与制作相关的内容，如打印说明、剪切标记和颜色条。默认值为页面的裁剪框。

* **作品框**&#x200B;页面创建者期望的页面有意义的内容（包括潜在空白）的范围。 默认值为页面的裁剪框。

您可以使用下表所示的修饰符来复制 Adobe Illustrator、InDesign 和 Acrobat 中的印刷标记：

| 修饰符/值 | 说明 |
|--- |--- |
| bleedMargin=top,left,bottom,right | 在 Acrobat 的“设置页面框”选项中指定。选择“出血框”，然后使用“页面边距控制”选项指定边距。<br><br>值表示从插图（媒体框）的原始边缘向内到上边缘、左边缘、下边缘和右边缘的距离。值(0-1000)以点为单位。<br><br>新高度=原始高度-（顶部+底部）<br><br>新宽度=原始宽度-（左侧+右侧） |
| mediaMargin=top,left,bottom,right | 在 Acrobat 的“设置页面框”选项中指定。在“更改页面大小”选项下修改自定义页面大小。<br><br>值表示从插图（媒体框）的原始边缘向外到上边缘、左边缘、下边缘和右边缘的距离。值(0-1000)以点为单位。<br><br>新高度=top+bottom+原始高<br><br>度新宽度=top+bottom+原始<br><br>宽度新高度和新宽度值决定生成的PDF的新页面大小。<br><br>定义新的媒体框之后，所有裁切边距和出血边距计算都需要将新的媒体框视为插图的边缘。 |
| trimMargin=top,left,bottom,right | 在 Acrobat 的“设置页面框”选项中指定。选择“裁切框”，然后使用“页面边距控制”选项指定边距。<br><br>值表示从插图（媒体框）的原始边缘向内到上边缘、左边缘、下边缘和右边缘的距离。值(0-1000)以点为单位。<br><br>新高度=原始高度-（顶部+底部）<br><br>新宽度=原始宽度-（左侧+右侧） |
| printerMark= trim marks, bleed marks, registration marks, color bars, page information, style, line weight, layer embed | 值如下：<br><br>裁切标记= 0,1（默认值为0）<br><br>出血标记= 0,1（默认值为0）<br><br>套版色标= 0,1（默认值为0）颜色条= 0,1（默认值为0）<br><br>page information = 0,1（默认值为0）<br><br>style = Default, InDesignJ1, InDesignJ2, IllustratorillustratorJ, QuarkXPress（默认为）<br><br><br><br><br><br><br><br>line权重（默认值为Default）= 0.125-0.2，两个值（默认值为0.25）embed = 0，都包含1个包含所有打印机标记的新图层（默认值为1）QuarkXPress)。acrobat. |

请注意以下有关印刷标记的事项：

* 指定印刷标记时，通过 URL 调用指定出血边距、裁切边距和媒体边距。如果指定印刷标记而没有指定这些边距，可能会导致这些标记显示在生成的 PDF 的可见区域之外。此外，裁切标记和出血标记也会重叠。
* Specifying the same margin values for the trim margin and bleed margin results in trim marks and bleed marks overlapping when both these flags are set to 1 in `&printerMark`.
* 通过 URL 指定 fmt=swf/image 格式会导致输出中没有任何印刷标记或边距，因为此功能特定于 PDF 输出。
* Specifying `&printerMark=`through the URL results in default values being used for all parameters. Specifying `&printerMark=1` results in trim marks being set to 1 and default values for other parameters. 但是，要将第 n 个元素设置为“开”，需要通过 URL 指定所有 (n-1) 个参数。
* Specifying only one value for `&trimMargin`, `&bleedMargin`, and `&mediaMargin` results in that value being applied to all the top, bottom, left, and right margins of the original artwork.
* Specifying only the top and left values through `&trimMargin`, `&bleedMargin`, and `&mediaMargin` results in the top value being assigned to the bottom value and the left value being equal to the right.
* Not specifying the right value through `&trimMargin`, `&bleedMargin`, and `&mediaMargin` results in the left value being assigned to the right.
* 对于多页 PDF，印刷标记/边距将应用于所有页面（在 Acrobat 中，用户可以为印刷标记/边距选择页面范围）。
* 除非另有说明，已启用印刷标记/边距的 PDF 输出与 Acrobat X 完全匹配。

如果您想通过 URL 中的 &amp;joboption 修饰符创建符合 PDF/X-4 的 PDF 文件，您应当注意 PDF ISO_15930-7-2008.pdf 中指定的与印刷标记相关的限制。

* PDF 文件的每个页面对象都包括一个“媒体框”。符合 PDF/X-4 的文件中的每个页面对象应该包括一个“裁切框”或一个“作品框”，但不能同时有两个。可以通过继承方式包括“媒体框”。
* 如果存在“出血框”，则“作品框”或“裁切框”不应该超出“出血框”的边界。如果存在“裁剪框”，则“作品框”、“裁切框”或“出血框”不能超出“裁剪框”的边界。
* “作品框”、“裁切框”、“裁剪框”或“出血框”均不应超出“媒体框”的边界。
* 一些行业实践要求使用“出血框”。应该遵循相应的商业惯例。
* 与“作品框”相比，建议使用“裁切框”。
* 除陷印网和印刷标记批注以外的所有批注的 Rect 值应该完全超出“出血框”（如果没有“出血框”，则为“裁切框”或“作品框”）范围。所有印刷标记批注的 Rect 值都应该完全超出“裁切框”或“作品框”范围。符合 PDF/X-4 的阅读器可能会完全忽略除 PDF 陷印网批注之外的批注。
* 如果 Rect 的所有坐标都超出了定界框范围或在其边缘上，并且两个矩形的交集为零，则应将 Rect 视为完全超出定界框的范围。
* 如果 ViewerPreferences 词典包含 ViewArea、ViewClip、PrintArea 或 PrintClip 键，则其中每个键都应当具有“媒体框”或（如果文件的所有页面对象都有“出血框”）“出血框”值。

