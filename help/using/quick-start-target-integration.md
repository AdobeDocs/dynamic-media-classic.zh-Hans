---
title: 快速入门：Adobe Target Standard/Premium集成
description: Adobe Target Standard/Premium简介和快速入门，可帮助您在Adobe Dynamic Media Classic中通过Adobe Target Standard/Premium集成技术快速启动和运行。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_classic_integration
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 4745ace5-7825-468e-8a82-bfbbcf1b0440
topic: Integrations
level: Experienced
source-git-commit: de6997fda88c4471625242ee9cca59b344cee945
workflow-type: tm+mt
source-wordcount: '522'
ht-degree: 0%

---

# 快速入门：Adobe Target Standard/Premium集成{#quick-start-target-integration}

Adobe Target Standard/Premium将控制权直接交到营销人员手中。 这样做有助于快速持续地运行多个A/B和多变量测试，并衡量有效性。 此外，它还可以通过分段、定位和Automated Personalization来提高在线内容的相关性。

通过Adobe Dynamic Media Classic，您可以为Adobe Target Standard/Premium营销活动创建优惠和优惠集。 例如，您可以创建一个选件集，其中包含同一富媒体资产的三个变体。 然后，您可以使用Adobe Target Standard或Premium来确定哪个资源提供了更好的转化提升。 您可以从基本模板或单个图像创建优惠和优惠集。 将选件集推送或保存到Adobe Target Standard/Premium（选件在此与mbox和体验相关联）后，Adobe Target Standard/Premium可以运行营销活动。 这些营销活动可确定网站的哪个变体可能最适合点进和转化。

要更好地自定义动态Adobe Dynamic Media Classic内容，请使用Adobe Target Standard/PremiumHTML选件。 有关详细信息，请参阅[Adobe Target Standard/Premium产品文档](https://experienceleague.adobe.com/zh-hans/docs/target)。

>[!NOTE]
>
>要将Adobe Target Standard/Premium与Adobe Dynamic Media Classic结合使用，需要有效的Adobe Target Standard/Premium帐户。

本快速入门指南旨在帮助您快速启动并运行Adobe Target Standard/PremiumHTML选件集。 请执行步骤 1 到 3。每一步之后，都会交叉引用主题标题，您可以在其中查找更多信息。

## 1.在“应用程序常规设置”页面中输入您的Adobe Target Standard/Premium URL

Adobe Dynamic Media Classic需要您的Adobe Target Standard/Premium URL才能与Adobe Target Standard/Premium集成。 将Adobe Target Standard/Premium URL的部分复制到并包括`.com`，然后在&#x200B;**[!UICONTROL 服务器]**&#x200B;组的&#x200B;**[!UICONTROL Test&amp;Target服务器名称]**&#x200B;文本字段的Adobe Dynamic Media Classic **[!UICONTROL 应用程序常规设置]**&#x200B;页中输入该部分。 请参阅[将Adobe Dynamic Media Classic与Adobe Target Standard/Premium集成](integrating-dmc-with-target.md#integrating-dmc-with-target)。

## 2.创建优惠套餐

使用参数化模板或图像创建选件集。 您可以在“Test&amp;Target选件集”页面上创建HTML选件集。 要打开此页面，请选择您的模板或图像，然后在全局导航栏上，转到&#x200B;**[!UICONTROL 生成]** > **[!UICONTROL Test&amp;Target选件集]**。

要使用模板创建选件，请选择&#x200B;**[!UICONTROL 添加并预览]**。 在添加和预览页面上，更改参数值。

要创建包含图像的选件，请将图像拖入Test&amp;Target选件集页面。 选择&#x200B;**[!UICONTROL 预览]**&#x200B;并为选件集中的图像或所有图像选择一个图像预设。

创建选件集后，请保存该选件集。

请参阅[创建选件集](creating-offer-set.md#creating_an_offer_set)。

## 3.将选件集推送到Adobe Target Standard/Premium

在“Test&amp;Target选件集”页面中，选择&#x200B;**[!UICONTROL 推送选件]**，然后在“Test&amp;Target登录”对话框中输入登录凭据。 查看[将选件集推送到Adobe Target Standard/Premium](pushing-offer-sets-target.md#pushing_offer_sets_to_target)。
