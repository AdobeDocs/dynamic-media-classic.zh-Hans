---
title: "快速入门：图像集"
description: 图像集简介和快速入门，帮助您快速使用Adobe Dynamic Media Classic中的图像集技术启动和运行。
uuid: daf17d13-9c06-41f0-8fc5-2e56d460d341
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sets
discoiquuid: 612a425f-2840-46c4-8e5a-c0bc5f738f4e
feature: Dynamic Media Classic,Viewers,Image Sets
role: User
exl-id: 280e7201-84d6-46b1-94bb-0499beca2992
topic: Content Management
level: Beginner
source-git-commit: d82f816553f807b514f4690827dab672a6baf690
workflow-type: tm+mt
source-wordcount: '673'
ht-degree: 21%

---

# 快速入门：图像集{#quick-start-image-sets}

Adobe Dynamic Media Classic图像集为用户提供了集成的查看体验。 在动态图像集查看器中，用户单击缩略图图像便可以看到物品的各种不同视图。图像集允许您呈现项目的替代高分辨率视图。

图像集查看器具有缩放工具，可用来仔细查看图像。如果需要，可以将引导式缩放目标和图像映射添加到图像集中。图像集可为用户带来更协调、更详尽的观看体验。

参见 [图像和旋转集：Dynamic Imaging](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/556_Image%20&amp;%20Spin%20Sets_converted%20renamed_Dynamic%20Imaging-AVS) 训练视频。

创建图像集时，Adobe建议采用以下最佳实践并强制实施以下限制：

| 限制类型 | 最佳实践 | 施加的限制 |
| --- | --- | --- |
| 每集的重复资产数 | 无重复项 | 20 |
| 每组图像的最大数量 | 每组5-10个图像 | 1000 |

另请参阅 [Dynamic Media限制](/help/using/limitations.md).

以下图像集快速入门旨在让您快速使用Adobe Dynamic Media Classic中的图像集技术启动并运行。

## 1.上传多个视图和样本的主图像

首先要向图像集上载图像。由于用户可以在图像集查看器中放大图像，因此选择图像时，请确保考虑到了这一点。 确保图像的最大大小至少为2000像素。 Adobe Dynamic Media Classic支持多种图像文件格式，但建议使用无损TIFF、PNG和EPS图像。

在全局导航栏上，选择 **[!UICONTROL 上传]** 将文件从计算机上传到Adobe Dynamic Media Classic上的某个文件夹。

参见 [准备图像集资源以供上传](preparing-image-set-assets-upload.md#preparing-image-set-assets-for-upload) 和 [上传您的文件](uploading-files.md#uploading-your-files).

## 2.创建图像集

在图像集中，用户在图像集查看器中选择缩略图图像，以便从不同侧面或角度查看图像。

要创建图像集，请在全局导航栏上选择 **[!UICONTROL 生成]**，然后选择 **[!UICONTROL 图像集]**. 在“图像集”窗口中，将图像拖动到页面上以构成图像集。 根据需要组织、添加和删除图像。

参见 [创建图像集](creating-image-set.md#creating-an-image-set).

另请参阅 [在图像集中包括缩放目标和图像映射](/help/using/including-zoom-targets-image-maps-image-sets.md)

## 3.根据需要准备图像集查看器预设

管理员可以创建或修改图像集查看器预设。Adobe Dynamic Media Classic为每种富媒体类型提供了默认的查看器预设。 使用缩放查看器： **[!UICONTROL 自定义]** > **[!UICONTROL 图像]** 或 **[!UICONTROL 图像集]**/**[!UICONTROL 多个视图]** 用于查看图像集的预设。

可在“应用程序设置”屏幕中添加或编辑查看器预设。

参见 [创建和编辑查看器预设](application-setup.md#adding-and-editing-viewer-presets).

## 4.预览图像集

在“浏览”面板中选择图像集，然后选择 **[!UICONTROL 预览]**. 在“预览”页面中，选择缩略图图标以在选定的查看器中检查图像集。 可以从“预设”菜单中选择不同的查看器。

参见 [预览资源](previewing-asset.md#previewing-an-asset).

## 5.发布图像集

发布图像集会将该图像集放置在Adobe Dynamic Media Classic服务器上并激活URL字符串。

>[!NOTE]
>
>如果在创建并保存图像集时选择了“**[!UICONTROL 保存后发布]**”（默认），则不需要执行此步骤。

选择 **[!UICONTROL 标记为发布]** 图标（其名称左侧）。 然后，选择 **[!UICONTROL Publish]**. 在发布页面上，选择 **[!UICONTROL 提交发布]**.

参见 [发布文件](publishing-files.md#publishing-files).

## 6.将图像集链接到您的网站

Adobe Dynamic Media Classic为图像集创建URL调用，并在您发布后激活它们。 可以从“预览”屏幕复制这些 URL。

选择图像集，然后选择 **[!UICONTROL 预览]**. 现在，选择图像集查看器预设，然后选择 **[!UICONTROL 复制URL]**.

参见 [将图像集链接到网页](linking-image-set-web-page.md#linking-an-image-set-to-a-web-page).