---
title: 发布文件
description: “了解如何将资源发布到Dynamic Media图像服务器。 您可以一次性发布资源，也可以安排Adobe Dynamic Media Classic按定期计划发布资源。 发布资源后，这些资源即可用来传送。您可以从Adobe Dynamic Media Classic复制URL调用，并将其添加到您的网站或应用程序。”
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/upload_and_publish_assets
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 91b73a09-c5b5-4001-b36f-6bebe65717ff
topic: Content Management
level: Intermediate
source-git-commit: d82f816553f807b514f4690827dab672a6baf690
workflow-type: tm+mt
source-wordcount: '1729'
ht-degree: 45%

---

# 发布文件{#publishing-files}

您可以将资源发布到Dynamic Media图像服务器。 您可以一次性发布资源，也可以安排Adobe Dynamic Media Classic按定期计划发布资源。 发布资源后，这些资源即可用来传送。您可以从Adobe Dynamic Media Classic复制URL调用，并将其添加到您的网站或应用程序。

Adobe Dynamic Media Classic现在支持通过HTTP/2交付所有图像和视频。 即，图像或视频的已发布URL或嵌入代码可与接受托管资产的任何应用程序集成。 随后，该已发布的资产将通过HTTP/2协议进行交付。 这种交付方法改进了浏览器和服务器的通信方式，从而可以为所有Adobe Dynamic Media Classic资源提供更好的响应和加载时间。 参见 [http2内容交付常见问题解答](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/http2.html#dynamic).

## 在上载之后发布 {#publish-after-uploading}

资源处于已发布或未发布的状态。默认情况下，您上传到Adobe Dynamic Media Classic的任何资源都会自动标记为发布。

欲了解更多信息，请参见 [即时发布通知PDF](/help/using/assets/rendering-instant-publish-notification.pdf).

使用以下方法将资源标记为发布：

* **[!UICONTROL 上传后发布]**  — 在上传页面底部附近，选择 **[!UICONTROL 上传后发布]**. 默认情况下，将处于选定状态。

* **[!UICONTROL 上传后发布]**  — 在“作业选项”对话框中，选择 **[!UICONTROL 上传后发布]**. 默认情况下，将处于选定状态。

如果父项资源标记为发布，则一些“子项”资源会自动标记为发布。该表列出自动标记为发布的子项资源。

| 父（组）项 | 子（成员）项 |
| --- | --- |
| 图像集 | 集中的图像。 |
| 样本集 | 集中的样本。 |
| 旋转集 | 集中的图像。 |
| 模板 | 模板文件、页面和图像。 |

在发布父图像时，也会自动将派生的图像标记为发布。派生图像包括您使用图像编辑选项调整的图像。您可以在“构建和派生”下的“详细信息视图”中查看这些派生的图像。

## 创建发布作业 {#creating-a-publish-job}

创建发布作业以发布已上传到Adobe Dynamic Media Classic服务器但尚未自动发布的资产。 您可以执行一次性发布作业，也可以将作业安排为定期重复执行。 Adobe Dynamic Media Classic提供高级发布选项以发布到特定服务器，并提供重新发布已发布资产的选项。

**创建发布作业:**

1. 在全局导航栏上，选择 **[!UICONTROL Publish]**.
1. 在“发布”对话框中，选择是要使用一次性还是重复发布作业。

   参见 [创建一次性发布作业](publishing-files.md#creating_a_one_time_publish_job) 和 [创建定期发布作业](publishing-files.md#creating_a_recurring_publish_job).

1. 输入作业名称。
1. 或者，显示“高级”选项并选择这些选项。

   请参阅[高级发布选项](publishing-files.md#advanced_publish_options)。

1. 选择 **[!UICONTROL 提交发布]**.

Adobe Dynamic Media Classic跟踪“作业”页面上的发布作业。 您可以在该页中查看发布作业。

>[!NOTE]
>
>由于内容交付网络(CDN)上的Web缓存机制，您重新发布的资产（之前已发布）不会立即显示在您的网站上。 请参阅[重新发布的资源和 CDN 延迟](publishing-files.md#republished_assets_and_cdn_delays)。

### 创建一次性发布作业 {#creating-a-one-time-publish-job}

通过选择 **[!UICONTROL 一次性]** 选项。

如果希望发布作业稍后发生，请在“发布”页面中，选择 **[!UICONTROL 一次性]**，然后选择 **[!UICONTROL 以后计划]** 下拉菜单。 使用日历和时间滑块选择运行发布作业的日期和时间。

### 创建定期发布作业 {#creating-a-recurring-publish-job}

通过选择创建循环发布作业 **[!UICONTROL 周期性]** 在“发布”页面上。

然后选择重复选项 **[!UICONTROL 每日]**， **[!UICONTROL 每周]**， **[!UICONTROL 每月]**，或 **[!UICONTROL 自定义]**，然后指定您希望发布作业重复发生的时间。 Adobe Dynamic Media Classic提供了用于计划定期发布作业的日历工具。 您可以选择 **[!UICONTROL 自定义]** 选项并在“规则”文本字段中输入规则以描述自定义作业间隔。

参见 [创建自定义上载或发布作业时间间隔](checking-job-files.md#creating_a_custom_upload_or_publish_job_time_interval).

>[!NOTE]
>
>重复发布（和上载）作业在“作业”页中列出。可以转到“作业”页的“已计划”选项卡以编辑或删除计划的作业。

### 高级发布选项 {#advanced-publish-options}

您可以在“发布”页中显示高级选项，并选择这些选项以处理发布作业：

* **[!UICONTROL 发布到]**  — 要仅将资产发布到特定服务器，请选择服务器类型。

* **[!UICONTROL Publish]**  — 默认情况下，Adobe Dynamic Media Classic仅发布新资产，并且以前未发布过这些资产（新的上次发布时间选项）。 但是，您可以选择 **[!UICONTROL 完全发布]** 用于同时发布自上次发布以来已更新或更改的资产。 选择 **[!UICONTROL 包含搜索数据的完整]** 如果您要发布eCatalog，并且希望读者能够按关键字搜索它。

* **[!UICONTROL 作业运行方式]**  — 从列表中选择用户名。 可以在“作业”页中按用户名对作业进行排序。可以通过选择名称将发布作业与用户关联。

**[!UICONTROL HTTP通知]**  — 输入URL以触发后续发布作业。

参见 [使用上载或发布作业作为触发器](checking-job-files.md#using_an_upload_or_publish_job_as_a_trigger).)

## 取消发布作业 {#canceling-a-publish-job}

您可以取消正在进行的发布作业。 此外，管理员还可以从公司的“作业”页中取消进行中的发布作业。

要取消发布作业，请转到“作业”页面并选择 **[!UICONTROL 取消]**. 在“作业”页的“已计划”选项卡上，您可以选中或取消选中作业的“活动”列中的对应复选框以暂停或恢复作业。

>[!NOTE]
>
>取消发布作业之后，其状态更改为“正在停止”，直至达到一个安全的停止点。如果作业正从数据库获取数据，则停止发布作业可能会花费一些时间。

## 手动发布资产 {#manually-publishing-assets}

您可以手动发布各个资源，而不是创建发布作业。在发布集（如图像集或自适应视频集）时，将发布集（或“父项”）和集中的所有成员（或“子项&quot;）。

未发布的资源在用户界面中由资源名称左侧的带斜杠（未发布状态）的灰色圆形图标表示。 在发布资源后，该图标将变为绿色，并且中心带有白色复选标记（已发布状态）。

**手动发布资源:**

1. 执行以下操作之一：

   * 在网格视图、列表视图或详细信息视图中，使用标准文件选择方法选择一个或多个未发布的资源。

     在全局导航栏上，转到 **[!UICONTROL 文件]** > **[!UICONTROL Publish]**.

   * 在“网格视图”、“列表视图”或“详细信息视图”中，选择资源名称左侧的带斜杠的灰色倒圆角图标。

## 手动取消发布资产 {#manually-unpublishing-assets}

您可以手动取消发布各个资源。在取消发布集（如样本集或 eCatalog）时，集（或“父项”）本身将变为未发布状态。不过，集中的成员（或“子项”）不受影响；它们分别保持现有的已发布或未发布状态。

在用户界面中，发布的资源以资源名称左侧中心带有白色复选标记的绿色圆形图标表示（已发布状态）。取消发布资产后，图标会变为灰色，并在其中插入一个斜杠（未发布状态）。

**手动取消发布资源:**

1. 执行以下任一操作：

   * 在“网格视图”、“列表视图”或“详细信息视图”中，选择一个或多个已发布的资源。

     在全局导航栏上，转到 **[!UICONTROL 文件]** > **[!UICONTROL 取消发布]**.

   * 在“网格视图”、“列表视图”或“详细信息视图”中，选择资源名称左侧的绿色圆环复选标记图标。

## 获取资源的发布历史记录 {#getting-an-asset-s-publish-history}

上次发布资产的日期将显示在面板顶部的详细信息视图中。 您可以通过在“详细信息”视图中打开“历史记录和已发布的服务器”面板，获取有关发布历史记录的更多详细信息。 在该面板中可以查看资源发布时间以及发布到的服务器。

## 重新发布的资源和 CDN 延迟 {#republished-assets-and-cdn-delays}

Adobe Dynamic Media Classic资源在内容交付网络(CDN)上分发。 CDN 是指联成网络的计算机服务器系统，这些服务器以完全透明的方式合作，将内容（尤其是大型媒体内容）传递给最终用户。在 CDN 系统中，Web 内容存储在整个 Internet 的网络缓存中（称为边缘缓存网络）。Web内容从Web缓存交付给最终用户，以实现更快的交付。

用户首次下载网页时，这些资源即传递到 CDN 网络缓存服务器。资源存储在该服务器上，这样，当下次同一区域中有人访问该网页时，可以更快地传递缓存的相同内容。内容传递速度更快是因为其位置更接近最终用户。CDN 提高了网页显示速度。它降低了中央服务器上的带宽要求，因为内容是从边缘缓存网络传递，而不是从每个实例的中央服务器传递。

新发布的Adobe Dynamic Media Classic内容可立即提供给最终用户并快速填充边缘缓存网络。 但重新发布的内容（与之前发布到图像服务器的图像完全同名的图像）在 CDN 上最多需要十个小时才会更新。最终用户看到的则是 CDN 网络上的网络缓存中的内容。因此，您的Adobe Dynamic Media Classic重新发布的资源在十小时内不会向最终用户显示。

如果希望重新发布的图像资源在可用前的延迟时间小于 10 小时，可以刷新 CDN 上的网络缓存。刷新这些网络缓存可以从 CDN 网络缓存中删除旧内容，并将其替换为最新发布的资源。

要刷新缓存，请在全局导航栏上，转到 **[!UICONTROL 文件]** > **[!UICONTROL 使CDN失效]**. 将从缓存中删除所有选定的文件。如果没有可发布资源，或者您不是公司管理员，则“从 CDN 删除”选项不可用。

>[!MORELIKETHIS]
>
>* [检查作业文件](checking-job-files.md)
>* [编辑、删除、暂停和恢复定期作业](checking-job-files.md#editing-deleting-pausing-and-resuming-recurring-jobs)
