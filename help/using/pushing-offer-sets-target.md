---
title: 将选件集推送到Adobe Target Standard/Premium
description: 了解如何从Adobe Dynamic Media Classic将选件集推送到Adobe Target Standard/Premium。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 778fd54b-a9e5-40c5-aff1-a156a5c15923
topic: Integrations, Development
level: Experienced
source-git-commit: de6997fda88c4471625242ee9cca59b344cee945
workflow-type: tm+mt
source-wordcount: '287'
ht-degree: 0%

---

# 将选件集推送到Adobe Target Standard/Premium {#pushing-offer-sets-to-target}

创建或编辑选件集后，按照以下步骤将其推送到Adobe Target Standard/Premium：

1. 在Test&amp;Target选件集屏幕中，选择 **[!UICONTROL 推送优惠]**.
1. 输入您的客户端代码和登录凭据。
1. 选择 **[!UICONTROL 登录]**.

在传输到Adobe Target Standard/Premium期间，前缀 `S7_` 自动附加到选件名称的开头。 此前缀旨在确保您可以在Test&amp;Target选件列表中轻松找到Adobe Dynamic Media Classic选件。 例如，选件显示为 `S7_<name of offer set>_<offer name>`.

Adobe Dynamic Media Classic推介Adobe Target Standard/Premium小组件选件。 您可以使用小组件选件在Adobe Target Standard/Premium上托管您自己提供的内容。 构件选件与Adobe Target Standard/Premium托管的标准选件类似。 它们允许Adobe Target Standard/Premium部署存储在服务器上的选件内容，从而实现更复杂的动态使用。 构件选件可从URL检索内容，缓存和提供该内容大约两小时。 小组件提供了一些Adobe Target Standard/Preimium以外的其他产品无法提供的动态内容生成功能。 如果提供选件的mbox包含mbox参数，例如 `mboxProductID` 和 `mbox.offerId`， `productId=[PRODUCT_ID]`和 `offerID=[OFFERID]` 将URL参数附加到请求的URL。 这些参数由在Widget选件URL上可用的服务使用，以返回使用mbox中的产品或订单信息的Adobe Target Standard/Premium以外的内容。 Widget选件也可以通过API访问，因此您可以在Adobe Target Standard/Premium之外以编程方式创建选件。
