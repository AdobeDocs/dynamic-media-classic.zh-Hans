---
title: AdobeDynamic Media经典平台概述
description: Dynamic Media经典平台和工作流程概述。
uuid: e7d3bfb3-1cfe-43ea-b862-aae3b3928c71
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/getting_started
discoiquuid: 2b134cfa-7f46-4f5f-959e-b30aae610bb9
translation-type: tm+mt
source-git-commit: ca12c96d3a76cfa52fd930d190476cb6fc4f4ac7
workflow-type: tm+mt
source-wordcount: '442'
ht-degree: 32%

---


# AdobeDynamic Media经典平台概述{#adobe-scene-platform-overview}

Dynamic Media经典是一个集成的富媒体管理、发布和服务环境。 富媒体可以传送给所有营销和销售渠道，包括网站，印刷材料、电子邮件营销活动、门户网站、桌面以及设备。

## 工作流程 {#workflow-process}

关键的Dynamic Media经典工作流程步骤是：

* **上传和管理资**
产将媒体资产上传到Dynamic Media经典。您可以组织、浏览和搜索系统上的资源，也可以将元数据应用到资源。

* **创建富**
媒体创建资产的不同配置，如eCatalog、图像集、旋转集、样本集、混合媒体集、基本模板和FXG模板。有关更多信息，请参阅关于富媒体。

* **发布和**
管理将资产发布到Dynamic Media经典Saas网络，并在资产发布时监控资产的状态，管理用户权限并维护安全。

* **服务**
将媒体从Dynamic Media经典SaaS网络交付到网页、应用程序和移动设备；媒体经过性能优化，并通过CDN缓存提供。Dynamic Media经典为您提供每个资产的URL。 在您发布资源之后，URL 即处于活动状态。

![Dynamic Media经典工作流程](/help/assets/gs_workflow.png)

## 单个主图象和单个 URL 调用 {#single-master-images-and-single-url-calls}

Dynamic Media经典与其他系统有根本区别，因为您可以使用Dynamic Media经典从单个主控资产和URL调用动态传送媒体。

您使用Dynamic Media经典生成的URL字符串包含说明，告诉服务器在交付资产时如何显示资产。 例如，传送同一主图象时，可以使用不同的大小、格式、粗细、颜色以及缩放视图。在使用Dynamic Media经典构建和发布媒体资源时，您可以直观地配置效果。 在此过程中，您可以创建 URL 调用，这些调用会正确指示服务器如何把您的主资源呈现给应用程序。

![Dynamic Media经典可以以不同的大小和格式向不同媒体提供相同的主控图像。](/help/assets/gs_dynamic_publishing.png)

## 内容缓存 {#content-caching}

Dynamic Media经典动态生成的图像是缓存友好的；在大多数情况下，它们是具有唯一URL调用的JPEG图像，用于识别它们。 图像会传送到内容传递网络 (CDN)，这是一个服务器系统，这些服务器在 Internet 上彼此互联以更快的速度传送内容。图像从位于全球的服务器发布到计算机。使用任何CDN供应商实施缓存机制时，您只需更改服务器名称以指向支持CDN的Dynamic Media图像服务器。 所有Dynamic Media经典版本都包括捆绑的CDN缓存。
