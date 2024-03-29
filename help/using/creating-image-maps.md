---
title: 创建图像映射
description: 了解如何在Adobe Dynamic Media Classic中创建图像映射。
uuid: 0dcc4956-006e-4a74-9d6a-6d4bb23790ce
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 4eddf983-38cb-4f00-b3be-85c20bdd6f69
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: deafbd03-06bc-4d7e-87a1-5620ebcac426
topic: Content Management
level: Intermediate
source-git-commit: d82f816553f807b514f4690827dab672a6baf690
workflow-type: tm+mt
source-wordcount: '2430'
ht-degree: 46%

---

# 创建图像映射 {#creating-image-maps}

图像映射是图像、eCatalog 页面上的区域或旋转集中的图像，显示含文本的变换面板。当用户选择图像映射时，将触发某种操作。 例如，将启动网页，供用户了解产品的更多相关信息。当用户将指针移到“图像映射”上时，其周围会显示一个轮廓。

除了在Adobe Dynamic Media Classic中创建图像映射的功能外，在Adobe Acrobat或Adobe InDesign中设计目录时，您还可以创建图像映射。

在创建图像映射时，可以执行以下任一操作：

* 输入变换文本。
* 输入用于启动网页的 JavaScript 和 URL。
* 为图像映射创建 URL 模板。
* 将图像映射复制到其他图像、eCatalog 页面或旋转集。
* 把图像映射导出到 CSV 或 XML。
* 从制表符分隔文件或XML文件导入图像元数据。
* 定义万维网联盟所确定的其他操作。
* 预览图像映射。

## 绘制和调整图像映射 {#drawing-and-adjusting-an-image-map}

1. 执行以下任一操作：

   * 如果正在网格视图或列表视图中使用图像，请在编辑下拉列表中选择 **[!UICONTROL 图像映射]**. 或者，在“详细信息视图”中打开它，然后选择 **[!UICONTROL 图像映射]** 在图像上方。
   * 如果正在网格视图或列表视图中使用旋转集，请选择 **[!UICONTROL 编辑]**. 或者，在“详细信息视图”中打开它，然后选择 **[!UICONTROL 编辑]**. 选择一个图像资源，然后选择 **[!UICONTROL 图像映射]**.
   * 如果使用eCatalog，请在“网格视图”、“列表视图”、“详细信息视图”中选择 **[!UICONTROL 编辑]**. 选择 **[!UICONTROL 映射页面]** 选项卡。

   ![图像映射图像](assets/ma_image_map.png)

1. 绘制矩形或多边形（多条边）图像映射：

   * **矩形地图**  — 选择“矩形图像映射”工具并在页面上拖动以创建矩形。 若要向矩形地图添加点（从而将其更改为多边形地图），请按Ctrl，然后将插入工具放置在所需位置并选择。

   * **多边形地图**  — 选择“多边形图像映射”工具，并在要包围的图像区域的周边上选择点。 使用多边形密度滑块改变多边形中的点密度。如果选择其他映射，将记住原始密度。如果在多边形中添加、删除或移动任何点，将丢失原始密度，同时滑块重置为其最大值。

1. 如果需要，在“图像映射”列表中为图像映射输入名称。绘制图像映射后，Adobe Dynamic Media Classic会为其指定一个名称。

   要创建名称，Adobe Dynamic Media Classic会在您使用的图像或eCatalog页面的名称后附加一个序列号。 您可以输入您选择的名称。

