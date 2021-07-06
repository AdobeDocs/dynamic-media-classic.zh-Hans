---
title: 发布文件
description: “了解如何将资产发布到Dynamic Media图像服务器。 您可以一次性发布资产，也可以安排Dynamic Media Classic按定期计划发布资产。 发布资源后，这些资源即可用来传送。您可以从Dynamic Media Classic复制URL调用，并将其添加到您的网站或应用程序。”
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/upload_and_publish_assets
feature: Dynamic Media Classic，Asset Management
role: User
exl-id: 91b73a09-c5b5-4001-b36f-6bebe65717ff
source-git-commit: df689ff5a127bfbc400ca5331168d1ff7bb0b42e
workflow-type: tm+mt
source-wordcount: '1712'
ht-degree: 59%

---

# 发布文件{#publishing-files}

您将资产发布到Dynamic Media图像服务器。 您可以一次性发布资产，也可以安排Dynamic Media Classic按定期计划发布资产。 发布资源后，这些资源即可用来传送。您可以从Dynamic Media Classic复制URL调用，并将其添加到您的网站或应用程序。

Dynamic Media Classic现在支持通过HTTP/2交付所有图像和视频。 即，图像或视频的已发布URL或嵌入代码可与接受托管资产的任何应用程序集成。 然后，将通过HTTP/2协议来交付已发布的资产。 这种交付方法改进了浏览器和服务器通信的方式，从而可以缩短所有Dynamic Media Classic资产的响应和加载时间。 请参阅[HTTP2内容交付常见问题解答](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/http2.html#dynamic)。

## 在上载之后发布 {#publish-after-uploading}

资源处于已发布或未发布的状态。默认情况下，您上传到Dynamic Media Classic的任何资产都会自动标记为要发布。

有关更多信息，请参阅[Instant Publish Notice PDF](/help/assets/rendering-instant-publish-notification.pdf)。

使用以下方法将资源标记为发布：

* **上传后发布**  — 在上传页面底部附近，选择上传后发布。默认情况下，将处于选定状态。

* **上传后发布**  — 在“作业选项”对话框中，选择上传后发布。默认情况下，将处于选定状态。

如果父项资源标记为发布，则一些“子项”资源会自动标记为发布。该表列出自动标记为发布的子项资源。

| 父（组）项 | 子（成员）项 |
|--- |--- |
| 图像集 | 集中的图像。 |
| 样本集 | 集中的样本。 |
| 旋转集 | 集中的图像。 |
| 模板 | 模板文件、页面和图像。 |

在发布父图像时，也会自动将派生的图像标记为发布。派生图像包括您使用图像编辑选项调整的图像。您可以在“构建和派生”下的详细信息视图中查看这些派生图像。

## 创建发布作业 {#creating-a-publish-job}

创建发布作业以发布已上传到Dynamic Media Classic服务器的资产，但选择不自动发布这些资产。 您可以执行一次性发布作业或计划定期重复执行的作业。 Dynamic Media Classic提供了高级发布选项，用于发布到特定服务器，以及用于重新发布已发布资产的选项。

**创建发布作业:**

1. 在全局导航栏上，单击“**[!UICONTROL 发布]**”。
1. 在“发布”对话框中，选择是要使用一次性还是重复发布作业。

   请参阅[创建一次性发布作业](publishing-files.md#creating_a_one_time_publish_job)和[创建重复发布作业](publishing-files.md#creating_a_recurring_publish_job)。

1. 输入作业名称。
1. 或者，显示“高级”选项并选择这些选项。

   请参阅[高级发布选项](publishing-files.md#advanced_publish_options)。

1. 单击“**[!UICONTROL 提交发布]**”。

Dynamic Media Classic跟踪“作业”页面上的发布作业。 您可以在该页中查看发布作业。

>[!NOTE]
>
>由于内容传递网络 (CDN) 上的网络缓存机制，您重新发布（以前发布）的资源不会立即显示在网站上。请参阅[重新发布的资源和 CDN 延迟](publishing-files.md#republished_assets_and_cdn_delays)。

### 创建一次性发布作业 {#creating-a-one-time-publish-job}

在“发布”页中，选择“一次”选项以创建一次性发布作业。

如果希望稍后发布作业，请在“发布”页中选择&#x200B;**[!UICONTROL One-Time]**，然后单击&#x200B;**[!UICONTROL 计划稍后执行]**&#x200B;下拉列表。 使用日历和时间滑块选择运行发布作业的日期和时间。

### 创建重复发布作业 {#creating-a-recurring-publish-job}

通过在“发布”页面上选择&#x200B;**[!UICONTROL Recuring]**&#x200B;来创建定期发布作业。

然后，选择&#x200B;**[!UICONTROL Daily]**、**[!UICONTROL Weekly]**、**[!UICONTROL Monthly]**&#x200B;或&#x200B;**[!UICONTROL Custom]**&#x200B;的“重复”选项，然后指定希望何时重复发布作业。 Dynamic Media Classic提供用于计划定期发布作业的日历工具。 您可以单击&#x200B;**[!UICONTROL Custom]**&#x200B;选项，并在规则文本字段中输入规则以描述自定义作业间隔。

请参阅[创建自定义上载或发布作业时间间隔](checking-job-files.md#creating_a_custom_upload_or_publish_job_time_interval)。

>[!NOTE]
>
>重复发布（和上载）作业在“作业”页中列出。可以转到“作业”页的“已计划”选项卡以编辑或删除计划的作业。

### 高级发布选项 {#advanced-publish-options}

您可以在“发布”页中显示高级选项，并选择这些选项以处理发布作业：

* **发布到**  — 要仅将资产发布到特定服务器，请选择服务器类型。

* **发布**  — 默认情况下，Dynamic Media Classic仅发布之前未发布的新资产（上次发布后新资产选项）。但是，您也可以单击&#x200B;**[!UICONTROL 完全发布]**&#x200B;来发布自上次发布以来更新或更改的资产。 如果要发布eCatalog并且希望读者能够按关键词进行搜索，请选择&#x200B;**[!UICONTROL 完全包含搜索数据]**。

* **作业运行方式**  — 从列表中选择用户名。可以在“作业”页中按用户名对作业进行排序。可以通过选择名称将发布作业与用户关联。

**HTTP通知**  — 输入URL以触发后续发布作业。

请参阅[使用上载或发布作业作为触发器](checking-job-files.md#using_an_upload_or_publish_job_as_a_trigger)。

## 取消发布作业 {#canceling-a-publish-job}

您可以取消进行中的发布作业。此外，管理员还可以从公司的“作业”页中取消进行中的发布作业。

要取消发布作业，请转到“作业”页面，然后单击&#x200B;**[!UICONTROL 取消]**。 在“作业”页的“已计划”选项卡上，您可以选中或取消选中作业的“活动”列中的对应复选框以暂停或恢复作业。

>[!NOTE]
>
>取消发布作业之后，其状态更改为“正在停止”，直至达到一个安全的停止点。如果作业正从数据库获取数据，则停止发布作业可能会花费一些时间。

## 手动发布资源 {#manually-publishing-assets}

您可以手动发布各个资源，而不是创建发布作业。在发布集（如图像集或自适应视频集）时，将发布集（或“父项”）和集中的所有成员（或“子项&quot;）。

未发布的资产在用户界面中由资产名称左侧的灰色圆形图标（带有斜杠）指示（未发布状态）。 在发布资源后，该图标将变为绿色，并且中心带有白色复选标记（已发布状态）。

**手动发布资源:**

1. 执行以下操作之一：

   * 在网格视图、列表视图或详细信息视图中，使用标准文件选择方法选择一个或多个未发布的资源。

      在全局导航栏上，单击“**[!UICONTROL 文件]**”>“**[!UICONTROL 发布]**”。

   * 在网格视图、列表视图或详细信息视图中，单击资产名称左侧带斜杠的灰色圆形图标。

## 手动取消发布资源 {#manually-unpublishing-assets}

您可以手动取消发布各个资源。在取消发布集（如样本集或 eCatalog）时，集（或“父项”）本身将变为未发布状态。不过，集中的成员（或“子项”）不受影响；它们分别保持现有的已发布或未发布状态。

在用户界面中，发布的资源以资源名称左侧中心带有白色复选标记的绿色圆形图标表示（已发布状态）。取消发布资产后，该图标会通过斜杠变灰（未发布状态），

**手动取消发布资源:**

1. 执行以下任一操作：

   * 在“网格视图”、“列表视图”或“详细信息视图”中，选择一个或多个已发布的资产。

      在全局导航栏上，单击“**[!UICONTROL 文件]**”>“**[!UICONTROL 取消发布]**”。

   * 在网格视图、列表视图或详细信息视图中，单击资源名称左侧的绿色圆形复选标记图标。

## 获得资源发布历史记录 {#getting-an-asset-s-publish-history}

资源上次发布的日期显示在面板顶部的详细信息视图中。您可以打开详细信息视图中的“历史记录和发布的服务器”面板，获取关于发布历史记录的更多详细信息。在该面板中可以查看资源发布时间以及发布到的服务器。

## 重新发布的资源和 CDN 延迟 {#republished-assets-and-cdn-delays}

Dynamic Media Classic资产分发到内容交付网络(CDN)。 CDN 是指联成网络的计算机服务器系统，这些服务器以完全透明的方式合作，将内容（尤其是大型媒体内容）传递给最终用户。在 CDN 系统中，Web 内容存储在整个 Internet 的网络缓存中（称为边缘缓存网络）。Web内容从Web缓存中提供给最终用户，以便更快地交付。

用户首次下载网页时，这些资源即传递到 CDN 网络缓存服务器。资源存储在该服务器上，这样，当下次同一区域中有人访问该网页时，可以更快地传递缓存的相同内容。内容传递速度更快是因为其位置更接近最终用户。CDN 提高了网页显示速度。它降低了中央服务器上的带宽要求，因为内容是从边缘缓存网络传递，而不是从每个实例的中央服务器传递。

新发布的Dynamic Media Classic内容可立即提供给最终用户，并快速填充边缘缓存网络。 但重新发布的内容（与之前发布到图像服务器的图像完全同名的图像）在 CDN 上最多需要十个小时才会更新。最终用户看到的则是 CDN 网络上的网络缓存中的内容。因此，您重新发布的Dynamic Media Classic资产在10小时内不会向最终用户显示。

如果希望重新发布的图像资源在可用前的延迟时间小于 10 小时，可以刷新 CDN 上的网络缓存。刷新这些网络缓存可以从 CDN 网络缓存中删除旧内容，并将其替换为最新发布的资源。

要刷新缓存，请在全局导航栏上单击&#x200B;**[!UICONTROL 文件]** > **[!UICONTROL 无效CDN]**。 将从缓存中删除所有选定的文件。如果没有可发布资源，或者您不是公司管理员，则“从 CDN 删除”选项不可用。

>[!MORELIKETHIS]
>
>* [检查作业文件](checking-job-files.md)
* [编辑、删除、暂停和恢复重复作业](checking-job-files.md#editing-deleting-pausing-and-resuming-recurring-jobs)

