---
title: 設定Adobe Analytics報表
description: 瞭解如何在Adobe Dynamic Media Classic中設定Adobe Analytics報表。
uuid: bf210f68-dcb0-4e86-be04-0a8b2117ef2a
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: f4c8c2b3-cc95-416f-9a5d-da81c231dfc2
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: d9fda3b8-7da8-4a30-a5f8-9bb34ec1b43d
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '1231'
ht-degree: 27%

---

# 設定Adobe Analytics報表{#configuring-adobe-analytics-reports}

若要告訴Adobe Analytics您想在Adobe Analytics報表中取得哪些資訊，請前往Adobe Analytics設定畫面。 設定報表後，此畫面會針對您想要取得相關資訊的每個檢視器事件，列出相對應的Adobe Analytics變數和Adobe Dynamic Media Classic變數。 這些檢視器事件 — Adobe Analytics變數 — Adobe Dynamic Media Classic變陣列合會決定要報告的資訊。

除了將檢視器事件與變數建立關聯之外， Adobe Analytics設定畫面還提供啟用、編輯和刪除檢視器事件的工具。

>[!NOTE]
>
>每當您在Adobe Analytics中變更Adobe Analytics報表設定時，請務必從Adobe Dynamic Media Classic中重新登入Adobe Analytics、重新儲存Adobe Analytics組態設定，然後重新發佈。

请参阅[登录到 Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics)。

另請參閱 [發佈設定資訊](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information).

## 將Adobe Analytics變數指派給Adobe Dynamic Media Classic檢視器事件和變數 {#assigning-adobe-analytics-variables-to-scene-viewer-events-and-variables}

