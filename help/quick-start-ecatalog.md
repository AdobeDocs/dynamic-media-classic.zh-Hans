---
title: “快速开始:eCatalogs”
description: 电子目录简介和快速开始，可帮助您快速使用电子目录技术。
uuid: 1ec41927-3df6-4845-8d9d-bb92cf6dca08
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
discoiquuid: 781dacd0-ef0c-42b7-92e0-12791994874d
feature: Dynamic Media Classic，查看器，电子目录
role: Business Practitioner
exl-id: 9e2df814-465d-412a-a032-ef3e8cb462ba
translation-type: tm+mt
source-git-commit: c5c8c4f96f18339734f4441733cdb1e7f34d3071
workflow-type: tm+mt
source-wordcount: '1427'
ht-degree: 51%

---

# 快速开始:eCatalogs{#quick-start-ecatalogs}

eCatalog 是数字网络版本的印刷材料，例如目录、小册子、传单、产品手册或广告传单。eCatalog 显示在网站的 eCatalog 查看器中。该查看器会模拟阅读印刷材料的体验。根据您为eCatalog选择的设置，查看器允许您执行以下操作：

* 在目录中搜索关键字或关键字。 搜索结果将作为缩略图的列表显示在目录左侧的搜索面板中。 每个可单击的缩略图都表示找到突出显示的搜索词的目录跨页。

* 通过社交媒体分享目录；下载目录以脱机视图;启用“收藏夹”可标记要快速返回的项目或打印目录。
* 使用目录或页面网格视图导航目录；通过单击页面的中间边缘向前或向后翻页。
* 放大、缩小及平移以仔细查看页面上的物品。
* 将指针移到页面区域（称为图像映射）上，这样您就可以看到一个包含项目相关信息的弹出窗口。
* 单击页面区域，以打开一个包含项目详细信息的新网页。
* 写入附注，并将其附加到 eCatalog 页面。
* 如果要启动相关网页或上下文信息面板，请点按图像映射图标。
* 使用手势交互，包括捏合缩放和点刷转页。
* 按关键字搜索物品。

![向用户显示的电子目录。A)电子目录打开页面。 B)eCatalog转到第2页。](/help/assets/ec_cat_viewer_popup.png)

要创建 eCatalog，通常使用在 Adobe® Acrobat® 或其他打印程序中创建的高分辨率 PDF 文件，也可以通过图像文件创建 eCatalog。

创建 eCatalog 过程中，可以按照所选顺序排列页面或跨页。也可以声明需要单页、双页跨页，还是多页跨页。例如，可以为页面区创建图像映射，以使观众能够单击页面上的某个区域，即打开您网站上的新页面。可以使用 eCatalog 屏幕内的“信息面板”设置来管理显示的变换文本。也可以从 100 多个不同的配置选项中选择，以配置 eCatalog 查看器。您可以为特殊受众定制查看器的功能和外观。

>[!NOTE]
>
>如果您是Dynamic Media - Scene7模式用户，并且想使用eCatalogs，则必须在CRXDE Lite中编辑`pdfbrochure`值。 为此，在Adobe Experience Manager中，单击&#x200B;**[!UICONTROL 工具]** > **[!UICONTROL 常规]** > **[!UICONTROL CRXDE Lite]**。 在左侧面板导航树中，导航到`/conf/global/settings/cloudconfigs/dmscene7/jcr:content/mimeTypes/application_pdf`。
>
>在右下方窗格的&#x200B;**[!UICONTROL 属性]**&#x200B;选项卡中，选择`jobParam`行。 将`pdfbrochure`的值从`false`设置为`true`。 如`pdfbrochure=true`中所示
>
>在CRXDE Lite页的左上角，单击&#x200B;**[!UICONTROL 保存全部]**。
>
>您现在可以在Dynamic Media Classic中创作eCatalog。

本 eCatalog 快速入门旨在帮助您快速学会如何使用 eCatalog。按照步骤 1 到 7 操作。每个步骤的后面都有一个交叉引用，可以跳转到相应的主题标题，供您了解更多信息。

## 1.上传PDF文件

eCatalog 通常由 Adobe PDF 文件生成。由于 PDF 文件要用于印刷，因此通常包含 CMYK 图像。Dynamic Media Classic会检测这些图像，并使用标准CMYK颜色用户档案转换它们。 但是，您必须上传并使用自定义颜色用户档案。

在“全局导航”栏上，单击&#x200B;**[!UICONTROL 上传]**&#x200B;以开始为您的eCatalog上传PDF文件或图像。 可以从桌面或通过 FTP 上载文件；如果上载大量文件或大于 100 MB 的文件，则推荐使用 FTP。

“上载”屏幕的“PDF 选项”下面提供了一些选项，用于上载分辨率合适并且颜色空间正确的 PDF 文件。推荐使用 150 PPI 的分辨率。上载 PDF 文件时，可以选择“自动生成 eCatalog”选项来创建 eCatalog。

