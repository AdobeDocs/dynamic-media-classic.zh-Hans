---
title: Adobe Dynamic Media Classic計畫總覽
description: 概述Adobe Dynamic Media Classic程式及其整個工作流程。
uuid: e7d3bfb3-1cfe-43ea-b862-aae3b3928c71
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/getting_started
discoiquuid: 2b134cfa-7f46-4f5f-959e-b30aae610bb9
feature: Dynamic Media Classic
role: Admin,User
exl-id: ac50cb9c-fd87-4608-80cb-8d40a0b8f131
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '528'
ht-degree: 17%

---

# Adobe Dynamic Media Classic計畫總覽{#adobe-scene-platform-overview}

Adobe Dynamic Media Classic是整合式多媒體管理、發佈和服務環境。 富媒体可以传送给所有营销和销售渠道，包括网站，印刷材料、电子邮件营销活动、门户网站、桌面以及设备。

另請參閱 [平台概觀](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/572_Platform%20Overview_converted%20renamed_Getting%20Started-AVS) 訓練影片。

## 工作流程 {#workflow-process}

Adobe Dynamic Media Classic工作流程的關鍵步驟為：

* **上傳和管理您的資產**  — 將您的媒體資產上傳至Adobe Dynamic Media Classic。 您可以组织、浏览和搜索系统上的资源，也可以将元数据应用到资源。

* **建立多媒體**  — 建立資產的不同設定，例如eCatalog、影像集、迴轉集、色票集、混合媒體集、基本範本和FXG範本。

* **發佈和管理**  — 將資產發佈至Adobe Dynamic Media Classic SaaS網路。 在資產發佈時監視資產狀態。 管理使用者許可權並維護安全性。

* **服務**  — 從Adobe Dynamic Media Classic SaaS網路傳送媒體至網頁、應用程式和行動裝置；媒體已最佳化效能，並透過CDN快取傳送。 Adobe Dynamic Media Classic會為您提供每個資產的URL。 在您发布资源之后，URL 即处于活动状态。

![Adobe Dynamic Media Classic工作流程程式](/help/assets/gs_workflow.png)

## 單一主要影像和單一URL呼叫 {#single-master-images-and-single-url-calls}

Adobe Dynamic Media Classic與其他系統截然不同，因為您可以使用Adobe Dynamic Media Classic以動態方式從單一主要資產和URL呼叫傳送媒體。

您透過Adobe Dynamic Media Classic產生的URL字串包含指示，告知伺服器如何在傳送資產時顯示資產。 例如，相同的主要影像可以不同大小、格式、重量、顏色和縮放檢視提供。 使用Adobe Dynamic Media Classic建置和發佈媒體資產時，您可以透過視覺化方式設定效果。 這樣做時，您會建立URL呼叫，正確地告知伺服器如何將您的主要資產呈現給應用程式。

![Adobe Dynamic Media Classic可將相同的主要影像傳送至不同大小和格式的不同媒體。](/help/assets/gs_dynamic_publishing.png)
*Adobe Dynamic Media Classic可確保為任何畫面提供一致、高品質的體驗，無論畫面大小或頻寬為何。*

## 内容缓存 {#content-caching}

Adobe Dynamic Media Classic動態產生的影像有利於快取；通常，它們是JPEG影像，具有可識別它們的唯一URL呼叫。 图像会传送到内容传递网络 (CDN)，这是一个服务器系统，这些服务器在 Internet 上彼此互联以更快的速度传送内容。图像从位于全球的服务器发布到计算机。使用任何CDN廠商實作快取機制時，只要將伺服器名稱變更為指向啟用CDN的Dynamic Media Image Server即可。 所有Adobe Dynamic Media Classic版本都包含套件式CDN快取。
