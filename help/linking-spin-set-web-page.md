---
title: 将旋转集链接到网页
description: 了解如何将旋转集关联到网页。
uuid: d3c5773e-60c4-4e8b-9c48-e1e3eb8028d0
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/spin_sets
discoiquuid: 651b21ef-e322-4e6d-8e37-45ffd56f7a58
feature: Dynamic Media Classic，查看器，旋转集
role: Business Practitioner
exl-id: af75547e-20e8-44c2-b165-01532d6e21d0
source-git-commit: 38d09bb78834c6b3614bf2b96fd6aee5661e0a5a
workflow-type: tm+mt
source-wordcount: '720'
ht-degree: 87%

---

# 将旋转集链接到网页{#linking-a-spin-set-to-a-web-page}

网站和应用程序通过URL字符串或嵌入代码访问Dynamic Media图像服务器内容（包括旋转集）。 这些 URL 字符串在发布过程中被激活。要将旋转集的URL字符串或嵌入代码放置在网页和应用程序中，请从Dynamic Media Classic中复制该代码。

>[!NOTE]
>
>在发布资源之前，URL 处于非激活状态。

## 复制旋转集 URL {#copying-a-spin-set-url}

1. 在“资源浏览”面板的“显示”下拉列表中，单击“**[!UICONTROL 旋转集]**”。
1. 在左侧的“资源库”面板中，导航至要复制其嵌入代码的旋转集所在的资源文件夹。
1. 在“资源浏览”面板上方的工具栏右侧，执行以下任一操作：

   * 单击“**[!UICONTROL 网格视图]**”。在“资源浏览”面板中，双击单个资源以便在详细信息视图中将其打开。在右侧的“URL 和嵌入代码”面板中，单击所需查看器右侧的“**[!UICONTROL 复制 URL]**”。
   * 单击“**[!UICONTROL 网格视图]**”。在“资源浏览”面板中，选择单个资源，然后在缩略图图像下方单击“**[!UICONTROL 预览]**”>“**[!UICONTROL 查看器列表]**”。

      在“查看器列表”页面中表的“操作”列下，单击“**[!UICONTROL 复制 URL]**”。

   * 单击“**[!UICONTROL 列表视图]**”。在“资源浏览”面板中，选择单个资源，然后在缩略图图像右侧单击“**[!UICONTROL 预览]**”>“**[!UICONTROL 查看器列表]**”。

      在“查看器列表”页面中表的“操作”列下，单击“**[!UICONTROL 复制 URL]**”。

   * 单击“**[!UICONTROL 网格视图]**”、“**[!UICONTROL 列表视图]**”或“**[!UICONTROL 详细信息视图]**”。在同一工具栏上，单击“**[!UICONTROL 预览]**”>“**[!UICONTROL 查看器列表]**”。

      在“查看器列表”页面中表的“操作”列下，单击“**[!UICONTROL 复制 URL]**”。

## 将旋转集 URL 添加到您的网页 {#adding-spin-set-urls-to-your-web-page}

旋转集的部署方式与所有缩放查看器一样，即通过在缩放窗口中显示旋转集的动态页面（ASP 或 JSP）进行部署。对Dynamic Media Classic平台的URL调用遵循缩放查看器上的相同协议。 不过，查看器预设名称取决于您的管理员所定义的默认旋转集查看器预设。例如，以下非实时 URL 语法示例包括名为 `viewer.jsp` 的预设名称，而 SKU 参数现在为旋转集名称：

```as3
https://sample.scene7.com/s7ondemand/spin/viewer.jsp?company=S7Web&sku=backpack_spin
```

在此 URL 语法示例中（链接处于不活动状态），请注意 SKU 编号 (`sku=backpack_spin`)。`sku=`后面的字符串是旋转集名称(`backpack spin`)。

## 复制旋转集查看器的嵌入代码 {#copying-the-embed-code-of-a-spin-set-viewer}

使用嵌入代码功能，您可以查看用于所选旋转集的查看器代码。您也可以将代码复制到剪贴板中，以便可以将其粘贴到网页中以部署查看器。不允许在“嵌入代码”对 话框中编辑代码 。

**复制旋转集查看器的嵌入代码:**

1. 在“资源浏览”面板的“显示”下拉列表中，单击“**[!UICONTROL 旋转集]**”。
1. 在左侧的“资源库”面板中，导航至要复制其嵌入代码的旋转集所在的资源文件夹。
1. 在“资源浏览”面板上方的工具栏右侧，执行以下任一操作：

   * 单击“**[!UICONTROL 网格视图]**”。在“资源浏览”面板中，双击单个资源以便在详细信息视图中将其打开。在右侧的“URL 和嵌入代码”面板中，单击所需查看器右侧的“**[!UICONTROL 嵌入代码]**”。
   * 单击“**[!UICONTROL 网格视图]**”。在“资源浏览”面板中，选择单个资源，然后在缩略图图像下方单击“**[!UICONTROL 预览]**”>“**[!UICONTROL 查看器列表]**”。

      在“查看器列表”页面中表的“操作”列下，单击“**[!UICONTROL 嵌入代码]**”。

   * 单击“**[!UICONTROL 列表视图]**”。在“资源浏览”面板中，选择单个资源，然后在缩略图图像右侧单击“**[!UICONTROL 预览]**”>“**[!UICONTROL 查看器列表]**”。

      在“查看器列表”页面中表的“操作”列下，单击“**[!UICONTROL 嵌入代码]**”。

   * 单击“**[!UICONTROL 网格视图]**”、“**[!UICONTROL 列表视图]**”或“**[!UICONTROL 详细信息视图]**”。在同一工具栏上，单击“**[!UICONTROL 预览]**”>“**[!UICONTROL 查看器列表]**”。

      在“查看器列表”页面中表的“操作”列下，单击“**[!UICONTROL 嵌入代码]**”。

1. 在“嵌入代码”对话框中，单击“**[!UICONTROL 复制到剪贴板]**”。

   在“嵌入代码”对话框中不允许编辑代码。

1. 单击&#x200B;**[!UICONTROL 关闭]**。
