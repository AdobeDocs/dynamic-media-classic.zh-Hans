---
title: 快速入门：缩放
description: 介绍和Zoom快速入门可帮助您快速启动和运行。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/zoom
feature: Dynamic Media Classic,Viewers,Zoom
role: User
exl-id: eae35207-000c-4ced-b9ab-714c2384a9e7
topic: Content Management
level: Beginner
autotag-review: '2026-05-13T20:11:12.792Z'
TQID: 'https://experienceleague.adobe.com/0ilSf9rbFcvh2-AVdVnifjNi7bOa5AjCqBFCUC95I5Q'
product_v2: id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
source-git-commit: 7971693d28a933ee56b27e65b87b6a992514e8f6
workflow-type: tm+mt
source-wordcount: 890
ht-degree: 8%

---

# 快速入门：缩放{#quick-start-zoom}

缩放允许您以交互方式查看图像中的高分辨率详细信息。 例如，您可以在可完全配置的动态集成查看器中查看图像详细信息。 此查看器可以嵌入到网页上或显示在弹出窗口中。 要仔细检查图像，可以放大图像并以高分辨率平移。 缩放可为您的用户提供引人入胜、信息丰富且交互式的观看体验。

Adobe Dynamic Media Classic还提供了引导式缩放 — 这是一种突出显示图像中的重要功能的方法。 例如，要将查看者的注意力集中于某个徽标上，可以为该徽标创建一个缩放目标。 当用户选择此缩放目标时，他们将缩放到徽标。

所有缩放图像都由单个主图像、图形和数据库驱动属性创建和提供。 Adobe Dynamic Media Classic缩放可大幅减少制作和交付图像的时间和成本。 可以使用“缩放查看器”放大和减少图像。 缩放查看器具有一些按钮，您可以选择这些按钮来缩放和平移；也可以通过在屏幕上移动指针来平移。 使用缩放查看器预设，您可以配置缩放查看器，以便放大图像。

查看[缩放目标： Dynamic Imaging](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/559_Zoom%20Target%20Tool_converted%20renamed_Dynamic%20Imaging-AVS)和[缩放： Dynamic Imaging](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/560_Zoom_converted%20renamed_Dynamic%20Imaging-AVS)培训视频。

以下缩放快速入门旨在帮助您开始使用Adobe Dynamic Media Classic中的缩放技术。 请按照下述步骤 1 至 6 进行操作。 每一步之后，都会交叉引用主题标题，您可以在其中查找更多信息。

## &#x200B;1. 上传缩放图像

将缩放图像上传到Adobe Dynamic Media Classic。 为了优化缩放，Adobe Dynamic Media Classic建议图像在最长维度中至少为2000像素。

在全局导航栏上，选择&#x200B;**[!UICONTROL 上传]**&#x200B;以将图像从您的计算机或网络上传到Adobe Dynamic Media Classic上的文件夹。 查看[上传缩放图像](uploading-zoom-images.md#uploading_zoom_images)。

## &#x200B;2. 创建用于引导缩放的缩放目标

缩放目标允许您识别图像的特定部分。 例如，可以突出显示图像的独特或独特部分。 在“缩放查看器”窗口中，“缩放目标”在图像一侧显示为缩略图。 选择其中一个缩放目标缩略图，可自动缩放到图像的指定之处。

要创建缩放目标，请选择&#x200B;**[!UICONTROL 编辑]** >缩放目标，或者在“浏览”面板的“详细信息视图”中打开图像并选择&#x200B;**[!UICONTROL 缩放目标]**。 然后，使用“缩放目标编辑器”页面上的“缩放”工具选择部分图像作为目标。 请参阅[创建引导缩放的缩放目标](creating-zoom-targets-guided-zoom.md#creating_zoom_targets_for_guided_zoom)。

## &#x200B;3. 设置缩放查看器预设

缩放查看器预设可确定缩放查看器的样式和行为。 如果您是管理员，可以设置缩放查看器预设；Adobe Dynamic Media Classic也随附默认的标准缩放查看器预设。

要创建缩放查看器预设，请在全局导航栏上，转到&#x200B;**[!UICONTROL 设置]** > **[!UICONTROL 查看器预设]**。 在“查看器预设”页面上，选择&#x200B;**[!UICONTROL 添加]**，选择平台和缩放查看器，然后选择&#x200B;**[!UICONTROL 添加]**。 然后在`Configure Viewer`页面上选择选项。

Adobe Dynamic Media Classic提供了&#x200B;**[!UICONTROL 缩放查看器预设]**&#x200B;选项，可让您选择查看器的按钮样式和整体外观。 您还可以自定义网站的缩放设置。 请参阅[设置缩放查看器预设](setting-zoom-viewer-presets.md#setting_up_zoom_viewer_presets)。

## &#x200B;4. 使用缩放查看器预览图像

要查看缩放体验，您可以在缩放查看器中预览图像。

要浏览不同的缩放查看器预设以及它们呈现缩放体验的方式，请在“浏览”面板中选择图像，然后选择&#x200B;**[!UICONTROL 预览]**。 转到&#x200B;**[!UICONTROL 预设]** > **[!UICONTROL 缩放]**，然后使用“缩放”菜单选择预设。

此时会出现“缩放”按钮。 您可以查看缩放图像在您的网站上的外观。 选择缩放按钮（和缩放目标）以测试您选择的缩放查看器预设的设置。 查看[使用不同的缩放查看器预览图像](previewing-image-assets-different-zoom.md#previewing_image_assets_with_different_zoom_viewers)。

## &#x200B;5. 发布缩放图像

发布缩放图像会将图像放在Dynamic Media图像服务器上，以便将其交付到您的网站和应用程序。 在发布过程中，Adobe Dynamic Media Classic会激活URL字符串。 这些URL字符串将缩放图像从Dynamic Media图像服务器调用到您的网站或应用程序。

在全局导航栏上，选择&#x200B;**[!UICONTROL 发布]**。 在“发布”对话框中，选择&#x200B;**[!UICONTROL 提交发布]**。 请参阅[发布缩放图像](publishing-zoom-images.md#publishing_zoom_images)。

## &#x200B;6. 将缩放查看器链接到网页

Adobe Dynamic Media Classic会创建缩放图像所需的URL标注字符串，并在将图像发布到Dynamic Media图像服务器时激活它们。 您可以从&#x200B;**[!UICONTROL 预览]**&#x200B;页面复制这些URL字符串。 复制URL字符串后，它们便可用于您的网站和应用程序。 查看[将缩放查看器链接到网页](linking-zoom-viewers-web-pages.md#linking_zoom_viewers_to_your_web_pages)
