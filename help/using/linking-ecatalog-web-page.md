---
title: 将eCatalog链接到网页
description: 了解如何将eCatalog链接到Adobe Dynamic Media Classic中的网页。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: aee72576-1e3e-401c-953d-cc2be27f7dfd
topic: Integrations, Development
level: Experienced
autotag-review: '2026-05-13T19:52:09.030Z'
TQID: 'https://experienceleague.adobe.com/cAIaFvlJ3jYoqu1LeLRILuuYsfvuYH6f-N8PqqkHkrk'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
  - id: d378ca77-2da1-4f39-ad92-1917fe974a38
source-git-commit: 0d05ca7402db1d8894db1127088905143fb97cff
workflow-type: tm+mt
source-wordcount: 698
ht-degree: 20%

---

# 将eCatalog链接到网页{#linking-an-ecatalog-to-a-web-page}

您的网站和应用程序通过URL字符串或嵌入代码访问Dynamic Media图像服务器内容，包括eCatalog。 这些 URL 字符串在发布过程中被激活。 要将eCatalog的URL字符串或嵌入代码置于网页和应用程序中，请从Adobe Dynamic Media Classic复制该字符串或嵌入代码。

>[!NOTE]
>
>在发布资源之前，URL 处于非激活状态。

## 复制eCatalog URL {#copying-an-ecatalog-url}

1. 在“资源浏览”面板的“显示”下拉列表中，选择&#x200B;**[!UICONTROL 目录]**。
1. 在左侧的“资产库”面板中，导航到资产文件夹，该文件夹包含要复制其嵌入代码的eCatalog。
1. 在“资源浏览”面板上方的工具栏右侧，执行以下任一操作：

   * 选择&#x200B;**[!UICONTROL 网格视图]**。 在“资源浏览”面板中，双击单个资源以便在详细信息视图中将其打开。 在右侧的“URL和嵌入代码”面板中，选择所需查看器右侧的&#x200B;**[!UICONTROL 复制URL]**。
   * 选择&#x200B;**[!UICONTROL 网格视图]**。 在“资源浏览”面板中，选择单个资源，然后在缩略图图像下面转到&#x200B;**[!UICONTROL 预览]** > **[!UICONTROL 查看器列表]**。

     在“查看器列表”页表的“操作”列下，选择&#x200B;**[!UICONTROL 复制URL]**。

   * 选择&#x200B;**[!UICONTROL 列表视图]**。 在“资源浏览”面板中，选择单个资源，然后在缩略图图像的右侧，转到&#x200B;**[!UICONTROL 预览]** > **[!UICONTROL 查看器列表]**。

     在“查看器列表”页表的“操作”列下，选择&#x200B;**[!UICONTROL 复制URL]**。

   * 选择&#x200B;**[!UICONTROL 网格视图]**、**[!UICONTROL 列表视图]**&#x200B;或&#x200B;**[!UICONTROL 详细信息视图]**。 在同一工具栏上，转到&#x200B;**[!UICONTROL 预览]** > **[!UICONTROL 查看器列表]**。

     在“查看器列表”页表的“操作”列下，选择&#x200B;**复制URL**。

## 将eCatalog URL添加到网页 {#adding-ecatalog-urls-to-your-web-page}

部署eCatalog的最常见方法是在网页上以eCatalog缩略图封面页的形式放置链接。 与 IT 团队合作，以确保在一个居中弹出的空白窗口中启动 eCatalog。 请您的 IT 团队协助在浏览器中不显示工具栏和地址栏。

有关更多详细信息和代码示例，请参阅“HTML查看器参考”中的[嵌入的Adobe5 eCatalog查看器](https://experienceleague.adobe.com/zh-hans/docs/dynamic-media-developer-resources/library/viewers-aem-assets-dmc/ecatalog/c-html5-20-ecatalog-viewer-about#section-e1c3106f5b3e445d9b95be337c2f94e2)。

## 复制eCatalog查看器的嵌入代码 {#copying-the-embed-code-of-an-ecatalog-viewer}

使用嵌入的代码功能，您可以查看选定eCatalog的查看器代码。 您还可以将代码复制到剪贴板，以便将其粘贴到网页中用于部署查看器。 在“嵌入代码”对话框中不允许编辑代码。

**复制eCatalog查看器的嵌入代码：**

1. 在“资源浏览”面板的“显示”下拉列表中，选择&#x200B;**[!UICONTROL 目录]**。
1. 在左侧的“资产库”面板中，导航到资产文件夹，该文件夹包含要复制其嵌入代码的eCatalog。
1. 在“资源浏览”面板上方的工具栏右侧，执行以下任一操作：

   * 选择&#x200B;**[!UICONTROL 网格视图]**。 在“资源浏览”面板中，双击单个资源以便在详细信息视图中将其打开。 在右侧的“URL”面板中，选择&#x200B;**[!UICONTROL 嵌入代码]**。
   * 选择&#x200B;**[!UICONTROL 网格视图]**。 在“资源浏览”面板中，选择单个资源，然后在缩略图图像下面转到&#x200B;**[!UICONTROL 预览]** > **[!UICONTROL 查看器列表]**。

     在“查看器列表”页表的“操作”列下，选择&#x200B;**[!UICONTROL 嵌入代码]**。

   * 选择&#x200B;**[!UICONTROL 列表视图]**。 在“资源浏览”面板中，选择单个资源，然后在缩略图图像的右侧，转到&#x200B;**[!UICONTROL 预览]** > **[!UICONTROL 查看器列表]**。

     在“查看器列表”页表的“操作”列下，选择&#x200B;**[!UICONTROL 嵌入代码]**。

   * 选择&#x200B;**[!UICONTROL 网格视图]**、**[!UICONTROL 列表视图]**&#x200B;或&#x200B;**[!UICONTROL 详细信息视图]**。 在同一工具栏上，转到&#x200B;**[!UICONTROL 预览]** > **[!UICONTROL 查看器列表]**。

     在“查看器列表”页表的“操作”列下，选择&#x200B;**[!UICONTROL 嵌入代码]**。

1. 在“嵌入代码”对话框中，选择&#x200B;**[!UICONTROL 复制到剪贴板]**。

   在“嵌入代码”对话框中不允许编辑代码。

1. 选择&#x200B;**[!UICONTROL 关闭]**。
