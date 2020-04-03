---
title: 发布文件
seo-title: 发布文件
description: 'null'
seo-description: 了解如何发布文件。
uuid: cdcf519b-4c1e-430b-b43a-2f20f75071b1
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/upload_and_publish_assets
discoiquuid: 39099bc0-9228-46f0-9bee-3542059f4695
translation-type: tm+mt
source-git-commit: 917ba4469b5ef22e62c572f80008e470dccdebe4

---


# 发布文件{#publishing-files}

您可以将资产发布到Dynamic Media Image Server。 您可以一次性发布资产，也可以安排Dynamic Media Classic在循环计划中发布资产。 发布资源后，这些资源即可用来传送。您可以从 Scene7 Publishing System 中复制 URL 调用，并将其添加到您的网站或应用程序中。

Scene7 Publishing System现在支持通过HTTP/2投放所有图像和视频。 即，图像或视频的已发布URL或嵌入代码可与接受托管资产的任何应用程序集成。 然后，通过HTTP/2协议传送已发布的资产。 此投放方法改进了浏览器和服务器通信的方式，使所有Dynamic Media Classic资源的响应和加载时间都更好。 请参 [阅HTTP2投放内容常见问题解答](https://docs.adobe.com/content/docs/en/aem/6-2/administer/integration/marketing-cloud/scene7/http2faq.html)。

## 在上载之后发布 {#publish-after-uploading}

资源处于已发布或未发布的状态。默认情况下，上传到Dynamic Media Classic中的所有资产都会自动标记为发布。

有关详细信息，请参阅“即 [时发布声明”PDF](/help/assets/rendering-instant-publish-notification.pdf)。

使用以下方法将资源标记为发布：

* **上传后发**&#x200B;布在上传页面底部附近，选择上传后发布。 默认情况下，将处于选定状态。

* **上传后发布**&#x200B;在“作业选项”对话框中，选择“上传后发布”。 默认情况下，将处于选定状态。

如果父项资源标记为发布，则一些“子项”资源会自动标记为发布。该表列出自动标记为发布的子项资源。

| 父（组）项 | 子（成员）项 |
|--- |--- |
| 图像集 | 集中的图像。 |
| 样本集 | 集中的样本。 |
| 旋转集 | 集中的图像。 |
| 模板 | 模板文件、页面和图像。 |

在发布父图像时，也会自动将派生的图像标记为发布。派生图像包括您使用图像编辑选项调整的图像。您可以在“构建和派生”下的详细信息视图中查看这些派生图像。

## 创建发布作业 {#creating-a-publish-job}

创建发布作业，以发布已上传到Dynamic Media Classic服务器的资产，但选择尚未自动发布这些资产。 您可以执行一次性发布作业，或者计划定期循环发布作业。Dynamic Media Classic优惠高级发布选项，用于发布到特定服务器，以及用于重新发布已发布的资产的选项。

**创建发布作业**

1. 在全局导航栏上，单击“**发布**”。
1. 在“发布”对话框中，选择是要使用一次性还是重复发布作业。

   请参阅[创建一次性发布作业](publishing-files.md#creating_a_one_time_publish_job)和[创建重复发布作业](publishing-files.md#creating_a_recurring_publish_job)。

1. 输入作业名称。
1. 或者，显示“高级”选项并选择这些选项。

   请参阅[高级发布选项](publishing-files.md#advanced_publish_options)。

1. 单击“**提交发布**”。

SPS 在“作业”页中跟踪发布作业。您可以在该页中查看发布作业。

>[!NOTE]
>
>由于内容传递网络 (CDN) 上的网络缓存机制，您重新发布（以前发布）的资源不会立即显示在网站上。请参阅[重新发布的资源和 CDN 延迟](publishing-files.md#republished_assets_and_cdn_delays)。

### 创建一次性发布作业 {#creating-a-one-time-publish-job}

在“发布”页中，选择“一次”选项以创建一次性发布作业。

如果希望在以后发布作业，选择“时间”菜单，然后选择“日后计划”。然后使用“日历和时间”滑块来选择执行发布作业的日期和时间。

### 创建重复发布作业 {#creating-a-recurring-publish-job}

在“发布”页中，选择“重复”选项以创建重复发布作业。

然后选择“重复”选项（“每天”、“每周”、“每月”或“自定义”），以声明重复发布作业的时间。Dynamic Media Classic提供日历工具，用于安排重复发布作业。 您可以选择“自定义”选项，并在“规则”框中输入规则来描述自定义作业时间间隔。

请参阅[创建自定义上载或发布作业时间间隔](checking-job-files.md#creating_a_custom_upload_or_publish_job_time_interval)。

>[!NOTE]
>
>重复发布（和上载）作业在“作业”页中列出。可以转到“作业”页的“已计划”选项卡以编辑或删除计划的作业。

### 高级发布选项 {#advanced-publish-options}

您可以在“发布”页中显示高级选项，并选择这些选项以处理发布作业：

* **发布到**&#x200B;选择一种服务器类型，以仅将资产发布到特定服务器，而不是所有服务器。

* **发布**&#x200B;默认情况下，SPS仅发布新资源，且之前尚未发布（“自上次发布后新建”选项）。 但也可以选择“完全发布”，从而发布自上次发布以来已经更新或更改的资源。如果要发布 eCatalog 并且希望读者能够通过关键字搜索到该 eCatalog，则选择“全部（包含搜索数据）”。

* **运行作业**&#x200B;从列表中选择用户名。 可以在“作业”页中按用户名对作业进行排序。可以通过选择名称将发布作业与用户关联。

**HTTP通知**&#x200B;输入URL以触发后续发布作业。

请参阅[使用上载或发布作业作为触发器](checking-job-files.md#using_an_upload_or_publish_job_as_a_trigger)。

## 取消发布作业 {#canceling-a-publish-job}

您可以取消进行中的发布作业。此外，管理员还可以从公司的“作业”页中取消进行中的发布作业。

要取消发布作业，请转到“作业”页并单击“取消”。在“作业”页的“已计划”选项卡上，您可以选中或取消选中作业的“活动”列中的对应复选框以暂停或恢复作业。

>[!NOTE]
>
>取消发布作业之后，其状态更改为“正在停止”，直至达到一个安全的停止点。如果作业正从数据库获取数据，则停止发布作业可能会花费一些时间。

## 手动发布资源 {#manually-publishing-assets}

您可以手动发布各个资源，而不是创建发布作业。在发布集（如图像集或自适应视频集）时，将发布集（或“父项”）和集中的所有成员（或“子项&quot;）。

在用户界面中，未发布的资源以资源名称左侧带有贯穿斜线的灰色圆形图标表示（未发布状态）。在发布资源后，该图标将变为绿色，并且中心带有白色复选标记（已发布状态）。

**手动发布资源**

1. 执行以下操作之一：

   * 在网格视图、列表视图或详细信息视图中，使用标准文件选择方法选择一个或多个未发布的资源。

      在全局导航栏上，单击“**文件”>“发布**”。

   * 在网格视图、列表视图或详细信息视图中，单击资源名称左侧带有贯穿斜线的灰色圆形图标。

## 手动取消发布资源 {#manually-unpublishing-assets}

您可以手动取消发布各个资源。在取消发布集（如样本集或 eCatalog）时，集（或“父项”）本身将变为未发布状态。不过，集中的成员（或“子项”）不受影响；它们分别保持现有的已发布或未发布状态。

在用户界面中，发布的资源以资源名称左侧中心带有白色复选标记的绿色圆形图标表示（已发布状态）。在取消发布资源后，图标将变为带有贯穿斜线的灰色图标（未发布状态）。

**手动取消发布资源**

1. 执行以下操作之一：

   * 在网格视图、列表视图或详细信息视图中，选择一个或多个发布的资源。

      On the Global Navigation Bar, click **File > **Unpublish**.

   * 在网格视图、列表视图或详细信息视图中，单击资源名称左侧的绿色圆形复选标记图标。

## 获得资源发布历史记录 {#getting-an-asset-s-publish-history}

资源上次发布的日期显示在面板顶部的详细信息视图中。您可以打开详细信息视图中的“历史记录和发布的服务器”面板，获取关于发布历史记录的更多详细信息。在该面板中可以查看资源发布时间以及发布到的服务器。

## 重新发布的资源和 CDN 延迟 {#republished-assets-and-cdn-delays}

Dynamic Media Classic资源分发在内容投放网络(CDN)上。 CDN 是指联成网络的计算机服务器系统，这些服务器以完全透明的方式合作，将内容（尤其是大型媒体内容）传递给最终用户。在 CDN 系统中，Web 内容存储在整个 Internet 的网络缓存中（称为边缘缓存网络）。Web 内容从这些网络缓存传递到最终用户，从而提高了传递速度。

用户首次下载网页时，这些资源即传递到 CDN 网络缓存服务器。资源存储在该服务器上，这样，当下次同一区域中有人访问该网页时，可以更快地传递缓存的相同内容。内容传递速度更快是因为其位置更接近最终用户。CDN 提高了网页显示速度。它降低了中央服务器上的带宽要求，因为内容是从边缘缓存网络传递，而不是从每个实例的中央服务器传递。

新发布的Dynamic Media Classic内容可立即向最终用户提供，并可快速填充边缘缓存网络。 但重新发布的内容（与之前发布到图像服务器的图像完全同名的图像）在 CDN 上最多需要十个小时才会更新。最终用户看到的则是 CDN 网络上的网络缓存中的内容。因此，您的Dynamic Media Classic重新发布的资产在十小时内可能无法显示给最终用户。

如果希望重新发布的图像资源在可用前的延迟时间小于 10 小时，可以刷新 CDN 上的网络缓存。刷新这些网络缓存可以从 CDN 网络缓存中删除旧内容，并将其替换为最新发布的资源。

要刷新缓存，请单击“文件”>“使 CDN 失效”。将从缓存中删除所有选定的文件。如果没有可发布资源，或者您不是公司管理员，则“从 CDN 删除”选项不可用。

>[!MORELIKETHIS]
>
>* [Checking job files](checking-job-files.md)
>* [编辑、删除、暂停和恢复重复作业](checking-job-files.md#editing-deleting-pausing-and-resuming-recurring-jobs)

