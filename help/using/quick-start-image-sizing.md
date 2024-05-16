---
title: “快速入门：调整图像大小”
description: 图像大小调整简介和快速入门，帮助您快速启动并运行Adobe Dynamic Media Classic中的图像大小调整技术。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
feature: Dynamic Media Classic,Asset Management
role: User
topic: Content Management
level: Beginner
exl-id: f1d46f03-57a1-43d8-a0ee-74b92b590736
source-git-commit: ad7e20fdbe9028c6255865cce95d109f9e9eeab2
workflow-type: tm+mt
source-wordcount: '873'
ht-degree: 6%

---

# 快速入门：调整图像大小{#quick-start-image-sizing}

图像大小调整是指Adobe Dynamic Media Classic根据单个高分辨率图像创建多个派生图像的功能。 您无需为网站或应用程序手动创建多个图像（例如，缩略图和放大的视图图像），而是提供单个主图像。 Adobe Dynamic Media Classic会生成您请求的所有修改后的图像。 能够从单个主映像动态投放映像有许多优点：

* 无需手动创建多个不同大小的映像副本。 您向Adobe Dynamic Media Classic提供一个主映像，Adobe Dynamic Media Classic会从主映像生成不同大小的派生项。
* 您可以在整个网站或应用程序中快速更改图像类型的大小。 例如，要更改所有缩略图图像，您可以修改“缩略图”图像预设。 图像预设 — 它类似于宏 — 是大小和格式属性的集合。 您可以修改“缩略图”图像预设，以更改整个网站或应用程序中的所有缩略图图像的大小。
* 您无需在内部或外部管理您的任何内容或资产管理系统中的主文件和所有各种衍生工具。

![您可以根据同一高分辨率主文件创建大小不同的多个派生图像。](/help/using/assets/is_derivative_sizes_popup.png)

请参阅 [图像大小：Dynamic Imaging](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/557_Image%20Sizing_converted%20renamed_Dynamic%20Imaging-AVS) 训练视频。

以下图像大小快速入门旨在帮助您快速启动并运行Adobe Dynamic Media Classic中的图像大小调整技术。 执行步骤1-5。 在每个步骤之后，都有一个交叉引用，您可以在其中查找所需的更多信息。

## 1.上传主图像

首先，将您的主图像上传到Adobe Dynamic Media Classic。 关于大小，Adobe Dynamic Media Classic建议使用您希望在网站或应用程序上使用的最大大小的图像。 例如，如果您希望查看器缩放图像，请上传最大大小至少为2000像素的图像。 Adobe Dynamic Media Classic支持多种图像文件格式，但建议使用无损TIFF和PNG图像。

在全局导航栏上，选择 **[!UICONTROL 上传]** 将文件从计算机上传到Adobe Dynamic Media Classic上的某个文件夹。 请参阅 [上传主图像](uploading-master-images.md#uploading_master_images).

## 2.设置图像预设

像宏一样，图像预设是用某个名称保存的一组预定义大小和格式命令。图像预设可控制从Dynamic Media图像服务器传送图像的大小和格式。 如果您拥有公司管理员状态，则可以自行设置图像预设。 您可以使用已随Adobe Dynamic Media Classic提供的默认图像预设动态交付图像。

要创建图像预设（如果您是管理员），请在全局导航栏上，转到 **[!UICONTROL 设置]** > **[!UICONTROL 应用程序设置]** > **[!UICONTROL 图像预设]**. 然后选择 **[!UICONTROL 添加]** 以创建图像预设，或选择 **[!UICONTROL 编辑]** 以更改现有的图像预设。

您创建的图像预设会添加到“预览”页面上的“图像预设”菜单中。 您可以使用新的图像预设在网站和应用程序上动态显示图像。 请参阅 [设置图像预设](setting-image-presets.md#setting_up_image_presets).

## 3.预览图像预设

下一步是预览管理员设置的不同预设大小的图像预设。

要浏览图像预设，请在全局导航栏上，转到 **[!UICONTROL 设置]** > **[!UICONTROL 图像预设]**，然后浏览到图像预设。

试用不同的图像预设。了解图像以不同大小动态传送到您的网站或应用程序时的显示方式。

请参阅 [预览基于其图像预设的图像资源](previewing-asset.md#previewing_an_image_asset_based_on_its_image_preset).

## 4.发布主图像

发布主图像文件有两个基本目的：

* 将您的主图像发布到Dynamic Media图像服务器，以便可以将图像动态传送到您的网站和应用程序。
* 发布会激活URL字符串，以便将图像从Dynamic Media图像服务器调用到您的网站或应用程序。 发布后，您可以根据需要将Adobe Dynamic Media Classic生成的URL复制并放置在网站或应用程序中。

在全局导航栏上，选择 **[!UICONTROL Publish]** 以启动发布作业。 在发布对话框中，选择 **[!UICONTROL 提交发布]**. 请参阅 [发布主图像](publishing-master-images.md#publishing_master_images).

## 5.将URL链接到您的Web应用程序

Adobe Dynamic Media Classic为图像创建URL标注字符串。 在将图像发布到Dynamic Media图像服务器时，URL会变为活动状态。 您可以从“浏览”面板（在“详细信息视图”中）或“预览”屏幕复制这些URL字符串。 复制URL字符串后，您可以在网站和应用程序中使用它们。 用于调整图像大小的URL将替换网页代码中对静态图像名称的引用。 URL引用了数据库为要显示的每个新图像替换的主图像名称。

由图像预设生成的 URL 字符串包含图像预设的名称。这个名称用美元符号括起来(`$`)。 例如， `$thumbnail$` 可以是旨在以缩略图大小显示主图像的图像预设。 请参阅 [将URL链接到您的Web应用程序](linking-urls-web-application.md#linking_urls_to_your_web_application).
