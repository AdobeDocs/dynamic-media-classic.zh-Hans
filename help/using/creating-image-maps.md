---
title: 创建图像映射
description: 了解如何在Adobe Dynamic Media Classic中创建图像映射。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: deafbd03-06bc-4d7e-87a1-5620ebcac426
topic: Content Management
level: Intermediate
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '2444'
ht-degree: 31%

---

# 创建图像映射 {#creating-image-maps}

图像映射是图像、eCatalog页面或SpinSet中用于显示包含文本的变换面板的图像上的区域。 当用户选择图像映射时，将触发某种操作。 例如，启动Web页，以便用户了解有关产品的更多信息。 当用户将鼠标指针移到“图像映射”上时，其周围会显示一个轮廓。

除了在Adobe Dynamic Media Classic中创建图像映射的功能外，在Adobe Acrobat或Adobe InDesign中设计目录时也可以创建图像映射。

在创建图像映射时，可以执行以下任一操作：

* 输入变换文本。
* 输入用于启动网页的JavaScript和URL。
* 为图像映射创建 URL 模板。
* 将图像映射复制到其他图像、eCatalog 页面或旋转集。
* 把图像映射导出到 CSV 或 XML。
* 从制表符分隔文件或XML文件导入图像元数据。
* 定义万维网联盟确定的其他操作。
* 预览图像映射。

## 绘制和调整图像映射 {#drawing-and-adjusting-an-image-map}

1. 执行以下任一操作：

   * 如果您正在网格视图或列表视图中使用图像，请在“编辑”下拉列表中选择&#x200B;**[!UICONTROL 图像映射]**。 或者，在“详细信息视图”中打开它，然后选择图像上方的&#x200B;**[!UICONTROL 图像映射]**。
   * 如果正在网格视图或列表视图中使用旋转集，请选择&#x200B;**[!UICONTROL 编辑]**。 或者，在“详细信息视图”中打开它，然后选择&#x200B;**[!UICONTROL 编辑]**。 选择一个图像资源，然后选择&#x200B;**[!UICONTROL 图像映射]**。
   * 如果您正在使用eCatalog，请在“网格视图”、“列表视图”、“详细信息视图”中，选择&#x200B;**[!UICONTROL 编辑]**。 选择&#x200B;**[!UICONTROL 映射页面]**&#x200B;选项卡。

   ![图像映射插图](assets/ma_image_map.png)

1. 绘制矩形或多边形（多条边）图像映射：

   * **矩形映射**：选择“矩形图像映射”工具并在页面上拖动以创建矩形。 若要向矩形地图添加点（从而将其更改为多边形地图），请按Ctrl，然后将插入工具放置在所需位置并选择。

   * **多边形映射**：选择“多边形图像映射”工具，并在要包围的图像区域的周边上选择点。 使用多边形密度滑块改变多边形中的点密度。如果选择其他映射，将记住原始密度。如果在多边形中添加、删除或移动了任何点，则原始密度将丢失。 滑块将重置为其最大值。

1. 如果需要，在“图像映射”列表中为图像映射输入名称。绘制图像映射后，Adobe Dynamic Media Classic会为其指定一个名称。

   要创建名称，Adobe Dynamic Media Classic会在您使用的图像或eCatalog页面的名称后附加一个序列号。 您可以输入您选择的名称。

