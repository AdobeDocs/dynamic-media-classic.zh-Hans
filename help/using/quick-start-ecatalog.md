---
title: 快速入门：eCatalogs
description: eCatalogs简介和快速入门，可帮助您在Adobe Dynamic Media Classic中使用eCatalog技术快速启动和运行。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: 9e2df814-465d-412a-a032-ef3e8cb462ba
topic: Integrations
level: Experienced
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '1470'
ht-degree: 25%

---

# 快速入门：eCatalogs{#quick-start-ecatalogs}

eCatalog是印刷材料的数字Web版本 — 例如，目录、小册子、传单、产品手册或广告通告。 eCatalog显示在网站上的eCatalog查看器中。 此查看器可模拟阅读印刷材料的体验。

另请观看以下培训视频：

* [快速入门1： eCatalogs](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/561_Quick%20Start%20-%20Part%201_converted%20renamed_eCatalogs-AVS)
* [快速入门2： eCatalogs](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/562_Quick%20Start%20-%20Part%202_converted%20renamed_eCatalogs-AVS)

根据您为eCatalog选择的设置，查看器可以让您执行以下操作：

* 在目录中搜索一个或多个关键字。 搜索结果将作为缩略图列表显示在目录左侧的搜索面板中。 每个可单击的缩略图表示一个目录跨页，其中找到了高亮显示的搜索词。

* 通过社交媒体共享目录；下载目录以离线查看；启用“收藏夹”以标记要快速返回的项目，或打印目录。
* 使用目录或页面网格视图导航目录；通过选择页面的中边缘来向前或向后导航页面。
* 放大、缩小及平移以仔细查看页面上的物品。
* 将指针移动到页面区域（称为图像映射）上，以便您能够看到包含项目相关信息的弹出窗口。
* 选择页面区域，以打开一个包含有关项目的更多信息的新网页。
* 写入附注，并将其附加到 eCatalog 页面。
* 如果要启动相关网页或上下文信息面板，请点按图像映射图标。
* 使用手势交互，包括捏合缩放和点刷转页。
* 按关键字搜索物品。

![向用户显示的eCatalog。 A) eCatalog打开页面。 B)eCatalog已转到第2页。](/help/using/assets/ec_cat_viewer_popup.png)

要创建eCatalog，通常使用在Adobe Acrobat或其他打印程序中创建的高分辨率PDF文件，但也可以从图像文件创建eCatalog。

创建 eCatalog 过程中，可以按照所选顺序排列页面或跨页。也可以声明需要单页、双页跨页，还是多页跨页。您可以为页面区域创建图像映射，以便查看者可以（例如）在页面上选择一个区域，然后在您的网站上打开一个新页面。 可以使用 eCatalog 屏幕内的“信息面板”设置来管理显示的变换文本。也可以从 100 多个不同的配置选项中选择，以配置 eCatalog 查看器。您可以为特殊受众定制查看器的功能和外观。

>[!NOTE]
>
>如果您是Dynamic Media： Scene7模式用户，并且要使用eCatalogs，请在CRXDE Lite中编辑`pdfbrochure`值。 为此，请在Adobe Experience Manager中转到&#x200B;**[!UICONTROL 工具]** > **[!UICONTROL 常规]** > **[!UICONTROL CRXDE Lite]**。 在左侧面板导航树中，导航到`/conf/global/settings/cloudconfigs/dmscene7/jcr:content/mimeTypes/application_pdf`。
>
>在右下窗格的&#x200B;**[!UICONTROL 属性]**&#x200B;选项卡中，选择`jobParam`行。 将`pdfbrochure`的值从`false`设置为`true`。 作为`pdfbrochure=true`
>
>在CRXDE Lite页面的左上角，选择&#x200B;**[!UICONTROL 全部保存]**。
>
>您现在可以在Adobe Dynamic Media Classic中创作eCatalogs。

本 eCatalog 快速入门旨在帮助您快速学会如何使用 eCatalog。按照步骤 1 到 7 操作。每一步之后，都会交叉引用主题标题，您可以在其中查找更多信息。

## 1.上传PDF文件

eCatalog 通常由 Adobe PDF 文件生成。由于 PDF 文件要用于印刷，因此通常包含 CMYK 图像。Adobe Dynamic Media Classic检测这些图像并使用标准CMYK颜色配置文件转换它们。 但是，您必须上传并使用自定义颜色配置文件。

在全局导航栏上，选择&#x200B;**[!UICONTROL 上传]**&#x200B;以开始上传eCatalog的PDF文件或图像。 您可以从桌面或通过FTP上传文件；如果要上传的文件数或文件数超过100 MB，建议使用FTP。

“上载”屏幕的“PDF 选项”下面提供了一些选项，用于上载分辨率合适并且颜色空间正确的 PDF 文件。推荐使用 150 PPI 的分辨率。您可以选择选项&#x200B;**[!UICONTROL 自动生成eCatalog]**&#x200B;在上传PDF文件时创建eCatalog。

