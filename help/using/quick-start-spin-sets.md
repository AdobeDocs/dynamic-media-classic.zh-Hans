---
title: 快速入门：旋转集
description: 介绍和旋转集快速入门，帮助您在Adobe Dynamic Media Classic中快速启动和运行。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/spin_sets
feature: Dynamic Media Classic,Viewers,Spin Sets
role: User
exl-id: 26e3cd5b-f070-4b92-af36-25631723460e
topic: Content Management
level: Beginner
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '803'
ht-degree: 22%

---

# 快速入门：旋转集{#quick-start-spin-sets}

旋转集用于模拟转动物品进行查看时的真实动作。利用旋转集能够从任意角度查看物品，从而获得任意角度的重要视觉详细信息。旋转集会模拟 360 度的查看体验。Adobe Dynamic Media Classic提供一维旋转集和二维旋转集，前者让查看者可以旋转项目，后者让查看者可以旋转和翻转项目。 此外，用户只需点击几下鼠标即可“自由变形”缩放和平移任何视图。 通过这种方式，用户能够以特定的视角，更仔细地查看物品。

旋转集的![图像。](/help/using/assets/spin_set.png)

旋转集也接受图像映射。图像映射是旋转集内的图像上用于显示含文本的变换面板的区域。当用户选择图像映射时，将触发某种操作。 例如，启动Web页，以便用户了解有关产品的更多信息。 要指出旋转集中的图像映射，当用户将鼠标指针移到图像映射本身上时，会在图像映射周围显示轮廓。

请参阅[创建图像映射](creating-image-maps.md)。

观看[图像和旋转集： Dynamic Imaging](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/556_Image%20&%20Spin%20Sets_converted%20renamed_Dynamic%20Imaging-AVS)培训视频。

在创建旋转集时，Adobe建议采用以下最佳实践并强制实施以下限制：

| 旋转集限制类型 | 最佳实践 | 施加的限制 |
| --- | --- | --- |
| 每个2D集的最大行/列数 | 每组12-18个图像 | 1000 |

另请参阅[Dynamic Media限制](/help/using/limitations.md)。

此旋转集快速入门旨在让您快速启动并运行Adobe Dynamic Media Classic中的旋转集技术。 按照步骤 1 到 7 操作。在每个步骤结束时，您可以选择主题链接以了解详情。

## 1.创建和上传图像

对于一维旋转集，一个物品最少需要拍摄 8 到 12 张照片，对于二维旋转集，最少需要 16 到 24 张照片。拍摄照片时必须间隔一定的角度，以便让人感觉物品正在旋转和翻转。例如，如果一维旋转集包含12个镜头，则为每个镜头旋转项目30° (360/12)。

在全局导航栏上，选择&#x200B;**[!UICONTROL 上传]**&#x200B;以将旋转图像从您的计算机或网络上传到Adobe Dynamic Media Classic。

请参阅[旋转集图像拍摄指南](creating-spin-set.md#guidelines-for-shooting-spin-set-images)。

## 2.创建旋转集

要创建旋转集，请在全局导航栏上，转到&#x200B;**[!UICONTROL 生成]** > **[!UICONTROL 旋转集]**。 在“旋转集大小”对话框中，选择所需的行和单元格数，然后选择&#x200B;**[!UICONTROL 确定]**。 然后将图像拖动到“旋转集”页面上的网格中。

请参阅[创建旋转集](creating-spin-set.md#creating-a-spin-set)。

## 3.编辑旋转集

若要编辑旋转集，请在全局导航栏上，转到&#x200B;**[!UICONTROL 设置]** > **[!UICONTROL 查看器预设]**。 选择一个旋转集，然后选择&#x200B;**[!UICONTROL 编辑]**。 添加、删除和更改图像的位置。可以更改二维旋转集中行的位置。

请参阅[编辑旋转集](creating-spin-set.md#editing-a-spin-set)。

## 4.设置旋转集查看器预设

管理员可以创建旋转集查看器预设。这些预设决定了旋转集查看器的外观。若要设置新的旋转集查看器预设，请在全局导航栏上，转到&#x200B;**[!UICONTROL 设置]** > **[!UICONTROL 查看器预设]**。

在“查看器预设”页面上，选择&#x200B;**[!UICONTROL 添加]**，然后从下拉列表中选择&#x200B;**[!UICONTROL 旋转集查看器]**，然后选择&#x200B;**[!UICONTROL 添加]**。 在`Configure Viewer`页面中选择选项，然后选择&#x200B;**[!UICONTROL 保存]**。

请参阅[设置旋转集查看器预设](setting-spin-set-viewer-presets.md#setting-up-spin-set-viewer-presets)。

## 5.预览旋转集

在浏览面板中选择旋转集，然后选择&#x200B;**[!UICONTROL 预览]**。 在“预览”页面上，按住鼠标按钮并向左或向右拖动指针以直观地“旋转”项目。

请参阅[预览旋转集](previewing-spin-set.md#previewing-a-spin-set)。

## 6.发布旋转集

发布旋转集会将该旋转集放置在Adobe Dynamic Media Classic服务器上，以便可以动态地将其交付到您的网站或应用程序。 它还激活了URL字符串，该字符串会将Dynamic Media图像服务器中的旋转集调用到您的网站或应用程序。

要发布旋转集，请在“浏览”面板中选择旋转集名称旁边的&#x200B;**[!UICONTROL 标记为发布]**&#x200B;图标，以将其标记为发布。 在全局导航栏上，选择&#x200B;**[!UICONTROL 发布]**&#x200B;以启动发布。 在发布页面上，选择&#x200B;**[!UICONTROL 提交发布]**。

请参阅[发布旋转集](publishing-spin-set.md#publishing-a-spin-set)。

## 7.将旋转集链接到网页

Adobe Dynamic Media Classic为旋转集创建URL标注字符串，并在发布后激活它们。 您可以从预览页面复制这些URL。

选择旋转集，然后选择&#x200B;**[!UICONTROL 预览]**。 选择旋转集查看器预设。然后选择&#x200B;**[!UICONTROL 复制URL]**。

请参阅[将旋转集链接到网页](linking-spin-set-web-page.md#linking-a-spin-set-to-a-web-page)。
