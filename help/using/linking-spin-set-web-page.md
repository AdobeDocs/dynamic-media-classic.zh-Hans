---
title: 将旋转集链接到网页
description: 了解如何将旋转集链接到Adobe Dynamic Media Classic中的网页。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/spin_sets
feature: Dynamic Media Classic,Viewers,Spin Sets
role: User
exl-id: af75547e-20e8-44c2-b165-01532d6e21d0
topic: Content Management
level: Intermediate
source-git-commit: ad7e20fdbe9028c6255865cce95d109f9e9eeab2
workflow-type: tm+mt
source-wordcount: '727'
ht-degree: 23%

---

# 将旋转集链接到网页{#linking-a-spin-set-to-a-web-page}

网站和应用程序通过URL字符串或嵌入代码访问Dynamic Media Image Server内容，包括旋转集。 这些 URL 字符串在发布过程中被激活。要将旋转集的URL字符串或嵌入代码放置到网页和应用程序中，请从Adobe Dynamic Media Classic复制该字符串或嵌入代码。

>[!NOTE]
>
>在发布资源之前，URL 处于非激活状态。

## 复制旋转集URL {#copying-a-spin-set-url}

1. 在“资产浏览”面板的“显示”下拉列表中，选择&#x200B;**[!UICONTROL 旋转集]**。
1. 在左侧的“资产库”面板中，导航到包含要复制其嵌入代码的旋转集的资产文件夹。
1. 在“资源浏览”面板上方的工具栏右侧，执行以下任一操作：

   * 选择&#x200B;**[!UICONTROL 网格视图]**。 在“资源浏览”面板中，双击单个资源以便在详细信息视图中将其打开。在右侧的“URL和嵌入代码”面板中，选择所需查看器右侧的&#x200B;**[!UICONTROL 复制URL]**。
   * 选择&#x200B;**[!UICONTROL 网格视图]**。 在“资源浏览”面板中，选择单个资源，然后在缩略图图像下面转到&#x200B;**[!UICONTROL 预览]** > **[!UICONTROL 查看器列表]**。

     在“查看器列表”页表的“操作”列下，选择&#x200B;**[!UICONTROL 复制URL]**。

   * 选择&#x200B;**[!UICONTROL 列表视图]**。 在“资源浏览”面板中，选择单个资源，然后在缩略图图像的右侧，转到&#x200B;**[!UICONTROL 预览]** > **[!UICONTROL 查看器列表]**。

     在“查看器列表”页表的“操作”列下，选择&#x200B;**[!UICONTROL 复制URL]**。

   * 选择&#x200B;**[!UICONTROL 网格视图]**、**[!UICONTROL 列表视图]**&#x200B;或&#x200B;**[!UICONTROL 详细信息视图]**。 在同一工具栏上，转到&#x200B;**[!UICONTROL 预览]** > **[!UICONTROL 查看器列表]**。

     在“查看器列表”页表的“操作”列下，选择&#x200B;**[!UICONTROL 复制URL]**。

## 将旋转集URL添加到网页 {#adding-spin-set-urls-to-your-web-page}

旋转集的部署方式与所有缩放查看器一样，即通过在缩放窗口中显示旋转集的动态页面（ASP 或 JSP）进行部署。对Adobe Dynamic Media Classic平台的URL调用在缩放查看器中遵循相同的协议。 不过，查看器预设名称取决于您的管理员所定义的默认旋转集查看器预设。例如，以下非实时URL语法示例包含一个名为`viewer.jsp`的预设名称，现在SKU参数是旋转集名称：

```as3
https://sample.scene7.com/s7ondemand/spin/viewer.jsp?company=S7Web&sku=backpack_spin
```

在此URL语法示例（链接未处于活动状态）中，请注意一个SKU编号( `sku=backpack_spin`)。 `sku=`之后的字符串是旋转集名称( `backpack spin`)。

## 复制旋转集查看器的嵌入代码 {#copying-the-embed-code-of-a-spin-set-viewer}

使用嵌入代码功能，您可以查看用于所选旋转集的查看器代码。您还可以将代码复制到剪贴板，以便将其粘贴到网页中用于部署查看器。 在“嵌入代码”对话框中不允许编辑代码。

**要复制旋转集查看器的嵌入代码：**

1. 在“资产浏览”面板的“显示”下拉列表中，选择&#x200B;**[!UICONTROL 旋转集]**。
1. 在左侧的“资产库”面板中，导航到包含要复制其嵌入代码的旋转集的资产文件夹。
1. 在“资源浏览”面板上方的工具栏右侧，执行以下任一操作：

   * 选择&#x200B;**[!UICONTROL 网格视图]**。 在“资源浏览”面板中，双击单个资源以便在详细信息视图中将其打开。在右侧的“URL和嵌入代码”面板中，选择所需查看器右侧的&#x200B;**[!UICONTROL 嵌入代码]**。
   * 选择&#x200B;**[!UICONTROL 网格视图]**。 在“资源浏览”面板中，选择单个资源，然后在缩略图图像下面转到&#x200B;**[!UICONTROL 预览]** > **[!UICONTROL 查看器列表]**。

     在“查看器列表”页表的“操作”列下，选择&#x200B;**[!UICONTROL 嵌入代码]**。

   * 选择&#x200B;**[!UICONTROL 列表视图]**。 在“资源浏览”面板中，选择单个资源，然后在缩略图图像的右侧，转到&#x200B;**[!UICONTROL 预览]** > **[!UICONTROL 查看器列表]**。

     在“查看器列表”页表的“操作”列下，选择&#x200B;**[!UICONTROL 嵌入代码]**。

   * 选择&#x200B;**[!UICONTROL 网格视图]**、**[!UICONTROL 列表视图]**&#x200B;或&#x200B;**[!UICONTROL 详细信息视图]**。 在同一工具栏上，转到&#x200B;**[!UICONTROL 预览]** > **[!UICONTROL 查看器列表]**。

     在“查看器列表”页表的“操作”列下，选择&#x200B;**[!UICONTROL 嵌入代码]**。

1. 在“嵌入代码”对话框中，选择&#x200B;**[!UICONTROL 复制到剪贴板]**。

   在“嵌入代码”对话框中不允许编辑代码。

1. 选择&#x200B;**[!UICONTROL 关闭]**。
