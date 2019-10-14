---
title: Adobe Dynamic Media Classic平台概述
seo-title: Adobe Dynamic Media Classic平台概述
description: 'null'
seo-description: Dynamic Media Classic平台和工作流程的概述。
uuid: e7d3bfb3-1cfe-43ea-b862-aae3b3928c71
contentOwner: admin
content-type: 引用
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENTONDEMAND_PK/categories/getting_started
discoiquuid: 2b134cfa-7f46-4f5f-959e-b30aae610bb9
translation-type: tm+mt
source-git-commit: 6fff3699f8a08af433df3f3a7790a11bf9d05b00

---


# Adobe Dynamic Media Classic平台概述{#adobe-scene-platform-overview}

Dynamic Media Classic是一个集成的富媒体管理、发布和服务环境。 富媒体可以传送给所有营销和销售渠道，包括网站，印刷材料、电子邮件营销活动、门户网站、桌面以及设备。

## 工作流程 {#workflow-process}

关键的Dynamic Media Classic工作流步骤包括：

* **上传和管理资源**&#x200B;将媒体资源上传到SPS。 您可以组织、浏览和搜索系统上的资源，也可以将元数据应用到资源。如果安装了 Adobe Scene7 Publishing System 桌面应用程序，您可以将文件和文件夹从桌面拖动到上载文件夹以上载这些文件和文件夹。

* **创建富媒体**&#x200B;创建资产的不同配置，如eCatalog、图像集、旋转集、样本集、混合媒体集、基本模板和FXG模板。 有关更多信息，请参阅关于富媒体。

* **发布和管理**&#x200B;将资产发布到Dynamic Media Classic saa网络，以及监视资产发布时的状态，管理用户权限并维护安全。

* **服务**-将媒体从Dynamic Media Classic saaS网络交付到网页、应用程序和移动设备；媒体经过性能优化，并通过CDN缓存提供。 Dynamic Media Classic为您提供每个资产的URL。 在您发布资源之后，URL 即处于活动状态。

![Dynamic Media Classic工作流程](/help/assets/gs_workflow.png)

## 单个主图象和单个 URL 调用 {#single-master-images-and-single-url-calls}

Dynamic Media Classic与其他系统有根本区别，因为您可以使用Dynamic Media Classic从单个主资产和URL调用动态传送媒体。

使用Dynamic Media Classic生成的URL字符串包含说明，告诉服务器在交付资产时如何显示资产。 例如，传送同一主图象时，可以使用不同的大小、格式、粗细、颜色以及缩放视图。在使用Dynamic Media Classic构建和发布媒体资源时，您可以以可视方式配置效果。 在此过程中，您可以创建 URL 调用，这些调用会正确指示服务器如何把您的主资源呈现给应用程序。

![Dynamic Media Classic可以将同一主图像以不同的大小和格式传送给不同媒体。](/help/assets/gs_dynamic_publishing.png)

## 内容缓存 {#content-caching}

动态媒体经典动态生成的图像是缓存友好型的；在大多数情况下，它们是JPEG图像，具有标识它们的唯一URL调用。 图像会传送到内容传递网络 (CDN)，这是一个服务器系统，这些服务器在 Internet 上彼此互联以更快的速度传送内容。图像从位于全球的服务器发布到计算机。使用任何CDN供应商实施缓存机制时，您只需将服务器名称更改为指向支持CDN的Dynamic Media Image Server。 所有Dynamic Media Classic版本都包括捆绑的CDN缓存。
