---
title: 将选件集推送到Adobe Target Standard/Premium
description: 了解如何从Adobe Dynamic Media Classic将选件集推送到Adobe Target Standard/Premium。
uuid: 8c895a7c-21b4-4d85-8b0b-a3d2a420bf2e
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
discoiquuid: 39a05654-4f66-4f1e-aec5-ebe6d174353f
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 778fd54b-a9e5-40c5-aff1-a156a5c15923
topic: Integrations, Development
level: Experienced
source-git-commit: 5d8b7cb8b4616a998346675d7324b568634698fb
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 0%

---

# 将选件集推送到Adobe Target Standard/Premium {#pushing-offer-sets-to-target}

创建或编辑选件集后，按照以下步骤将其推送到Adobe Target Standard/Premium：

1. 在Test&amp;Target选件集屏幕中，选择 **[!UICONTROL 推送优惠]**.
1. 输入您的客户端代码和登录凭据。
1. 选择 **[!UICONTROL 登录]**.

在转移到Adobe Target Standard/Premium的过程中，前缀 `S7_` 将自动附加到选件名称的开头。 附加此前缀是为了确保您可以在Test&amp;Target选件列表中轻松找到Adobe Dynamic Media Classic选件。 例如，选件显示为 `S7_<name of offer set>_<offer name>`.

Adobe Dynamic Media Classic推入Adobe Target Standard/Premium小组件选件。 您可以使用小组件选件在Adobe Target Standard/Premium之外托管您自己的选件内容。 构件选件类似于Adobe Target Standard/Premium以外托管的标准选件。 它们允许Adobe Target Standard/Premium部署存储在服务器上的选件内容，从而实现更复杂的动态使用。 构件选件可从URL检索内容，缓存并提供该内容约两小时。 小组件提供了一些Adobe Target Standard/Preimium之外的其他产品无法提供的动态内容生成功能。 如果提供选件的mbox包含mbox参数，例如 `mboxProductID` 和 `mbox.offerId`，则 `productId=[PRODUCT_ID]`和 `offerID=[OFFERID]` 将URL参数附加到请求的URL。 这些参数可由小组件选件URL上提供的服务使用，以返回使用mbox中的产品或订单信息的Adobe Target Standard/Premium以外的内容。 也可以通过API访问构件选件，以便在Adobe Target Standard/Premium之外以编程方式创建选件。
