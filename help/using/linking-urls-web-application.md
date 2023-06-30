---
title: 将URL链接到您的Web应用程序
description: 了解如何从Adobe Dynamic Media Classic将URL链接到您的Web应用程序。
uuid: 1179bdd3-9b39-47f9-945d-1c1ca186bf96
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
discoiquuid: 71299640-676d-49b7-841d-6118f31044e8
feature: Dynamic Media Classic
role: User
exl-id: ca629427-da33-4bab-9d08-6d9368042f7e
topic: Administration, Content Management, Development
level: Intermediate
source-git-commit: 5d8b7cb8b4616a998346675d7324b568634698fb
workflow-type: tm+mt
source-wordcount: '843'
ht-degree: 37%

---

# 将URL链接到您的Web应用程序{#linking-urls-to-your-web-application}

您的网站和应用程序可通过URL字符串访问Dynamic Media Image Server内容。 发布图像后，Adobe Dynamic Media Classic会激活一个引用Dynamic Media图像服务器上的图像预设的URL字符串。 可将这些 URL 粘贴至 Web 浏览器进行测试。

要将这些URL字符串放置在网页和应用程序中，请从Adobe Dynamic Media Classic复制它们。 要获取由图像预设生成的URL字符串，请转到“预览”屏幕或“浏览”面板（在“详细信息”视图中）。

## 获取图像预设URL {#obtaining-an-image-preset-url}

可从“预览”或详细信息视图中获得由图像预设生成的 URL 字符串。复制 URL 后，该字符串将放置在剪贴板上，以便在必要时进行粘贴。

>[!NOTE]
>
>在发布资源之前，URL 处于非激活状态。

### 从预览中获取图像预设URL {#obtaining-an-image-preset-url-from-preview}

1. 在左侧“资源库”面板中，导航到包含要预览的图像资源的“资源”文件夹。
1. 执行以下任一操作：

   * 在“资源”窗口上方的工具栏右侧，选择 **[!UICONTROL 网格视图]**. 在“资源”窗口中，选择单个图像资源，然后转到缩略图图像下方 **[!UICONTROL 预览]** > **[!UICONTROL 图像预设列表]**.
   * 在“资源”窗口上方的工具栏右侧，选择 **[!UICONTROL 列表视图]**. 在“资源”窗口中，选择单个图像资源，然后转到缩略图图像右侧的 **[!UICONTROL 预览]** > **[!UICONTROL 图像预设列表]**.
   * 在“资源”窗口上方的工具栏右侧，选择 **[!UICONTROL 详细信息视图]**. 在同一工具栏上，转到 **[!UICONTROL 预览]** > **[!UICONTROL 图像预设列表]**.

1. （可选）在“图像预设”列表的“用于生成复制URL的URL编码”下拉列表中，选择您希望在复制图像资源的URL时应用的URL编码。
1. 在“图像预设列表”窗口的预览窗格的右上角区域中选择 **[!UICONTROL 复制URL]** 所选预设类型。
1. 在“图像预设列表”窗口的右下角，选择 **[!UICONTROL 关闭]** 以返回到“资产”屏幕。

### 从浏览面板获取图像预设URL {#obtaining-an-image-preset-url-from-the-browse-panel}

1. 在左侧“资源库”面板中，导航到包含要预览的图像资源的“资源”文件夹。
1. 在“资源”窗口上方的工具栏右侧，选择 **[!UICONTROL 网格视图]**. 在“资源”窗口中，选择单个图像资源。
1. 在“资源”窗口上方的工具栏右侧，选择 **[!UICONTROL 详细信息视图]**.
1. 选择 **[!UICONTROL URL]** ，以便展开图像预设列表。
1. 选择 **[!UICONTROL 复制URL]** 图像预设名称旁边的链接，其中包含要复制到剪贴板的URL。

## 关于图像预设 URL 字符串 {#about-image-preset-url-strings}

Dynamic Media图像服务器图像大小调整的URL调用具有以下基本语法：

*路径*/*图像服务器名称*/*帐户名称*/*图像名称*?*修饰符1*&amp;*修饰符2*&amp;...

在Dynamic Media Image Server URL中，服务器显示图像的说明显示在问号(？)之后。 例如，以下 URL 调用将传送一个名为“backpack”宽度为 250 个像素的图像：

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

在 URL 中图像预设名称用美元符号 ($) 括起。当Dynamic Media Image Server遇到URL的图像预设部分时( `Large` 在本例中)，使用“大”图像预设定义的大小和格式说明。

## 将动态图像添加到网页 {#adding-dynamic-images-to-your-web-page}

要将动态图像添加到网页，请 `<IMG>` HTML网页代码中的标记通常使用Adobe Dynamic Media Classic URL字符串进行修改，以向Dynamic Media图像服务器发出请求。 该字符串会按图像预设定义的大小和格式规范生成图像。

例如，与以下用于打开静态图像的典型调用不同

```as3
img src="/company_images/products/backpack_thumbnail.jpg"
```

您现在使用 `<IMG>`标记，以使用对Adobe Dynamic Media Classic平台的图像预设调用替换对静态图像的引用。 示例调用如下所示：

```as3
img src="https://s7d2.scene7.com/is/image/S7learn/backpack_trns?$thumbnail$”
```

在此示例中，Dynamic Media Image Server“查找”定义 `$thumbnail$` ，并根据由定义的尺寸和格式规范动态生成适当的图像 `thumbnail`图像预设。 在 URL 字符串中，除产品图像文件名称（本例中为`backpack_trns` ）之外的所有项目都由网页模版所固定。唯一可从商业服务器自动插入到网页模版的元素是 IPS ID 或图像名称。
