---
title: '"快速入门：调整图像大小"'
description: 图像大小调整的简介和快速入门可帮助您快速启动和运行图像大小调整技术。
uuid: 6c4ad4b7-549d-4daa-b6b9-5997a8427af8
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
discoiquuid: dcaa9b21-b925-4dbb-865e-7918cdbda50c
feature: Dynamic Media Classic，Asset Management
role: User
exl-id: f1d46f03-57a1-43d8-a0ee-74b92b590736
source-git-commit: df689ff5a127bfbc400ca5331168d1ff7bb0b42e
workflow-type: tm+mt
source-wordcount: '844'
ht-degree: 37%

---

# 快速入门：调整图像大小{#quick-start-image-sizing}

图像大小调整是指Dynamic Media Classic根据单个高分辨率图像创建多个派生图像的功能。 您不必为网站或应用程序手动创建多个图像（例如缩略图和放大视图图像），而是提供单个主控图像。 Dynamic Media Classic会按照您的请求生成所有修改的图像。 能根据单个主图像动态提交图像有许多优势：

* 不必手动创建多个不同大小的图像副本。您向Dynamic Media Classic提供一个主控图像，而Dynamic Media Classic则会从该主控图像生成不同大小的派生项。
* 可以快速更改整个网站或应用程序中某图像类型的大小。例如，要更改所有缩略图图像，可修改“缩略图”图像预设。图像预设（类似于宏）是大小和格式属性的集合。可以通过修改“缩略图”图像预设来更改整个网站或应用程序中的所有缩略图图像的大小。
* 您无需在内部或外部管理任何内容或资产管理系统中的主页和所有各种派生项。

![您可以创建多个不同大小的衍生图像，这些图像与同一高分辨率主控文件不同。](/help/assets/is_derivative_sizes_popup.png)

此图像大小调整快速入门旨在帮助您快速启动和运行Dynamic Media Classic中的图像大小调整技术。 按照步骤1-5操作。 每个步骤末尾都有一个交叉引用，如果需要可从中找到更多信息。

## 1.上传主控图像

首先，将主控图像上传到Dynamic Media Classic。 至于大小，Dynamic Media Classic建议使用您预计在网站或应用程序中使用的最大大小的图像。 例如，如果您希望查看者缩放图像，请上传至少2000像素的最大大小图像。 Dynamic Media Classic支持多种图像文件格式，但建议使用无损的TIFF和PNG图像。

在全局导航栏上，单击&#x200B;**[!UICONTROL Upload]** ，将文件从计算机上传到Dynamic Media Classic上的文件夹。 请参阅[上载主图像](uploading-master-images.md#uploading_master_images)。

## 2.设置图像预设

像宏一样，图像预设是用某个名称保存的一组预定义大小和格式命令。图像预设可控制从Dynamic Media图像服务器传送图像的大小和格式。 如果您是公司的管理员，则可以自己设置图像预设。Dynamic Media Classic还附带默认的图像预设，您可以使用这些预设动态传送图像。

要创建图像预设（如果您是管理员），请在全局导航栏中单击&#x200B;**[!UICONTROL 设置]** > **[!UICONTROL 应用程序设置]** > **[!UICONTROL 图像预设]**。 然后，单击&#x200B;**[!UICONTROL 添加]**&#x200B;以创建图像预设，或单击&#x200B;**[!UICONTROL 编辑]**&#x200B;以更改现有的图像预设。

您创建的图像预设将添加到预览页面的图像预设菜单。 您可以在网站和应用程序中使用新图像预设来动态地显示图像。请参阅[设置图像预设](setting-image-presets.md#setting_up_image_presets)。

## 3.预览图像预设

下一步是预览管理员设置的不同预设大小的图像预设。

要浏览图像预设，请在全局导航栏中单击&#x200B;**[!UICONTROL 设置]** > **[!UICONTROL 图像预设]**，然后浏览到图像预设。

试用不同的图像预设。了解以不同大小将图像动态传送到网站或应用程序时图像的显示方式。

请参阅[基于图像预设预览图像资源](previewing-asset.md#previewing_an_image_asset_based_on_its_image_preset)。

## 4.发布主控图像

发布主图像文件有两个主要目的：

* 将您的主控图像发布到Dynamic Media图像服务器，以便能够将图像动态交付到您的网站和应用程序。
* 发布可激活URL字符串，以便将图像从Dynamic Media图像服务器调用到您的网站或应用程序。 发布后，您可以根据需要复制并放置Dynamic Media Classic生成的URL，以包含在您的网站或应用程序中。

在全局导航栏上，单击&#x200B;**[!UICONTROL Publish]**&#x200B;以开始发布作业。 在“发布”对话框中，单击&#x200B;**[!UICONTROL 提交发布]**。 请参阅[发布主图像](publishing-master-images.md#publishing_master_images)。

## 5.将URL关联到您的Web应用程序

Dynamic Media Classic为图像创建URL标注字符串。 将图像发布到Dynamic Media图像服务器时，URL会变为活动状态。 可从浏览面板（在中）或“预览”屏幕复制这些 URL 字符串。在复制 URL 字符串之后，便可以在网站和应用程序中使用它们了。用于调整图像大小的 URL 将取代网页代码中对静态图像名称的引用。对于每个要显示的新图像，URL 将引用一个由数据库取代的主图像名称。

由图像预设生成的 URL 字符串包含图像预设的名称。此名称用美元符号(`$`)括起来。 例如，`$thumbnail$`可以是图像预设，设计为以缩略图大小显示主控图像。 请参阅[将 URL 链接至 Web 应用程序](linking-urls-web-application.md#linking_urls_to_your_web_application)。
