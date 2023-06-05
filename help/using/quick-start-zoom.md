---
title: "快速入门：缩放"
description: 介绍和快速入门缩放，帮助您快速启动和运行。
uuid: 31eda632-3469-4f90-885b-e90c6a2e5e75
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/zoom
discoiquuid: 559c986d-313d-46df-a5ff-0b49316ad3a7
feature: Dynamic Media Classic,Viewers,Zoom
role: User
exl-id: eae35207-000c-4ced-b9ab-714c2384a9e7
source-git-commit: 65e3b69bdcbd651a5f9ab100592217e61a8c05ef
workflow-type: tm+mt
source-wordcount: '945'
ht-degree: 25%

---

# 快速入门：缩放{#quick-start-zoom}

缩放允许您以交互方式查看图像中的高分辨率详细信息。 例如，可以在动态的、完全可配置的集成查看器中查看图像的颜色、选项、角度以及细节。此查看器可以嵌在网页中，也可以显示在弹出式窗口中。您可以在近距离审核图像并以高分辨率平移图像以仔细检查它们。 缩放功能可以为您的客户带来丰富多彩的交互式查看体验。

Adobe Dynamic Media Classic还提供了引导式缩放 — 这是一种突出显示图像中的重要功能的方法。 例如，要将查看者的注意力集中于某个徽标上，可以为该徽标创建一个缩放目标。当用户选择此缩放目标时，他们将缩放到徽标。

所有缩放图像都是从单个主图像、图形和数据库驱动属性创建和提供的。 Adobe Dynamic Media Classic缩放可大幅减少制作和交付图像的时间和成本。 您可以使用缩放查看器放大和缩小图像。 缩放查看器具有一些按钮，您可以选择这些按钮来缩放和平移；您还可以通过在屏幕上拖动来平移。 通过缩放查看器预设，可以配置要用于缩放图像的缩放查看器。

参见 [缩放目标：Dynamic Imaging](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/559_Zoom%20Target%20Tool_converted%20renamed_Dynamic%20Imaging-AVS) 和 [缩放：Dynamic Imaging](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/560_Zoom_converted%20renamed_Dynamic%20Imaging-AVS) 培训视频。

以下“缩放快速入门”旨在通过Adobe Dynamic Media Classic中的“缩放”技术让您快速启动并运行。 请按照下述步骤 1 至 6 进行操作。每个步骤后，都会有一个对主题标题的交叉引用，您可以在其中查找更多信息。

## 1.上传缩放图像

首先，将缩放图像上传到Adobe Dynamic Media Classic。 为了优化缩放，Adobe Dynamic Media Classic建议图像的最长大小至少为2000像素。

在全局导航栏上，选择 **[!UICONTROL 上传]** 将图像从您的计算机或网络上传到Adobe Dynamic Media Classic上的文件夹。 参见 [上传缩放图像](uploading-zoom-images.md#uploading_zoom_images).

## 2.创建用于引导缩放的缩放目标

缩放目标可用于突出显示图像的特定部分。例如，您可以将注意力集中在图像与众不同之处。在“缩放查看器”窗口中，缩放目标以缩略图图像的形式显示在图像一侧。选择其中一个缩放目标缩略图，可自动缩放到图像的指定之处。

要创建缩放目标，请选择 **[!UICONTROL 编辑]** 并选择“缩放目标”，或在“浏览”面板的“详细信息”视图中打开图像并选择 **[!UICONTROL 缩放目标]**. 然后，使用“缩放目标编辑器”页面上的“缩放”工具，以便隔离部分图像作为目标。 参见 [为引导缩放创建缩放目标](creating-zoom-targets-guided-zoom.md#creating_zoom_targets_for_guided_zoom).

## 3.设置缩放查看器预设

缩放查看器预设可确定缩放查看器的样式和行为。如果您是管理员，则可以设置缩放查看器预设；Adobe Dynamic Media Classic还附带默认“最佳实践”缩放查看器预设。

要创建缩放查看器预设，请在全局导航栏上，转到 **[!UICONTROL 设置]** > **[!UICONTROL 查看器预设]**. 在“查看器预设”页面上，选择 **[!UICONTROL 添加]**，选择平台和缩放查看器，然后选择 **[!UICONTROL 添加]**. 然后，在“配置查看器”页上选择选项。

Adobe Dynamic Media Classic优惠 **[!UICONTROL 缩放查看器预设]** 允许您选择按钮样式和查看器整体外观的选项。 您还可以自定义网站的缩放设置。参见 [设置缩放查看器预设](setting-zoom-viewer-presets.md#setting_up_zoom_viewer_presets).

## 4.使用缩放查看器预览图像

您可以在缩放查看器中预览图像，查看图像缩放时的缩放效果。

要探索不同的缩放查看器预设及其呈现缩放体验的方式，请在“浏览”面板中选择图像，然后选择 **[!UICONTROL 预览]**. 转到 **[!UICONTROL 预设]** > **[!UICONTROL 缩放]**，然后使用缩放菜单选择预设。

此时会出现“缩放”按钮。可以查看图像在网站上的缩放效果。选择缩放按钮（和缩放目标），以便测试所选缩放查看器预设的设置。 参见 [使用不同的缩放查看器预览图像](previewing-image-assets-different-zoom.md#previewing_image_assets_with_different_zoom_viewers).

## 5.发布缩放图像

发布缩放图像会将它们放在Dynamic Media图像服务器上，以便可以将其交付到您的网站和应用程序。 在发布过程中，Adobe Dynamic Media Classic会激活URL字符串。 这些URL字符串将缩放图像从Dynamic Media图像服务器调用到您的网站或应用程序。

在全局导航栏上，选择 **[!UICONTROL Publish]**. 在“发布”对话框中，选择 **[!UICONTROL 提交发布]**. 请参阅[发布缩放图像](publishing-zoom-images.md#publishing_zoom_images)。

## 6.将Zoom Viewers链接到网页

Adobe Dynamic Media Classic会创建缩放图像所需的URL标注字符串，并在您将图像发布到Dynamic Media图像服务器时激活它们。 您可以从以下位置复制这些URL字符串： **[!UICONTROL 预览]** 页面。 复制 URL 字符串之后，即可在网站和应用程序上使用。参见 [将缩放查看器链接到网页](linking-zoom-viewers-web-pages.md#linking_zoom_viewers_to_your_web_pages).
