---
title: “快速入门：电子目录”
seo-title: “快速入门：电子目录”
description: 'null'
seo-description: 电子目录简介和快速入门，帮助您使用eCatalog技术快速上手和运行。
uuid: 1ec41927-3df6-4845-8d9d-bb92 cf6 dca08
contentOwner: admin
content-type: 引用
products: SG_ EXPERIENCE MANAGER/Dynamic-Media-Scene-7
geptopics: SG_ SCENESELEFERENDER_ PK/categories/ecatalloc
discoiquuid: 781dacd0-ef0 c-42b7-92e0-127919944874d
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# 快速入门：电子目录{#quick-start-ecatalogs}

eCatalog 是数字网络版本的印刷材料，例如目录、小册子、传单、产品手册或广告传单。eCatalog 显示在网站的 eCatalog 查看器中。该查看器会模拟阅读印刷材料的体验。根据您为eCatalog选择的设置，查看器可允许您执行以下操作：

* 搜索关键字或关键字的目录。搜索结果将作为缩略图列表显示在目录左侧的搜索面板中。每个可单击缩略图表示在找到高亮显示的搜索词的目录。

* 通过社交媒体共享目录；下载目录以脱机查看；启用“收藏夹”以标记要返回的项目，或打印目录。
* 使用目录或页面网格视图导航目录；通过单击页面的中间边缘向前或向后翻页。
* 放大、缩小及平移以仔细查看页面上的物品。
* 将指针移动到页面上某个区域（称为图像映射），可以看到一个弹出窗口，其中包含关于某个物品的信息。
* 单击页面某个区域可以打开新的网页，其中包含关于某个物品的更多信息。
* 写入附注，并将其附加到 eCatalog 页面。
* 点击图像映射图标以启动相关网页或上下文信息面板。
* 使用手势交互，包括捏合缩放和点刷转页。
* 按关键字搜索物品。

![用户看到的 eCatalog 外观。A) 电子目录打开页面。B)eCatalog turned to page 2.](/help/assets/ec_cat_viewer_popup.png)

要创建 eCatalog，通常使用在 Adobe® Acrobat® 或其他打印程序中创建的高分辨率 PDF 文件，也可以通过图像文件创建 eCatalog。

创建 eCatalog 过程中，可以按照所选顺序排列页面或跨页。也可以声明需要单页、双页跨页，还是多页跨页。例如，可以为页面区创建图像映射，以使观众能够单击页面上的某个区域，即打开您网站上的新页面。可以使用 eCatalog 屏幕内的“信息面板”设置来管理显示的变换文本。也可以从 100 多个不同的配置选项中选择，以配置 eCatalog 查看器。您可以为特殊受众定制查看器的功能和外观。

**快速入门**

本 eCatalog 快速入门旨在帮助您快速学会如何使用 eCatalog。按照步骤 1 到 7 操作。每个步骤的后面都有一个交叉引用，可以跳转到相应的主题标题，供您了解更多信息。

**1. 上载 PDF 文件**

eCatalog 通常由 Adobe PDF 文件生成。由于 PDF 文件要用于印刷，因此通常包含 CMYK 图像。Scene7 Publishing System 会检测到这些图像，并使用标准 CMYK 颜色配置文件转换这些图像。但您可能必须上载并使用自定颜色配置文件。

单击全局导航栏上的上传以开始上传电子目录中的PDF文件或图像。可以从桌面或通过 FTP 上载文件；如果上载大量文件或大于 100 MB 的文件，则推荐使用 FTP。

“上载”屏幕的“PDF 选项”下面提供了一些选项，用于上载分辨率合适并且颜色空间正确的 PDF 文件。推荐使用 150 PPI 的分辨率。上载 PDF 文件时，可以选择“自动生成 eCatalog”选项来创建 eCatalog。

