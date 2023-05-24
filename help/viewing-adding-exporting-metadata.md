---
title: 查看、添加和导出元数据
description: 了解如何在Adobe Dynamic Media Classic中查看、添加和导出元数据。
uuid: a5254c51-9e04-45ae-8236-3eab2925e5fc
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: 5414b4f5-6e05-468c-8725-385423596342
feature: Dynamic Media Classic,Asset Management,Metadata
role: User
exl-id: 2be50cc7-9a8b-4f7b-8ebf-18a3208654f2
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '2261'
ht-degree: 45%

---

# 查看、添加和导出元数据{#viewing-adding-and-exporting-metadata}

您可以存储特定于您在Adobe Dynamic Media Classic中使用的文件的信息；此信息称为 *元数据*. 您可以在Adobe Dynamic Media Classic中使用元数据来组织、搜索、筛选和排序资源。

元数据与Adobe Dynamic Media Classic生成的信息（如文件创建日期、发布日期和关键词）一起显示在详细信息视图中。 要查看元数据，请在详细信息视图中打开资源，然后选择元数据面板。 可以在详细信息视图中输入和编辑 元数据。

一些元数据直接嵌入到文件中。如果文件包含此元数据，Adobe Dynamic Media Classic会自动将其与文件一起上传。 您可以将元数据嵌入到Adobe Photoshop、InDesign、Illustrator和其他应用程序的源资源中；Adobe Dynamic Media Classic可识别此元数据。 您还可以在“详细信息视图”的“元数据”面板中将元数据添加到各个文件。 为了确保资源的一致性，公司管理员创建了元数据模板，提供可以填写的元数据字段。

