---
title: 将优惠集推送到Adobe Target标准版／高级版
seo-title: 将优惠集推送到Adobe Target标准版／高级版
description: 'null'
seo-description: 了解如何将优惠集推送至Adobe Target标准／高级版。
uuid: 8c895a7c-21b4-4d85-8b0b-a3d2a420bf2e
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
discoiquuid: 39a05654-4f66-4f1e-aec5-ebe6d174353f
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 11%

---


# 将优惠集推送到Adobe Target标准版／高级版 {#pushing-offer-sets-to-target}

创建或编辑优惠集后，请按照以下步骤将其推送到Target Standard/高级：

1. In the Test&amp;Target Offer Set screen, click **[!UICONTROL Push Offers]**.
1. 输入您的客户端代码和登录凭据。
1. 按一下&#x200B;**[!UICONTROL 登入]**。

在传输到Target Standard/高级版时，前缀S7_会自动附加到优惠名称的开始。 附加此前缀可确保您在Test&amp;Dynamic Media优惠列表中轻松找到目标经典优惠。 例如，优惠显示为 S7_&lt;优惠套餐的名称>_&lt;优惠名称>。

Dynamic Media经典推入Target Standard/高级构件优惠。 您可以使用构件优惠在Target Standard/高级版之外托管您自己的优惠内容。 构件优惠类似于托管在Target Standard/Premium外的标准优惠。 它们允许Target Standard/高级版部署存储在您服务器上的优惠内容，从而允许更复杂、更动态地使用。 小工具选件从 URL 处检索内容，缓存并提供该内容，时限为两小时左右。构件优惠提供某些动态内容生成功能，而Target Standard/Premium以外的优惠则不提供这些功能。 If the mbox serving the offer contains mbox parameters such as `mboxProductID` and `mbox.offerId`, the `productId=[PRODUCT_ID]`and `offerID=[OFFERID]` URL parameters are appended to the requested URL. 这些参数可由构件优惠URL中提供的服务使用，以在Target Standard/高级版外返回使用mbox中的产品或订单信息的内容。 构件优惠还可通过API访问，以编程方式在Target Standard/高级版之外创建优惠。
