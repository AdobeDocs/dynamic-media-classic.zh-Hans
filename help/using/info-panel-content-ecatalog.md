---
title: 管理eCatalogs中的信息面板内容
description: 了解如何在Adobe Dynamic Media Classic中管理eCatalogs中的信息面板内容。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: bfb9c5a4-5068-4adb-9fe2-a4ead8656289
topic: Integrations
level: Experienced
source-git-commit: de6997fda88c4471625242ee9cca59b344cee945
workflow-type: tm+mt
source-wordcount: '877'
ht-degree: 40%

---

# 管理eCatalogs中的信息面板内容{#managing-info-panel-content-in-ecatalogs}

除了在 eCatalog 中将图像映射文本用于变换之外，还可以使用“信息面板”添加大量变换文本（包括链接）。您还可以通过使用定时缓存和计划内容更新来管理信息面板。

您可以使用Adobe Dynamic Media Classic中的以下功能管理信息面板设置和数据：

* “信息面板设置”面板允许您指定用于显示“信息面板”文本的模板、默认错误响应以及信息缓存的小时数。 此外，可以指定是否自动发布 eCatalog。
* “信息面板数据馈送”面板允许您指定包含要在“信息面板”变换文本中显示的文本的CSV文件，并安排更新信息的时间。
* 通过“导入元数据”对话框（从“映射页面”视图中访问），可以导入包含变换文本信息的以Tab分隔的TXT文件。 您可以将此TXT选项或具有CSV文件选项的数据馈送面板用于变换文本。
* “映射页面”视图提供了一个选项，用于预览针对特定图像映射显示的xml。

## 为eCatalogs设置响应模板 {#set-up-a-response-template-for-ecatalogs}

可以选择三个预设响应模板之一用来在“信息面板”中显示文本。这些预设响应模板决定了在“信息面板”中显示信息的方式：列数和行数、字样大小、字体等等。您可以选择预设的响应模板或创建自己的响应模板。

>[!NOTE]
>
>也可以在“查看器预设”中设置响应模板。要在查看器预设中使用响应模板，请添加 `fmt=1` 到查看器预设中的信息服务器URL的末尾。
>
>请参阅 [设置eCatalog查看器预设](setting-ecatalog-viewer-presets.md#setting_up_ecatalog_viewer_presets).

1. 双击eCatalog，以在“详细信息视图”中打开它。
1. 选择 **[!UICONTROL 信息面板设置]** 面板。
1. 选择“响应模板”：

   * 从“响应模板”菜单中选择预设。模板设计的 XML 显示在“用户模板”框中。
   * 要创建自己的响应模板，请选择 **[!UICONTROL 自定义]**. 在“用户模板”框中键入模板 XML 定义。可以将预设模板作为您自己的模板的基础。

1. （可选）在默认响应框中，键入当Adobe Dynamic Media Classic在检索图像映射信息时遇到错误时要显示的文本。 例如，如果系统收到公司名称和 eCatalog 名称，但是没有变换标识符，则将为用户显示该消息。
1. 在“响应 TTL”框中，输入要在缓存数据之前等待的小时数：

   * 如果在一整天内需要频繁更新数据，则设置一个较小的值。
   * 如果数据相对稳定并且不需要在一天中频繁更新，则设置较高的数字。 默认为十小时。

1. 选择 **[!UICONTROL Publish]**.

## 导入eCatalogs中信息面板的源内容 {#import-source-content-for-the-info-panel-in-ecatalogs}

可以为 eCatalog 的“信息面板”源文本使用逗号分隔值文件 (CSV) 或制表符分隔文件 (TXT)。制表符分隔文件必须使用 UTF16 (Unicode) 编码。您可以使用不同的方法导入不同的文件类型。

格式化源内容时，谨记以下指导原则：

* 确保制表符分隔数据和逗号分隔数据包含变换模板所必需的列数。
* 确保数据的第一项或第一列是变换标识符（与图像映射URL中的rollover_key值关联）。
* 确保标识符之后的每个以制表符或逗号分隔的项目都是要替换到响应模板中的项目。 因此，第一列将替换为$1$，第二列将替换为$2$，依此类推。

### 将CSV内容从外部托管位置导入eCatalogs {#import-csv-content-into-ecatalogs-from-an-externally-hosted-location}

1. 双击eCatalog ，以在“详细信息视图”中打开它。
1. 选择 **[!UICONTROL 信息面板数据馈送]** 面板。
1. 在“外部承载的 CSV 文件位置”框中，输入 CSV 文件的 URL。可以将 URL 粘贴至该字段，或直接键入。
1. （可选）使用“计划更新”菜单指定更新内容的时间，然后选择 **[!UICONTROL 添加]**. 可以选择多个更新时间。每个更新时间显示在“更新时间”框中。(要删除时间，请选择该时间，然后选择 **[!UICONTROL 删除]**.)
1. （可选）选择 **[!UICONTROL 立即运行更新]** 以便立即更新内容。

### 导入制表符分隔文件或 CSV 文件 {#import-a-tab-delimited-or-csv-file}

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>SR changed this section 10/23/2012</p>

 -->

1. 双击eCatalog ，以在“详细信息视图”中将其打开。
1. 选择 **[!UICONTROL 信息面板设置]** 面板。
1. 选择 **[!UICONTROL 上传S7Info内容]**.
1. 选择 **[!UICONTROL 浏览]**，选择要使用的以制表符分隔的TXT文件、CSV或SSV文件，然后选择 **[!UICONTROL 打开]**.
1. 选择 **[!UICONTROL 上传]**.

Adobe Dynamic Media Classic会向您发送一封电子邮件，告知您上传是否成功。

## 预览图像映射的变换键文本 {#preview-rollover-key-text-for-an-image-map}

使用“映射页面”屏幕，您可以快速、轻松地查看 eCatalog 特定页面上“图像映射”的“信息面板”文本。

1. 选择目录的变换图像 **[!UICONTROL 编辑]** 按钮。
1. 选择 **[!UICONTROL 映射页面]**.
1. 在屏幕右侧的表格顶部，选择 **[!UICONTROL 信息面板]** 从“显示”菜单中。

   变换键文本显示在包含“信息面板”文本的每个图像映射旁。
