---
title: Adobe Dynamic Media Classic程序概述
description: Adobe Dynamic Media Classic项目及其整个工作流过程的概述。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/getting_started
feature: Dynamic Media Classic
role: Admin,User
exl-id: ac50cb9c-fd87-4608-80cb-8d40a0b8f131
topic: Administration
level: Beginner
source-git-commit: edd893482cbafd9674a44cf9878b8ee3079d98f7
workflow-type: tm+mt
source-wordcount: '477'
ht-degree: 12%

---

# Adobe Dynamic Media Classic程序概述{#adobe-scene-platform-overview}

Adobe Dynamic Media Classic是一个集成的富媒体管理、发布和服务环境。 富媒体可以传送到所有营销和销售渠道。 这些渠道包括Web、打印材料、电子邮件营销活动、Web门户、桌面和设备。

另请参阅 [平台概述](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/572_Platform%20Overview_converted%20renamed_Getting%20Started-AVS) 训练视频。

## 工作流程 {#workflow-process}

Adobe Dynamic Media Classic工作流的关键步骤包括：

* **上传和管理您的资源**  — 将您的媒体资源上传到Adobe Dynamic Media Classic。 您可以组织、浏览和搜索系统上的资源，您还可以将元数据应用到资源。

* **创建富媒体**  — 创建资产的不同配置，如eCatalog、图像集、旋转集、样本集、混合媒体集、基本模板和FXG模板。

* **发布和管理**  — 将资源发布到Adobe Dynamic Media Classic SaaS网络。 在发布资产时监控资产的状态。 管理用户权限并保持安全性。

* **服务**  — 将媒体从Adobe Dynamic Media Classic SaaS网络交付到网页、应用程序和移动设备；媒体已优化性能，并带有CDN缓存进行交付。 Adobe Dynamic Media Classic会为您提供每个资源的URL。 在您发布资源之后，URL 即处于活动状态。

![Adobe Dynamic Media Classic工作流过程](/help/using/assets/gs_workflow.png)

## 单个主图像和单个URL调用 {#single-master-images-and-single-url-calls}

Adobe Dynamic Media Classic与其他系统有着根本性的不同，因为您可以使用Adobe Dynamic Media Classic从单个主要资产和URL调用动态地交付媒体。

您通过Adobe Dynamic Media Classic生成的URL字符串中包含一些说明，告知服务器在交付资源时如何显示资源。 例如，同一主图像可以以不同的大小、格式、粗细、颜色和缩放视图交付。 在使用Adobe Dynamic Media Classic构建和发布媒体资源时，您可以可视化地配置效果。 在这样做时，您将创建URL调用，以正确告知服务器如何将您的主要资源呈现给应用程序。

![Adobe Dynamic Media Classic可以将相同的主图像交付给不同大小和格式的不同媒体。](/help/using/assets/gs_dynamic_publishing.png)
*Adobe Dynamic Media Classic确保向任何屏幕提供一致、优质的体验，而不管其大小或带宽如何。*

## 内容缓存 {#content-caching}

Adobe Dynamic Media Classic动态生成的图像有利于缓存；通常，它们是JPEG图像，具有标识它们的唯一URL调用。 图像会传送到内容传递网络 (CDN)，这是一个服务器系统，这些服务器在 Internet 上彼此互联以更快的速度传送内容。图像从位于全球的服务器发布到计算机。使用任何CDN供应商实施缓存机制时，您只需将服务器名称更改为指向启用了CDN的Dynamic Media Image Server即可。 所有Adobe Dynamic Media Classic版本都包含捆绑的CDN缓存。
