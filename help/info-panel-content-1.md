---
title: 管理图像集中的信息面板内容
description: 了解如何管理图像集中的“信息面板”内容。
uuid: ed7b4344-f180-41fc-a95a-62a9767dc056
contentOwner: rbrough
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
content-type: reference
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sets
discoiquuid: ba5d1fb1-af54-471c-a471-853ace7f72fd
feature: Dynamic Media Classic，查看器，图像集
role: 业务从业者
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '776'
ht-degree: 73%

---


# 管理图像集{#managing-info-panel-content-in-image-sets}中的信息面板内容

除了在图像集中将图像映射文本用于变换之外，还可以使用“信息面板”添加大量变换文本（包括链接）。还可以使用定时缓存和计划内容更新来管理信息面板。

您可以使用Dynamic Media Classic中的以下功能管理InfoPanel设置和数据：

* “信息面板设置”面板可用来指定用于显示“信息面板”文本、默认错误响应以及信息缓存的小时数等信息的模板。此外，可以指定是否自动发布图像集。
* “信息面板数据输入”面板可用来指定包含要在信息面板变换文本中显示的文本的 CSV 文件，以及计划更新信息的时间。
* “导入元数据”对话框可用来导入包含变换文本信息的制表符分隔 TXT 文件。可以将该 TXT 选项或“信息面板数据输入”面板与“CSV 文件”选项结合，用于变换文本。

## 为图像集{#set-up-a-response-template-for-image-sets}设置响应模板

可以选择三个预设响应模板之一用来在“信息面板”中显示文本。这些预设响应模板决定了在“信息面板”中显示信息的方式：列数和行数、字样大小、字体等等。可以选择预设响应模板，或者创建一个自己的模板。

**设置响应模板**

1. 双击图像集以在详细信息视图中将其打开。
1. 单击&#x200B;**InfoPanel Setup**&#x200B;打开面板。
1. 在“响应模板”下拉列表中，执行下列操作之一：

   * 选择“默认”以使用默认响应。模板设计的 XML 在“用户模板”文本框中灰显。
   * 选择“自定义”创建自己的响应模板。在“用户模板”文本框中，键入模板 XML 定义。您可以使用已在该文本框定义的默认模板作为您自己的响应的基模板。

1. （可选）在“默认响应”框中，键入在Dynamic Media Classic检索图像映射信息时遇到错误时要显示的文本。 例如，如果系统收到公司名称和图像集名称，但是没有变换标识符，则将为用户显示该消息。
1. 在“响应 TTL”文本字段中，输入要在缓存数据之前等待的小时数。

   * 如果在一整天内需要频繁更新数据，则设置一个较小的值。
   * 如果数据相对稳定并且不需要整天频繁更新，则设置一个较大的值。默认为十小时。

1. 单击&#x200B;**上载**&#x200B;可根据rollover_key值将信息面板内容上载到s7info。
1. 在“S7Info上传”对话框中，浏览到要使用的文件，然后单击&#x200B;**上传**。

   支持的文件格式包括采用 UTF-16 编码的制表符分隔文件以及采用 ASCII 编码的 CSV 文件。对于 CSV 文件，必须对非 ASCII 字符进行 HTML 编码。

1. 在“信息面板设置”面板中，单击&#x200B;**发布**。

## 导入图像集{#import-source-content-for-the-info-panel-in-image-sets}中“信息”面板的源内容

您可以将采用 ASCII 编码（必须对非 ASCII 字符进行 HTML 编码）的 CSV（逗号分隔值）文件或制表符分隔文件用于图像集信息面板的源文本。制表符分隔文件必须使用 UTF-16 (Unicode) 编码。使用不同的方法导入不同的文件类型。

格式化源内容时，谨记以下指导原则：

* 制表符分隔和逗号分隔的数据应包含变换模板所需的列数。
* 数据的第一项或列应是变换标识符（与图像映射 URL 的 rollover_key 值关联）。
* 确保标识符后面的每个制表符分隔或逗号分隔的项目都是要替换到响应模板中的项目（因此第一列取代 $1$，第二列取代 $2$，依此类推）。

### 从外部托管位置{#import-csv-content-into-image-sets-from-an-externally-hosted-location}将CSV内容导入图像集

1. 双击图像集以在详细信息视图中将其打开。
1. 单击&#x200B;**InfoPanel Datafeed**&#x200B;打开面板。
1. 在“外部承载的 CSV 文件位置 (HTTP)”文本字段中，输入指向 CSV 文件的 URL。
1. （可选）在“计划更新”字段中，指定更新内容的时间，然后单击&#x200B;**添加**。

   可以选择多个更新时间。每个更新时间显示在“更新时间”文本框中。要删除预定时间，请选择该时间，然后单击&#x200B;**删除**。

1. （可选）单击&#x200B;**运行更新**&#x200B;以立即更新内容。

