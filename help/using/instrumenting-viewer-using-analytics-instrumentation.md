---
title: 使用Adobe Analytics检测工具包检测查看器
description: 了解如何使用Adobe Dynamic Media Classic中的Adobe Analytics Instrumentation Kit检测查看器。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Developer,Admin,User
exl-id: 9ea1546d-e6d1-4ba4-8fa1-26b4e69375ba
topic: Integrations, Development
level: Experienced
autotag-review: '2026-05-13T19:51:34.654Z'
TQID: 'https://experienceleague.adobe.com/veMzN35J6flKfCAFvdPfZPgxJ9oGy0LYYGhjr-hZLcY'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
level_v2:
  - id: d378ca77-2da1-4f39-ad92-1917fe974a38
topic_v2:
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
source-git-commit: 0d05ca7402db1d8894db1127088905143fb97cff
workflow-type: tm+mt
source-wordcount: 307
ht-degree: 14%

---

# 使用Adobe Analytics检测工具包检测查看器{#instrumenting-a-viewer-using-the-adobe-analytics-instrumentation-kit}

您可以使用Adobe Analytics Instrumentation Kit将HTML5查看器与Adobe Analytics集成。

如果您使用任何预定义的Adobe Dynamic Media Classic HTML5查看器预设，则这些预设已包含所有用于向Adobe Analytics发送数据的实施代码。 您无需添加任何进一步的检测。

## 从Adobe Dynamic Media Classic设置Adobe Analytics跟踪 {#set-up-adobe-analytics-tracking-from-scene-publishing-system}

对于所有HTML5查看器，将以下JavaScript添加到HTML容器中（通常在&lt;head>元素中）：

```as3
<!-- ***** Adobe Analytics Tracking ***** --><script type="text/javascript" src="https://s7d6.scene7.com/s7viewers/s_code.jsp?company=<Adobe Dynamic Media Classic Company ID>&preset=companypreset-1"></script>
```

其中，`Adobe Dynamic Media Classic Company ID`设置为Adobe Dynamic Media Classic公司名称。 而`&preset`是可选的。 如果公司预设名称不是`companypreset`，则它不是可选的。 在这种情况下，可以是`companypreset-1, companypreset-2`，依此类推。 数字越大预设实例越新。 要确定正确的公司预设值名称，请选择&#x200B;**[!UICONTROL 复制URL]**，然后查看`preset=`参数以查找公司预设名称。

继续，现在添加一个将查看器事件传输到Adobe Analytics跟踪代码的函数。

将`s7ComponentEvent()`函数添加到容器HTML（或JSP、ASPX或其他）：

```as3
function s7ComponentEvent(objectId, componentClass, instanceName, timeStamp, eventData) {     s7track(eventData); }
```

函数名称区分大小写。 传递给`s7componentEvent`的唯一一个必需参数是最后一个参数： `eventData`。 其中`s7track()`在上面包含的s_code.jsp中定义。 并且`s7track`处理每个事件的所有跟踪。 （在此区域，您可以进一步自定义传输到Adobe Analytics的数据。）

## 启用HREF和ITEM事件 {#enabling-href-and-item-events}

可以通过图像映射编辑，在查看器中启用 HREF（变换）和 ITEM（鼠标单击/点按）事件。 在与查看器内容关联的图像映射中定义 HREF 和 ITEM 标识符。 向图像映射中的HREF值添加一个`&rolloverKey=`参数。