请参阅[上载 PDF 文件](uploading-pdf-files.md#uploading_the_pdf_files)。

## 2.创建电子目录

通过在浏览面板中选择PDF或图像文件来创建电子目录。 单击&#x200B;**[!UICONTROL 构建]**，然后选择&#x200B;**[!UICONTROL eCatalogs]**。

在eCatalog页面的&#x200B;**[!UICONTROL Order Pages]**&#x200B;选项卡上，选择布局选项：**[!UICONTROL 1向上]**、**[!UICONTROL 2向上]**&#x200B;或&#x200B;**[!UICONTROL 自定义]**。 可以通过拖动的方式，或者在大型 eCatalog 中在“移至”菜单中选择页面名称，来重新排列页面或跨页。

要添加页面，在“资源库”中选择一个文件夹，然后将其中的 PDF 或图像文件拖动到“排序页面”屏幕中。您可以提供自定义页面名称或导入许多页面名称，而不是默认页码。

单击&#x200B;**[!UICONTROL 保存]**，输入eCatalog的名称，选择一个Dynamic Media Classic文件夹进行存储，然后单击&#x200B;**[!UICONTROL 保存]**。 每次更改页面顺序或编辑eCatalog时，请单击&#x200B;**[!UICONTROL 保存]**&#x200B;以保存更改。

请参阅[创建 eCatalog](creating-ecatalog.md)。

## 3.创建图像映射

图像映射向eCatalog页面添加了另一个方面。 图像映射是页面上的一个区域，可提供关于某个物品的更多信息。当观众在“图像映射”上滚动鼠标指针时，他们会看到物品的说明。单击“图像映射”会激活一个外部引用，该引用打开一个新的网页，您可以从中了解关于某个物品的更多信息。

要创建图像映射，打开 eCatalog 屏幕。然后，转到eCatalog屏幕的&#x200B;**[!UICONTROL 映射页面]**&#x200B;选项卡，并使用矩形图像映射工具或多边形图像映射工具对映射进行框架设置。 可以使用“平移”工具  拖动映射边框来调整“图像映射”的位置和大小。

在对图像映射进行帧化后，输入在单击图像映射时要转到的URL地址。 也可以输入当您将指针移动到图像映射上时所显示的变换文本。

请参阅[创建 eCatalog 图像映射](creating-ecatalog-image-maps.md#creating-ecatalog-image-maps)。

请参阅[使用图像映射在 eCatalog 中嵌入富媒体](creating-ecatalog-image-maps.md#embedding-rich-media-in-an-ecatalog)。

可以在 eCatalog 屏幕中使用“信息面板”设置来建立和管理图像映射文本。

请参阅[管理信息面板内容](info-panel-content.md#managing-info-panel-content)。

## 4.设置电子目录查看器预设

最终用户在“eCatalog 查看器中”看到您的 eCatalog。如果您是管理员，还可以配置 eCatalog 查看器。可以更改其轮廓颜色，并选择新的“外观”来确立 eCatalog 品牌。Dynamic Media Classic附带了多种“最佳实践” eCatalog查看器预设。 可以选择这些预设中的一个预设来显示 eCatalog。如果您是管理员，还可以创建自己的 eCatalog 查看器预设。

要创建eCatalog查看器预设，请在全局导航栏上单击&#x200B;**[!UICONTROL 设置]**，然后选择&#x200B;**[!UICONTROL 查看器预设]**。 然后，单击&#x200B;**[!UICONTROL 添加]**，选择平台，然后单击&#x200B;**[!UICONTROL eCatalog > Viewer]**。

请参阅[设置 eCatalog 查看器预设](setting-ecatalog-viewer-presets.md#setting-up-ecatalog-viewer-presets)。

## 5.在eCatalog Viewer中预览eCatalog

eCatalog 查看器预设决定了 eCatalog 查看器的样式和行为。

要了解eCatalog查看器预设如何显示您的eCatalog，请在浏览面板中选择您的eCatalog，然后单击&#x200B;**[!UICONTROL 预览]**。 “预览”屏幕随即在默认查看器中打开。

注意方向、配色方案、更改页面的控件的外观以及页面翻转时的显示效果。

请参阅[在 eCatalog 查看器中预览 eCatalog](previewing-ecatalogs-ecatalog-viewer.md#previewing-ecatalogs-in-the-ecatalog-viewer)。

## 6.发布电子目录和关联的PDF

发布电子目录和关联的PDF会将其放在Dynamic Media图像服务器上，以便能够将其交付到您的网站和应用程序。 在发布过程中，Dynamic Media Classic会激活您的eCatalog的URL字符串。 使用此URL将eCatalog从Dynamic Media Image Servers调用到您的网站或应用程序。

在浏览面板中标记要发布的电子目录和PDF后，选择全局导航栏上的“发布”按钮以启动发布。 在“发布”屏幕上，单击&#x200B;**[!UICONTROL 提交发布]**。

请参阅[发布eCatalog和关联的PDF](publishing-ecatalogs-associated-pdfs.md#publishing-ecatalogs-and-associated-pdfs)。

## 7.将电子目录链接到网页

Dynamic Media Classic在将eCatalog发布到Dynamic Media Image Server时，将激活显示该eCatalog所需的URL标注字符串。 可以在“预览”屏幕和浏览面板（在详细信息视图中）上选择 URL 来复制该 URL 字符串。复制 URL 字符串之后，该 URL 便可用于您的网站和应用程序。

与您的 IT 团队合作，将 eCatalog 链接放在网页中的合适位置。当用户单击该链接时，将显示 eCatalog 查看器，用户即可浏览您的 eCatalog。

请参阅[将 eCatalog 链接到网页](linking-ecatalog-web-page.md#linking-an-ecatalog-to-a-web-page)。
