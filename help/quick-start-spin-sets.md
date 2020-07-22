---
title: '"快速入门：旋转集"'
seo-title: '"快速入门：旋转集"'
description: 'null'
seo-description: 旋转集简介和快速开始，帮助您快速入门和运行。
uuid: d0af9db6-cb6f-48f0-89f6-f3ab2da0659f
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/spin_sets
discoiquuid: 282b8e83-b20f-43f7-b9f8-6eebd5b1c5a7
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '757'
ht-degree: 68%

---


# 快速入门：旋转集{#quick-start-spin-sets}

旋转集用于模拟转动物品进行查看时的真实动作。利用旋转集能够从任意角度查看物品，从而获得任意角度的重要视觉详细信息。旋转集会模拟 360 度的查看体验。Dynamic Media经典优惠查看器可以旋转项目的一维旋转集，以及查看器可以旋转和翻转项目的二维旋转集。 此外，用户只需单击几下鼠标即可“自由缩放”并平移任何视图。 通过这种方式，用户能够以特定的视角，更仔细地查看物品。

![旋转集的图像。](/help/assets/spin_set.png)

旋转集也接受图像映射。图像映射是旋转集内的图像上用于显示含文本的变换面板的区域。当用户单击图像映射时，将触发某种操作。例如，将启动网页，供用户了解产品的更多相关信息。为让用户注意到图像映射在旋转集中的使用，当用户将鼠标指针移到图像映射上方时，图像映射自身周围将出现轮廓线。

请参阅[创建图像映射](creating-image-maps.md)。

**快速开始**

此旋转集快速开始旨在借助Dynamic Media经典中的旋转集技术快速启动和运行。 按照步骤 1 到 7 操作。每个步骤的结尾都有到某个主题标题的交叉引用，如需要，可从中找到更多详细信息。

**1. 创建和上载图像**

对于一维旋转集，一个项目至少需要8-12张照片；对于二维旋转集，一个项目至少需要16-24张照片。 拍摄照片时必须间隔一定的角度，以便让人感觉物品正在旋转和翻转。例如，如果某个一维旋转集中有 12 张照片，则每拍一张照片将物品旋转 30 度 (360/12)。

选择全局导航栏上的“上传”按钮，将旋转图像从您的计算机或网络上传到Dynamic Media经典。

请参阅[旋转集图像拍摄指南](creating-spin-set.md#guidelines-for-shooting-spin-set-images)。

**2. 创建旋转集**

要创建旋转集，请单击“构建”按钮，然后选择“旋转集”。在“旋转集大小”对话框中，选择需要的行数和单元格数，然后单击“确定”。随后将图像拖入旋转集屏幕上的网格中。

请参阅[创建旋转集](creating-spin-set.md#creating-a-spin-set)。

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>See <a href="#UnresolvedLink-sc7_spinsets_sp.xml#WS98ca2e6790647c06-245331fc135ab744793-8000">Including Image Maps in Spin Sets</a> to add clickable, hotspot regions, known as Image Maps, to images in a Spin Set. </p>

 -->

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>See also <a href="#UnresolvedLink-sc7_spinsets_sp.xml#WS98ca2e6790647c06229f600f135ab7cc461-8000">Managing InfoPanel content</a>.</p>

 -->

**3. 编辑旋转集**

要编辑某个旋转集，请选择该旋转集的“编辑”变换按钮。“旋转集”屏幕随即打开。添加、删除和更改图像的位置。您可以更改二维旋转集中行的位置。

请参阅[编辑旋转集](creating-spin-set.md#editing-a-spin-set)。

**4. 设置旋转集查看器预设**

管理员可以创建旋转集查看器预设。这些预设决定了旋转集查看器的外观。要设置新的旋转集查看器预设，请在全局导航栏上选择“设置”按钮。在“设置”屏幕上，显示“应用程序设置”选项，然后选择“查看器预设”。

在“查看器预设”屏幕上，选择“添加”菜单，然后在“添加查看器预设”对话框中选择“旋转集查看器”。接下来在“配置查看器”屏幕中选择选项。

请参阅[设置旋转集查看器预设](setting-spin-set-viewer-presets.md#setting-up-spin-set-viewer-presets)。

**5. 预览旋转集**

在浏览面板中选择您的旋转集，然后单击其变换“预览”按钮。在“预览”屏幕上，按住鼠标按钮并向左或向右拖动指针以从视觉上“旋转”项目。

请参阅[预览旋转集](previewing-spin-set.md#previewing-a-spin-set)。

**6. 发布旋转集**

发布旋转集会将其放置在Dynamic Media经典服务器上，以便能够动态地将其交付到您的网站或应用程序。 它还会激活URL字符串，该字符串将旋转集从Dynamic Media图像服务器调用到您的网站或应用程序。

To publish a Spin Set, mark it for publish by selecting the **Mark for Publish** icon beside its name in the Browse Panel. 单击 **全局导** 航栏上的“发布”以启动发布。 On the Publish screen, click **Start Publish**.

请参阅[发布旋转集](publishing-spin-set.md#publishing-a-spin-set)。

**7. 将旋转集链接到网页**

Dynamic Media经典为旋转集创建URL标注字符串，并在发布后将其激活。 可以从“预览”屏幕复制这些 URL。

选择旋转集，然后单击 **预览**。 “预览”屏幕随即打开。选择旋转集查看器预设。然后，单 **击复制URL**。

请参阅[将旋转集链接到网页](linking-spin-set-web-page.md#linking-a-spin-set-to-a-web-page)。
