---
title: 快速入门：图像集
description: 图像集简介和快速入门，帮助您快速启动和运行Adobe Dynamic Media Classic中的图像集技术。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sets
feature: Dynamic Media Classic,Viewers,Image Sets
role: User
exl-id: 280e7201-84d6-46b1-94bb-0499beca2992
topic: Content Management
level: Beginner
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '671'
ht-degree: 11%

---

# 快速入门：图像集{#quick-start-image-sets}

Adobe Dynamic Media Classic图像集为用户提供了集成的查看体验。 在动态图像集查看器中，用户可以通过选择缩略图图像来查看项目的不同视图。 图像集允许您呈现项目的替代高分辨率视图。

图像集查看器具有缩放工具，可用来仔细查看图像。如果需要，可以将引导式缩放目标和图像映射作为图像集的一部分。 图像集可为用户带来更协调、更详尽的观看体验。

观看[图像和旋转集：Dynamic Imaging](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/556_Image%20&amp;%20Spin%20Sets_converted%20renamed_Dynamic%20Imaging-AVS)训练视频。

在创建图像集时，Adobe建议以下最佳实践并强制实施以下限制：

| 限制类型 | 最佳实践 | 施加的限制 |
| --- | --- | --- |
| 每集的重复资产数 | 无重复项 | 20‡ |
| 每组的最大图像数 | 每组5至10个图像 | 1000 |

‡最佳做法是不要在一个集中拥有重复的资产。 单个资产的限制为20个重复项。 如果为该资产添加其他重复项（在该集中），请求将会产生错误或忽略重复项。

另请参阅[Dynamic Media限制](/help/using/limitations.md)。

以下图像集快速入门旨在让您快速启动并运行Adobe Dynamic Media Classic中的图像集技术。

## 1.上传多个视图和样本的主图像

首先要向图像集上载图像。由于用户可以在图像集查看器中放大图像，因此选择图像时，请确保考虑到了这一点。 确保图像的最大大小至少为2000像素。 Adobe Dynamic Media Classic支持多种图像文件格式，但建议使用无损TIFF、PNG和EPS图像。

在全局导航栏上，选择&#x200B;**[!UICONTROL 上传]**&#x200B;以将文件从您的计算机上传到Adobe Dynamic Media Classic上的文件夹。

查看[准备图像集资源以进行上传](preparing-image-set-assets-upload.md#preparing-image-set-assets-for-upload)和[上传您的文件](uploading-files.md#uploading-your-files)。

## 2.创建图像集

在图像集中，用户在图像集查看器中选择缩略图图像，以便从不同侧面或角度查看图像。

要创建图像集，请在全局导航栏上选择&#x200B;**[!UICONTROL 生成]**，然后选择&#x200B;**[!UICONTROL 图像集]**。 在“图像集”窗口中，将图像拖动到页面上以构成图像集。 根据需要组织、添加和删除图像。

请参阅[创建图像集](creating-image-set.md#creating-an-image-set)。

另请参阅[在图像集中包含缩放目标和图像映射](/help/using/including-zoom-targets-image-maps-image-sets.md)

## 3.根据需要准备图像集查看器预设

管理员可以创建或修改图像集查看器预设。Adobe Dynamic Media Classic为每种富媒体类型提供了默认查看器预设。 使用缩放查看器： **[!UICONTROL 自定义]** > **[!UICONTROL 图像]**&#x200B;或&#x200B;**[!UICONTROL 图像集]**/**[!UICONTROL 多个视图]**&#x200B;预设来查看您的图像集。

您可以在“应用程序设置”屏幕中添加或编辑查看器预设。

请参阅[创建和编辑查看器预设](application-setup.md#adding-and-editing-viewer-presets)。

## 4.预览图像集

在浏览面板中选择图像集，然后选择&#x200B;**[!UICONTROL 预览]**。 在“预览”页面中，选择缩略图图标以在选定的查看器中检查图像集。 可以从“预设”菜单中选择不同的查看器。

请参阅[预览资源](previewing-asset.md#previewing-an-asset)。

## 5. Publish和图像集

发布图像集会将其放置在Adobe Dynamic Media Classic服务器上并激活URL字符串。

>[!NOTE]
>
>如果您在创建和保存图像集时选择了&#x200B;**[!UICONTROL Publish进行保存]**（默认值），则无需执行此步骤。

在“浏览”面板中，选择名称左侧的&#x200B;**[!UICONTROL 标记为Publish]**&#x200B;图标。 然后选择&#x200B;**[!UICONTROL Publish]**。 在发布页面上，选择&#x200B;**[!UICONTROL 提交Publish]**。

查看[Publish文件](publishing-files.md#publishing-files)。

## 6.将图像集链接到您的网站

Adobe Dynamic Media Classic为图像集创建URL调用，并在发布后激活它们。 可以从“预览”屏幕复制这些 URL。

选择图像集，然后选择&#x200B;**[!UICONTROL 预览]**。 现在，选择图像集查看器预设，然后单击&#x200B;**[!UICONTROL 复制URL]**&#x200B;按钮。

请参阅[将图像集链接到网页](linking-image-set-web-page.md#linking-an-image-set-to-a-web-page)。
