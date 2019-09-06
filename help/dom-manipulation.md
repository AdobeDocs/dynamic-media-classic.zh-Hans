---
title: DOM 处理
seo-title: DOM 处理
description: 'null'
seo-description: 了解DOM操作。
uuid: 275cd49d-2a55-41f9-80b0-e147 d0 cd2907
contentOwner: admin
content-type: 引用
products: SG_ EXPERIENCE MANAGER/Dynamic-Media-Scene-7
geptopics: SG_ SCENESELEFERENDER_ PK/类别/模板发布
discoiquuid: 890ca93e-3146-4347-864b-bd5 e94037038
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# DOM 处理{#dom-manipulation}

DOM（文档对象模型）处理是一种通过直接控制设计文件的 XML 代码来编辑设计文件的方法。DOM 处理可使您更好地控制变量设计元素（包括更改其内容和外观）；您甚至可以根据需要创建新元素。

动态媒体经典允许您在模板发布后通过URL命令操作Dynamic Media经典FXG模板的DOM。FXG 模板中的设计元素是通过 URL 传递命令来进行处理的。这样，您可以动态地处理属性以及向图形中添加属性。

要使用DOM操作，您创建s7：在Illustrator文件中将Elements转换为Dynamic Media经典FXG文件并将其上传到SPS。

>[!NOTE]
>
>在使用 DOM 处理命令时，所有传入的值必须进行 URL 编码。

>[!NOTE]
>
>Illustrator Plug-in for Web-to-Print (for converting Illustrator files) converts to FXG 2.0. For information about this specification, see [www.adobe.com/go/learn_s7_fxg2_en](https://www.adobe.com/go/learn_s7_fxg2_en).

## 在 Illustrator 文件中创建 s7:elementID {#creating-s-elementids-in-illustrator-files}

要在 Illustrator 中创建的设计中使用 DOM 处理，请在您的 Illustrator 设计中创建 s7:elementID。创建 s7:elementID 可以在模板发布之后使用 URL 命令来修改设计元素。

### 为文本 DOM 处理创建 s7:elementID {#creating-s-elementids-for-dom-manipulation-of-text}

要为文本对象的 DOM 处理创建一个 s7:elementID，请在 Illustrator 中打开“图层”面板。然后，在包含变量文本的文本图层上，使用 s7:elementID 命名该图层。To do so, enter the letters `id` (for identification), a colon ( `:`), and a name. 以下是 s7:elementID 文本图层名称的示例：

`id:BirthdayBoyName`

`id:DateofBirth`

`id:EnterFirstNameHer`

### 为对象 DOM 处理创建 s7:elementID {#creating-s-elementids-for-dom-manipulation-of-objects}

如果您希望最终用户能够更改对象的属性，请为对象创建 s7:elementID。对象可以构成整个文本框架、图形和图像。彩色背景是对象元素 ID 的一个示例。当季节改变时，最终用户可以变换海报的背景颜色，使海报顺应季节。

在 Illustrator 中为某个对象创建 s7:element ID 之前，请先为该对象创建一个单独的图层。

在 Illustrator 中按照以下步骤为对象创建 s7:elementID：

1. 选择该对象。
1. 单击 **“窗口** ”&gt; **“图层**”。
1. 在“图层”面板中，将对象图层命名为s7：ElementID。To do so, enter the letters `id` (for identification), a colon ( `:`), and description to identify the element. 以下是 s7:elementID 对象图层名称的示例：

   `id:BackgroundColor`

   `id:RotationPercentage`

   `id:JacketJPG`

## 发布 FXG 模板 {#publish-fxg-templates}

发布FXG模板可将其放置在Dynamic Media经典服务器上，在该服务器上可访问网站和应用程序。在发布过程期间，Scene7 Publishing System 会激活您的网站或应用程序所需的 URL。

>[!NOTE]
>
>要使用 FXG 模板，请发布其所含的所有内容，包括字体和图像。如果未包括所有必需的文件，则在发布时会出现错误消息。

### 将 FXG 模板标记为发布 {#mark-fxg-templates-for-publish}

必须将模板及其所有支持文件标记为发布，以便将其放置在Dynamic Media图像服务器上。

1. 在浏览面板中，选择 FXG 模板以及使用的所有图形、图像和字体。
1. 单击 **“标记为发布**”。

### 发布 FXG 模板 {#publish-your-fxg-template}

1. 在全局导航栏上，单击“**发布**”。
1. 选择“时间”选项，并可选择输入发布作业的名称。
1. Click **Start Publish**.

### 文本溢出指示符显示 {#text-overflow-indicator-display}

当文本超出在文本框架内为其分配的空间（或者，如果是串接文本，则为在最后一个文本框架中分配的空间）时，会显示&#x200B;*文本溢出指示符*。该指示符是一个内含加号的红色方框。SPS 上的文本溢出指示符始终处于启用状态。

文本溢出指示符通过 `markOverflowingTextFrame` 修饰符进行控制。如下所示使用该修饰符：

| 修饰符/值 | 说明 |
|--- |--- |
| markOverflowingTextFrame=0,1 | 值为 1 时表示显示文本流指示符。默认值为 0。（虽然默认值为 0，但是 SPS 中的文本溢出指示符始终处于启用状态。）请注意 markOverflowingTextFrame 修饰符区分大小写。 |

>[!MORELIKETHIS]
>
>* [定义可变性：参数化与 DOM 处理](defining-variability-parameterization-versus-dom.md#defining_variability_parameterization_versus_dom_manipulation)
>* [Publishing](publishing-files.md#publishing_files)