使用Adobe Analytics設定畫面將檢視器事件與Adobe Analytics變數和Adobe Dynamic Media Classic變數建立關聯。 請為每個檢視器事件選擇一個Adobe Analytics變數和一個Adobe Dynamic Media Classic變數。 有关打开“Adobe Analytics 配置”屏幕的说明，请参阅[登录到 Adobe Analytics](log-analytics.md#log_in_to_adobe_analytics)。

**若要將Adobe Analytics變數指派給Adobe Dynamic Media Classic檢視器事件和變數：**

1. 從Adobe Dynamic Media Classic登入Adobe Analytics並選取報表套裝後，請在「Adobe Analytics設定」頁面的右側表格欄中，選取以啟動檢視器事件 **[!UICONTROL 啟用]**.
1. 在「變數」欄下，選取所需「檢視器事件」的箭頭按鈕，以顯示變數配對選擇器。

   请参阅[查看器事件](configuring-analytics-reports.md#viewer_events)。

1. 新增Adobe Dynamic Media Classic變數。

   另請參閱 [Adobe Dynamic Media Classic變數](configuring-analytics-reports.md#scene7_variables).

1. 添加一个 Adobe Analytics 变量。
1. （選用）若要新增其他變陣列，請選取 **[!UICONTROL 新增]**.
1. 選取 **[!UICONTROL 儲存]**.

   在您選取之後 **[!UICONTROL 儲存]**、檢視器事件、其Adobe Analytics變數及其Adobe Dynamic Media Classic變數會列在Adobe Analytics設定畫面中。

1. 在右下角，選取 **[!UICONTROL 關閉]**.
1. 前往 **[!UICONTROL 發佈]** > **[!UICONTROL 提交發佈]** 以執行「影像伺服」發佈。

   您必須發佈，才能在Adobe Dynamic Media Classic伺服器上取得檢視器中包含的資訊。

### 查看器事件 {#viewer-events}

檢視器事件說明使用者使用Adobe Dynamic Media Classic檢視器執行的動作。 當使用者起始特定動作（例如選取縮圖或開始或停止視訊）時，檢視器會將事件連同與該事件相關聯的資料「廣播」至網頁。

下表說明可新增至「Adobe Analytics設定」畫面的檢視器事件。

| 查看器事件 | HTML5 查看器平台支持和查看器 | 说明 |
| --- | --- | --- |
| LOAD | **X**（eCatalog、弹出、旋转集、视频、缩放） | 當使用者啟動檢視器時 |
| PAGE | **X** (eCatalog) | 在eCatalogs中，當使用者轉動頁面時；在目標縮放檢視器中，當使用者選取不同的目標或色票時。 |
| SWAP | **X**（eCatalog、弹出、旋转集、视频、缩放） | 當使用者選擇不同的縮圖來檢視不同的影像時。 |
| ITEM | **X** (eCatalog) | 在支持已定义变换的图像映射的查看器中，用户将指针悬停在图像映射上以读取变换文本时。 |
| HREF | **X** (eCatalog) | 在支援「影像地圖」的檢視器中，當使用者在「影像地圖」中選取URL時。 |
| TARGET |  | 在目標縮放檢視器中，使用者選取縮放目標以縮放至影像的一部分時。 |
| SEARCH |  | 在 eCatalog 中用户执行关键词搜索时。 |
| PLAY | **X**（视频） | 在視訊檢視器中，當使用者選取「播放」開始播放視訊時。<br><br>**注意：** 如果您使用Adobe Analytics心率型視訊報表，在Adobe Dynamic Media Classic中設定Adobe Analytics時，不需要將任何變數對應至此檢視器事件。 視訊心率適用於現成可用的Adobe Dynamic Media Classic HTML5視訊和MixedMedia檢視器。 视频播放器生成跟踪数据以在 Adobe Analytics 视频报告中查看。另請參閱 [啟用Adobe Analytics視訊報表](enabling-analytics-video-reports.md). |
| PAUSE | **X**（视频） | 在視訊檢視器中，當使用者選取 **[!UICONTROL 暫停]** 以凍結視訊。<br><br>**注意：** 如果您使用Adobe Analytics心率型視訊報表，在Adobe Dynamic Media Classic中設定Adobe Analytics時，不需要將任何變數對應至此檢視器事件。 視訊心率適用於現成可用的Adobe Dynamic Media Classic HTML5視訊和MixedMedia檢視器。 视频播放器生成跟踪数据以在 Adobe Analytics 视频报告中查看。另請參閱 [啟用Adobe Analytics視訊報表](enabling-analytics-video-reports.md). |
| STOP | **X**（视频） | 在視訊檢視器中，當使用者選取 **[!UICONTROL 停止]** 以停止播放視訊。<br><br>**注意：** 如果您使用Adobe Analytics心率型視訊報表，在Adobe Dynamic Media Classic中設定Adobe Analytics時，不需要將任何變數對應至此檢視器事件。 視訊心率適用於現成可用的Adobe Dynamic Media Classic HTML5視訊和MixedMedia檢視器。 视频播放器生成跟踪数据以在 Adobe Analytics 视频报告中查看。另請參閱 [啟用Adobe Analytics視訊報表](enabling-analytics-video-reports.md). |
| MILESTONE | **X**  (视频) | 在视频查看器中，用户在观看到视频的 0%、25%、50%、75% 或 100% 时会生成里程碑事件。<br><br>**注意：** 如果您使用Adobe Analytics心率型視訊報表，在Adobe Dynamic Media Classic中設定Adobe Analytics時，不需要將任何變數對應至此檢視器事件。 視訊心率適用於現成可用的Adobe Dynamic Media Classic HTML5視訊和MixedMedia檢視器。 视频播放器生成跟踪数据以在 Adobe Analytics 视频报告中查看。另請參閱 [啟用Adobe Analytics視訊報表](enabling-analytics-video-reports.md). |
| 样本 | **X** （弹出、缩放） | 此檢視器事件對應至Adobe Dynamic Media Classic中的頁面檢視器事件。 |
| 缩放 | **X**（eCatalog、旋转集、缩放） | Adobe Analytics 不进行跟踪。 |
| 平移 | **X**（eCatalog、旋转集、缩放） | Adobe Analytics 不进行跟踪。 |
| 旋转 | **X**（旋转集） | Adobe Analytics 不进行跟踪。 |

### Adobe Dynamic Media Classic變數 {#scene-variables}

針對Adobe Analytics設定畫面上的每個檢視器事件，選擇一個Adobe Analytics變數和 *Adobe Dynamic Media Classic變數*. Adobe Dynamic Media Classic變數代表您可以為報表取得的資料。 例如，`searchTerm` 变量可列出在 eCatalog 搜索中使用的关键字。

下表說明Adobe Dynamic Media Classic變數：

| Adobe Dynamic Media Classic變數 | 说明 |
| --- | --- |
| asset | Adobe Dynamic Media Classic資產ID或視訊路徑檔案。 |
| viewerId | 指定给各个不同的查看器类型的任意编号。 |
| pageLabel | 在 eCatalog 中，查看器显示的页面。 |
| label | 标签值（字符串）。 |
| frame | 图像集中的页面或页面引用。 |
| rollover_keyRaw | 完整的 HREF 值，不仅是已处理部分。 |
| rollover_keyProc | 在图像映射中引用的项目的 ID（对 href 和项目事件有效）。 |
| searchTerm | 在 eCatalog 搜索中使用的搜索词。 |
| timeStamp | 在视频查看器中选择的“播放”、“停止”和“暂停”。 |
| progress | 完成的里程碑事件的百分比。 |
| targetId | ID 值（数值）。 |

## 啟動、編輯和刪除檢視器事件 {#activating-editing-and-deleting-viewer-events}

可以在“Adobe Analytics 配置”屏幕上激活、编辑和删除查看器事件：

* **啟動**  — 選取 **[!UICONTROL 啟用]** 以啟動或 **[!UICONTROL 停用]** 停用選取的檢視器事件。

* **編輯**  — 選取檢視器事件並選取 **[!UICONTROL 檢視/編輯]** 變數灰色按鈕。 在「Adobe Dynamic Media Classic變數」和「Adobe Analytics變數」下拉式清單中，從各個不同的清單中選擇不同的變數。 如需詳細資訊，請參閱 [將Adobe Analytics變數指派給Adobe Dynamic Media Classic檢視器事件和變數](#assigning-adobe-analytics-variables-to-scene-viewer-events-and-variables).

* **刪除**  — 選取檢視器事件，然後選取 **[!UICONTROL 檢視/編輯]** 變數灰色按鈕。 選取 **[!UICONTROL 刪除]**.
