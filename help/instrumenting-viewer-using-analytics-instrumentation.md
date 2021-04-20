---
title: 使用 Adobe Analytics 仪器包实施查看器
description: 了解如何使用Adobe Analytics Instrumentation Kit对查看器进行指导。
uuid: cf9a4002-966d-4641-9cd0-2ee8b5454f60
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: a2824244-1755-42de-a167-42af117cf038
feature: Dynamic Media Classic
role: Data Engineer,Administrator,Business Practitioner
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 35%

---


# 使用 Adobe Analytics 仪器包实施查看器{#instrumenting-a-viewer-using-the-adobe-analytics-instrumentation-kit}

您可以使用Adobe Analytics Instrumentation Kit将HTML5查看器与Adobe Analytics集成。

如果您使用任何预定义的Dynamic Media Classic HTML5查看器预设，请注意，它们已包含将数据发送到Adobe Analytics所需的所有实施代码，您无需进行进一步的检测。

## 从Dynamic Media Classic {#set-up-adobe-analytics-tracking-from-scene-publishing-system}设置Adobe Analytics跟踪

对于所有HTML5查看器，将以下JavaScript添加到HTML容器，通常在&lt;head>元素中：

```as3
<!-- ***** Site Catalyst Tracking ***** --><script type="text/javascript" src="https://s7d6.scene7.com/s7viewers/s_code.jsp?company=<Dynamic Media Classic Company ID>&preset=companypreset-1"></script>
```

`Company` 设置为Dynamic Media经典公司名称。`&preset` 为可选项，除非公司预设名称不 `companypreset`是。在这种情况下，它可能为`companypreset-1, companypreset-2`，依此类推。 数字越大预设实例越新。要确定正确的公司预设值名称，请单击&#x200B;**复制URL**，然后查看`preset=`参数以查找公司预设名称。

接下来，添加一个将查看器事件传送到 Adobe Analytics 跟踪代码的函数。

将`s7ComponentEvent()`函数添加到容器 HTML（或JSP、ASPX或其他）：

```as3
function s7ComponentEvent(objectId, componentClass, instanceName, timeStamp, eventData) {     s7track(eventData); }
```

函数名区分大小写。传递给`s7componentEvent`的唯一必需参数是最后一个：`eventData`。 `s7track()` 定义。`s7track` 处理每个事件的所有跟踪。（要进一步自定义传送到 Adobe Analytics 的数据，可以在该区域执行此操作。）

## 启用 HREF 和 ITEM 事件 {#enabling-href-and-item-events}

可以通过图像映射编辑，在查看器中启用 HREF（变换）和 ITEM（鼠标单击/点按）事件。在与查看器内容关联的图像映射中定义 HREF 和 ITEM 标识符。将`&rolloverKey=`参数添加到图像映射中的HREF值。
