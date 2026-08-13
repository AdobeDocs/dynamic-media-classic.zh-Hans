---
title: 将选件集推送到Adobe Target Standard/Premium
description: 了解如何从Adobe Dynamic Media Classic将选件集推送到Adobe Target Standard/Premium。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
feature: Dynamic Media Classic
role: Developer,Admin,User
exl-id: 778fd54b-a9e5-40c5-aff1-a156a5c15923
topic: Integrations, Development
level: Experienced
autotag-review: '2026-05-13T19:55:22.850Z'
TQID: 'https://experienceleague.adobe.com/8j9sRn1zhAhgj-wMV6hYix1F9aARZjDUiFZofcVVcBw'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
level_v2:
  - id: d378ca77-2da1-4f39-ad92-1917fe974a38
source-git-commit: 8a9d304ced3a218ae6393961a278f5ab9581c229
workflow-type: tm+mt
source-wordcount: 283
ht-degree: 0%

---

# 将选件集推送到Adobe Target Standard/Premium {#pushing-offer-sets-to-target}

创建或编辑选件集后，按照以下步骤将其推送到Adobe Target Standard/Premium：

1. 在Test &amp; Target选件集屏幕中，选择&#x200B;**[!UICONTROL 推送选件]**。
1. 输入您的客户端代码和登录凭据。
1. 选择&#x200B;**[!UICONTROL 登录]**。

在传输到Adobe Target Standard/Premium期间，前缀`S7_`会自动添加到选件名称的开头。 添加前缀是为了确保您可以在Test &amp; Target选件列表中轻松找到Adobe Dynamic Media Classic选件。 例如，选件显示为`S7_<name of offer set>_<offer name>`。

Adobe Dynamic Media Classic将小组件优惠推送到Adobe Target Standard/Premium。 您可以使用小组件选件在Adobe Target Standard/Premium上托管提供的内容。 小组件选件可与Adobe Target Standard/Premium托管的标准选件相比。 它们允许Adobe Target Standard/Premium部署存储在您服务器上的选件内容，从而实现更复杂、更动态的使用。 小组件提供从URL检索内容、缓存和提供该内容两个小时的功能。 小组件提供了一些Adobe Target Standard/Premium以外的其他产品无法提供的动态内容生成功能。 如果提供优惠的mbox包含mbox参数（如`mboxProductID`和`mbox.offerId`），则`productId=[PRODUCT_ID]`和`offerID=[OFFERID]` URL参数将附加到请求的URL。 在Widget选件URL上提供的服务可使用这些参数返回Adobe Target Standard/Premium以外的内容，这些内容使用mbox中的产品或订单信息。 Widget选件也可以通过API访问，因此您可以在Adobe Target Standard/Premium之外以编程方式创建选件。
