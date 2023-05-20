---
title: 使用Adobe Analytics Instrumentation Kit檢測檢視器
description: 瞭解如何使用Adobe Dynamic Media Classic中的Adobe Analytics Instrumentation Kit檢測檢視器。
uuid: cf9a4002-966d-4641-9cd0-2ee8b5454f60
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: a2824244-1755-42de-a167-42af117cf038
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 9ea1546d-e6d1-4ba4-8fa1-26b4e69375ba
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 20%

---

# 使用Adobe Analytics Instrumentation Kit檢測檢視器{#instrumenting-a-viewer-using-the-adobe-analytics-instrumentation-kit}

您可以使用Adobe Analytics Instrumentation Kit將HTML5檢視器與Adobe Analytics整合。

如果您使用任何預先定義的Adobe Dynamic Media Classic HTML5檢視器預設集，這些預設集已包含所有用於傳送資料至Adobe Analytics的實作程式碼；您不需要進一步檢測。

## 從Adobe Dynamic Media Classic設定Adobe Analytics追蹤 {#set-up-adobe-analytics-tracking-from-scene-publishing-system}

對於所有HTML5檢視器，將以下JavaScript新增至HTML容器，通常在 &lt;head> 元素：

```as3
<!-- ***** Adobe Analytics Tracking ***** --><script type="text/javascript" src="https://s7d6.scene7.com/s7viewers/s_code.jsp?company=<Adobe Dynamic Media Classic Company ID>&preset=companypreset-1"></script>
```

位置 `Adobe Dynamic Media Classic Company ID` 設為Adobe Dynamic Media Classic公司名稱。 和 `&preset` 是選用專案，除非公司預設集名稱不是 `companypreset`. 在這種情況下，可能是 `companypreset-1, companypreset-2`、等等。 数字越大预设实例越新。若要判斷正確的公司預設值名稱，請選取「 」 **[!UICONTROL 複製URL]** ，然後檢視 `preset=`用於尋找公司預設集名稱的引數。

繼續進行，現在新增將檢視器事件傳輸至Adobe Analytics追蹤代碼的函式。

新增 `s7ComponentEvent()` 容器HTML（或JSP、ASPX或其他）的函式：

```as3
function s7ComponentEvent(objectId, componentClass, instanceName, timeStamp, eventData) {     s7track(eventData); }
```

函式名稱區分大小寫。 唯一傳遞至的引數 `s7componentEvent`最後一個要求為： `eventData`. 位置 `s7track()` 定義於上述包含的s_code.jsp中。 和 `s7track` 處理每個事件的所有追蹤。 （要进一步自定义传送到 Adobe Analytics 的数据，可以在该区域执行此操作。）

## 啟用HREF和ITEM事件 {#enabling-href-and-item-events}

可以通过图像映射编辑，在查看器中启用 HREF（变换）和 ITEM（鼠标单击/点按）事件。在与查看器内容关联的图像映射中定义 HREF 和 ITEM 标识符。新增 `&rolloverKey=` 引數對應影像地圖中的HREF值。
