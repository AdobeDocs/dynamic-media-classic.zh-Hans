---
title: '"快速入门：旋转集"'
description: 旋转集简介和快速入门可帮助您在Adobe Dynamic Media Classic中快速启动并运行。
uuid: d0af9db6-cb6f-48f0-89f6-f3ab2da0659f
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/spin_sets
discoiquuid: 282b8e83-b20f-43f7-b9f8-6eebd5b1c5a7
feature: Dynamic Media Classic,Viewers,Spin Sets
role: User
exl-id: 26e3cd5b-f070-4b92-af36-25631723460e
source-git-commit: 352b1c383195fa03294ad3501207d63f3cfe3e42
workflow-type: tm+mt
source-wordcount: '796'
ht-degree: 23%

---

# 快速入门：旋转集{#quick-start-spin-sets}

旋转集用于模拟转动物品进行查看时的真实动作。利用旋转集能够从任意角度查看物品，从而获得任意角度的重要视觉详细信息。旋转集模拟360°的查看体验。 Adobe Dynamic Media Classic提供了一维旋转集（查看者可在其中旋转项目）和二维旋转集（查看者可在其中旋转和翻转项目）。 此外，用户只需单击几下鼠标即可“自由”缩放和平移任何视图。 通过这种方式，用户能够以特定的视角，更仔细地查看物品。

![旋转集的图像。](/help/assets/spin_set.png)

旋转集也接受图像映射。图像映射是旋转集内的图像上用于显示含文本的变换面板的区域。当用户单击图像映射时，将触发某种操作。例如，将启动网页，供用户了解产品的更多相关信息。要指出旋转集中的图像映射，当用户将鼠标指针移动到图像映射上时，图像映射本身周围会显示一个轮廓。

请参阅[创建图像映射](creating-image-maps.md)。

请参阅[图像和旋转集：Dynamic Imaging](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/556_Image%20&amp;%20Spin%20Sets_converted%20renamed_Dynamic%20Imaging-AVS)培训视频。

此旋转集快速入门旨在通过Adobe Dynamic Media Classic中的旋转集技术帮助您快速启动并运行。 按照步骤 1 到 7 操作。在每个步骤的末尾，您可以选择主题链接以了解更多信息。

## 1.创建和上传图像

对于一维旋转集，您至少需要一个项目8-12张拍照；对于二维旋转集，您至少需要16-24张拍照。 拍摄照片时必须间隔一定的角度，以便让人感觉物品正在旋转和翻转。例如，如果一维旋转集包含12张照片，则对每张照片旋转项目30°(360°/12)。

在全局导航栏上，选择&#x200B;**[!UICONTROL Upload]** ，将旋转图像从计算机或网络上传到Adobe Dynamic Media Classic。

请参阅[旋转集图像拍摄指南](creating-spin-set.md#guidelines-for-shooting-spin-set-images)。

## 2.创建旋转集

要创建旋转集，请在全局导航栏上，转到&#x200B;**[!UICONTROL Build]** > **[!UICONTROL Spin Sets]**。 在“旋转集大小”对话框中，选择所需的行和单元格数，然后选择&#x200B;**[!UICONTROL 确定]**。 然后，将图像拖到旋转集页面的网格中。

请参阅[创建旋转集](creating-spin-set.md#creating-a-spin-set)。

## 3.编辑旋转集

要编辑旋转集，请在全局导航栏上，转到&#x200B;**[!UICONTROL Setup]** > **[!UICONTROL 查看器预设]**。 选择旋转集，然后选择&#x200B;**[!UICONTROL 编辑]**。 添加、删除和更改图像的位置。您可以更改二维旋转集中行的位置。

请参阅[编辑旋转集](creating-spin-set.md#editing-a-spin-set)。

## 4.设置旋转集查看器预设

管理员可以创建旋转集查看器预设。这些预设决定了旋转集查看器的外观。要设置新的旋转集查看器预设，请在全局导航栏中，转到&#x200B;**[!UICONTROL Setup]** > **[!UICONTROL 查看器预设]**。

在“查看器预设”页面上，选择&#x200B;**[!UICONTROL 添加]**，然后从下拉列表中选择&#x200B;**[!UICONTROL 旋转集查看器]**，然后选择&#x200B;**[!UICONTROL 添加]**。 在“配置查看器”页面中选择选项，然后选择&#x200B;**[!UICONTROL 保存]**。

请参阅[设置旋转集查看器预设](setting-spin-set-viewer-presets.md#setting-up-spin-set-viewer-presets)。

## 5.预览旋转集

在浏览面板中选择旋转集，然后选择&#x200B;**[!UICONTROL 预览]**。 在“预览”页面上，按住鼠标按钮并向左或向右拖动指针，以可视方式“旋转”项目。

请参阅[预览旋转集](previewing-spin-set.md#previewing-a-spin-set)。

## 6.发布旋转集

发布旋转集会将其放置在Adobe Dynamic Media Classic服务器上，以便能够将其动态交付到您的网站或应用程序。 它还会激活URL字符串，以将旋转集从Dynamic Media图像服务器调用到您的网站或应用程序。

要发布旋转集，请在浏览面板中选择旋转集名称旁边的&#x200B;**[!UICONTROL 标记为发布]**&#x200B;图标，以将其标记为发布。 在全局导航栏上，选择&#x200B;**[!UICONTROL Publish]**&#x200B;以启动发布。 在“发布”屏幕上，选择&#x200B;**[!UICONTROL 提交发布]**。

请参阅[发布旋转集](publishing-spin-set.md#publishing-a-spin-set)。

## 7.将旋转集关联到网页

Adobe Dynamic Media Classic会为旋转集创建URL标注字符串，并在您发布它们后将其激活。 您可以从预览页面复制这些URL。

选择旋转集，然后选择&#x200B;**[!UICONTROL 预览]**。 选择旋转集查看器预设。然后选择&#x200B;**[!UICONTROL 复制URL]**。

请参阅[将旋转集关联到网页](linking-spin-set-web-page.md#linking-a-spin-set-to-a-web-page)。
