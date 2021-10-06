---
title: Adobe Dynamic Media Classic计划概述
description: Adobe Dynamic Media Classic计划及其整个工作流程的概述。
uuid: e7d3bfb3-1cfe-43ea-b862-aae3b3928c71
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/getting_started
discoiquuid: 2b134cfa-7f46-4f5f-959e-b30aae610bb9
feature: Dynamic Media Classic
role: Admin,User
exl-id: ac50cb9c-fd87-4608-80cb-8d40a0b8f131
source-git-commit: 352b1c383195fa03294ad3501207d63f3cfe3e42
workflow-type: tm+mt
source-wordcount: '530'
ht-degree: 25%

---

# Adobe Dynamic Media Classic计划概述{#adobe-scene-platform-overview}

Adobe Dynamic Media Classic是一个集成的富媒体管理、发布和服务环境。 富媒体可以传送给所有营销和销售渠道，包括网站，印刷材料、电子邮件营销活动、门户网站、桌面以及设备。

另请参阅[平台概述](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/572_Platform%20Overview_converted%20renamed_Getting%20Started-AVS)培训视频。

## 工作流程 {#workflow-process}

关键的Adobe Dynamic Media Classic工作流步骤包括：

* **上传和管理资产**  — 将媒体资产上传到Adobe Dynamic Media Classic。您可以组织、浏览和搜索系统上的资源，也可以将元数据应用到资源。

* **创建富媒体**  — 创建资产的不同配置，如电子目录、图像集、旋转集、色板集、混合媒体集、基本模板和FXG模板。

* **发布和管理**  — 将资产发布到Adobe Dynamic Media Classic SaaS网络，以及在资产发布时监控资产的状态，管理用户权限并维护安全。

* **提供**  — 将媒体从Adobe Dynamic Media Classic SaaS网络传送到网页、应用程序和移动设备；媒体经过性能优化，可通过CDN缓存提供。Adobe Dynamic Media Classic会为您提供每个资产的URL。 在您发布资源之后，URL 即处于活动状态。

![Adobe Dynamic Media Classic工作流流程](/help/assets/gs_workflow.png)

## 单个主图象和单个 URL 调用 {#single-master-images-and-single-url-calls}

Adobe Dynamic Media Classic与其他系统有着根本的不同，因为您可以使用Adobe Dynamic Media Classic通过单个主控资产和URL调用动态交付媒体。

您通过Adobe Dynamic Media Classic生成的URL字符串中包含相关说明，这些说明会告知服务器在交付资产时如何显示资产。 例如，传送同一主图象时，可以使用不同的大小、格式、粗细、颜色以及缩放视图。在使用Adobe Dynamic Media Classic构建和发布媒体资产时，您可以直观地配置效果。 在此过程中，您可以创建 URL 调用，这些调用会正确指示服务器如何把您的主资源呈现给应用程序。

![Adobe Dynamic Media Classic可以将相同的主控图像以不同的大小和格式提供给不同的媒体。](/help/assets/gs_dynamic_publishing.png)
*Adobe Dynamic Media Classic可确保向任何屏幕提供一致的优质体验，而无论其大小或带宽如何。*

## 内容缓存 {#content-caching}

Adobe Dynamic Media Classic动态生成的图像对缓存友好；通常，它们是JPEG图像，其具有可识别它们的唯一URL调用。 图像会传送到内容传递网络 (CDN)，这是一个服务器系统，这些服务器在 Internet 上彼此互联以更快的速度传送内容。图像从位于全球的服务器发布到计算机。使用任何CDN供应商实施缓存机制时，您只需更改服务器名称以指向启用CDN的Dynamic Media图像服务器即可。 所有Adobe Dynamic Media Classic版本都包含捆绑的CDN缓存。
