---
title: 發佈檔案
description: 「瞭解如何將資產發佈至Dynamic Media影像伺服器。 您可以發佈資產為單次使用，或安排Adobe Dynamic Media Classic定期發佈資產。 发布资源后，这些资源即可用来传送。您可以複製Adobe Dynamic Media Classic的URL呼叫，並將其新增至您的網站或應用程式。」
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/upload_and_publish_assets
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 91b73a09-c5b5-4001-b36f-6bebe65717ff
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '1729'
ht-degree: 45%

---

# 發佈檔案{#publishing-files}

您將資產發佈至Dynamic Media影像伺服器。 您可以發佈資產為單次使用，或安排Adobe Dynamic Media Classic定期發佈資產。 发布资源后，这些资源即可用来传送。您可以複製Adobe Dynamic Media Classic的URL呼叫，並將其新增至您的網站或應用程式。

Adobe Dynamic Media Classic現在支援透過HTTP/2傳送所有影像和視訊。 也就是說，影像或視訊的已發佈URL或內嵌程式碼可整合至任何接受託管資產的應用程式。 然後會透過HTTP/2通訊協定傳遞該已發佈的資產。 此傳遞方法可改善瀏覽器和伺服器的通訊方式，讓您的所有Adobe Dynamic Media Classic資產獲得更好的回應和載入時間。 另請參閱 [HTTP2傳送內容常見問答](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/http2.html#dynamic).

## 在上载之后发布 {#publish-after-uploading}

资源处于已发布或未发布的状态。依預設，您上傳至Adobe Dynamic Media Classic的任何資產都會自動標示為發佈。

如需詳細資訊，請參閱 [即時發佈通知PDF](/help/assets/rendering-instant-publish-notification.pdf).

使用以下方法将资源标记为发布：

* **[!UICONTROL 上傳後發佈]**  — 在上傳頁面底部附近，選取 **[!UICONTROL 上傳後發佈]**. 默认情况下，将处于选定状态。

* **[!UICONTROL 上傳後發佈]**  — 在「工作選項」對話方塊中，選取 **[!UICONTROL 上傳後發佈]**. 默认情况下，将处于选定状态。

如果父项资源标记为发布，则一些“子项”资源会自动标记为发布。该表列出自动标记为发布的子项资源。

| 父（组）项 | 子（成员）项 |
| --- | --- |
| 图像集 | 集中的图像。 |
| 样本集 | 集中的样本。 |
| 旋转集 | 集中的图像。 |
| 模板 | 模板文件、页面和图像。 |

在发布父图像时，也会自动将派生的图像标记为发布。派生图像包括您使用图像编辑选项调整的图像。您可以在「建置和衍生物」下的「詳細檢視」中檢視這些衍生影像。

## 建立發佈工作 {#creating-a-publish-job}

建立發佈工作以發佈您已上傳至Adobe Dynamic Media Classic伺服器，但尚未想要自動發佈的資產。 您可以執行一次性發佈工作或排程工作，以定期重複執行。 Adobe Dynamic Media Classic提供進階發佈選項，可發佈至特定伺服器，以及重新發佈已發佈資產的選項。

**创建发布作业:**

1. 在全域導覽列上，選取 **[!UICONTROL 發佈]**.
1. 在“发布”对话框中，选择是要使用一次性还是重复发布作业。

   另請參閱 [建立一次性發佈工作](publishing-files.md#creating_a_one_time_publish_job) 和 [建立週期性發佈工作](publishing-files.md#creating_a_recurring_publish_job).

1. 输入作业名称。
1. 或者，显示“高级”选项并选择这些选项。

   请参阅[高级发布选项](publishing-files.md#advanced_publish_options)。

1. 選取 **[!UICONTROL 提交發佈]**.

Adobe Dynamic Media Classic會追蹤「工作」頁面上的發佈工作。 您可以在该页中查看发布作业。

>[!NOTE]
>
>由於內容傳遞網路(CDN)上的網頁快取機制，您重新發佈的資產（先前已發佈）不會立即出現在網站上。 请参阅[重新发布的资源和 CDN 延迟](publishing-files.md#republished_assets_and_cdn_delays)。

### 建立一次性發佈工作 {#creating-a-one-time-publish-job}

選取「 」，建立一次性發佈工作 **[!UICONTROL 一次性]** 選項。

如果您希望發佈工作稍後發生，請在「發佈」頁面中選取 **[!UICONTROL 一次性]**，然後選取 **[!UICONTROL 排程供日後使用]** 下拉式清單。 使用「行事曆」和「時間」滑桿來選取執行發佈工作的日期和時間。

### 建立週期性發佈工作 {#creating-a-recurring-publish-job}

透過選取以下專案建立週期性發佈工作 **[!UICONTROL 週期性]** （在發佈頁面上）。

然後選擇重複選項： **[!UICONTROL 每日]**， **[!UICONTROL 每週]**， **[!UICONTROL 每月]**，或 **[!UICONTROL 自訂]**，然後指定您希望發佈工作重複發生的時間。 Adobe Dynamic Media Classic提供日曆工具來排程週期性發佈工作。 您可以選取 **[!UICONTROL 自訂]** 選項並在「規則」文字欄位中輸入規則，以說明自訂作業間隔。

另請參閱 [建立自訂上載或發佈工作時間間隔](checking-job-files.md#creating_a_custom_upload_or_publish_job_time_interval).

>[!NOTE]
>
>重复发布（和上载）作业在“作业”页中列出。可以转到“作业”页的“已计划”选项卡以编辑或删除计划的作业。

### 高级发布选项 {#advanced-publish-options}

您可以在“发布”页中显示高级选项，并选择这些选项以处理发布作业：

* **[!UICONTROL 發佈至]**  — 若要僅將資產發佈至特定伺服器，請選擇伺服器型別。

* **[!UICONTROL 發佈]**  — 依預設，Adobe Dynamic Media Classic只會發佈新資產且之前未發佈的資產（「上次發佈後新增的專案」選項）。 不過，您可以選取 **[!UICONTROL 完整發佈]** 亦可發佈自上次發佈後已更新或變更的資產。 選取 **[!UICONTROL 包含搜尋資料的完整]** 如果您要發佈eCatalog，且希望讀者能依關鍵字進行搜尋。

* **[!UICONTROL 工作執行身分]**  — 從清單中選擇使用者名稱。 可以在“作业”页中按用户名对作业进行排序。可以通过选择名称将发布作业与用户关联。

**[!UICONTROL HTTP通知]**  — 輸入URL以觸發後續發佈工作。

另請參閱 [使用上載或發佈工作作為觸發器](checking-job-files.md#using_an_upload_or_publish_job_as_a_trigger).)

## 取消發佈工作 {#canceling-a-publish-job}

您可以取消進行中的發佈工作。 此外，管理员还可以从公司的“作业”页中取消进行中的发布作业。

若要取消發佈工作，請前往「工作」頁面並選取 **[!UICONTROL 取消]**. 在“作业”页的“已计划”选项卡上，您可以选中或取消选中作业的“活动”列中的对应复选框以暂停或恢复作业。

>[!NOTE]
>
>取消发布作业之后，其状态更改为“正在停止”，直至达到一个安全的停止点。如果作业正从数据库获取数据，则停止发布作业可能会花费一些时间。

## 手動發佈資產 {#manually-publishing-assets}

您可以手动发布各个资源，而不是创建发布作业。在发布集（如图像集或自适应视频集）时，将发布集（或“父项”）和集中的所有成员（或“子项&quot;）。

未發佈的資產會在使用者介面中以灰色圓形圖示表示，在資產名稱的左側會有斜線（未發佈狀態）。 在发布资源后，该图标将变为绿色，并且中心带有白色复选标记（已发布状态）。

**手动发布资源:**

1. 执行以下操作之一：

   * 在网格视图、列表视图或详细信息视图中，使用标准文件选择方法选择一个或多个未发布的资源。

      在全域導覽列上，前往 **[!UICONTROL 檔案]** > **[!UICONTROL 發佈]**.

   * 在「格點檢視」、「清單檢視」或「詳細資料檢視」中，選取資產名稱左邊具有斜線的灰色圓形圖示。

## 手動取消發佈資產 {#manually-unpublishing-assets}

您可以手动取消发布各个资源。在取消发布集（如样本集或 eCatalog）时，集（或“父项”）本身将变为未发布状态。不过，集中的成员（或“子项”）不受影响；它们分别保持现有的已发布或未发布状态。

在用户界面中，发布的资源以资源名称左侧中心带有白色复选标记的绿色圆形图标表示（已发布状态）。取消發佈資產後，圖示會透過斜線變成灰色（未發佈狀態），

**手动取消发布资源:**

1. 执行以下任一操作：

   * 在「網格檢視」、「清單檢視」或「詳細資料檢視」中，選取一或多個已發佈的資產。

      在全域導覽列上，前往 **[!UICONTROL 檔案]** > **[!UICONTROL 取消發佈]**.

   * 在「格點檢視」、「清單檢視」或「詳細資訊檢視」中，選取資產名稱左側的圓形綠色勾號圖示。

## 取得資產的發佈歷史記錄 {#getting-an-asset-s-publish-history}

資產上次發佈的日期會顯示在「詳細資料檢視」的面板頂端。 您可以在「詳細資訊」檢視中開啟「歷程記錄和已發佈的伺服器」面板，以取得有關發佈歷程記錄的更多詳細資訊。 在该面板中可以查看资源发布时间以及发布到的服务器。

## 重新发布的资源和 CDN 延迟 {#republished-assets-and-cdn-delays}

Adobe Dynamic Media Classic資產會在內容傳遞網路(CDN)上發佈。 CDN 是指联成网络的计算机服务器系统，这些服务器以完全透明的方式合作，将内容（尤其是大型媒体内容）传递给最终用户。在 CDN 系统中，Web 内容存储在整个 Internet 的网络缓存中（称为边缘缓存网络）。網頁內容會從網頁快取傳送給一般使用者，以加快傳送速度。

用户首次下载网页时，这些资源即传递到 CDN 网络缓存服务器。资源存储在该服务器上，这样，当下次同一区域中有人访问该网页时，可以更快地传递缓存的相同内容。内容传递速度更快是因为其位置更接近最终用户。CDN 提高了网页显示速度。它降低了中央服务器上的带宽要求，因为内容是从边缘缓存网络传递，而不是从每个实例的中央服务器传递。

使用者可立即使用新發佈的Adobe Dynamic Media Classic內容，並快速填入Edge快取網路。 但重新发布的内容（与之前发布到图像服务器的图像完全同名的图像）在 CDN 上最多需要十个小时才会更新。最终用户看到的则是 CDN 网络上的网络缓存中的内容。因此，您的Adobe Dynamic Media Classic重新發佈資產不會在十小時內對一般使用者顯示。

如果希望重新发布的图像资源在可用前的延迟时间小于 10 小时，可以刷新 CDN 上的网络缓存。刷新这些网络缓存可以从 CDN 网络缓存中删除旧内容，并将其替换为最新发布的资源。

若要清除快取，請在全域導覽列上，前往 **[!UICONTROL 檔案]** > **[!UICONTROL 使CDN失效]**. 将从缓存中删除所有选定的文件。如果没有可发布资源，或者您不是公司管理员，则“从 CDN 删除”选项不可用。

>[!MORELIKETHIS]
>
>* [檢查工作檔案](checking-job-files.md)
>* [編輯、刪除、暫停和恢復週期性工作](checking-job-files.md#editing-deleting-pausing-and-resuming-recurring-jobs)

