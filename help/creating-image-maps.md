---
title: 创建图像映射
seo-title: 创建图像映射
description: 'null'
seo-description: 了解如何创建图像映射。
uuid: 0dcc4956-006e-4a74-9d6a-6d4bb23790ce
contentOwner: admin
content-type: 引用
products: SG_ EXPERIENCE MANAGER/Dynamic-Media-Scene-7
geptopics: SG_ SCENESELEFERENDER_ PK/categories/master_ files
discoiquuid: eddf983-38cb-4f00-b3 be3 f-85c20 bdd6 f69
translation-type: tm+mt
source-git-commit: 32f5e03766466ceaafe58780e9e80dbdd4a0c3dd

---


# 创建图像映射{#creating-image-maps}

图像映射是图像、eCatalog 页面上的区域或旋转集中的图像，显示含文本的变换面板。当用户单击图像映射时，将触发某种操作。例如，将启动网页，供用户了解产品的更多相关信息。为了使用户注意到图像映射，当用户将指针移到图像映射上时，其四周会显示轮廓。

除了在Dynamic Media经典中创建图像映射的能力外，当您在Adobe Acrobat或Adobe InDesign中设计目录时，还可以创建图像映射。

创建图像映射时，您可以执行以下任何操作：

* 输入变换文本。
* 输入用于启动网页的 JavaScript 和 URL。
* 为图像映射创建 URL 模板。
* 将图像映射复制到其他图像、eCatalog 页面或旋转集。
* 把图像映射导出到 CSV 或 XML。
* 从制表符分隔文件或 XML 文件导入图像元数据。
* 定义万维网联盟所确定的其他操作。
* 预览图像映射。

## 绘制和调整图像映射 {#drawing-and-adjusting-an-image-map}

1. 执行以下任一操作：

   * If you are working with an image in the Grid View or List View, in the Edit drop-down list click **Image Map**. Or, open it in Detail View, and then click **Image Map** above the image.
   * If you are working with a SpinSet in the Grid View or List View, click **Edit**. Or, open it in Detail View, and then click **Edit**. Select an image asset, and then click **Image Map**.
   * If you are working with an eCatalog, in the Grid View, List View, Detail View, click **Edit**. Click the **Map Pages** tab.
   ![](assets/ma_image_map.png)

1. 绘制矩形或多边形（多条边）图像映射：

   **矩形映射** 选择矩形图像映射工具并在页面上拖动以创建矩形。要向矩形映射中添加点（从而将其更改为多边形映射），请按住 Ctrl 键，接下来在所需位置放置插入工具，然后单击。

   **多边形映射** 选择多边形图像映射工具，并单击要包含的图像区域周围的点。使用多边形密度滑块改变多边形中的点密度。如果选择其他映射，将记住原始密度。如果在多边形中添加、删除或移动任何点，将丢失原始密度，同时滑块重置为其最大值。

1. 如果需要，在“图像映射”列表中为图像映射输入名称。绘制图像映射后，Dynamic Media经典将为其分配名称。

   要创建名称，Dynamic Media经典将一个序号附加到您处理的图像或电子目录页面的名称。您可以输入您选择的名称。

