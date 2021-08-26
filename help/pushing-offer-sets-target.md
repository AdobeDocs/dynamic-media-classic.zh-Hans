---
title: 将选件集推送到Adobe Target Standard/Premium
description: 了解如何将选件集推送到Adobe Target Standard/Premium。
uuid: 8c895a7c-21b4-4d85-8b0b-a3d2a420bf2e
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
discoiquuid: 39a05654-4f66-4f1e-aec5-ebe6d174353f
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 778fd54b-a9e5-40c5-aff1-a156a5c15923
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '282'
ht-degree: 6%

---

# 将选件集推送到Adobe Target Standard/Premium {#pushing-offer-sets-to-target}

在创建或编辑选件集后，按照以下步骤将其推送到Adobe Target Standard/Premium:

1. 在Test&amp;Target选件集屏幕中，单击&#x200B;**[!UICONTROL 推送选件]**。
1. 输入您的客户端代码和登录凭据。
1. 按一下&#x200B;**[!UICONTROL 登入]**。

在传输到Adobe Target Standard/Premium期间，前缀`S7_`会自动附加到选件名称的开头。 附加此前缀，以确保您能够在Test&amp;Target选件列表中轻松找到AdobeDynamic Media Classic选件。 例如，选件显示为`S7_<name of offer set>_<offer name>`。

AdobeDynamic Media Classic将推出Adobe Target Standard/Premium小组件选件。 您可以使用小组件选件在Adobe Target Standard/Premium之外托管您自己的选件内容。 小组件选件与在Adobe Target Standard/Premium外托管的标准选件类似。 它们允许Adobe Target Standard/Premium部署存储在您服务器上的选件内容，从而允许更复杂、更动态地使用。 小工具选件从 URL 处检索内容，缓存并提供该内容，时限为两小时左右。小组件选件提供了一些动态内容生成功能，Adobe Target Standard/Premium以外的其他选件则不提供这些功能。 如果提供选件的mbox包含mbox参数（如`mboxProductID`和`mbox.offerId`），则`productId=[PRODUCT_ID]`和`offerID=[OFFERID]` URL参数会附加到请求的URL中。 这些参数可供小组件选件URL上提供的服务使用，以返回Adobe Target Standard/Premium以外的内容，该内容使用您的mbox中的产品或订单信息。 小组件选件也可通过API访问，以通过编程方式在Adobe Target Standard/Premium之外创建选件。
