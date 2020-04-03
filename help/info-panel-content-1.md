---
title: 管理图像集中的信息面板内容
seo-title: 管理图像集中的信息面板内容
description: 'null'
seo-description: 了解如何管理图像集中的信息面板内容。
uuid: ed7b4344-f180-41fc-a95a-62a9767dc056
contentOwner: rbrough
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
content-type: reference
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sets
discoiquuid: ba5d1fb1-af54-471c-a471-853ace7f72fd
translation-type: tm+mt
source-git-commit: d5bf894d56687561c93ef08762bc19d3597225e6

---


# 管理图像集中的信息面板内容{#managing-info-panel-content-in-image-sets}

除了在图像集中将图像映射文本用于变换之外，还可以使用“信息面板”添加大量变换文本（包括链接）。还可以使用定时缓存和计划内容更新来管理信息面板。

可以使用 Scene7 Publishing System 中的以下功能管理信息面板设置和数据：

* “信息面板设置”面板可用来指定用于显示“信息面板”文本、默认错误响应以及信息缓存的小时数等信息的模板。此外，可以指定是否自动发布图像集。
* “信息面板数据输入”面板可用来指定包含要在信息面板变换文本中显示的文本的 CSV 文件，以及计划更新信息的时间。
* “导入元数据”对话框可用来导入包含变换文本信息的制表符分隔 TXT 文件。可以将该 TXT 选项或“信息面板数据输入”面板与“CSV 文件”选项结合，用于变换文本。

## 为图像集设置响应模板 {#set-up-a-response-template-for-image-sets}

可以选择三个预设响应模板之一用来在“信息面板”中显示文本。这些预设响应模板决定了在“信息面板”中显示信息的方式：列数和行数、字样大小、字体等等。可以选择预设响应模板，或者创建一个自己的模板。

**设置响应模板**

1. 双击图像集以在详细信息视图中将其打开。
1. Click **InfoPanel Setup** to unfold the panel.
1. 在“响应模板”下拉列表中，执行下列操作之一：

   * 选择“默认”以使用默认响应。模板设计的 XML 在“用户模板”文本框中灰显。
   * 选择“自定义”创建自己的响应模板。在“用户模板”文本框中，键入模板 XML 定义。您可以使用已在该文本框定义的默认模板作为您自己的响应的基模板。

1. （可选）在“默认响应”框中，键入当Dynamic Media Classic在检索图像映射的信息时遇到错误时要显示的文本。 例如，如果系统收到公司名称和图像集名称，但是没有变换标识符，则将为用户显示该消息。
1. 在“响应 TTL”文本字段中，输入要在缓存数据之前等待的小时数。

   * 如果在一整天内需要频繁更新数据，则设置一个较小的值。
   * 如果数据相对稳定并且不需要整天频繁更新，则设置一个较大的值。默认为十小时。

1. Click **Upload** to upload info panel content, based on the rollover_key values, to s7info.
1. In the S7Info Upload dialog box, browse to the file that you want to use, and then click **Upload**.

   支持的文件格式包括采用 UTF-16 编码的制表符分隔文件以及采用 ASCII 编码的 CSV 文件。对于 CSV 文件，必须对非 ASCII 字符进行 HTML 编码。

1. In the InfoPanel Setup panel, click **Publish**.

## 为图像集中的“信息”面板导入源内容 {#import-source-content-for-the-info-panel-in-image-sets}

您可以将采用 ASCII 编码（必须对非 ASCII 字符进行 HTML 编码）的 CSV（逗号分隔值）文件或制表符分隔文件用于图像集信息面板的源文本。制表符分隔文件必须使用 UTF-16 (Unicode) 编码。使用不同的方法导入不同的文件类型。

格式化源内容时，谨记以下指导原则：

* 制表符分隔和逗号分隔的数据应包含变换模板所需的列数。
* 数据的第一项或列应是变换标识符（与图像映射 URL 的 rollover_key 值关联）。
* 确保标识符后面的每个制表符分隔或逗号分隔的项目都是要替换到响应模板中的项目（因此第一列取代 $1$，第二列取代 $2$，依此类推）。

### 将CSV内容从外部托管位置导入图像集 {#import-csv-content-into-image-sets-from-an-externally-hosted-location}

1. 双击图像集以在详细信息视图中将其打开。
1. Click **InfoPanel Datafeed** to unfold the panel.
1. 在“外部承载的 CSV 文件位置 (HTTP)”文本字段中，输入指向 CSV 文件的 URL。
1. (Optional) In the Schedule Update fields, specify a time to update the content, and then click **Add**.

   可以选择多个更新时间。每个更新时间显示在“更新时间”文本框中。To remove a scheduled time, select it, and then click **Delete**.

1. (Optional) Click **Run Update** to immediately update the content.

