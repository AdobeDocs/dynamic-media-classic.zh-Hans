---
title: 将优惠集推送到Adobe Target标准版／高级版
seo-title: 将优惠集推送到Adobe Target标准版／高级版
description: 'null'
seo-description: 了解如何将优惠集推送到Adobe Target标准版／高级版。
uuid: 8c895a7c-21b4-4d85-8b0b-a3d2a420bf2e
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
discoiquuid: 39a05654-4f66-4f1e-aec5-ebe6d174353f
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 11%

---


# 将优惠集推送到Adobe Target标准版／高级版{#pushing-offer-sets-to-target}

在创建或编辑优惠集后，请按照以下步骤将其推送到Target Standard/Premium:

1. 在Test&amp;目标优惠集屏幕中，单击&#x200B;**[!UICONTROL 推送优惠]**。
1. 输入您的客户端代码和登录凭据。
1. 按一下&#x200B;**[!UICONTROL 登入]**。

在传输到Target Standard/Premium期间，前缀S7_会自动附加到开始优惠名。 附加此前缀可确保在Test&amp;DDynamic Media优惠列表中轻松找到Test&amp;D目标优惠。 例如，优惠显示为 S7_&lt;优惠套餐的名称>_&lt;优惠名称>。

Dynamic Media经典推出Target Standard/Premium构件优惠。 您可以使用构件优惠在Target Standard/Premium外托管您自己的优惠内容。 构件优惠类似于托管在Target Standard/Premium外的标准优惠。 它们允许Target Standard/Premium部署存储在您的服务器上的优惠内容，从而允许更复杂、更动态地使用。 小工具选件从 URL 处检索内容，缓存并提供该内容，时限为两小时左右。构件优惠提供一些Target Standard/Premium外的其他优惠不提供的动态内容生成功能。 如果提供优惠的mbox包含mbox参数，如`mboxProductID`和`mbox.offerId`，则`productId=[PRODUCT_ID]`和`offerID=[OFFERID]` URL参数将附加到所请求的URL。 这些参数可由构件优惠URL中提供的服务使用，以返回Target Standard/Premium外的内容，这些内容使用mbox中的产品或订单信息。 构件优惠还可通过API访问，以在Target Standard/Premium外以编程方式创建优惠。