1. 如果希望用户在单击图像映射时打开新的网页，请在“图像映射”列表中输入 URL。

   请参见[输入 JavaScript 和 URL](creating-image-maps.md#using_a_template_to_enter_javascript_and_urls)。

1. 要在用户将指针移动到图像映射上时显示变换文本，请在“图像映射”列表中输入文本。在“图像映射”列表中，选择“显示”菜单，并选择“变换文本”。接下来输入您想要用户在屏幕上看到的文本。可以在文字处理程序中写入文本，然后将其复制到“变换文本”字段中。
1. 如果您希望在用户将鼠标移动到图像映射上时发生其他操作效果，请定义该操作。在“显示”下拉列表中，单击“其他操作”。输入操作的属性。（单击“显示”&gt;“两者全部”可为图像映射创建滚动文本和操作。）

   请参阅[定义图像映射的其他操作](creating-image-maps.md#defining_other_actions_for_image_maps)。

1. （可选）请执行下列操作之一：

   * 单击“预览”来预览图像映射。
   * 要删除图像映射或多边形顶点，请选择图像上的形状，然后单击“删除”。或者，对于 eCatalog，在“排序页面”选项卡上，单击“清除映射”从所有页面中删除图像映射。
   * 要将某个图像映射临时从图像、旋转集中的图像或 eCatalog 页面中移走而不删除，请在“图像映射”列表中取消选中相应的“开”选项。

1. 单击“保存”。

### 调整图像映射的位置、形状和大小 {#adjusting-the-position-shape-and-size-of-image-maps}

要更改图像映射的位置、形状和大小，请选择“图像映射”按钮 。然后，选择“平移”工具并按照以下说明操作：

**更改位置** 在图像映射的边框附近移动指针，但不移动。当您看见四向箭头图标时，将映射拖到新位置。

**更改大小和形状** 如何更改图像映射的形状和大小取决于您使用的是矩形还是多边形图像映射：

***提示**：您可以拖动屏幕底部的“大小”滑块来更改视图，并更好地查看图像映射。*

**矩形图像映射** 将指针移到图像映射的一侧或角上方。当您看见双向箭头图标时，开始拖动。拖动时，按住 Shift 键，以更改大小，但保持高宽比（形状）不变。

**多边形图像映射** 拖动方形选择手柄。要创建选择手柄，单击图像映射的边框，然后开始拖动。

### 处理重叠的图像映射 {#handling-overlapping-image-maps}

如果您的图像或 eCatalog 页面包括多个图像映射且映射重叠，您可以确定映射的重叠方式。为此，请更改“图像映射”列表上映射的顺序。将它们的名称拖到列表上的更高或更低位置。名称在列表中的高低位置决定其图像映射是否重叠其他图像映射。

### 导入图像映射数据 {#importing-image-map-data}

可以将图像、旋转集或 eCatalog 的数据导入到“映射摘要”屏幕中，而不必在每个页面上都输入图像映射数据。可以通过制表符分隔的文件或 XML DTD 的形式导入图像映射数据。文件中的字段必须与“映射摘要”屏幕中显示的顺序相同：“名称”、“TOC 标签”、“映射”、“URL”、“变换文本”、“其他操作”和“搜索字符串”。导入图像映射数据可以免去创建每个图像映射时在“图像映射”列表中输入数据的麻烦。

**导入图像映射数据**

1. 转到“图像映射”编辑器页（对于图像或旋转集中的图像）或 eCatalog 编辑屏幕的“映射页面”选项卡。
1. 单击“导入元数据”。
1. 在“上载元数据”对话框中，单击“图像”或“图像映射”从所需的资源属性类型中上载元数据。
1. 在“生成文件”下拉列表中，选择要创建的文件类型。
1. （可选）单击“生成”来基于要创建的文件类型预览生成的数据。单击“关闭”以返回到“上载元数据”对话框。
1. 浏览至您要上载的文件。在“文件名”文本字段中，指定所生成文件的名称。
1. （可选）在“作业名称”字段中，指定元数据上载作业的名称。
1. 单击“上载”。

### 复制图像映射 {#copying-image-maps}

您可以将图像映射从一个图像或 eCatalog 页面复制到另一个。使用“复制图像映射”能够提高创建的速度。您还可以通过复制图像映射，在共用相同布局或映射结构的图像或页面中重新创建这些图像映射。

例如，在 eCatalog 中复制图像映射是一种在相同 eCatalog 的不同外语版本之间复制所有图像映射的简便方式。为获得最佳结果，如果您在具有相同数量的页面和相同图像的不同 eCatalog 之间复制，则复制是最成功的。如果图像映射所复制到的 eCatalog 已经包含图像映射，请注意复制时将删除原有的图像映射。

**复制图像映射**

1. 转到“图像映射”编辑器页（对于图像或旋转集中的图像）或 eCatalog 编辑屏幕的“映射页面”选项卡。
1. 单击“将映射复制到”。
1. 根据您是从图像复制图像映射还是从 eCatalog 复制图像映射，执行下列操作之一：

   * （图像）在“选择图像”屏幕中，选择您要将图像映射复制到的图像。
   * (eCatalog) 在“选择资源”屏幕中，选择您要将图像映射复制到的图像或 eCatalog 页面。

1. 单击“选择”。

## 使用模板输入 JavaScript 和 URL {#using-a-template-to-enter-javascript-and-urls}

您可以定义 URL 模板（也称为 Href 模板），以便在输入图像映射 URL 时更轻松更有效。如果您的大部分图像映射 URL 都共享通用的固定格式，请定义 URL 模板。在输入固定 URL 部分以作为 URL 模板后，每次创建图像映射时，无需输入该部分 URL。您的 URL 模板也可以包含 JavaScript 命令、路径名和参数。By default, the URL template contains a proprietary Dynamic Media Classic JavaScript handler called `loadProduct` that opens the image in a new window.

>[!NOTE]
>
>请注意，在图像映射的 HREF 属性中添加 Javascript 代码时，将在客户端计算机上运行该代码。因此，请确保 Javascript 代码是安全的。

### 关于 URL 模板 {#about-url-templates}

URL 模板的工作方式是，在模板中使用两个美元符号 ('$$') 代替“图像映射”列表中 URL 列的内容：

```as3
Javascript:loadProduct(‘$$’);void(0);
```

请将在图像映射之间不会发生变化的所有值放在 URL 模板中。仅仅将那些会在 URL 列中发生变化的值添加到“图像映射”列表中。例如：

* URL模板：j `avascript:loadProduct(‘https://www.examplesitehere.com/$$’);void(0);`
* URL值： `product.htm`
* 生成的实际URL： `javascript:loadProduct(‘https://www.examplesitehere.com/product.html);void(0);`

By default, the URL template includes a proprietary Dynamic Media Classic JavaScript handler called `loadProduct` that opens a new window with the URL destination. 但是，您可以使用任何JavaScript代码替换此JavaScript处理程序或使用下列Dynamic Media经典句柄之一：

* `loadProductCW`

   在当前窗口中显示在 URL 列中指定的 URL 目标。该处理函数主要用于集成到网站中的页面的 eCatalog。

* `loadProductPW`

   在父窗口（打开当前窗口的页面）中显示在 URL 列中指定的 URL 目标。当前窗口仍处于打开状态，但父窗口切换为显示 URL 目标。

   ***注意**：处理程序`loadProductPW`不支持DHTML和HTML查看器。*

### 创建 URL 模板 {#creating-a-url-template}

要创建 URL 模板，请执行以下操作：

1. 在“映射编辑器”屏幕（图像或旋转集）或 eCatalog 屏幕 (eCatalog) 的“映射页面”选项卡上，选择“URL 模板”选项旁边的“编辑”。将打开“编辑映射模板”对话框。
1. Enter the JavaScript code and the complete URL (with the variable portion replaced by dollar signs [$$]). 您可以通过右键单击并选择“粘贴”来粘贴代码。
1. 选择“保存”按钮。

### 处理 URL 模板 {#handling-url-templates}

“映射编辑器”页面（图像和旋转集）和 eCatalog 屏幕 (eCatalog) 的“映射页面”选项卡提供以下用于处理 URL 模板的命令：

**URL模板选项** 选择URL模板选项可将您的URL模板应用于图像或电子目录页面上的所有图像映射。

**如果不希望单个图像映射使用URL模板，则在URL图像映射列表中** 取消选择“模板”选项。

## 定义图像映射的其他操作 {#defining-other-actions-for-image-maps}

您可以选择“显示”菜单，然后选择“其他操作”以触发除变换文本和网页启动之外的操作。当用户将指针移动到图像映射上时，您可以启动一个操作。这些操作是万维网联盟 HTML 规范为客户端图像映射定义的属性。它们是：

**辅助键** 在用户按下键盘上的指定键时触发操作。

**焦点** 在图像映射接收焦点(由光标、按下Tab键或按下访问键)时触发事件。例如，当图像映射被激活时，您可以启动网页，当图像映射被取消激活时，您可以将其关闭。

**当图像映射失去焦点或按下Tab键时，模糊将** 触发事件。

**定义图像映射的其他操作**

1. 在“映射编辑器”屏幕（图像和旋转集）或 eCatalog 屏幕 (eCatalog) 的“映射页面”选项卡上，选择“显示”菜单，然后选择“其他操作”。
1. 使用由万维网联盟 HTML 规范指定的语法，在“图像映射”列表的“其他操作”列中添加支持的属性。
1. 单击“**保存**”。

选择“显示”菜单，然后选择“两者全部”（如果您希望图像映射同时具有变换文本和操作）。

## 在 Adobe Acrobat 或 Adobe InDesign 中创建图像映射 {#creating-image-maps-in-adobe-acrobat-or-adobe-indesign}

在 Adobe Acrobat 或 Adobe InDesign 中设计 eCatalog 时，您可以创建图像映射。

在 Acrobat 或 InDesign 中，创建您希望在其中出现图像映射的超链接引用，然后为图像映射指定 URL 位置。在将PDF文件上传到Dynamic Media经典时选择“提取链接”选项会自动转换到图像映射的链接。

有关更多信息，请参阅 InDesign 帮助或 Acrobat 帮助。

### 在 Adobe InDesign 中创建图像映射 {#to-create-image-maps-in-adobe-indesign}

1. 在 InDesign 中，单击“窗口”&gt;“交互”&gt;“超链接”，打开“超链接”面板。
1. 选择要创建图像映射的文本、帧或图形。
1. 在“超链接”面板中，单击面板菜单中的“新建超链接”。
1. 在“新建超链接”对话框中，从“链接到”菜单中选择 URL。
1. 在 URL 框中键入或粘贴产品 ID，然后单击“确定”。(动态媒体经典使用图像映射URL模板完成URL。)

   >[!NOTE]
   >
   >您不需要在 InDesign 中设置外观选项。您可以在Dynamic Media经典中指定外观。

1. 对于您想要创建的所有图像映射，重复步骤 2 到 5。
1. 将文件导出为 PDF。
1. 将PDF上传到Dynamic Media经典，然后从“PDF选项”中选择“提取链接”。

### 在 Adobe Acrobat 中创建图像映射 {#to-create-image-maps-in-adobe-acrobat}

1. 在 Acrobat 中，选择“工具”&gt;“高级编辑”&gt;“链接工具”。
1. 拖动以创建图像映射。将打开“创建链接”框。
1. 选择“自定义链接”，然后单击“下一步”。

   ***注意**：您无需在Acrobat中设置外观选项。您可以在Dynamic Media经典中指定外观。*

1. 在“链接属性”框中，单击“动作”。
1. 从“选择动作”菜单中选择“打开网络链接”，然后单击“添加”。
1. 在“编辑 URL”框中键入图像映射的产品 ID，然后单击“确定”。(动态媒体经典使用图像映射URL模板完成URL。)
1. 对于您想要创建的所有图像映射，重复步骤 1 到 7。
1. 保存文件。
1. 将PDF上传到Dynamic Media经典，然后从“PDF选项”中选择“提取链接”。

