---
title: 将优惠集推送到Adobe Target Standard/Premium
description: 了解如何将优惠集推送到Adobe Target Standard/Premium。
uuid: 8c895a7c-21b4-4d85-8b0b-a3d2a420bf2e
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
discoiquuid: 39a05654-4f66-4f1e-aec5-ebe6d174353f
feature: Dynamic Media Classic
role: Data Engineer,Administrator,Business Practitioner
exl-id: 778fd54b-a9e5-40c5-aff1-a156a5c15923
translation-type: tm+mt
source-git-commit: c4e2b8b42b56420269087d0d4f262490464270c0
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 6%

---

# 将优惠集推送到Adobe Target Standard/Premium {#pushing-offer-sets-to-target}

在创建或编辑优惠集后，请按照以下步骤将其推送到Adobe Target Standard/Premium:

1. 在Test&amp;目标优惠集屏幕中，单击&#x200B;**[!UICONTROL 推送优惠]**。
1. 输入您的客户端代码和登录凭据。
1. 按一下&#x200B;**[!UICONTROL 登入]**。

在传输到Adobe Target Standard/Premium期间，前缀`S7_`会自动附加到优惠名称的开始。 附加此前缀是为了确保您可以在Test&amp;目标优惠列表中轻松找到Dynamic Media Classic优惠。 例如，优惠显示为`S7_<name of offer set>_<offer name>`。

Dynamic Media Classic推出Adobe Target Standard/Premium构件优惠。 您可以使用Widget优惠在Adobe Target Standard/Premium之外托管您自己的优惠内容。 构件优惠类似于Adobe Target Standard/Premium外托管的标准优惠。 它们允许Adobe Target Standard/Premium部署存储在您的服务器上的优惠内容，从而允许更复杂、更动态地使用。 小工具选件从 URL 处检索内容，缓存并提供该内容，时限为两小时左右。Widget优惠提供了Adobe Target Standard/Premium外的其他优惠无法提供的一些动态内容生成功能。 如果提供优惠的mbox包含mbox参数，如`mboxProductID`和`mbox.offerId`，则`productId=[PRODUCT_ID]`和`offerID=[OFFERID]` URL参数将附加到所请求的URL。 这些参数可供Widget优惠URL中提供的服务使用，以在Adobe Target Standard/Premium外返回使用mbox中的产品或订单信息的内容。 Widget优惠还可通过API访问，以在Adobe Target Standard/Premium之外有序创建优惠。
