---
title: “快速入门：混合媒体集”
description: 混合媒体集简介和快速入门，帮助您在Adobe Dynamic Media Classic中快速启动和运行。
uuid: 0ef033d5-b053-4d7c-b1e1-1980f899fd88
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/mixed_media_sets
discoiquuid: 2708d077-94fc-4045-8992-ad3589ed9cfd
feature: Dynamic Media Classic,Viewers,Mixed Media Sets
role: User
exl-id: 757893ae-7507-42a0-a67b-f6542e7231c7
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '701'
ht-degree: 34%

---

# 快速入门：混合媒体集{#quick-start-mixed-media-sets}

 混合媒体集为用户提供了集成的查看体验。混合媒体集可以包括图像、图像集、样本集、旋转集和视频。用户可以选择混合媒体查看器中的不同选项卡，以查看不同查看器中的项目。 如果未指定选项卡，所有资源都将一起显示在样本行中。

“混合媒体集查看器预设”包括最终用户用来嵌入代码、复制 URL 以及链接到主网站的社区选项。用户可以使用这些选项在其个人网站或社交网站上共享有关产品的信息。

此混合媒体集快速入门旨在通过Adobe Dynamic Media Classic中的混合媒体集技术让您快速启动并运行。

## 1.上传图像、样本文件和视频

首先为混合媒体集上载图像、样本文件和视频。由于用户可以在混合媒体集查看器中放大图像，因此选择图像时，请确保考虑到了这一点。 确保图像的最大大小至少为2000像素。

在全局导航栏上，选择 **[!UICONTROL 上传]** 将文件从计算机上传到Adobe Dynamic Media Classic上的某个文件夹。

参见 [上传您的文件](uploading-files.md#uploading-your-files).

## 2.创建在混合媒体集中使用的媒体集

可以将图像、图像集、样本集、旋转集和视频添加到混合媒体集中。先准备好媒体集，然后再将其添加到混合媒体集中。

参见 [创建图像集](creating-image-set.md#creating-an-image-set)， [创建样本集](creating-swatch-set.md#creating-a-swatch-set)、和 [创建旋转集](creating-spin-set.md#creating-a-spin-set).

## 3.创建混合媒体集

在全局导航栏上，转到 **[!UICONTROL 生成]** > **[!UICONTROL 混合媒体集]**. 将图像、样本集、图像集和视频拖动到“混合媒体集”页面。 要添加音轨，将音频文件拖动到“音轨”框中。

参见 [创建混合媒体集](creating-mixed-media-set.md#creating-a-mixed-media-set).

## 4.设置混合媒体查看器预设

Adobe Dynamic Media Classic为混合媒体集提供了默认查看器预设。 管理员可以创建或修改混合媒体集查看器预设。

设置混合媒体集查看器预设时，为集中的所有其他资产添加查看器预设。 例如，如果混合媒体集包括视频，则在混合媒体查看器预设中添加视频查看器预设。也可以将音轨添加到查看器中。该音轨在查看器打开时播放，但在视频处于活动状态时不播放。

参见 [设置混合媒体集查看器预设](setting-mixed-media-set-viewer.md#setting-up-a-mixed-media-set-viewer-preset) 和 [创建和编辑查看器预设](application-setup.md#adding-and-editing-viewer-presets).

另请参阅 [查看器预设](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/550_viewer-presets_converted%20renamed_Done-AVS) 训练视频。

## 5.预览混合媒体集

选择混合媒体集的 **[!UICONTROL 预览]** 按钮。 您可以选择缩略图和样本图标以在混合媒体集查看器中检查混合媒体集。 可以从“预设”菜单中选择不同的查看器。

参见 [预览资源](previewing-asset.md#previewing-an-asset).

## 6.发布混合媒体集

发布混合媒体集会将其放在Adobe Dynamic Media Classic服务器上并激活URL字符串。

混合媒体集要求同时发布到&#x200B;**视频服务器**&#x200B;和&#x200B;**图像服务器**。使用&#x200B;**视频服务器**&#x200B;发布已标记为发布的实际视频。并且，您使用 **图像服务器** 发布相关资产（如视频缩略图），并为任何自适应视频集设置信息。

参见 [发布混合媒体集](publishing-mixed-media-set.md#publishing-a-mixed-media-set).

## 7.将混合媒体集链接到网页

在发布混合媒体集后，Adobe Dynamic Media Classic会为其激活URL调用。 您可以从“预览”页面复制这些URL。

选择混合媒体集，然后选择 **[!UICONTROL 预览]**. 在“预览”页面中，选择一个混合媒体集查看器预设，然后选择 **[!UICONTROL 复制URL]**. 请参阅[将混合媒体集与网页链接](linking-mixed-media-set-web.md#linking-a-mixed-media-set-to-a-web-page)。
