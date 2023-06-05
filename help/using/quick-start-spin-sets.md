---
title: "快速入门：旋转集"
description: 介绍和旋转集快速入门，帮助您在Adobe Dynamic Media Classic中快速启动和运行。
uuid: d0af9db6-cb6f-48f0-89f6-f3ab2da0659f
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/spin_sets
discoiquuid: 282b8e83-b20f-43f7-b9f8-6eebd5b1c5a7
feature: Dynamic Media Classic,Viewers,Spin Sets
role: User
exl-id: 26e3cd5b-f070-4b92-af36-25631723460e
source-git-commit: 38d7f8d6e5888e1c5ba9260ada45b79fb16b338f
workflow-type: tm+mt
source-wordcount: '839'
ht-degree: 22%

---

# 快速入门：旋转集{#quick-start-spin-sets}

旋转集用于模拟转动物品进行查看时的真实动作。利用旋转集能够从任意角度查看物品，从而获得任意角度的重要视觉详细信息。旋转集模拟360°观看体验。 Adobe Dynamic Media Classic提供一维旋转集和二维旋转集，前者让查看者可以旋转项目，后者让查看者可以旋转和翻转项目。 此外，用户只需单击几下鼠标，即可“自由变形”缩放和平移任何视图。 通过这种方式，用户能够以特定的视角，更仔细地查看物品。

![旋转集的图像。](/help/using/assets/spin_set.png)

旋转集也接受图像映射。图像映射是旋转集内的图像上用于显示含文本的变换面板的区域。当用户单击图像映射时，将触发某种操作。例如，将启动网页，供用户了解产品的更多相关信息。要指出旋转集中的图像映射，当用户将鼠标指针移动到图像映射本身周围时，会出现一个轮廓。

参见 [创建图像映射](creating-image-maps.md).

参见 [图像和旋转集：Dynamic Imaging](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/556_Image%20&amp;%20Spin%20Sets_converted%20renamed_Dynamic%20Imaging-AVS) 训练视频。

在创建旋转集时，Adobe建议采用以下最佳实践并强制实施以下限制：

| 旋转集限制类型 | 最佳实践 | 施加的限制 |
| --- | --- | --- |
| 每个2D集的最大行数/列数 | 每组12-18个图像 | 1000 |

另请参阅 [Dynamic Media限制](/help/using/limitations.md).

此旋转集快速入门旨在让您快速启动并运行Adobe Dynamic Media Classic中的旋转集技术。 按照步骤 1 到 7 操作。在每个步骤结束时，您可以选择主题链接以了解详情。

## 1.创建和上传图像

对于一维旋转集，至少需要8-12次项目快照；对于二维旋转集，至少需要16-24次项目快照。 拍摄照片时必须间隔一定的角度，以便让人感觉物品正在旋转和翻转。例如，如果一维旋转集包含12个镜头，则每个镜头应将项目旋转30°(360°/12)。

在全局导航栏上，选择 **[!UICONTROL 上传]** 将旋转图像从计算机或网络上传到Adobe Dynamic Media Classic。

请参阅[旋转集图像拍摄指南](creating-spin-set.md#guidelines-for-shooting-spin-set-images)。

## 2.创建旋转集

要创建旋转集，请在全局导航栏上，转到 **[!UICONTROL 生成]** > **[!UICONTROL 旋转集]**. 在“旋转集大小”对话框中，选择要使用的行和单元格数，然后选择 **[!UICONTROL 确定]**. 然后，将图像拖动到“旋转集”页面上的网格中。

参见 [创建旋转集](creating-spin-set.md#creating-a-spin-set).

## 3.编辑旋转集

要编辑旋转集，请在全局导航栏上，转到 **[!UICONTROL 设置]** > **[!UICONTROL 查看器预设]**. 选择一个旋转集，然后选择 **[!UICONTROL 编辑]**. 添加、删除和更改图像的位置。您可以更改二维旋转集中行的位置。

参见 [编辑旋转集](creating-spin-set.md#editing-a-spin-set).

## 4.设置旋转集查看器预设

管理员可以创建旋转集查看器预设。这些预设决定了旋转集查看器的外观。要设置新的旋转集查看器预设，请在全局导航栏上，转到 **[!UICONTROL 设置]** > **[!UICONTROL 查看器预设]**.

在“查看器预设”页面上，选择 **[!UICONTROL 添加]**，然后选择 **[!UICONTROL 旋转集查看器]** 从下拉列表中，然后选择 **[!UICONTROL 添加]**. 在“配置查看器”页中选择选项，然后选择 **[!UICONTROL 保存]**.

参见 [设置旋转集查看器预设](setting-spin-set-viewer-presets.md#setting-up-spin-set-viewer-presets).

## 5.预览旋转集

在浏览面板中选择旋转集，然后选择 **[!UICONTROL 预览]**. 在“预览”页面上，按住鼠标按钮并向左或向右拖动指针以直观地“旋转”项目。

参见 [预览旋转集](previewing-spin-set.md#previewing-a-spin-set).

## 6.发布旋转集

发布旋转集会将它置于Adobe Dynamic Media Classic服务器上，以便动态地将其交付到您的网站或应用程序。 它还激活URL字符串，以便从Dynamic Media图像服务器将旋转集调用到您的网站或应用程序。

要发布旋转集，请通过选择 **[!UICONTROL 标记为发布]** 图标（位于浏览面板中其名称旁边）。 在全局导航栏上，选择 **[!UICONTROL Publish]** 以启动发布。 在“发布”屏幕上，选择 **[!UICONTROL 提交发布]**.

参见 [发布旋转集](publishing-spin-set.md#publishing-a-spin-set).

## 7.将旋转集链接到网页

Adobe Dynamic Media Classic为旋转集创建URL标注字符串，并在发布后激活它们。 您可以从“预览”页面复制这些URL。

选择旋转集，然后选择 **[!UICONTROL 预览]**. 选择旋转集查看器预设。然后选择 **[!UICONTROL 复制URL]**.

参见 [将旋转集链接到网页](linking-spin-set-web-page.md#linking-a-spin-set-to-a-web-page).
