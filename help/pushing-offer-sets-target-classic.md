---
title: 将优惠集推送到Adobe目标经典
seo-title: 将优惠集推送到Adobe目标经典
description: 'null'
seo-description: 了解如何将优惠集推送到Adobe目标Classic。
uuid: 8c895a7c-21b4-4d85-8b0b-a3d2a420bf2e
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_classic_integration
discoiquuid: 39a05654-4f66-4f1e-aec5-ebe6d174353f
translation-type: tm+mt
source-git-commit: a1722c15d3c049f05959d895e85297d47d730872

---


# 将优惠集推送到Adobe目标经典{#pushing-offer-sets-to-adobe-target-classic}

创建或编辑优惠集后，请按照以下步骤将其推送到目标经典：

1. 在“目标经典优惠集”屏幕中，单击“推送优惠”按钮。
1. 输入您的登录凭据。
1. 单击“登录”按钮。

在传输到目标经典时，前缀S7_会自动附加到优惠名称的开始。 附加此前缀，以确保您可以在目标经典优惠列表中轻松找到Dynamic Media Classic优惠。 例如，优惠显示为 S7_&lt;优惠套餐的名称>_&lt;优惠名称>。

SPS推入目标经典构件优惠。 您可以使用构件优惠在目标经典之外托管您自己的优惠内容。 构件优惠与托管在目标经典之外的标准优惠类似。 它们允许目标经典部署存储在服务器上的优惠内容，从而允许更复杂、更动态地使用。 小工具选件从 URL 处检索内容，缓存并提供该内容，时限为两小时左右。构件优惠提供一些动态内容生成功能，而目标经典之外的其他优惠则不提供这些功能。 If the mbox serving the offer contains mbox parameters such as `mboxProductID` and `mbox.offerId`, the `productId=[PRODUCT_ID]`and `offerID=[OFFERID]` URL parameters are appended to the requested URL. 这些参数可由构件优惠URL上的可用服务使用，以返回目标经典之外的内容，该服务使用mbox中的产品或订单信息。 构件优惠还可通过API访问，以编程方式在目标经典之外创建优惠。
