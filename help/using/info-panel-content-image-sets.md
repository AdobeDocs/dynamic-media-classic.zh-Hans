---
title: 管理图像集中的信息面板内容
description: 了解如何在Adobe Dynamic Media Classic中管理图像集中的信息面板内容。
contentOwner: rbrough
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
content-type: reference
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sets
feature: Dynamic Media Classic,Viewers,Image Sets
role: User
exl-id: 09fafdb4-51e2-4719-83b6-056f79d1ba9e
topic: Content Management
level: Intermediate
source-git-commit: ae7d0c6d3047d68ed3da4187ef516dc51c95de30
workflow-type: tm+mt
source-wordcount: '769'
ht-degree: 51%

---

# 管理图像集中的信息面板内容{#managing-info-panel-content-in-image-sets}

除了在图像集中将图像映射文本用于变换之外，还可以使用“信息面板”添加大量变换文本（包括链接）。还可以使用定时缓存和计划内容更新来管理信息面板。

您可以使用Adobe Dynamic Media Classic中的以下功能管理信息面板设置和数据：

* “信息面板设置”面板可用来指定用于显示“信息面板”文本、默认错误响应以及信息缓存的小时数等信息的模板。此外，可以指定是否自动发布图像集。
* “信息面板数据馈送”面板允许您指定包含要在信息面板变换文本中显示的文本的CSV文件，并安排更新信息的时间。
* “导入元数据”对话框可用来导入包含变换文本信息的制表符分隔 TXT 文件。您可以将此TXT选项或“信息面板数据馈送”面板与CSV文件选项一起用于变换文本。

## 为图像集设置响应模板 {#set-up-a-response-template-for-image-sets}

可以选择三个预设响应模板之一用来在“信息面板”中显示文本。这些预设响应模板决定了在“信息面板”中显示信息的方式：列数和行数、字样大小、字体等等。可以选择预设响应模板，或者创建一个自己的模板。

**要为图像集设置响应模板，请执行以下操作：**

1. 双击图像集，使其在“详细信息视图”中打开。
1. 选择 **[!UICONTROL 信息面板设置]**.
1. 在“响应模板”下拉列表中，执行下列操作之一：

   * 要使用默认响应，请选择 **[!UICONTROL 默认]**. 模板设计的 XML 在“用户模板”文本框中灰显。
   * 要创建自己的响应模板，请选择 **[!UICONTROL 自定义]**. 在“用户模板”文本框中，键入模板 XML 定义。您可以使用已在该文本框定义的默认模板作为您自己的响应的基模板。

1. （可选）在默认响应框中，键入当Adobe Dynamic Media Classic在检索图像映射信息时遇到错误时要显示的文本。 例如，如果系统收到公司名称和图像集名称，但是没有变换标识符，则将为用户显示该消息。
1. 在“响应 TTL”文本字段中，输入要在缓存数据之前等待的小时数。

   * 如果在一整天内需要频繁更新数据，则设置一个较小的值。
   * 如果数据相对稳定并且不需要整天频繁更新，则设置一个较大的值。默认为十小时。

1. 选择 **[!UICONTROL 上传]** 要基于rollover_key值将信息面板内容上载到s7info，请执行以下操作：
1. 在“S7Info上载”对话框中，浏览到要使用的文件，然后选择 **[!UICONTROL 上传]**.

   支持的文件格式包括采用UTF-16编码的制表符分隔文件以及采用ASCII编码的CSV文件。 对于 CSV 文件，必须对非 ASCII 字符进行 HTML 编码。

1. 在“信息面板设置”面板中，选择 **[!UICONTROL Publish]**.

## 导入图像集中信息面板的源内容 {#import-source-content-for-the-info-panel-in-image-sets}

您可以将采用 ASCII 编码（必须对非 ASCII 字符进行 HTML 编码）的 CSV（逗号分隔值）文件或制表符分隔文件用于图像集信息面板的源文本。制表符分隔文件必须使用 UTF-16 (Unicode) 编码。使用不同的方法导入不同的文件类型。

格式化源内容时，谨记以下指导原则：

* 以制表符和逗号分隔的数据可以包含变换模板所需的任意数量的列。
* 数据的第一项或第一列是变换标识符（与图像映射URL中的rollover_key值相关联）。
* 确保标识符之后的每个以制表符或逗号分隔的项目都是要替换到响应模板中的项目。 因此，第一列将替换为$1$，第二列将替换为$2$，依此类推。

### 将CSV内容从外部托管位置导入图像集 {#import-csv-content-into-image-sets-from-an-externally-hosted-location}

1. 双击图像集，使其在“详细信息视图”中打开。
1. 选择 **[!UICONTROL 信息面板数据馈送]**.
1. 在“外部承载的 CSV 文件位置 (HTTP)”文本字段中，输入指向 CSV 文件的 URL。
1. （可选）在计划更新字段中，指定更新内容的时间，然后选择 **[!UICONTROL 添加]**.

   可以选择多个更新时间。每个更新时间显示在“更新时间”文本框中。要删除计划时间，请选择它，然后选择 **[!UICONTROL 删除]**.

1. （可选）选择 **[!UICONTROL 运行更新]** 以立即更新内容。
