---
title: 将 URL 链接至 Web 应用程序
seo-title: 将 URL 链接至 Web 应用程序
description: 'null'
seo-description: 了解如何将URL关联到您的Web应用程序。
uuid: 1179bdd3-9b39-47f9-945d-1c1ca186ff96
contentOwner: admin
content-type: 引用
products: SG_ EXPERIENCE MANAGER/Dynamic-Media-Scene-7
geptopics: SG_ SCENESELEFERENDER_ PK/categories/image_ sizing
discoiquuid: 71299640-676d-49b7-841d-6118f31044e8
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# 将 URL 链接至 Web 应用程序{#linking-urls-to-your-web-application}

您的网站和应用程序通过URL字符串访问Dynamic Media图像服务器内容。在您发布图像后，动态媒体经典会激活引用动态媒体图像服务器上的图像预设的URL字符串。可将这些 URL 粘贴至 Web 浏览器进行测试。

要将这些 URL 字符串放置到网页和应用程序中，请从 Scene7 Publishing System 复制它们。要获得由图像预设生成的 URL 字符串，请转到“预览”屏幕或浏览面板（在中）。

## 获得图像预设 URL {#obtaining-an-image-preset-url}

可从“预览”或详细信息视图中获得由图像预设生成的 URL 字符串。复制 URL 后，该字符串将放置在剪贴板上，以便在必要时进行粘贴。

***注意**：在发布资产之前，URL才处于活动状态。*

### 从预览中获得图像预设 URL {#obtaining-an-image-preset-url-from-preview}

1. 在左侧“资源库”面板中，导航到包含要预览的图像资源的“资源”文件夹。
1. 执行以下任一操作：

   * 在“资源”窗口上方，工具栏的右侧，单击“网格视图”。在“资源”窗口中，选择单个图像资源，然后在缩略图图像下方，单击“预览”&gt;“图像预设列表”。
   * 在“资源”窗口上方，工具栏的右侧，单击“列表视图”。在“资源”窗口中，选择单个图像资源，然后在缩略图图像右侧，单击“预览”&gt;“图像预设列表”。
   * 在“资源”窗口上方，工具栏的右侧，单击“详细信息视图”。在同一工具栏上，单击“预览”&gt;“图像预设列表”。

1. （可选）在“图像预设列表”窗口底部的“用于生成副本 URL 的 URL 编码”下拉列表中，选择要在复制图像资源的 URL 时应用的 URL 编码。
1. 在“图像预设列表”窗口中，在预览窗格的右上角区域中，单击所选预设类型对应的“复制 URL”。
1. 在“图像预设列表”窗口的右下角，单击“关闭”以返回到“资源”屏幕。

### 从浏览面板中获得图像预设 URL {#obtaining-an-image-preset-url-from-the-browse-panel}

1. 在左侧“资源库”面板中，导航到包含要预览的图像资源的“资源”文件夹。
1. 在“资源”窗口上方，工具栏的右侧，单击“网格视图”。在“资源”窗口中，选择单个图像资源。
1. 在“资源”窗口上方，工具栏的右侧，单击“详细信息视图”。
1. 单击屏幕右侧面板上的 URL 以展开图像预设列表。
1. 单击带有要复制到剪贴板的 URL 的图像预设名称旁的“复制 URL”链接。

## 关于图像预设 URL 字符串 {#about-image-preset-url-strings}

对Dynamic Media图像服务器进行图像大小调整的URL调用具有以下基本语法：

*路径*/*图像服务器名称*/*帐户名称*/*图像名称*?*修饰符1*&amp;*修饰符2*&amp;...

在Dynamic Media图像服务器URL中，用于显示图像的服务器说明显示在问号(？)之后。例如，以下 URL 调用将传送一个名为“backpack”宽度为 250 个像素的图像：

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

在 URL 中图像预设名称用美元符号 ($) 括起。When a Dynamic Media Image Server encounters the Image Preset portion of the URL (the `Large` in this case), using the size and formatting instructions defined by the “Large” Image Preset.

## 将动态图像添加到网页中 {#adding-dynamic-images-to-your-web-page}

To add dynamic images to your web page, the `<IMG>` tag in your HTML web page code typically is modified using the Dynamic Media Classic URL string to make a request to Dynamic Media Image Servers. 该字符串会按图像预设定义的大小和格式规范生成图像。

例如，与以下用于打开静态图像的典型调用不同

```as3
img src="/company_images/products/backpack_thumbnail.jpg"
```

you now use the `<IMG>`tag to replace the reference to a static image with an Image Preset call to the Dynamic Media Classic platform. 示例调用如下所示：

```as3
img src="https://s7d2.scene7.com/is/image/S7learn/backpack_trns?$thumbnail$”
```

In this example, a Dynamic Media Image Server “looks up” the definition of `$thumbnail$` and dynamically generates the appropriate image with the sizing and formatting specifications defined by the `thumbnail`Image Preset. 在 URL 字符串中，除产品图像文件名称（本例中为`backpack_trns` ）之外的所有项目都由网页模版所固定。唯一可从商业服务器自动插入到网页模版的元素是 IPS ID 或图像名称。