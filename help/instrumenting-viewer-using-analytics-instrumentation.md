---
title: 使用 Adobe Analytics 仪器包实施查看器
seo-title: 使用 Adobe Analytics 仪器包实施查看器
description: 'null'
seo-description: 了解如何使用Adobe Analytics仪器包进行查看器。
uuid: cf9a4002-966d-4641-9cd0-2ee8b5454f60
contentOwner: admin
content-type: 引用
products: SG_ EXPERIENCE MANAGER/Dynamic-Media-Scene-7
geptopics: SG_ SCENEESFERENONDAND_ PK/categories/adobe_ analytics_ contracting_ kit
discoiquuid: a2824244-1755-42de-a167-42af117 cf038
translation-type: tm+mt
source-git-commit: 32f5e03766466ceaafe58780e9e80dbdd4a0c3dd

---


# 使用 Adobe Analytics 仪器包实施查看器{#instrumenting-a-viewer-using-the-adobe-analytics-instrumentation-kit}

您可以使用Adobe Analytics Instrumentation Kit将HTML查看器与Adobe Analytics集成。

如果您使用任何预定义的Dynamic Media经典HTML查看器预设，请注意它们已经包含向Adobe Analytics发送数据所需的所有实施代码。—不需要再进行检测。

## 通过 Scene7 Publishing System 设置 Adobe Analytics 跟踪 {#set-up-adobe-analytics-tracking-from-scene-publishing-system}

对于所有HTML查看器，向HTML容器添加以下JavaScript，通常位于&lt; head&gt;元素中：

```as3
<!-- ***** Site Catalyst Tracking ***** --><script type="text/javascript" src="https://s7d6.scene7.com/s7viewers/s_code.jsp?company=<SPS Company ID>&preset=companypreset-1"></script>
```

将 `Company` 设置为 SPS 公司名。`&preset` 为可选，除非公司预设名称 `companypreset`不然。In such cases, it could be `companypreset-1, companypreset-2`, and so on. 数字越大预设实例越新。To determine the correct company preset value name, click **Copy URL** , and then look at the `preset=`parameter to find the company preset name.

接下来，添加一个将查看器事件传送到 Adobe Analytics 跟踪代码的函数。

Add the `s7ComponentEvent()` function to the container HTML (or JSP, or ASPX or other):

```as3
function s7ComponentEvent(objectId, componentClass, instanceName, timeStamp, eventData) {     s7track(eventData); }
```

函数名区分大小写。The only parameter passed to `s7componentEvent`that is required is the last one: `eventData`. `s7track()` 在上面包含的s_ code. jsp中定义。`s7track` 处理每个事件的所有跟踪。（要进一步自定义传送到 Adobe Analytics 的数据，可以在该区域执行此操作。）

## 启用 HREF 和 ITEM 事件 {#enabling-href-and-item-events}

可以通过图像映射编辑，在查看器中启用 HREF（变换）和 ITEM（鼠标单击/点按）事件。在与查看器内容关联的图像映射中定义 HREF 和 ITEM 标识符。Add a `&rolloverKey=` parameter to the HREF value within the Image Map.