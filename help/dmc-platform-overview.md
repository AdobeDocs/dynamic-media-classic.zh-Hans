---
title: AdobeDynamic Media Classic计划概述
description: Dynamic Media Classic计划和工作流流程的概述。
uuid: e7d3bfb3-1cfe-43ea-b862-aae3b3928c71
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/getting_started
discoiquuid: 2b134cfa-7f46-4f5f-959e-b30aae610bb9
feature: Dynamic Media Classic
role: Admin,User
exl-id: ac50cb9c-fd87-4608-80cb-8d40a0b8f131
source-git-commit: df689ff5a127bfbc400ca5331168d1ff7bb0b42e
workflow-type: tm+mt
source-wordcount: '454'
ht-degree: 30%

---

# AdobeDynamic Media Classic计划概述{#adobe-scene-platform-overview}

Dynamic Media Classic是一个集成的富媒体管理、发布和服务环境。 富媒体可以传送给所有营销和销售渠道，包括网站，印刷材料、电子邮件营销活动、门户网站、桌面以及设备。

## 工作流程 {#workflow-process}

关键的Dynamic Media Classic工作流步骤包括：

* **上传和管理资产**  — 将媒体资产上传到Dynamic Media Classic。您可以组织、浏览和搜索系统上的资源，也可以将元数据应用到资源。

* **创建富媒体**  — 创建资产的不同配置，如电子目录、图像集、旋转集、色板集、混合媒体集、基本模板和FXG模板。

* **发布和管理**  — 将资产发布到Dynamic Media Classic SaaS网络，以及在资产发布时监控资产的状态，管理用户权限并维护安全。

* **提供**  — 将媒体从Dynamic Media Classic SaaS网络传送到网页、应用程序和移动设备；媒体经过性能优化，可通过CDN缓存提供。Dynamic Media Classic为您提供每个资产的URL。 在您发布资源之后，URL 即处于活动状态。

![Dynamic Media Classic工作流流程](/help/assets/gs_workflow.png)

## 单个主图象和单个 URL 调用 {#single-master-images-and-single-url-calls}

Dynamic Media Classic与其他系统有根本区别，因为您可以使用Dynamic Media Classic通过单个主控资产和URL调用动态交付媒体。

您通过Dynamic Media Classic生成的URL字符串中包含一些说明，用于告知服务器在交付资产时如何显示资产。 例如，传送同一主图象时，可以使用不同的大小、格式、粗细、颜色以及缩放视图。在使用Dynamic Media Classic构建和发布媒体资产时，您可以直观地配置效果。 在此过程中，您可以创建 URL 调用，这些调用会正确指示服务器如何把您的主资源呈现给应用程序。

![Dynamic Media Classic可以以不同的大小和格式，将相同的主控图像传送给不同的媒体。](/help/assets/gs_dynamic_publishing.png)
*Dynamic Media Classic可确保向任何屏幕提供一致的高质量体验，无论其大小或带宽如何。*

## 内容缓存 {#content-caching}

Dynamic Media Classic动态生成的图像对缓存友好；通常，它们是具有唯一URL调用的JPEG图像，用于识别它们。 图像会传送到内容传递网络 (CDN)，这是一个服务器系统，这些服务器在 Internet 上彼此互联以更快的速度传送内容。图像从位于全球的服务器发布到计算机。使用任何CDN供应商实施缓存机制时，您只需更改服务器名称以指向启用CDN的Dynamic Media图像服务器即可。 所有Dynamic Media Classic版本都包含捆绑的CDN缓存。