有关嵌入元数据的更多信息，请参阅 [可扩展的元数据平台](https://www.adobe.com/products/xmp.html).

## 查看元数据 {#view-metadata}

要查看资源的元数据，请在详细信息视图中打开该资源，然后点按元数据面板。 要选择一组元数据字段，请在“元数据视图”菜单中选择一个选项。 Adobe Dynamic Media Classic提供以下元数据视图：

* **压缩视图**  — 基本值列表。

* **IPTC**  — 国际新闻电讯委员会界定的价值观。

* **XMP**  — 由可扩展元数据程序定义的值。

管理员可以创建元数据视图。这些视图也显示在“元数据视图”菜单中。

参见 [元数据视图](application-setup.md#metadata_views) 有关创建元数据视图的信息。

## 为资源手动输入元数据 {#manually-enter-metadata-for-an-asset}

1. 在“详细信息”视图中打开资产。
1. 打开“元数据”面板并执行以下一项操作或全部操作：

   * 选择一种元数据视图，以确定面板中显示哪些元数据字段。
   * 选择一个预设值，然后选择 **[!UICONTROL 应用]** 以使用预设值填充元数据字段。 这些预设值由公司管理员创建。

1. 在“元数据”面板中输入值。

>[!NOTE]
>
>要一次编辑多个资源的元数据，请选择资源并转到 **[!UICONTROL 文件]** > **[!UICONTROL 编辑信息]**. 在“编辑信息”窗口中对元数据所进行的编辑会应用于所有选定资源。

## 添加或编辑关键字 {#add-or-edit-keywords}

除了元数据之外，您还可以使用关键字来帮助搜索和管理资源。

如果您在此会话期间将关键字添加到其他文件，或者如果您已将关键字从列表中删除，则这些关键字将出现在“关键字建议”表中。

1. 在详细信息视图中打开文件。
1. 选择 **[!UICONTROL 关键字]**.
1. 要添加关键字，请执行以下任意操作：

   * 在文本框中键入关键字并选择 **[!UICONTROL 添加]**.
   * 在 **[!UICONTROL 关键词建议]** 表格。

1. 要删除关键字，请选择该关键字并选择 **[!UICONTROL 移除]**. 该关键字会移到“关键字建议”表中。

>[!NOTE]
>
>您可以在将关键字上传到Adobe Dynamic Media Classic时将其添加到文件。 在“上载作业选项”对话框中，选择 **[!UICONTROL 其他元数据]** 并输入关键字。
>请参阅[上载选项](uploading-files.md#upload_options)。

## 导入元数据 {#import-metadata}

可以从制表符分隔的文件或 XML 文件为多个不同资源导入元数据，而不必每次一个为资源手动输入元数据。在制表符分隔文件或 XML 文件中输入元数据并导入该文件比在各个资源中输入元数据节省时间。在制表符分隔文件的第一行中，输入要为其记录元数据的字段的 ID 和名称。在每个后续行中，输入资源 ID 名称，后跟元数据值。系统不会对制表符分隔文件或 XML 文件中未包括的字段进行修改。要从 XML 文件导入元数据，请确保您符合 DTD。

>[!NOTE]
>
>您可以创建一个用于输入元数据的模板，以便可以将它正确导入到Adobe Dynamic Media Classic。 创建模板之后，可以使用该模板输入元数据。
>请参阅[创建模板以输入要上载的元数据](viewing-adding-exporting-metadata.md#create_a_template_for_entering_metadata_to_upload)。

您可以在以下位置找到有关标准化属性的更多信息： [AdobeXMP开发人员中心](https://www.adobe.com/devnet/xmp.html).

1. 在浏览面板中，选择要从制表符分隔的文件或 XML 文件为其添加元数据的图像。
1. 转到 **[!UICONTROL 文件]** > **[!UICONTROL 导入元数据]**.
1. 在 **[!UICONTROL 上载元数据]** 对话框中，选择 **[!UICONTROL 浏览]**.
1. 在“**[!UICONTROL 选择要上载的文件]**”对话框中，选择包含元数据的制表符分隔文件或 XML 文件。
1. 输入作业名称。
1. 选择 **[!UICONTROL 上传]**.

### 识别导入中的不同元数据类型

在识别要导入的不同元数据类型时，请记住以下几点：

* 用户定义的字段由其名称标识，如中所创建 **[!UICONTROL 设置]** > **[!UICONTROL 应用程序设置]** > **[!UICONTROL 元数据]** > **[!UICONTROL 用户定义的字段]**. 使用“生成文件”功能来获取采用正确导入格式的所有已定义 UDF 的列表。
* “XMP 元数据”属性在（属性-）名称之前必须具有相关 XMP- 前缀。前缀和名称之间用冒号分隔。XMP前缀可在 **[!UICONTROL 设置]** > **[!UICONTROL 应用程序设置]** > **[!UICONTROL 元数据]** > **[!UICONTROL 元数据架构]** 编辑者。 技术名称可在相关 XMP 架构文档中找到。XMP属性名称未出现在生成文件功能中。
* “元数据架构”属性在（属性-）名称之前必须具有相关前缀。前缀和名称之间用冒号分隔。前缀和属性名称是在元数据架构编辑器中定义的。元数据架构属性名称未显示在生成文件功能中。

例如：关键字的XMP属性是前缀为“Dublin Core”的XMP架构 `dc` 和 `subject` 是技术XMP名称。 前缀和技术XMP名称将合并到 `dc:subject` 完整的属性名称。 在XML元数据导入格式中， `dc.subject` 必须为属性名称。 在制表符分隔的导入格式中，它必须是列标题。

### 导入关键字

关键字可以导入为以逗号分隔的列表。 如果逗号出现在任何单个值中，则必须使用反斜杠(\)进行转义。 反斜杠字母为常见的双反斜杠 (\\)。

例如，包含值的元数据导入文件 `Hello\, World!,back\\slash,foo` 对象 `dc:subject` 在资源上设置三个XMP关键字： `Hello, World!,` `back\slash,` 和 `foo`.

### 导入 XMP 和元数据架构元数据 XMP 文件

XML 导入仅接受有效的 XML。导入XMP或元数据架构字段时，会添加命名空间前缀，其行为在此处类似于XMP-namespace。 必须声明此命名空间。 例如，在顶级标记中。

例如：

```as3
<ips> 
    <ghw_object vc_objectname="img_001" dc:subject="word1,word2" 
</ips>
```

### 导入XMP和元数据架构元数据制表符分隔文件

必须在导入字段的相关列标题中添加前缀。

## 导入元数据（通过 FTP） {#import-metadata-via-ftp}

通过在制表符分隔或XML文件中输入元数据并选择 **[!UICONTROL 处理元数据文件]** 在上传作业选项（通过FTP选项卡）页面上。

确保制表符分隔文件或 XML 文件中的数据格式正确。在第一行中，输入 ID 字段，随后输入要修改的元数据字段名称。在每个后续行中，输入资源 ID 名称，后跟元数据值。系统不会对制表符分隔文件或 XML 文件中未包括的字段进行修改。

在全局导航栏上，选择 **[!UICONTROL 上传]**. 要导入元数据，请在“上载”页面上，选择 **[!UICONTROL 通过FTP]** 选项卡，然后选择 **[!UICONTROL 作业选项]**. 在“上载作业选项”对话框中，选择 **[!UICONTROL 作业]**，然后选择 **[!UICONTROL 处理元数据文件]** 复选框。

## 使用元数据批量重命名 ID {#batch-rename-ids-using-metadata}

使用从制表符分隔文件或XML文件导入的元数据，可以重命名Adobe Dynamic Media Classic ID。 导入的元数据仅适用于在元数据文件自身中指定的图像。无论是否在“浏览”面板中选择了图像。

要重命名图像的Adobe Dynamic Media Classic ID，请添加一个标记为的列 *newipsid* 到以制表符分隔的文件中，或添加一个名为的字段 `new_vc_objectname` 到XML数据。

例如：

|  | newipsid |
| --- | --- |
| testjacket_1 | Jacket_test_1 |
| testjacket_blue | Jacket_test_2 |

元数据作业的作业日志显示已成功重命名的ID和未重命名的ID。

## 创建模板以输入要上载的元数据 {#create-a-template-for-entering-metadata-to-upload}

Adobe Dynamic Media Classic提供了一个用于创建用于记录元数据的模板的命令。 使用模板可确保以正确的格式输入元数据，以便能够将其正确上传到Adobe Dynamic Media Classic。 要创建用于记录元数据并将其导入到Adobe Dynamic Media Classic的模板，请执行以下步骤：

1. 选择包含您想要用于模板的元数据字段的图像资源。
1. 转到 **[!UICONTROL 文件]** > **[!UICONTROL 导入元数据]**.
1. 对于 **[!UICONTROL 资产属性类型]**，选择 **[!UICONTROL 图像]**.
1. 从 **[!UICONTROL 生成文件]** 下拉列表，选择 **[!UICONTROL 制表符分隔模板]**， **[!UICONTROL 资产的XML元数据]**，或 **[!UICONTROL XML DTD]**.
1. 选择 **[!UICONTROL 生成]**.
1. 在显示的对话框中，复制数据。使用此数据构建模板。

## 使用元数据架构 {#working-with-metadata-schemas}

公司管理员可以查看所有可用的架构的列表。在全局导航栏上，转到 **[!UICONTROL 设置]** > **[!UICONTROL 应用程序设置]** > **[!UICONTROL 元数据]** > **[!UICONTROL 元数据架构]**.

最初，XMP等全局标准架构的列表是隐藏的。 通过选中列表底部的复选框，可以显示该列表。

公司管理员可以创建自定义架构，或编辑现有的自定义架构。

您可以使用元数据架构编辑器来执行以下操作：

| 操作 | 说明 |
| --- | --- |
| 添加 | 向架构中添加属性。 模式对话框收集以下信息：ID、标签、结构和数据类型。 |
| 添加选项值 | 向结构为开放式选项或限定式选项的属性中添加新的可选择选项。所有选项值的类型相同。选择资产本身以启用按钮。 |
| 编辑 | 编辑属性或选项值的标签。您仅可更改标签、ID，类型信息不可变。 |
| 上移/下移 | 架构的顺序反映在 UI 中。要更改此顺序，请选择属性或选项值，并通过按钮进行移动。当前不支持拖放。 |
| 删除 | 从架构中删除属性或选项值。它不会从XMP块或数据库中删除值。 该属性不再可用于元数据视图，将从资产详细信息视图中删除。 如果属性已发布到元数据服务器，请执行强制发布以从面向公众的元数据服务器中删除数据。 |

系统会自动为用户定义的字段生成一个前缀为的自定义架构 `s7udf`. 它是现有的用户定义的字段，并在其自己的设置部分中编辑。

>[!NOTE]
>
>对架构所做的更改永远不会更改资源元数据自身。但是，它们并非对所有Adobe Dynamic Media Classic和元数据服务器功能均可见，并且在更改后无法访问。 同样，如果资源的元数据存在，则创建匹配架构会使该元数据在Adobe Dynamic Media Classic和元数据服务器中可用。

元数据架构编辑器提供了一种在Adobe Dynamic Media Classic中添加或编辑自定义公司架构的图形方式。 架构由前缀、命名空间和一系列属性定义。

* **[!UICONTROL 名称]**  — 架构的UI名称。 用于在元数据视图和高级搜索中识别属性。类似于 XMP 部分，如“基本”、IPTC、PDF。

* **[!UICONTROL 前缀]**  — 架构的技术唯一标识符。 仅限字母a-z和A-Z。当资源的元数据存储在XMP块和数据库中时，前缀在Adobe Dynamic Media Classic UI中不可见，但已使用。 前缀用于在元数据服务器上的元数据搜索查询中或导入时唯一识别元数据字段。

* **[!UICONTROL 命名空间]**  — 架构的技术唯一标识符，通常为表单中的URL `https://your.company.com/name/version/`. 有关示例，请参阅标准架构列表。命名空间在Adobe Dynamic Media Classic UI中不可见，但用于在XMP块中存储元数据。

* **[!UICONTROL 描述]**  — 架构的自由形式描述。

>[!NOTE]
>
>前缀和命名空间无法编辑。要更改这些属性，您必须删除并重新创建架构。

属性用于描述可与此架构一起存储在 XMP 块中的元数据。属性包括：

| 属性 | 说明 |
| --- | --- |
| ID | 该属性的技术性标识符。该ID在Adobe Dynamic Media Classic UI中不可见，但在资源的元数据存储在XMP块和数据库中时使用。 ID 用于在元数据服务器上创建搜索查询。ID 具有以下限制： <ul><li>不得包含空格</li><li>不得包含“.”、“:”和“$”</li><li>第一个字符不得为数字</li><li>最好使用 a-z 或 A-Z 作为第一个字符</li></ul> <br>创建后，ID 即无法更改。 |
| 标签 | 该属性的 UI 名称。 |
| 结构 | 与数据类型一起确定属性的类型。结构可能为：<ul><li>简单类型：单个数据类型值</li><li>序列：相同数据类型的值的列表</li><li>开放式选项：从预定义的值列表中选择一项，或随意输入文本。数据类型仅可为字符串型或整型</li><li>限定式选项：从预定义的值列表（弹出窗口或组合框）中选择一项</li></ul> |
| 数据类型 | 从以下可用的类型中选择： <ul><li>字符串型</li><li>整型</li><li>浮点型</li><li>是/否（布尔型）</li><li>日期</li></ul> |

当属性的结构为“开放式选项”或“限定式选项”时，您必须提供至少一个选项值。开放式选项可以更改。限定式选项不可更改。所有选项值都具有属性的数据类型。

| 属性 | 说明 |
| --- | --- |
| ID | 该值的技术性标识符。ID在Adobe Dynamic Media Classic UI中不可见，但当资源的元数据存储在XMP块和数据库中时，会使用该ID。 ID 用于元数据服务器上的搜索查询。ID 不可包含空格。创建后，ID 即无法更改。 |
| 标签 | 该值的 UI 名称。 |

>[!MORELIKETHIS]
>
>* [Viewer Presets](application-setup.md#viewer_presets)
>* [Metadata Presets](application-setup.md#metadata_presets)

