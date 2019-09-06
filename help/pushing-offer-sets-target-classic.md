---
title: 将优惠套餐推送到Adobe Target Classic
seo-title: 将优惠套餐推送到Adobe Target Classic
description: 'null'
seo-description: 了解如何将优惠套餐推送到Adobe Target Classic。
uuid: 8c895a7c-21b4-4d85-8b0b-a3 d420 bf2 e
contentOwner: admin
content-type: 引用
products: SG_ EXPERIENCE MANAGER/Dynamic-Media-Scene-7
geptopics: SG_ SCENESELEFERENDER_ PK/categories/target_ classic_ integration
discoiquuid: 39a05654-4f66-4f1e-aec5-ebis6 d174353 f
translation-type: tm+mt
source-git-commit: a1722c15d3c049f05959d895e85297d47d730872

---


# 将优惠套餐推送到Adobe Target Classic{#pushing-offer-sets-to-adobe-target-classic}

在创建或编辑选件集后，请按照以下步骤将其推送到Target Classic：

1. 在“目标经典选件集”屏幕中，单击“推送选件”按钮。
1. 输入您的登录凭据。
1. 单击“登录”按钮。

在传输到Target Classic期间，前缀S7_会自动附加到选件名称的开头。附加此前缀以确保您可以在Target Classic选件列表中轻松找到Dynamic Media经典选件。例如，优惠显示为 S7_&lt;优惠套餐的名称&gt;_&lt;优惠名称&gt;。

SPS推送进入Target经典构件选件。您可以使用构件选件在Target Classic之外托管选件内容。构件选件类似于在Target Classic之外托管的标准选件。它们允许Target Classic部署存储在服务器上的选件内容，从而允许更复杂和动态的使用。小工具选件从 URL 处检索内容，缓存并提供该内容，时限为两小时左右。构件选件提供了一些在Target Classic之外提供的动态内容生成功能。If the mbox serving the offer contains mbox parameters such as `mboxProductID` and `mbox.offerId`, the `productId=[PRODUCT_ID]`and `offerID=[OFFERID]` URL parameters are appended to the requested URL. 在Widget选件URL提供的服务可使用这些参数返回Target Classic之外使用产品或订单信息的内容。还可通过API访问构件选件，以在Target Classic之外有计划地创建选件。
