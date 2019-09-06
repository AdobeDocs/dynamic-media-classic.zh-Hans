---
title: “快速入门：目标经典集成”
seo-title: “快速入门：目标经典集成”
description: 'null'
seo-description: Adobe Target Classic简介和快速入门，帮助您使用Target Classic集成技术快速入门和运行。
uuid: d8f79fbf-8be1-44fa-8058-3508060fcd70
contentOwner: admin
content-type: 引用
products: SG_ EXPERIENCE MANAGER/Dynamic-Media-Scene-7
geptopics: SG_ SCENESELEFERENDER_ PK/categories/target_ classic_ integration
discoiquuid: f8c25768-cf59-45ec-8193-522404191d57
translation-type: tm+mt
source-git-commit: a1722c15d3c049f05959d895e85297d47d730872

---


# 快速入门：Target Classic集成{#quick-start-target-classic-integration}

Adobe Target Classic可直接控制营销人员，从而快速、持续地运行多个A/B和多变量测试，衡量有效性并通过细分、定位和自动个性化提高在线内容相关性。

Scene Publishing Systems允许您为Target Classic系列活动创建选件和选件集。例如，您可以创建包含同一富媒体资产的三种变体的优惠套餐。然后，您可以让Target Classic确定哪个资产可提供更好的转化提升。您可以通过基本模板或各个图像创建优惠和优惠套餐。将选件集推送或保存到Adobe Target Classic之后，如果选件与mbox和体验相关联，则Target Classic可运行营销活动以确定网站的哪种变体可能最适于点击率和转化率。

要更好地自定义动态Dynamic Media经典内容，请使用Target经典HTML选件。有关更多信息，请参阅Target Classic产品文档。

>[!NOTE]
>
>使用Scene Publishing System需要有效的Adobe Target Classic帐户才能使用Target Classic。

**快速入门**

此快速入门旨在使用Target经典HTML选件集快速上手和运行。请执行步骤 1 到 3。每个步骤的后面都有一个交叉引用，可以跳转到相应的主题标题，供您了解更多信息。

**1. Enter your Target Classic URL in the Application General Settings screen.**

动态媒体经典需要您的Target经典URL与Target Classic集成。Copy the portion of your Target Classic URL up to and including *.com*, and enter it in the Dynamic Media Classic Application General Settings screen. 请参阅 [将Dynamic Media经典与Target Classic集成](integrating-scene7-target-classic.md#integrating_scene7_with_target_classic)。

**2. 创建优惠套餐**

使用参数化模板或图像来创建优惠套餐。您可以在Target Classic Offer Set屏幕上创建HTML选件集。To open this screen, select your template or images, and click **Build** &gt; **Target Classic Offer Set**.

要使用模板创建选件，请单击 **添加和预览**。在“添加和预览”屏幕上，更改参数值。

要使用图像创建选件，请将图像拖到Target Classic Offer Set屏幕中。Click **Preview** to choose an Image Preset for an image or all the images in the offer set.

创建优惠套餐后请将其保存。

请参阅[创建优惠套餐](creating-offer-set.md#creating_an_offer_set)。

**3. Push the offer set to Target Classic**

In the Target Classic Offer Set screen, click **Push Offers**, and enter your login credentials in the Target Classic Login dialog box. See [Pushing offer sets to Target Classic](pushing-offer-sets-target-classic.md#pushing_offer_sets_to_target_classic).
