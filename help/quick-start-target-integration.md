---
title: “快速开始:Target Standard/Premium集成”
description: Adobe Target Standard/Premium的简介和快速开始，可帮助您借助Target Standard/Premium集成技术快速入门和使用。
uuid: d8f79fbf-8be1-44fa-8058-3508060fcd70
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_classic_integration
discoiquuid: f8c25768-cf59-45ec-8193-522404191d57
feature: Dynamic Media Classic
role: 数据工程师，管理员，业务从业者
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '482'
ht-degree: 19%

---


# 快速开始:Adobe Target Standard/Premium集成{#quick-start-target-integration}

Adobe Target Standard/Premium将控制权直接交给营销人员，以便快速、持续地运行多个A/B和多变量测试，衡量有效性，并通过细分、定位和自动个性化提高在线内容的相关性。

Dynamic Media Classic允许您为Target Standard/Premium活动创建优惠和优惠集。 例如，您可以创建一个优惠集，其中包含同一富媒体资产的三种变体。 然后，您可以让Target Standard/Premium确定哪个资产可提供更好的转化率提升。 您可以通过基本模板或各个图像创建优惠和优惠套餐。在将优惠集推送或保存到Adobe Target Standard/Premium(优惠与mbox和体验关联)后，Target Standard/Premium可以运行活动来确定哪种网站变体在点击和转换方面表现最佳。

要更好地自定义动态Dynamic Media Classic内容，请使用Target Standard/Premium HTML优惠。 有关更多信息，请参阅Target Standard/Premium产品文档。

>[!NOTE]
>
>要将Target Standard/Premium与Dynamic Media Classic结合使用，需要有效的Adobe Target Standard/Premium帐户。

**快速开始**

此快速开始旨在帮助您快速设置并运行Target Standard/Premium HTML优惠集。 请执行步骤 1 到 3。每个步骤的后面都有一个交叉引用，可以跳转到相应的主题标题，供您了解更多信息。

**1. 在“应用程序常规设置”屏幕中输入Adobe Target Standard/Premium URL。**

Dynamic Media Classic需要您的Target Standard/Premium URL与Target Standard/Premium集成。 将您的Target Standard/Premium URL的部分复制到&#x200B;*.com*&#x200B;并包括其中，然后在“Dynamic Media Classic Application General Settings”屏幕中输入。 请参阅[将Dynamic Media Classic与Target Standard/Premium](integrating-dmc-with-target.md#integrating-dmc-with-target)集成。

**2.创建优惠套餐**

使用参数化模板或图像来创建优惠套餐。请在“Test&amp;Target 优惠套餐”屏幕上创建 HTML 优惠套餐。要打开此屏幕，请选择模板或图像，然后单击&#x200B;**构建** > **测试和目标优惠集**。

要使用模板创建优惠，请单击&#x200B;**添加和预览**。 在“添加和预览”屏幕上，更改参数值。

要使用图像创建优惠，请将图像拖入“Test&amp;Target 优惠套餐”屏幕。单击&#x200B;**预览**&#x200B;为图像或优惠集中的所有图像选择图像预设。

创建优惠套餐后请将其保存。

请参阅[创建优惠套餐](creating-offer-set.md#creating_an_offer_set)。

**3.将优惠集推送到Adobe Target Standard/Premium**

在“Test&amp;目标优惠集”屏幕中，单击&#x200B;**推送优惠**，然后在“Test&amp;目标登录”对话框中输入登录凭据。 请参阅[将优惠集推送到Target Standard/Premium](pushing-offer-sets-target.md#pushing_offer_sets_to_target)。
