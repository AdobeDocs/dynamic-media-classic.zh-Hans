---
title: '"快速入门：缩放"'
description: 简介和缩放快速入门可帮助您快速启动并运行。
uuid: 31eda632-3469-4f90-885b-e90c6a2e5e75
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/zoom
discoiquuid: 559c986d-313d-46df-a5ff-0b49316ad3a7
feature: Dynamic Media Classic，查看器，缩放
role: User
exl-id: eae35207-000c-4ced-b9ab-714c2384a9e7
source-git-commit: df689ff5a127bfbc400ca5331168d1ff7bb0b42e
workflow-type: tm+mt
source-wordcount: '813'
ht-degree: 41%

---

# 快速入门：缩放{#quick-start-zoom}

缩放功能允许您以交互方式查看图像中的高分辨率详细信息。 例如，可以在动态的、完全可配置的集成查看器中查看图像的颜色、选项、角度以及细节。此查看器可以嵌在网页中，也可以显示在弹出式窗口中。您可以在近距离审核图像，以高分辨率平移图像，以便仔细检查它们。 缩放功能可以为您的客户带来丰富多彩的交互式查看体验。

Dynamic Media Classic还提供了引导式缩放功能，这是您突出显示图像中重要功能的一种方式。 例如，要将查看者的注意力集中于某个徽标上，可以为该徽标创建一个缩放目标。查看者单击该缩放目标时，即可缩放到该徽标。

所有缩放图像都可以从单个主图像、图形和数据库驱动的属性中创建并供人们使用。Dynamic Media Classic缩放功能可显着减少制作和传送图像的时间和成本。 您可以使用缩放查看器来放大和缩小图像。 缩放查看器上带有可单击实现缩放和平移的按钮；也可以在屏幕上拖动来进行平移。通过缩放查看器预设，可以配置要用于缩放图像的缩放查看器。

此缩放快速入门旨在使用Dynamic Media Classic中的缩放技术快速启动并运行。 请按照下述步骤 1 至 6 进行操作。每个步骤的后面都有一个交叉引用，可以跳转到相应的主题标题，供您了解更多信息。

## 1.上传缩放图像

首先，将缩放图像上传到Dynamic Media Classic。 为了获得最佳缩放效果，Dynamic Media Classic建议图像的最大大小至少为2000像素。

在全局导航栏上，单击&#x200B;**[!UICONTROL Upload]** ，将图像从您的计算机或网络上传到Dynamic Media Classic上的文件夹。 请参阅[上载缩放图像](uploading-zoom-images.md#uploading_zoom_images)。

## 2.为引导式缩放创建缩放目标

缩放目标可用于突出显示图像的特定部分。例如，您可以将注意力集中在图像与众不同之处。在“缩放查看器”窗口中，缩放目标以缩略图图像的形式显示在图像一侧。选择其中一个缩放目标缩略图，可自动缩放到图像的指定之处。

要创建缩放目标，请单击&#x200B;**[!UICONTROL 编辑]**&#x200B;并选择“缩放目标”，或在“浏览”面板的“详细信息”视图中打开图像，然后单击&#x200B;**[!UICONTROL 缩放目标]**。 然后，使用“缩放目标编辑器”页面上的缩放工具，以便能够将部分图像隔离为目标。 请参阅[为引导式缩放创建缩放目标](creating-zoom-targets-guided-zoom.md#creating_zoom_targets_for_guided_zoom)。

## 3.设置缩放查看器预设

缩放查看器预设可确定缩放查看器的样式和行为。如果您是管理员，则可以设置缩放查看器预设；Dynamic Media Classic还附带默认的“最佳实践”缩放查看器预设。

要创建缩放查看器预设，请在全局导航栏上单击&#x200B;**[!UICONTROL 设置]** > **[!UICONTROL 查看器预设]**。 在“查看器预设”页面上，单击&#x200B;**[!UICONTROL 添加]**，选择平台和缩放查看器，然后单击&#x200B;**[!UICONTROL 添加]**。 然后，在“配置查看器”页面上选择选项。

Dynamic Media Classic提供了&#x200B;**[!UICONTROL 缩放查看器预设]**&#x200B;选项，允许您选择查看器的按钮样式和整体外观。 您还可以自定义网站的缩放设置。请参阅[设置缩放查看器预设](setting-zoom-viewer-presets.md#setting_up_zoom_viewer_presets)。

## 4.使用缩放查看器预览图像

您可以在缩放查看器中预览图像，查看图像缩放时的缩放效果。

要浏览不同的缩放查看器预设以及它们如何显示缩放体验，请在浏览面板中选择一个图像，然后单击&#x200B;**[!UICONTROL 预览]**。 单击&#x200B;**[!UICONTROL 预设]** > **[!UICONTROL 缩放]**，然后使用缩放菜单选择预设。

此时会出现“缩放”按钮。可以查看图像在网站上的缩放效果。单击缩放按钮（和缩放目标），以便您可以测试所选缩放查看器预设的设置。 请参阅[使用不同缩放查看器预览图像](previewing-image-assets-different-zoom.md#previewing_image_assets_with_different_zoom_viewers)。

## 5.发布缩放图像

发布缩放图像会将图像放置在Dynamic Media图像服务器上，以便能够将它们交付到您的网站和应用程序。 在发布过程中，Dynamic Media Classic会激活URL字符串。 这些URL字符串将调用从Dynamic Media图像服务器到您的网站或应用程序的缩放图像。

在全局导航栏上，单击“**[!UICONTROL 发布]**”。在“发布”对话框中，单击&#x200B;**[!UICONTROL 提交发布]**。 请参阅[发布缩放图像](publishing-zoom-images.md#publishing_zoom_images)。

## 6.将缩放查看器关联到网页

Dynamic Media Classic会创建缩放图像所需的URL标注字符串，并在您将图像发布到Dynamic Media图像服务器时激活它们。 可以从&#x200B;**[!UICONTROL Preview]**&#x200B;页面复制这些URL字符串。 复制 URL 字符串之后，即可在网站和应用程序上使用。请参阅[将缩放查看器链接到网页](linking-zoom-viewers-web-pages.md#linking_zoom_viewers_to_your_web_pages)。