1. 如果您希望用户在选择“图像映射”时打开一个新网页，请在“图像映射”列表中输入URL。

   请参见[输入 JavaScript 和 URL](creating-image-maps.md#using_a_template_to_enter_javascript_and_urls)。

1. 要在用户将指针移动到图像映射上时显示变换文本，请在“图像映射”列表中输入文本。在“图像映射”列表中，选择 **[!UICONTROL 显示]** 菜单并选择 **[!UICONTROL 变换文本]**. 然后输入您希望用户在屏幕上看到的文本。 可以在文字处理程序中写入文本，然后将其复制到“变换文本”字段中。

1. 如果您希望在用户将鼠标移动到图像映射上时发生其他操作效果，请定义该操作。在 **[!UICONTROL 显示]** 下拉列表，选择 **[!UICONTROL 其他操作]**. 输入操作的属性。(转到 **[!UICONTROL 显示]** > **[!UICONTROL 两者]** 用于为“图像映射”创建变换文本和操作。)

   参见 [定义图像映射的其他操作](creating-image-maps.md#defining_other_actions_for_image_maps).

1. （可选）请执行下列操作之一：

   * 要预览图像映射，请选择 **[!UICONTROL 预览]**.
   * 要删除图像映射或多边形顶点，请在图像上选择一个形状，然后选择 **[!UICONTROL 删除]**. 或者，对于eCatalog，在订单页选项卡上，选择 **[!UICONTROL 清除映射]** 以从所有页面中删除图像映射。
   * 要将某个图像映射临时从图像、旋转集中的图像或 eCatalog 页面中移走而不删除，请在“图像映射”列表中取消选中相应的“开”选项。

1. 选择 **[!UICONTROL 保存]**.

### 调整图像映射的位置、形状和大小 {#adjusting-the-position-shape-and-size-of-image-maps}

要更改图像映射的位置、形状和大小，请选择“图像映射”按钮 。然后，选择 **[!UICONTROL 平移]** 工具并按照以下说明操作：

* **更改位置**  — 将指针移到“图像映射”边框附近，但不移到“图像映射”边框上方。 当您看见四向箭头图标时，将映射拖到新位置。

* **更改大小和形状**  — 如何更改图像映射的形状和大小取决于您使用的是矩形还是多边形图像映射：

>[!TIP]
>
>您可以拖动屏幕底部的“大小”滑块以更改视图，使您更轻松地查看图像映射。

* **矩形图像映射**  — 将指针移到“图像映射”的边或角上。 当您看见双向箭头图标时，开始拖动。拖动时，按住 Shift 键，以更改大小，但保持高宽比（形状）不变。

* **多边形图像映射**  — 拖动方形选择手柄。 要创建选区手柄，请选择“图像映射”的边框并开始拖动。

### 处理重叠的图像映射 {#handling-overlapping-image-maps}

如果您的图像或 eCatalog 页面包括多个图像映射且映射重叠，您可以确定映射的重叠方式。为此，请更改“图像映射”列表上映射的顺序。将它们的名称拖到列表上的更高或更低位置。名称在列表中的高低位置决定其图像映射是否重叠其他图像映射。

### 导入图像映射数据 {#importing-image-map-data}

可以将图像、旋转集或 eCatalog 的数据导入到“映射摘要”屏幕中，而不必在每个页面上都输入图像映射数据。可以通过制表符分隔的文件或 XML DTD 的形式导入图像映射数据。文件中的字段必须与“映射摘要”屏幕中显示的顺序相同：“名称”、“TOC 标签”、“映射”、“URL”、“变换文本”、“其他操作”和“搜索字符串”。导入图像映射数据可以免去创建每个图像映射时在“图像映射”列表中输入数据的麻烦。

**导入图像映射数据:**

1. 转到“图像映射”编辑器页（对于图像或旋转集中的图像）或 eCatalog 编辑屏幕的“映射页面”选项卡。
1. 选择 **[!UICONTROL 导入元数据]**.
1. 在上载元数据对话框中，选择图像或图像映射，以从所需的资源属性类型上载元数据。
1. 在“生成文件”下拉列表中，选择要创建的文件类型。
1. （可选）选择 **[!UICONTROL 生成]** 以根据要创建的文件类型预览结果数据。 选择 **[!UICONTROL 关闭]** 以返回上载元数据对话框。
1. 浏览至您要上载的文件。在“文件名”文本字段中，指定所生成文件的名称。
1. （可选）在“作业名称”字段中，指定元数据上载作业的名称。
1. 选择 **[!UICONTROL 上传]**.

### 复制图像映射 {#copying-image-maps}

您可以将图像映射从一个图像或 eCatalog 页面复制到另一个。使用 **[!UICONTROL 复制图像映射]** 开始创造它们。 您还可以复制图像映射，以在共享布局或映射结构的图像或页面中重新创建图像映射。

例如，在 eCatalog 中复制图像映射是一种在相同 eCatalog 的不同外语版本之间复制所有图像映射的简便方式。为获得最佳结果，如果您在具有相同数量的页面和相同图像的不同 eCatalog 之间复制，则复制是最成功的。如果您复制的eCatalog中已经包含图像映射，则在复制时将删除这些图像映射。

**复制图像映射:**

1. 转到“图像映射”编辑器页（对于图像或旋转集中的图像）或 eCatalog 编辑屏幕的“映射页面”选项卡。
1. 选择 **[!UICONTROL 将映射复制到]**.
1. 根据您是从图像复制图像映射还是从 eCatalog 复制图像映射，执行下列操作之一：

   * （图像）在“选择图像”屏幕中，选择您要将图像映射复制到的图像。
   * (eCatalog) 在“选择资源”屏幕中，选择您要将图像映射复制到的图像或 eCatalog 页面。

1. 选择 **[!UICONTROL 选择]**.

## 使用模板输入JavaScript和URL {#using-a-template-to-enter-javascript-and-urls}

您可以定义 URL 模板（也称为 Href 模板），以便在输入图像映射 URL 时更轻松更有效。如果您的大部分图像映射 URL 都共享通用的固定格式，请定义 URL 模板。在输入固定 URL 部分以作为 URL 模板后，每次创建图像映射时，无需输入该部分 URL。您的 URL 模板也可以包含 JavaScript 命令、路径名和参数。默认情况下，URL模板包含一个名为的专有Adobe Dynamic Media Classic JavaScript处理程序 `loadProduct` 在新窗口中打开图像。

>[!NOTE]
>
>将JavaScript代码添加到图像映射的HREF属性中时，将在客户端计算机上运行该代码。 因此，请确保JavaScript代码是安全的。

### 关于 URL 模板 {#about-url-templates}

URL 模板的工作方式是，在模板中使用两个美元符号 (&#39;$$&#39;) 代替“图像映射”列表中 URL 列的内容：

```as3
Javascript:loadProduct(‘$$’);void(0);
```

您可以在URL模板中的图像映射之间放置所有未更改的值。 仅仅将那些会在 URL 列中发生变化的值添加到“图像映射”列表中。例如：

* URL模板 —  `javascript:loadProduct(‘https://www.examplesitehere.com/$$’);void(0);`
* URL值 —  `product.htm`
* 实际生成的URL - `javascript:loadProduct(‘https://www.examplesitehere.com/product.html);void(0);`

默认情况下，URL模板包含一个名为的专有Adobe Dynamic Media Classic JavaScript处理程序 `loadProduct` 以打开一个包含URL目标的新窗口。 但是，您可以使用任何JavaScript代码来替换此JavaScript处理程序，也可以使用以下Adobe Dynamic Media Classic处理程序之一：

* `loadProductCW`  — 在当前窗口的URL列中显示指定的URL目标。 该处理函数主要用于集成到网站中的页面的 eCatalog。

* `loadProductPW`  — 在父窗口（打开当前窗口的页面）的URL列中显示指定的URL目标。 当前窗口仍处于打开状态，但父窗口切换为显示 URL 目标。

  >[!NOTE]
  >
  >处理程序 `loadProductPW` 不支持 DHTML 和 HTML5 查看器。

### 创建URL模板 {#creating-a-url-template}

1. 在“映射编辑器”屏幕（图像或旋转集）或 eCatalog 屏幕 (eCatalog) 的“映射页面”选项卡上，选择“URL 模板”选项旁边的“编辑”。将打开“编辑映射模板”对话框。
1. 输入JavaScript代码和完整URL（使用美元符号替换变量部分） [$$])。 通过右键单击并选择 **[!UICONTROL 粘贴]**.
1. 选择 **[!UICONTROL 保存]**.

### 处理URL模板 {#handling-url-templates}

“映射编辑器”页面（图像和旋转集）和 eCatalog 屏幕 (eCatalog) 的“映射页面”选项卡提供以下用于处理 URL 模板的命令：

* **URL模板选项**  — 选择“URL模板”选项可将URL模板应用于图像或eCatalog页面上的所有图像映射。

* **模板选项**  — 如果不想让单个图像映射使用URL模板，请取消选择“URL图像映射”列表中的模板选项。

## 定义图像映射的其他操作 {#defining-other-actions-for-image-maps}

您可以选择 **[!UICONTROL 显示]** 菜单并选择 **[!UICONTROL 其他操作]** 用于触发除变换文本和网页启动项以外的操作。 当用户将指针移动到图像映射上时，您可以启动一个操作。这些操作是万维网联盟 HTML 规范为客户端图像映射定义的属性。它们是：

* **`accesskey`**  — 用户按下键盘上的指定键时会触发操作。

* **`onfocus`**  — 当图像映射收到焦点时（通过光标、Tab键或按访问键），将触发事件。 例如，当图像映射被激活时，您可以启动网页，当图像映射被取消激活时，您可以将其关闭。

* **`onblur`**  — 在图像映射因光标或Tab键而失去焦点时触发事件。

**定义图像映射的其他操作:**

1. 在“映射编辑器”屏幕（图像和旋转集）或eCatalog屏幕的“映射页面”选项卡(eCatalog)上，选择 **[!UICONTROL 显示]** 菜单并选择 **[!UICONTROL 其他操作]**.
1. 使用由万维网联盟 HTML 规范指定的语法，在“图像映射”列表的“其他操作”列中添加支持的属性。
1. 选择 **[!UICONTROL 保存]**.

选择 **[!UICONTROL 显示]** 菜单并选择 **[!UICONTROL 两者]** 如果希望图像映射包含变换文本和操作。

## 在Adobe Acrobat或Adobe InDesign中创建图像映射 {#creating-image-maps-in-adobe-acrobat-or-adobe-indesign}

在 Adobe Acrobat 或 Adobe InDesign 中设计 eCatalog 时，您可以创建图像映射。

在Adobe Acrobat或Adobe InDesign中，创建要在其中显示图像映射的超链接引用，并指定图像映射的URL位置。 在上传PDF文件到Adobe Dynamic Media Classic时，选择提取链接选项会自动将链接转换为图像映射。

有关更多信息，请参阅Adobe InDesign帮助或Adobe Acrobat帮助。

### 在 Adobe InDesign 中创建图像映射 {#to-create-image-maps-in-adobe-indesign}

1. 在Adobe InDesign中，转到 **[!UICONTROL Windows®]** > **[!UICONTROL 交互式]** > **[!UICONTROL 超链接]**.
1. 在“超链接”面板中，选择要生成为“图像映射”的文本、框架或图形。
1. 选择 **[!UICONTROL 新建超链接]** 从面板菜单中。
1. 在“新建超链接”对话框中， **[!UICONTROL 链接到]** 菜单，选择 **[!UICONTROL URL]**.
1. 在URL框中键入或粘贴产品ID。
1. 选择 **[!UICONTROL 确定]**. (Adobe Dynamic Media Classic使用图像映射URL模板完成该URL。)

   >[!NOTE]
   >
   >您无需在Adobe InDesign中设置外观选项。 您可以在Adobe Dynamic Media Classic中指定外观。

1. 对于您想要创建的所有图像映射，重复步骤 2 到 6。
1. 将文件导出为 PDF。
1. 将PDF上传到Adobe Dynamic Media Classic。
1. In **[!UICONTROL PDF选项]**，选择 **[!UICONTROL 提取链接]**.

### 在 Adobe Acrobat 中创建图像映射 {#to-create-image-maps-in-adobe-acrobat}

1. 在Adobe Acrobat中，转到 **[!UICONTROL 工具]** > **[!UICONTROL 高级编辑]** > **[!UICONTROL 链接工具]**.
1. 拖动以创建图像映射。
1. 在创建链接框中，选择 **[!UICONTROL 自定义链接]**，并选择 **[!UICONTROL 下一个]**.

>[!NOTE]
>
>您无需在Adobe Acrobat中设置外观选项。 您可以在Adobe Dynamic Media Classic中指定外观。

1. 在链接属性框中，选择 **[!UICONTROL 操作]**.
1. 选择 **[!UICONTROL 打开Web链接]** 从“选择操作”菜单中，然后选择 **[!UICONTROL 添加]**.
1. 在“编辑URL”框中键入图像映射的产品ID，然后选择 **[!UICONTROL 确定]**. (Adobe Dynamic Media Classic使用图像映射URL模板来完成URL。)
1. 对于您想要创建的所有图像映射，重复步骤 1 到 7。
1. 保存文件。
1. 将PDF上传到Adobe Dynamic Media Classic，然后从“PDF选项”中选择“提取链接”。
