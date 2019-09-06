---
title: '"快速入门：调整图像大小"'
seo-title: '"快速入门：调整图像大小"'
description: 'null'
seo-description: “图像大小调整”简介和“快速入门”，可帮助您使用“图像大小调整”技术快速上手和运行。
uuid: 6c ad4b7-549d-4daa-b6 b9-5997a8427 af8
contentOwner: admin
content-type: 引用
products: SG_ EXPERIENCE MANAGER/Dynamic-Media-Scene-7
geptopics: SG_ SCENESELEFERENDER_ PK/categories/image_ sizing
discoiquuid: dcaa9b21-b925-4dbb-865e-7918cdbda50 c
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# 快速入门：调整图像大小{#quick-start-image-sizing}

图像大小调整是指动态媒体经典能够基于单个高分辨率图像创建多个派生图像。您提供单个主图象，而不是手动为网站或应用程序创建多个图像(例如缩略图和放大视图图象)。Dynamic Media Classic可在您请求所有修改的图像时生成所有修改的图像。能根据单个主图像动态提交图像有许多优势：

* 不必手动创建多个不同大小的图像副本。您将一个主图象提供到动态媒体经典，Dynamic Media经典将从主图象生成大小不同的衍生图像。
* 可以快速更改整个网站或应用程序中某图像类型的大小。例如，要更改所有缩略图图像，可修改“缩略图”图像预设。图像预设（类似于宏）是大小和格式属性的集合。可以通过修改“缩略图”图像预设来更改整个网站或应用程序中的所有缩略图图像的大小。
* 不必在任何内容或资源管理系统内部或外部管理主图像和所有各种各样的派生图像。

![您可以创建不同于同一高分辨率主文件的多个派生图像。](/help/assets/is_derivative_sizes_popup.png)

**快速入门**

该调整图像大小快速入门旨在帮助您快速学会如何使用 Scene7 Publishing System 中的调整图像大小技术。按照步骤1-5。每个步骤末尾都有一个交叉引用，如果需要可从中找到更多信息。

**1. 上载主图像**

首先，将主图像上载至 Scene7 Publishing System。对于规模，Dynamic Media经典建议使用在网站或应用程序中使用最大大小的图像。例如，如果希望观众能够缩放图像，请上载长边像素至少为 2000 的图像。Dynamic Media Classic支持许多图像文件格式，但建议使用无损的TIFF和PNG图像。

选择全局导航栏上的“上载”按钮即可将文件从您的计算机上载到 Scene7 Publishing System 的一个文件夹。请参阅[上载主图像](uploading-master-images.md#uploading_master_images)。

**2. 设置图像预设**

像宏一样，图像预设是用某个名称保存的一组预定义大小和格式命令。图像预设控制从Dynamic Media图像服务器传送图像的大小和格式。如果您是公司的管理员，则可以自己设置图像预设。动态媒体经典还附带默认的图像预设，您可以使用它们动态地传送图像。

要创建图像预设（如果您是管理员），请选择“设置”&gt;“应用程序设置”。在“设置”屏幕上，显示“应用程序设置”选项并选择“图像预设”。然后，单击 **添加** 或 **编辑** 以创建图像预设。

您创建的图像预设将添加到“预览”屏幕上的“图像预设”菜单中。您可以在网站和应用程序中使用新图像预设来动态地显示图像。请参阅[设置图像预设](setting-image-presets.md#setting_up_image_presets)。

**3. 预览图像预设**

下一步是预览管理员设置的不同预设大小的图像预设。

To explore Image Presets, click **Setup** &gt; **Image Presets**, and then browse to an Image Preset.

试用不同的图像预设。观察以不同大小将图像动态传送至网站或应用程序后此图像的外观。

请参阅[基于图像预设预览图像资源](previewing-asset.md#previewing_an_image_asset_based_on_its_image_preset)。

**4. 发布主图像**

发布主图像文件有两个主要目的：

* 将主图象发布到动态媒体图像服务器，以便将图像动态传送到您的网站和应用程序。
* 发布会激活URL字符串，以便将图像从Dynamic Media图像服务器调用到您的网站或应用程序。发布后，您可以在网站或应用程序中必要时复制并放置Dynamic Media经典生成的URL。

选择全局导航栏上的“发布”按钮来启动发布。在“发布”屏幕上，选择“开始发布”按钮。请参阅[发布主图像](publishing-master-images.md#publishing_master_images)。

**5. 将 URL 链接至 Web 应用程序**

动态媒体经典为图像创建URL标注字符串。将图像发布到Dynamic Media图像服务器时，URL变为活动状态。可从浏览面板（在中）或“预览”屏幕复制这些 URL 字符串。在复制 URL 字符串之后，便可以在网站和应用程序中使用它们了。用于调整图像大小的 URL 将取代网页代码中对静态图像名称的引用。对于每个要显示的新图像，URL 将引用一个由数据库取代的主图像名称。

由图像预设生成的 URL 字符串包含图像预设的名称。This name is enclosed in dollar signs (`$`). For example, `$thumbnail$` can be the Image Preset designed to show master images at thumbnail size. 请参阅[将 URL 链接至 Web 应用程序](linking-urls-web-application.md#linking_urls_to_your_web_application)。
