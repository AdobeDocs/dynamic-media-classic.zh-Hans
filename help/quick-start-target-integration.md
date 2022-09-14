---
title: “快速入门：Adobe Target Standard/Premium集成”
description: Adobe Target Standard/Premium的简介和快速入门，可帮助您快速启动并运行Adobe Dynamic Media Classic中的Adobe Target Standard/Premium集成技术。
uuid: d8f79fbf-8be1-44fa-8058-3508060fcd70
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_classic_integration
discoiquuid: f8c25768-cf59-45ec-8193-522404191d57
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 4745ace5-7825-468e-8a82-bfbbcf1b0440
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '515'
ht-degree: 7%

---

# 快速入门：Adobe Target Standard/Premium集成{#quick-start-target-integration}

Adobe Target Standard/Premium将控制权直接交由营销人员掌握，以便快速持续地运行多个A/B和多变量测试，衡量有效性，并通过分段、定位和Automated Personalization提高在线内容的相关性。

Adobe Dynamic Media Classic允许您为Adobe Target Standard/Premium促销活动创建选件和选件集。 例如，您可以创建一个选件集，其中包含同一富媒体资产的三个变体。 然后，您可以让Adobe Target Standard/Premium确定哪种资产可提供更好的转化提升度。 您可以通过基本模板或各个图像创建优惠和优惠套餐。将选件集推送或保存到Adobe Target Standard/Premium（选件与mbox和体验关联）后，Adobe Target Standard/Premium可以运行营销活动。 这些促销活动确定哪个网站变体对点进次数和转化效果最佳。

要更好地自定义动态Adobe Dynamic Media Classic内容，请使用Adobe Target Standard/PremiumHTML选件。 请参阅 [Adobe Target Standard/Premium产品文档](https://experienceleague.adobe.com/docs/target.html) 以了解更多信息。

>[!NOTE]
>
>要将Adobe Target Standard/Premium与Adobe Dynamic Media Classic结合使用，需要拥有有效的Adobe Target Standard/Premium帐户。

此快速入门旨在帮助您快速启动和运行Adobe Target Standard/PremiumHTML选件集。 请执行步骤 1 到 3。在每个步骤之后，都会有一个对主题标题的交叉引用，您可以在该标题中找到更多信息。

## 1.在“应用程序常规设置”页面中输入Adobe Target Standard/Premium URL

Adobe Dynamic Media Classic需要您的Adobe Target Standard/Premium URL才能与Adobe Target Standard/Premium集成。 将Adobe Target Standard/Premium URL的部分复制到（包括） `.com`，并在Adobe Dynamic Media Classic中输入 **[!UICONTROL 应用程序常规设置]** 页面，在 **[!UICONTROL 服务器]** 组， **[!UICONTROL Test&amp;Target服务器名称]** 文本。 请参阅 [将Adobe Dynamic Media Classic与Adobe Target Standard/Premium集成](integrating-dmc-with-target.md#integrating-dmc-with-target).

## 2.创建选件集

使用参数化模板或图像来创建优惠套餐。您可以在“Test&amp;Target选件集”页面上创建HTML选件集。 要打开此页面，请选择您的模板或图像，然后在全局导航栏中，转到 **[!UICONTROL 生成]** > **[!UICONTROL Test&amp;Target选件集]**.

要使用模板创建选件，请选择 **[!UICONTROL 添加和预览]**. 在“添加并预览”页面上，更改参数值。

要创建包含图像的选件，请将图像拖到Test&amp;Target选件集页面中。 选择 **[!UICONTROL 预览]** ，然后为图像或选件集中的所有图像选择图像预设。

创建优惠套餐后请将其保存。

请参阅 [创建选件集](creating-offer-set.md#creating_an_offer_set).

## 3.将选件集推送到Adobe Target Standard/Premium

在Test&amp;Target选件集页面中，选择 **[!UICONTROL 推送选件]**，然后在Test&amp;Target登录对话框中输入登录凭据。 请参阅 [将选件集推送到Adobe Target Standard/Premium](pushing-offer-sets-target.md#pushing_offer_sets_to_target).
