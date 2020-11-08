---
title: '"快速入门：缩放"'
seo-title: '"快速入门：缩放"'
description: 'null'
seo-description: 简介和快速缩放开始可帮助您快速入门。
uuid: 31eda632-3469-4f90-885b-e90c6a2e5e75
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/zoom
discoiquuid: 559c986d-313d-46df-a5ff-0b49316ad3a7
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '841'
ht-degree: 65%

---


# 快速入门：缩放{#quick-start-zoom}

通过缩放，您可以交互视图图像中的高分辨率细节。 例如，可以在动态的、完全可配置的集成查看器中查看图像的颜色、选项、角度以及细节。此查看器可以嵌在网页中，也可以显示在弹出式窗口中。可以近距离检查图像，以及在高分辨率下平移图像以便更仔细地对其进行检查。缩放功能可以为您的客户带来丰富多彩的交互式查看体验。

Dynamic Media Classic还优惠了引导缩放——一种突出显示图像中重要功能的方法。 例如，要将查看者的注意力集中于某个徽标上，可以为该徽标创建一个缩放目标。查看者单击该缩放目标时，即可缩放到该徽标。

所有缩放图像都可以从单个主图像、图形和数据库驱动的属性中创建并供人们使用。动态媒体经典缩放功能大大减少了制作和传送图像的时间和成本。 您可以使用缩放查看器放大和缩小图像。 缩放查看器上带有可单击实现缩放和平移的按钮；也可以在屏幕上拖动来进行平移。通过缩放查看器预设，可以配置要用于缩放图像的缩放查看器。

**快速开始**

此快速缩放开始旨在利用Dynamic Media Classic中的缩放技术快速启动和运行。 请按照下述步骤 1 至 6 进行操作。每个步骤的后面都有一个交叉引用，可以跳转到相应的主题标题，供您了解更多信息。

**1. 上载缩放图像**

开始，即可将缩放图像上传到Dynamic Media Classic。 为获得最佳缩放效果，Dynamic Media Classic建议图像的最长尺寸至少为2000像素。

选择全局导航栏上的“上传”按钮，将图像从您的计算机或网络上传到Dynamic Media Classic上的文件夹。 请参阅[上载缩放图像](uploading-zoom-images.md#uploading_zoom_images)。

**2. 创建缩放目标以进行引导式缩放**

缩放目标可用于突出显示图像的特定部分。例如，您可以将注意力集中在图像与众不同之处。在“缩放查看器”窗口中，缩放目标以缩略图图像的形式显示在图像一侧。选择其中一个缩放目标缩略图，可自动缩放到图像的指定之处。

要创建缩放目标，请单击鼠标悬停在“编辑”按钮并选择“缩放目标”，或在浏览面板的“详细信息”视图中打开图像，然后单击“缩放目标”。 然后，使用“缩放目标编辑器”屏幕上的缩放工具划分出要设为目标的图像部分。请参阅[为引导式缩放创建缩放目标](creating-zoom-targets-guided-zoom.md#creating_zoom_targets_for_guided_zoom)。

**3. 设置缩放查看器预设**

缩放查看器预设可确定缩放查看器的样式和行为。如果您是管理员，则可以设置缩放查看器预设；Dynamic Media Classic也附带默认的“最佳实践”缩放查看器预设。

要创建缩放查看器预设，请在全局导航栏上单击“设置”按钮，然后选择“查看器预设”。然后在“查看器预设”屏幕上单击“添加”按钮，选择一个平台并选择缩放查看器，然后单击“添加”。然后选择“配置查看器”屏幕上的选项。

动态媒体经典优惠缩放查看器预设选项允许您选择查看器的按钮样式和整体外观。 您还可以自定义网站的缩放设置。请参阅[设置缩放查看器预设](setting-zoom-viewer-presets.md#setting_up_zoom_viewer_presets)。

**4. 使用缩放查看器预览图像**

您可以在缩放查看器中预览图像，查看图像缩放时的缩放效果。

要浏览各种缩放查看器预设及其缩放效果，请在浏览面板中选择图像，然后单击“预览”按钮。“预览”屏幕随即打开。选择“预设”>“缩放”，然后在缩放菜单中选择一个预设。

此时会出现“缩放”按钮。可以查看图像在网站上的缩放效果。选择“缩放”按钮（及缩放目标）以测试所选的缩放查看器预设的设置。请参阅[使用不同缩放查看器预览图像](previewing-image-assets-different-zoom.md#previewing_image_assets_with_different_zoom_viewers)。

**5. 发布缩放图像**

发布缩放图像会将其放置在Dynamic Media图像服务器上，以便能够将其交付到您的网站和应用程序。 在发布过程中，Dynamic Media Classic会激活URL字符串。 这些URL字符串将缩放图像从Dynamic Media图像服务器调用到您的网站或应用程序。

选择全局导航栏上的“发布”按钮来启动发布。在“发布”屏幕上，选择“开始发布”按钮。请参阅[发布缩放图像](publishing-zoom-images.md#publishing_zoom_images)。

**6. 将缩放查看器链接到网页**

Dynamic Media Classic创建缩放图像所需的URL标注字符串，并在将图像发布到Dynamic Media图像服务器时将其激活。 可从“预览”屏幕复制这些 URL 字符串。复制 URL 字符串之后，即可在网站和应用程序上使用。请参阅[将缩放查看器链接到网页](linking-zoom-viewers-web-pages.md#linking_zoom_viewers_to_your_web_pages)。
