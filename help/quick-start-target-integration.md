---
title: '“快速开始: Target Standard/高级集成”'
seo-title: '“快速开始: Target Standard/高级集成”'
description: 'null'
seo-description: Adobe Target标准版／高级版的简介和快速开始，可帮助您使用Target Standard/高级版集成技术快速入门和使用。
uuid: d8f79fbf-8be1-44fa-8058-3508060fcd70
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_classic_integration
discoiquuid: f8c25768-cf59-45ec-8193-522404191d57
translation-type: tm+mt
source-git-commit: 38f5cf5264f9775a225d354ed9dc2f6caee236f2
workflow-type: tm+mt
source-wordcount: '478'
ht-degree: 19%

---


# 快速开始: Target Standard/高级版集成{#quick-start-target-integration}

Adobe Target标准／高级版将控制权直接交付给营销人员，以便快速、持续地运行多个A/B和多变量测试，衡量有效性，并通过细分、定位和自动个性化提高在线内容的相关性。

Dynamic Media经典允许您为Target Standard/高级活动创建优惠和优惠集。 例如，您可以创建一个优惠集，其中包含同一富媒体资产的三个变体。 然后，您可以让Target Standard/高级版确定哪个资产可提供更好的转化率提升。 您可以通过基本模板或各个图像创建优惠和优惠套餐。在将优惠集推送或保存到Adobe Target标准／高级版(优惠与mbox和体验关联)后，Target Standard/高级版可以运行活动，以确定哪种网站变体最适合点击和转换。

要更好地自定义动态Dynamic Media经典内容，请使用Target Standard/高级HTML优惠。 有关详细信息，请参阅Target Standard/高级产品文档。

>[!NOTE]
>
>要将Adobe Target/高级帐户与Target Standard经典结合使用，必须具有有效的Dynamic Media标准／高级帐户。

**快速开始**

此快速开始旨在帮助您快速设置和运行Target Standard/高级HTML优惠集。 请执行步骤 1 到 3。每个步骤的后面都有一个交叉引用，可以跳转到相应的主题标题，供您了解更多信息。

**1. Enter your Target Standard/Premium URL in the Application General Settings screen.**

Dynamic Media经典需要您的Target Standard/高级URL与Target Standard/高级集成。 Copy the portion of your Target Standard/Premium URL up to and including *.com*, and enter it in the Dynamic Media Classic Application General Settings screen. 请参 [阅将Dynamic Media经典与Target Standard/高级集成](integrating-dmc-with-target.md#integrating-dmc-with-target)。

**2. 创建优惠套餐**

使用参数化模板或图像来创建优惠套餐。请在“Test&amp;Target 优惠套餐”屏幕上创建 HTML 优惠套餐。To open this screen, select your template or images, and click **Build** > **Test&amp;Target Offer Set**.

要创建带有模板的优惠，请单 **击添加和预览**。 在“添加和预览”屏幕上，更改参数值。

要使用图像创建优惠，请将图像拖入“Test&amp;Target 优惠套餐”屏幕。Click **Preview** to choose an Image Preset for an image or all the images in the offer set.

创建优惠套餐后请将其保存。

请参阅[创建优惠套餐](creating-offer-set.md#creating_an_offer_set)。

**3. 将优惠集推送到Target Standard/高级**

In the Test&amp;Target Offer Set screen, click **Push Offers**, and enter your login credentials in the Test&amp;Target Login dialog box. 请参 [阅将优惠集推送到Target Standard/高级](pushing-offer-sets-target.md#pushing_offer_sets_to_target)。
