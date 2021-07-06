---
title: 管理电子目录中的信息面板内容
description: 了解如何管理电子目录中的信息面板内容。
uuid: 5aa634f9-0874-4bb5-a3d9-8ce4d5577941
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
discoiquuid: be277831-77cc-4011-ae30-e75c18eec99b
feature: Dynamic Media Classic，查看器，eCatalog
role: User
exl-id: bfb9c5a4-5068-4adb-9fe2-a4ead8656289
source-git-commit: df689ff5a127bfbc400ca5331168d1ff7bb0b42e
workflow-type: tm+mt
source-wordcount: '862'
ht-degree: 67%

---

# 管理电子目录中的信息面板内容{#managing-info-panel-content-in-ecatalogs}

除了在 eCatalog 中将图像映射文本用于变换之外，还可以使用“信息面板”添加大量变换文本（包括链接）。还可以使用定时缓存和计划内容更新来管理信息面板。

您可以在Dynamic Media Classic中使用以下功能管理InfoPanel设置和数据：

* “信息面板设置”面板可用来指定用于显示“信息面板”文本、默认错误响应以及信息缓存的小时数等信息的模板。此外，可以指定是否自动发布 eCatalog。
* 通过“信息面板数据馈送”面板，可以指定包含要在“信息面板”滚动文本中显示的文本的CSV文件，并计划更新信息的时间。
* “导入元数据”对话框（从“映射页面”视图访问）可用来导入包含变换文本信息的制表符分隔 TXT 文件。可以将该 TXT 选项或“数据输入”面板与“CSV 文件”选项结合，用于变换文本。
* “映射页面”视图提供了用于预览为特定图像映射而显示的 XML 的选项。

## 为eCatalogs设置响应模板 {#set-up-a-response-template-for-ecatalogs}

可以选择三个预设响应模板之一用来在“信息面板”中显示文本。这些预设响应模板决定了在“信息面板”中显示信息的方式：列数和行数、字样大小、字体等等。可以选择预设响应模板，或者创建一个自己的模板。

>[!NOTE]
>
>也可以在“查看器预设”中设置响应模板。要改用查看器预设中的响应模板，请在查看器预设中的信息服务器URL末尾添加`fmt=1`。
>
>请参阅[设置 eCatalog 查看器预设](setting-ecatalog-viewer-presets.md#setting_up_ecatalog_viewer_presets)。

1. 双击 eCatalog 以在详细信息视图中将其打开。
1. 单击“信息”(Info)“面板设置”(Panel Setup)面板。
1. 选择“响应模板”：

   * 从“响应模板”菜单中选择预设。模板设计的 XML 显示在“用户模板”框中。
   * 要创建自己的响应模板，请选择&#x200B;**[!UICONTROL Custom]**。 在“用户模板”框中键入模板 XML 定义。可以将预设模板作为您自己的模板的基础。

1. （可选）在默认响应框中，键入当Dynamic Media Classic在检索图像映射信息时遇到错误时要显示的文本。 例如，如果系统收到公司名称和 eCatalog 名称，但是没有变换标识符，则将为用户显示该消息。
1. 在“响应 TTL”框中，输入要在缓存数据之前等待的小时数：

   * 如果在一整天内需要频繁更新数据，则设置一个较小的值。
   * 如果数据相对稳定并且不需要整天频繁更新，则设置一个较大的值。默认为十小时。

1. 单击&#x200B;**[!UICONTROL Publish]**。

## 在电子目录中导入“信息”面板的源内容 {#import-source-content-for-the-info-panel-in-ecatalogs}

可以为 eCatalog 的“信息面板”源文本使用逗号分隔值文件 (CSV) 或制表符分隔文件 (TXT)。制表符分隔文件必须使用 UTF16 (Unicode) 编码。使用不同的方法导入不同的文件类型。

格式化源内容时，谨记以下指导原则：

* 确保制表符分隔数据和逗号分隔数据包含变换模板所必需的列数。
* 确保数据的第一项或列是变换标识符（与图像映射 URL 的 rollover_key 值关联）。
* 确保标识符后面的每个制表符或逗号分隔的项目都是要替换到响应模板中的项目。因此，第一列被替换为$1$，第二列被替换为$2$，依此类推。

### 从外部托管位置将CSV内容导入电子目录 {#import-csv-content-into-ecatalogs-from-an-externally-hosted-location}

1. 双击 eCatalog，以在详细信息视图中将其打开。
1. 单击“信息面板”“数据馈送”面板。
1. 在“外部承载的 CSV 文件位置”框中，输入 CSV 文件的 URL。可以将 URL 粘贴至该字段，或直接键入。
1. （可选）指定使用“计划更新”菜单更新内容的时间，然后单击“添加”。可以选择多个更新时间。每个更新时间显示在“更新时间”框中。（要删除时间，请将其选中，然后单击“删除”。）
1. （可选）单击“立即运行更新”以立即更新内容。

### 导入制表符分隔文件或 CSV 文件 {#import-a-tab-delimited-or-csv-file}

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>SR changed this section 10/23/2012</p>

 -->

1. 双击 eCatalog，以在详细信息视图中将其打开。
1. 单击“信息”(Info)“面板设置”(Panel Setup)面板。
1. 单击&#x200B;**[!UICONTROL 上传S7Info内容]**。
1. 单击&#x200B;**[!UICONTROL 浏览]**，选择要使用的以制表符分隔的TXT文件、CSV或SSV文件，然后单击&#x200B;**[!UICONTROL 打开]**。
1. 按一下&#x200B;**[!UICONTROL 上載]**。

Dynamic Media Classic会向您发送一封电子邮件，告知您上传是否成功。

## 预览图像映射的变换键文本 {#preview-rollover-key-text-for-an-image-map}

使用“映射页面”屏幕，您可以快速、轻松地查看 eCatalog 特定页面上“图像映射”的“信息面板”文本。

1. 单击目录的滚动更新&#x200B;**[!UICONTROL 编辑]**&#x200B;按钮。
1. 单击&#x200B;**[!UICONTROL 映射页面]**。
1. 在屏幕右侧的表顶部，从“显示”菜单中选择“**[!UICONTROL 信息面板]**”。

   在每个包含“信息面板”文本的“图像映射”旁边，都会出现密钥滚动更新文本。
