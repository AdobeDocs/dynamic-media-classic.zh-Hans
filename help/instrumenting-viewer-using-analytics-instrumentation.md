---
title: 使用Adobe Analytics检测工具包检测查看器
description: 了解如何使用Adobe Dynamic Media Classic中的Adobe Analytics Instrumentation Kit检测查看器。
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

# 使用Adobe Analytics检测工具包检测查看器{#instrumenting-a-viewer-using-the-adobe-analytics-instrumentation-kit}

您可以使用Adobe Analytics Instrumentation Kit将HTML5查看器与Adobe Analytics集成。

如果您使用任何预定义的Adobe Dynamic Media ClassicHTML5查看器预设，则这些预设中已包含所有用于向Adobe Analytics发送数据的实现代码；您无需进一步检测。

## 从Adobe Dynamic Media Classic设置Adobe Analytics跟踪 {#set-up-adobe-analytics-tracking-from-scene-publishing-system}

对于所有HTML5查看器，将以下JavaScript添加到HTML容器中，通常位于 &lt;head> 元素：

```as3
<!-- ***** Adobe Analytics Tracking ***** --><script type="text/javascript" src="https://s7d6.scene7.com/s7viewers/s_code.jsp?company=<Adobe Dynamic Media Classic Company ID>&preset=companypreset-1"></script>
```

位置 `Adobe Dynamic Media Classic Company ID` 设置为Adobe Dynamic Media Classic公司名称。 和 `&preset` 是可选的，除非公司预设名称不是 `companypreset`. 在这种情况下，它可以 `companypreset-1, companypreset-2`，等等。 数字越大预设实例越新。要确定正确的公司预设值名称，请选择 **[!UICONTROL 复制URL]** ，然后查看 `preset=`用于查找公司预设名称的参数。

继续，现在添加一个函数，用于将查看器事件传输到Adobe Analytics跟踪代码。

添加 `s7ComponentEvent()` 函数到容器HTML（或JSP、ASPX或其他）：

```as3
function s7ComponentEvent(objectId, componentClass, instanceName, timeStamp, eventData) {     s7track(eventData); }
```

函数名称区分大小写。 传递给的唯一参数 `s7componentEvent`最后一个选项是必需的： `eventData`. 位置 `s7track()` 是在上面包含的s_code.jsp中定义的。 和 `s7track` 处理每个事件的所有跟踪。 （要进一步自定义传送到 Adobe Analytics 的数据，可以在该区域执行此操作。）

## 启用HREF和ITEM事件 {#enabling-href-and-item-events}

可以通过图像映射编辑，在查看器中启用 HREF（变换）和 ITEM（鼠标单击/点按）事件。在与查看器内容关联的图像映射中定义 HREF 和 ITEM 标识符。添加 `&rolloverKey=` 参数到图像映射中的HREF值。
