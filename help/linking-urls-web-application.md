---
title: 将 URL 链接至 Web 应用程序
seo-title: 将 URL 链接至 Web 应用程序
description: 'null'
seo-description: 了解如何将URL关联到您的Web应用程序。
uuid: 1179bdd3-9b39-47f9-945d-1c1ca186bf96
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
discoiquuid: 71299640-676d-49b7-841d-6118f31044e8
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '841'
ht-degree: 72%

---


# 将 URL 链接至 Web 应用程序{#linking-urls-to-your-web-application}

您的网站和应用程序通过URL字符串访问Dynamic Media图像服务器内容。 发布图像后，Dynamic Media经典会激活引用Dynamic Media图像服务器上的图像预设的URL字符串。 可将这些 URL 粘贴至 Web 浏览器进行测试。

要将这些URL字符串放置到网页和应用程序中，请从Dynamic Media经典中复制它们。 要获得由图像预设生成的 URL 字符串，请转到“预览”屏幕或浏览面板（在中）。

## 获得图像预设 URL {#obtaining-an-image-preset-url}

可从“预览”或详细信息视图中获得由图像预设生成的 URL 字符串。复制 URL 后，该字符串将放置在剪贴板上，以便在必要时进行粘贴。

***注意&#x200B;**:在您发布资产之前，该URL不会处于活动状态。*

### 从预览中获得图像预设 URL {#obtaining-an-image-preset-url-from-preview}

1. 在左侧“资源库”面板中，导航到包含要预览的图像资源的“资源”文件夹。
1. 执行以下任一操作：

   * 在“资源”窗口上方，工具栏的右侧，单击“网格视图”。在“资源”窗口中，选择单个图像资源，然后在缩略图图像下方，单击“预览”>“图像预设列表”。
   * 在“资源”窗口上方，工具栏的右侧，单击“列表视图”。在“资源”窗口中，选择单个图像资源，然后在缩略图图像右侧，单击“预览”>“图像预设列表”。
   * 在“资源”窗口上方，工具栏的右侧，单击“详细信息视图”。在同一工具栏上，单击“预览”>“图像预设列表”。

1. （可选）在“图像预设列表”窗口底部的“用于生成副本 URL 的 URL 编码”下拉列表中，选择要在复制图像资源的 URL 时应用的 URL 编码。
1. 在“图像预设列表”窗口中，在预览窗格的右上角区域中，单击所选预设类型对应的“复制 URL”。
1. 在“图像预设列表”窗口的右下角，单击“关闭”以返回到“资源”屏幕。

### 从浏览面板中获得图像预设 URL  {#obtaining-an-image-preset-url-from-the-browse-panel}

1. 在左侧“资源库”面板中，导航到包含要预览的图像资源的“资源”文件夹。
1. 在“资源”窗口上方，工具栏的右侧，单击“网格视图”。在“资源”窗口中，选择单个图像资源。
1. 在“资源”窗口上方，工具栏的右侧，单击“详细信息视图”。
1. 单击屏幕右侧面板上的 URL 以展开图像预设列表。
1. 单击带有要复制到剪贴板的 URL 的图像预设名称旁的“复制 URL”链接。

## 关于图像预设 URL 字符串  {#about-image-preset-url-strings}

对Dynamic Media图像服务器的图像大小调整URL调用具有以下基本语法：

*路径*/*图像服务器名称*/*帐户名称*/*图像名称*?*修饰符1*&amp;*修饰符2*&amp;...

在Dynamic Media图像服务器URL中，在问号(?)后将显示显示图像的服务器说明。 例如，以下 URL 调用将传送一个名为“backpack”宽度为 250 个像素的图像：

```as3
https://s7d1.scene7.com/is/image/S7learn/backpack?wid=250
```

图像预设 URL 包含按相应大小和格式规范显示图像的所有修饰符指令。对于没有图像预设的情况，请注意此 URL 字符串中问号 (?) 之后的所有修饰符指令：

```as3
https://s7d1.scene7.com/is/image/S7learn/backpack?wid=250&fmt=jpeg&qlt=80,0&resMode=sharp&op_usm=1.1,0.5,1,0
```

然而，在图像预设生成的 URL 字符串中，图像预设的名称将代替图像预设定义的指令。例如，对于上面的长 URL，此 URL 字符串为：

```as3
https://s7d1.scene7.com/is/image/S7learn/backpack?$Large$
```

在 URL 中图像预设名称用美元符号 ($) 括起。当Dynamic Media图像服务器遇到URL的“图像预设”部分（本例中为`Large`）时，请使用“大”图像预设定义的大小和格式说明。

## 将动态图像添加到网页中 {#adding-dynamic-images-to-your-web-page}

要向网页添加动态图像，HTML网页代码中的`<IMG>`标记通常会使用Dynamic Media经典URL字符串进行修改，以向Dynamic Media图像服务器发出请求。 该字符串会按图像预设定义的大小和格式规范生成图像。

例如，与以下用于打开静态图像的典型调用不同

```as3
img src="/company_images/products/backpack_thumbnail.jpg"
```

您现在使用`<IMG>`标记将对静态图像的引用替换为对Dynamic Media经典平台的图像预设调用。 示例调用如下所示：

```as3
img src="https://s7d2.scene7.com/is/image/S7learn/backpack_trns?$thumbnail$”
```

在此示例中，Dynamic Media图像服务器“查找”`$thumbnail$`的定义，并动态生成相应的图像，其大小调整和格式设置规范由`thumbnail`图像预设定义。 在 URL 字符串中，除产品图像文件名称（本例中为`backpack_trns` ）之外的所有项目都由网页模版所固定。唯一可从商业服务器自动插入到网页模版的元素是 IPS ID 或图像名称。