请参阅[上载 PDF 文件](uploading-pdf-files.md#uploading_the_pdf_files)。

**2. 创建 eCatalog**

在浏览面板中选择 PDF 或图像文件，然后单击“构建”按钮并选择 eCatalog，便可以创建 eCatalog。eCatalog 屏幕随即打开。

在“排序页面”选项卡上，选择“布局”按钮（“单页”、“二合一”或“自定义”），以选择要单页跨页、双页跨页还是自定义页面跨页。可以通过拖动的方式，或者在大型 eCatalog 中在“移至”菜单中选择页面名称，来重新排列页面或跨页。

要添加页面，在“资源库”中选择一个文件夹，然后将其中的 PDF 或图像文件拖动到“排序页面”屏幕中。除默认提供页码外，您还可以提供自定义页面名称或导入大量页面名称。

单击“保存”按钮，输入 eCatalog 的名称，选择用来存储 eCatalog 的 SPS 文件夹，然后选择“保存”按钮。每次更改页面顺序或编辑 eCatalog 时，要单击“保存”按钮来保存更改。

请参阅[创建 eCatalog](creating-ecatalog.md)。

**3. 创建图像映射**

图像映射为 eCatalog 页面增加了另一项特色。图像映射是页面上的一个区域，可提供关于某个物品的更多信息。当观众在“图像映射”上滚动鼠标指针时，他们会看到物品的说明。单击“图像映射”会激活一个外部引用，该引用打开一个新的网页，您可以从中了解关于某个物品的更多信息。

要创建图像映射，打开 eCatalog 屏幕。然后转至 eCatalog 屏幕的“映射页面”选项卡，并使用“矩形图像映射”工具  或“多边形图像映射”工具  以绘制映射。可以使用“平移”工具  拖动映射边框来调整“图像映射”的位置和大小。

在绘制图像映射之后，输入希望在单击“图像映射”后所转到的 URL 地址。也可以输入当您将指针移动到图像映射上时所显示的变换文本。

请参阅[创建 eCatalog 图像映射](creating-ecatalog-image-maps.md#creating-ecatalog-image-maps)。

请参阅[使用图像映射在 eCatalog 中嵌入富媒体](creating-ecatalog-image-maps.md#embedding-rich-media-in-an-ecatalog)。

可以在 eCatalog 屏幕中使用“信息面板”设置来建立和管理图像映射文本。

请参阅[管理信息面板内容](info-panel-content.md#managing-info-panel-content)。

**4. 设置 eCatalog 查看器预设**

最终用户在“eCatalog 查看器中”看到您的 eCatalog。如果您是管理员，还可以配置 eCatalog 查看器。可以更改其轮廓颜色，并选择新的“外观”来确立 eCatalog 品牌。动态媒体经典附带几个“最佳实践”eCatalog查看器预设。可以选择这些预设中的一个预设来显示 eCatalog。如果您是管理员，还可以创建自己的 eCatalog 查看器预设。

要创建 eCatalog 查看器预设，单击全局导航栏上的“设置”按钮并选择“查看器预设”。然后单击“添加”，选择平台，再选择“eCatalog”&gt;“查看器”。

请参阅[设置 eCatalog 查看器预设](setting-ecatalog-viewer-presets.md#setting-up-ecatalog-viewer-presets)。

**5. 在 eCatalog 查看器中预览 eCatalog**

eCatalog 查看器预设决定了 eCatalog 查看器的样式和行为。

要了解 eCatalog 查看器预设如何显示 eCatalog，在浏览面板中选择 eCatalog，然后单击“预览”。“预览”屏幕随即在默认查看器中打开。

注意方向、配色方案、更改页面的控件的外观以及页面翻转时的显示效果。

请参阅[在 eCatalog 查看器中预览 eCatalog](previewing-ecatalogs-ecatalog-viewer.md#previewing-ecatalogs-in-the-ecatalog-viewer)。

**6. 发布电子目录和关联的PDF**

发布eCatalog和关联的PDF可将其放置在动态媒体图像服务器上，以便将其传送到您的网站和应用程序。在发布过程中，Scene7 Publishing System 会激活 eCatalog 的 URL 字符串。使用此URL将电子目录从Dynamic Media图像服务器调用到您的网站或应用程序。

在浏览面板中标记要发布的电子目录和PDF后，在全局导航栏上选择“发布”按钮以启动发布。在“发布”屏幕上，单击“开始发布”。

请参阅 [发布电子目录和关联的PDF](publishing-ecatalogs-associated-pdfs.md#publishing-ecatalogs-and-associated-pdfs)。

**7. 将 eCatalog 链接到网页**

动态媒体经典激活将电子目录发布到Dynamic Media图像服务器时所需的URL标注字符串。可以在“预览”屏幕和浏览面板（在详细信息视图中）上选择 URL 来复制该 URL 字符串。复制 URL 字符串之后，该 URL 便可用于您的网站和应用程序。

与您的 IT 团队合作，将 eCatalog 链接放在网页中的合适位置。当用户单击该链接时，将显示 eCatalog 查看器，用户即可浏览您的 eCatalog。

请参阅[将 eCatalog 链接到网页](linking-ecatalog-web-page.md#linking-an-ecatalog-to-a-web-page)。