请参阅[上传PDF文件](uploading-pdf-files.md#uploading_the_pdf_files)。

## 2.创建eCatalog

通过在“浏览”面板中选择PDF或图像文件来创建eCatalog。 选择&#x200B;**[!UICONTROL 生成]**，然后选择&#x200B;**[!UICONTROL eCatalogs]**。

在eCatalog页面的&#x200B;**[!UICONTROL 订购页]**&#x200B;选项卡上，选择布局选项： **[!UICONTROL 1 Up]**、**[!UICONTROL 2 Up]**&#x200B;或&#x200B;**[!UICONTROL 自定义]**。 可以通过拖动的方式，或者在大型 eCatalog 中在“移至”菜单中选择页面名称，来重新排列页面或跨页。

要添加页面，在“资源库”中选择一个文件夹，然后将其中的 PDF 或图像文件拖动到“排序页面”屏幕中。您可以提供自定义页面名称或导入多个页面名称，而不是默认页码。

选择&#x200B;**[!UICONTROL 保存]**，输入eCatalog的名称，选择用于存储它的Adobe Dynamic Media Classic文件夹，然后选择&#x200B;**[!UICONTROL 保存]**。 每次更改页面顺序或编辑eCatalog时，请选择&#x200B;**[!UICONTROL 保存]**&#x200B;以保存更改。

请参阅[创建eCatalog](creating-ecatalog.md)。

## 3.创建图像映射

图像映射为eCatalog页面添加了其他方面。 图像映射是页面上的一个区域，可提供关于某个物品的更多信息。当观众在“图像映射”上滚动鼠标指针时，他们会看到物品的说明。单击图像映射可激活外部引用，该引用会打开一个新网页，您可以在其中了解有关项目的更多信息。

要创建图像映射，打开 eCatalog 屏幕。然后转到eCatalog屏幕的&#x200B;**[!UICONTROL 映射页面]**&#x200B;选项卡，并使用“矩形图像映射”工具或“多边形图像映射”工具将映射框架化。 可以使用“平移”工具拖动映射边框，调整图像映射的位置和大小。

在构建图像映射框架后，输入要在选择图像映射时转到的URL地址。 也可以输入当您将指针移动到图像映射上时所显示的变换文本。

查看[创建eCatalog图像映射](creating-ecatalog-image-maps.md#creating-ecatalog-image-maps)。

请参阅[使用图像映射在eCatalog中嵌入富媒体](creating-ecatalog-image-maps.md#embedding-rich-media-in-an-ecatalog)。

您可以使用eCatalog屏幕中的“信息面板”设置来设置和管理图像映射文本。

查看[在eCatalogs](/help/using/info-panel-content-ecatalog.md)中管理信息面板内容。

## 4.设置eCatalog查看器预设

最终用户在“eCatalog 查看器中”看到您的 eCatalog。如果您是管理员，还可以配置 eCatalog 查看器。您可以更改其轮廓颜色并选择新的“外观”来标记您的eCatalog。 Adobe Dynamic Media Classic附带多个“最佳实践”eCatalog查看器预设。 可以选择这些预设中的一个预设来显示 eCatalog。如果您是管理员，还可以创建自己的 eCatalog 查看器预设。

要创建eCatalog查看器预设，请在全局导航栏上选择&#x200B;**[!UICONTROL 设置]**，然后选择&#x200B;**[!UICONTROL 查看器预设]**。 选择&#x200B;**[!UICONTROL 添加]**，选择一个平台，然后选择&#x200B;**[!UICONTROL eCatalog]** > **[!UICONTROL 查看器]**。

请参阅[设置eCatalog查看器预设](setting-ecatalog-viewer-presets.md#setting-up-ecatalog-viewer-presets)。

## 5.在eCatalog查看器中预览eCatalog

eCatalog 查看器预设决定了 eCatalog 查看器的样式和行为。

要了解eCatalog查看器预设如何显示您的eCatalog，请在“浏览”面板中选择您的eCatalog，然后选择&#x200B;**[!UICONTROL 预览]**。 “预览”屏幕随即在默认查看器中打开。

注意方向、配色方案、更改页面的控件的外观以及页面翻转时的显示效果。

查看[在eCatalog查看器](previewing-ecatalogs-ecatalog-viewer.md#previewing-ecatalogs-in-the-ecatalog-viewer)中预览eCatalog。

## 6. Publish eCatalog和相关PDF

发布eCatalog和相关的PDF会将其放在Dynamic Media图像服务器上，以便可以将其交付到您的网站和应用程序。 在发布过程中，Adobe Dynamic Media Classic会激活eCatalog的URL字符串。 使用此URL可从Dynamic Media图像服务器向您的网站或应用程序调用eCatalog。

在“浏览”面板中将eCatalog和PDF标记为发布后，选择全局导航栏上的“Publish”按钮以启动发布。 在发布页面上，选择&#x200B;**[!UICONTROL 提交Publish]**。

查看[Publish eCatalogs和相关的PDF](publishing-ecatalogs-associated-pdfs.md#publishing-ecatalogs-and-associated-pdfs)。

## 7.将eCatalog链接到网页

在将eCatalog发布到Adobe Dynamic Media Classic图像服务器时，Dynamic Media会激活显示它所需的URL标注字符串。 您可以通过在“预览”屏幕和“浏览”面板（在“详细信息”视图中）中选择URL，来复制此URL字符串。 复制URL字符串后，您的网站和应用程序即可使用该字符串。

与您的IT团队合作，将指向eCatalog的链接放置在网页中的适当位置。 当用户选择该链接时，会显示eCatalog查看器，用户可以浏览您的eCatalog。

请参阅[将eCatalog链接到网页](linking-ecatalog-web-page.md#linking-an-ecatalog-to-a-web-page)。