1. 如果希望用户在选择图像映射时打开一个新网页，请在“图像映射”列表中输入URL。

   请参阅[以输入JavaScript和URL](creating-image-maps.md#using_a_template_to_enter_javascript_and_urls)。

1. 要在用户将指针移动到图像映射上时显示变换文本，请在“图像映射”列表中输入文本。在“图像映射”列表中，选择&#x200B;**[!UICONTROL 显示]**&#x200B;菜单，然后选择&#x200B;**[!UICONTROL 变换文本]**。 然后输入您希望用户在屏幕上看到的文本。 可以在文字处理程序中写入文本，然后将其复制到“变换文本”字段中。

1. 如果您希望在用户将鼠标移动到图像映射上时发生其他操作效果，请定义该操作。在&#x200B;**[!UICONTROL 显示]**&#x200B;下拉列表中，选择&#x200B;**[!UICONTROL 其他操作]**。 输入操作的属性。（转到&#x200B;**[!UICONTROL 显示]** > **[!UICONTROL 两者]**&#x200B;以创建图像映射的变换文本和操作。）

   请参阅[定义图像映射的其他操作](creating-image-maps.md#defining_other_actions_for_image_maps)。

1. （可选）请执行下列操作之一：

   * 要预览图像映射，请选择&#x200B;**[!UICONTROL 预览]**。
   * 要删除图像映射或多边形顶点，请选择图像上的形状，然后选择&#x200B;**[!UICONTROL 删除]**。 或者，对于eCatalog，在顺序页选项卡上，选择&#x200B;**[!UICONTROL 清除映射]**&#x200B;以从所有页面中删除图像映射。
   * 要删除：
      * 来自图像的图像映射
      * 旋转集中的图像
      * 或者，eCatalog页面

     暂时取消选择“图像映射”列表中的相应“开启”选项，而不删除它。

1. 选择&#x200B;**[!UICONTROL 保存]**。

### 调整图像映射的位置、形状和大小 {#adjusting-the-position-shape-and-size-of-image-maps}

要更改图像映射的位置、形状和大小，请选择图像映射按钮。 然后，选择&#x200B;**[!UICONTROL 平移]**&#x200B;工具并按照以下说明操作：

* **更改位置**：将指针移近图像映射的边框，但移近图像映射的边框。 当您看见四向箭头图标时，将映射拖到新位置。

* **更改大小和形状**：更改图像映射形状和大小的方式取决于您使用的是矩形还是多边形图像映射：

>[!TIP]
>
>您可以拖动屏幕底部的“大小”滑块以更改视图，使您更轻松地查看图像映射。

* **矩形图像映射**：将指针移动到图像映射的边或角上。 当您看见双向箭头图标时，开始拖动。拖动时按住Shift键可更改大小，但保持宽高比（形状）。

* **多边形图像映射**：拖动正方形选区手柄。 要创建选区手柄，请选择图像映射的边框并开始拖动。

### 处理重叠的图像映射 {#handling-overlapping-image-maps}

如果您的图像或eCatalog页面包含多个图像映射，并且映射重叠，则可以确定映射重叠的方式。 为此，请更改“图像映射”列表上映射的顺序。将它们的名称拖到列表上的更高或更低位置。名称在列表中的高低位置决定其图像映射是否重叠其他图像映射。

### 导入图像映射数据 {#importing-image-map-data}

可以将图像、旋转集或 eCatalog 的数据导入到“映射摘要”屏幕中，而不必在每个页面上都输入图像映射数据。可以通过制表符分隔的文件或 XML DTD 的形式导入图像映射数据。文件中的字段必须与“映射摘要”屏幕中显示的顺序相同：“名称”、“TOC 标签”、“映射”、“URL”、“变换文本”、“其他操作”和“搜索字符串”。导入图像映射数据可省去在创建每个图像映射时在“图像映射”列表中输入数据的麻烦。

**要导入图像映射数据：**

1. 转到“图像映射”编辑器页（对于图像或旋转集中的图像）或 eCatalog 编辑屏幕的“映射页面”选项卡。
1. 选择&#x200B;**[!UICONTROL 导入元数据]**。
1. 在上载元数据对话框中，选择图像或图像映射，以从所需的资源属性类型上传元数据。
1. 在`Generate File`下拉列表中，选择要创建的文件类型。
1. （可选）选择&#x200B;**[!UICONTROL 生成]**&#x200B;以根据要创建的文件类型预览结果数据。 选择&#x200B;**[!UICONTROL 关闭]**&#x200B;以返回到“上载元数据”对话框。
1. 浏览至您要上载的文件。在“文件名”文本字段中，指定所生成文件的名称。
1. （可选）在“作业名称”字段中，指定元数据上载作业的名称。
1. 选择&#x200B;**[!UICONTROL 上传]**。

### 复制图像映射 {#copying-image-maps}

您可以将图像映射从一个图像或 eCatalog 页面复制到另一个。使用&#x200B;**[!UICONTROL 复制图像映射]**&#x200B;开始创建它们。 您还可以复制图像映射，以在共享布局或映射结构的图像或页面中重新创建图像映射。

例如，在eCatalog中复制图像映射是一种在同一eCatalog的外语版本之间复制所有图像映射的便捷方法。 为获得最佳结果，如果在具有相同页数和相同图像的eCatalog之间复制，则复制最为成功。 如果您复制的eCatalog中已经包含图像映射，则在复制时会删除这些图像映射。

**要复制图像映射：**

1. 转到“图像映射”编辑器页（对于图像或旋转集中的图像）或 eCatalog 编辑屏幕的“映射页面”选项卡。
1. 选择&#x200B;**[!UICONTROL 将映射复制到]**。
1. 根据您是从图像复制图像映射还是从 eCatalog 复制图像映射，执行下列操作之一：

   * （图像）在“选择图像”屏幕中，选择您要将图像映射复制到的图像。
   * (eCatalog) 在“选择资源”屏幕中，选择您要将图像映射复制到的图像或 eCatalog 页面。

1. 选择&#x200B;**[!UICONTROL 选择]**。

## 使用模板输入JavaScript和URL {#using-a-template-to-enter-javascript-and-urls}

您可以定义 URL 模板（也称为 Href 模板），以便在输入图像映射 URL 时更轻松更有效。如果您的大部分图像映射 URL 都共享通用的固定格式，请定义 URL 模板。在输入固定 URL 部分以作为 URL 模板后，每次创建图像映射时，无需输入该部分 URL。URL模板还可以包含JavaScript命令、路径名和参数。 默认情况下，URL模板包含名为`loadProduct`的专有Adobe Dynamic Media Classic JavaScript处理程序，该处理程序会在新窗口中打开图像。

>[!NOTE]
>
>将JavaScript代码添加到图像映射的HREF属性中时，该代码会在客户端计算机上运行。 因此，请确保JavaScript代码是安全的。

### 关于 URL 模板 {#about-url-templates}

URL模板可通过替换“图像映射”列表中URL列的内容来工作。 在模板中用双美元符号(“$$”)替换它：

```as3
Javascript:loadProduct('$$');void(0);
```

您可以在URL模板中的图像映射之间放置所有未更改的值。 仅仅将那些会在 URL 列中发生变化的值添加到“图像映射”列表中。例如：

* URL模板： `javascript:loadProduct('https://www.examplesitehere.com/$$');void(0);`
* URL值： `product.htm`
* 实际生成的URL： `javascript:loadProduct('https://www.examplesitehere.com/product.html);void(0);`

默认情况下，URL模板包含名为`loadProduct`的专有Adobe Dynamic Media Classic JavaScript处理程序，该处理程序将打开一个包含URL目标的新窗口。 但是，您可以使用任何JavaScript代码来替换此JavaScript处理程序，或者使用以下Adobe Dynamic Media Classic处理程序之一：

* `loadProductCW`：在当前窗口中显示URL列中指定的URL目标。 该处理函数主要用于集成到网站中的页面的 eCatalog。

* `loadProductPW`：在父窗口（打开当前窗口的页面）的URL列中显示指定的URL目标。 当前窗口仍处于打开状态，但父窗口切换为显示 URL 目标。

  >[!NOTE]
  >
  >处理程序`loadProductPW`不支持DHTML和HTML5查看器。

### 创建URL模板 {#creating-a-url-template}

1. 在“映射编辑器”屏幕（图像或旋转集）或eCatalog屏幕的“映射页面”选项卡(eCatalogs)上，选择“URL模板”选项旁边的“编辑”。 将打开“编辑映射模板”对话框。
1. 输入JavaScript代码和完整URL（变量部分替换为美元符号[$$]）。 您可以通过右键单击并选择&#x200B;**[!UICONTROL 粘贴]**&#x200B;来粘贴代码。
1. 选择&#x200B;**[!UICONTROL 保存]**。

### 处理URL模板 {#handling-url-templates}

“映射编辑器”页面（图像和旋转集）和 eCatalog 屏幕 (eCatalog) 的“映射页面”选项卡提供以下用于处理 URL 模板的命令：

* **URL模板选项**：选择URL模板选项可将URL模板应用于图像或eCatalog页面上的所有图像映射。

* **模板选项**：如果不希望单个图像映射使用URL模板，请取消选择“URL图像映射”列表中的模板选项。

## 定义图像映射的其他操作 {#defining-other-actions-for-image-maps}

您可以选择&#x200B;**[!UICONTROL 显示]**&#x200B;菜单并选择&#x200B;**[!UICONTROL 其他操作]**&#x200B;以触发除变换文本和网页启动项之外的操作。 当用户将指针移动到图像映射上时，您可以启动一个操作。这些操作是万维网联盟 HTML 规范为客户端图像映射定义的属性。它们是：

* **`accesskey`**：用户按下键盘上的指定键时会触发操作。

* **`onfocus`**：当图像映射收到焦点时，通过光标、Tab键或按访问键触发事件。 例如，您可以在图像映射收到焦点时启动网页，并在图像映射失去焦点时关闭网页。

* **`onblur`**：在图像映射失去焦点时触发一个事件，该事件通过光标或Tab键设置。

**要定义图像映射的其他操作：**

1. 在“映射编辑器”屏幕（图像和旋转集）或eCatalog屏幕(eCatalogs)的“映射页面”选项卡上，选择&#x200B;**[!UICONTROL 显示]**&#x200B;菜单，然后选择&#x200B;**[!UICONTROL 其他操作]**。
1. 使用由万维网联盟 HTML 规范指定的语法，在“图像映射”列表的“其他操作”列中添加支持的属性。
1. 选择&#x200B;**[!UICONTROL 保存]**。

如果希望图像映射具有变换文本和操作，请选择&#x200B;**[!UICONTROL 显示]**&#x200B;菜单并选择&#x200B;**[!UICONTROL 两者]**。

## 在Adobe Acrobat或Adobe InDesign中创建图像映射 {#creating-image-maps-in-adobe-acrobat-or-adobe-indesign}

在 Adobe Acrobat 或 Adobe InDesign 中设计 eCatalog 时，您可以创建图像映射。

在Adobe Acrobat或Adobe InDesign中，创建要在其中显示图像映射的超链接引用，并指定图像映射的URL位置。 在上传PDF文件到Adobe Dynamic Media Classic时，选择提取链接选项会自动将链接转换为图像映射。

有关更多信息，请参阅Adobe InDesign帮助或Adobe Acrobat帮助。

### 在 Adobe InDesign 中创建图像映射 {#to-create-image-maps-in-adobe-indesign}

1. 在Adobe InDesign中，转到&#x200B;**[!UICONTROL Windows®]** > **[!UICONTROL 交互式]** > **[!UICONTROL 超链接]**。
1. 在“超链接”面板中，选择要生成图像映射的文本、框架或图形。
1. 从面板菜单中选择&#x200B;**[!UICONTROL 新建超链接]**。
1. 在“新建超链接”对话框中，从&#x200B;**[!UICONTROL 链接到]**&#x200B;菜单中，选择&#x200B;**[!UICONTROL URL]**。
1. 在URL框中键入或粘贴产品ID。
1. 选择&#x200B;**[!UICONTROL 确定]**。 (Adobe Dynamic Media Classic使用图像映射URL模板来完成URL。)

   >[!NOTE]
   >
   >您无需在Adobe InDesign中设置外观选项。 您可以在Adobe Dynamic Media Classic中指定外观。

1. 对于您想要创建的所有图像映射，重复步骤 2 到 6。
1. 将文件导出为 PDF。
1. 将PDF上传到Adobe Dynamic Media Classic。
1. 在&#x200B;**[!UICONTROL PDF选项]**&#x200B;中，选择&#x200B;**[!UICONTROL 提取链接]**。

### 在 Adobe Acrobat 中创建图像映射 {#to-create-image-maps-in-adobe-acrobat}

1. 在Adobe Acrobat中，转到&#x200B;**[!UICONTROL 工具]** > **[!UICONTROL 高级编辑]** > **[!UICONTROL 链接工具]**。
1. 拖动以创建图像映射。
1. 在“创建链接”框中，选择&#x200B;**[!UICONTROL 自定义链接]**，然后选择&#x200B;**[!UICONTROL 下一步]**。

>[!NOTE]
>
>您无需在Adobe Acrobat中设置外观选项。 您可以在Adobe Dynamic Media Classic中指定外观。

1. 在“链接属性”框中，选择&#x200B;**[!UICONTROL 操作]**。
1. 从“选择操作”菜单中选择&#x200B;**[!UICONTROL 打开Web链接]**，然后选择&#x200B;**[!UICONTROL 添加]**。
1. 在“编辑URL”框中键入图像映射的产品ID，然后选择&#x200B;**[!UICONTROL 确定]**。 (Adobe Dynamic Media Classic使用图像映射URL模板来完成URL。)
1. 对于您想要创建的所有图像映射，重复步骤 1 到 7。
1. 保存文件。
1. 将PDF上传到Adobe Dynamic Media Classic并从PDF选项中选择提取链接。
