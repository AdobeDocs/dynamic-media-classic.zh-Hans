---
title: 使用Adobe Analytics Instrumentation Kit设置查看器
description: 了解如何使用Dynamic Media Classic中的Adobe Analytics Instrumentation Kit来乐器查看器。
uuid: cf9a4002-966d-4641-9cd0-2ee8b5454f60
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: a2824244-1755-42de-a167-42af117cf038
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 9ea1546d-e6d1-4ba4-8fa1-26b4e69375ba
source-git-commit: bb387446f294cf1e90d26ae1df4422879ad29db7
workflow-type: tm+mt
source-wordcount: '300'
ht-degree: 20%

---

# 使用Adobe Analytics Instrumentation Kit设置查看器{#instrumenting-a-viewer-using-the-adobe-analytics-instrumentation-kit}

您可以使用Adobe Analytics Instrumentation Kit将HTML5查看器与Adobe Analytics集成。

如果您使用任何预定义的Dynamic Media Classic HTML5查看器预设，则它们已包含所有用于将数据发送到Adobe Analytics的实施代码；您无需进行进一步的检测。

## 从Dynamic Media Classic设置Adobe Analytics跟踪 {#set-up-adobe-analytics-tracking-from-scene-publishing-system}

对于所有HTML5查看器，将以下JavaScript添加到HTML容器中，通常是在&lt;head>元素中：

```as3
<!-- ***** Adobe Analytics Tracking ***** --><script type="text/javascript" src="https://s7d6.scene7.com/s7viewers/s_code.jsp?company=<Dynamic Media Classic Company ID>&preset=companypreset-1"></script>
```

其中，将`Dynamic Media Classic Company ID`设置为Dynamic Media Classic公司名称。 和`&preset`是可选的，除非公司预设名称不是`companypreset`。 在这种情况下，该参数可能为`companypreset-1, companypreset-2`，依此类推。 数字越大预设实例越新。要确定正确的公司预设值名称，请选择&#x200B;**[!UICONTROL 复制URL]** ，然后查看`preset=`参数以查找公司预设名称。

继续，现在添加一个函数，以将查看器事件传输到Adobe Analytics跟踪代码。

将`s7ComponentEvent()`函数添加到容器HTML（或JSP、ASPX或其他）：

```as3
function s7ComponentEvent(objectId, componentClass, instanceName, timeStamp, eventData) {     s7track(eventData); }
```

函数名称区分大小写。 传递到`s7componentEvent`的唯一必需参数是最后一个参数：`eventData`。 其中`s7track()`在上面包含的s_code.jsp中定义。 而`s7track`则处理每个事件的所有跟踪。 （要进一步自定义传送到 Adobe Analytics 的数据，可以在该区域执行此操作。）

## 启用HREF和项目事件 {#enabling-href-and-item-events}

可以通过图像映射编辑，在查看器中启用 HREF（变换）和 ITEM（鼠标单击/点按）事件。在与查看器内容关联的图像映射中定义 HREF 和 ITEM 标识符。向图像映射中的HREF值添加`&rolloverKey=`参数。
