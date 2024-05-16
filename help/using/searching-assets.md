---
title: 搜索Dynamic Media Classic资源
description: 了解如何在Adobe Dynamic Media Classic中搜索资源。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 4b3f690c-7dff-4bf0-9366-085ba918fe6b
topic: Content Management
level: Intermediate
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '1513'
ht-degree: 17%

---

# 在Adobe Dynamic Media Classic中搜索资源{#searching-assets}

要在Adobe Dynamic Media Classic中查找文件资源，您可以按类型查看资源，在“浏览”面板中排序资源，执行简单搜索，执行高级搜索，以及筛选资源。

>[!NOTE]
>
>“个人设置”页提供了选择搜索方式的选项。 例如，可以选择一个默认的搜索类型，并选择搜索中是否包括用户定义的字段。有关更多信息，请参阅[个人设置](personal-setup.md#personal_setup)。

## 按类型查看资源 {#viewing-assets-by-type}

要在浏览时只查看特定类型的文件，请在左侧资产库的 **[!UICONTROL 显示]** 从下拉列表中选择文件类型。 只有您选择显示的类型资产才会显示在资产库中。

>[!NOTE]
>
>如果在左侧看不到“资源库”面板，请单击Dynamic Media Classic窗口下半侧右侧的三角形箭头以打开资源库。

## 在“浏览”面板中对文件排序 {#sorting-files-in-the-browse-panel}

您可以对右侧“浏览”面板中显示的文件夹内容或搜索结果进行排序。 在全局导航栏上，选择 **[!UICONTROL 排序]**，然后选择一个选项。 选项包括 **[!UICONTROL 名称]**， **[!UICONTROL 大小(KB)]**， **[!UICONTROL 类型]**， **[!UICONTROL 创建日期]**、和 **[!UICONTROL 上次修改时间]**.

您还可以选择 **[!UICONTROL 升序]** 或 **[!UICONTROL 降序]** 要按您选择的标准以升序或降序对资源排序，请执行以下操作：

在“列表视图”中，可以通过选择列名进行排序。

## 执行简单搜索 {#conducting-a-simple-search}

使用资产库中的搜索字段，以便进行简单的搜索。 可以按名称搜索项目，也可以搜索其元数据包含某个关键字的项目。

1. 在资产库中的 **[!UICONTROL 文件夹]** 面板，选择要在特定文件夹及其子文件夹中搜索的文件夹。
1. 在资产库中的搜索字段的左侧，选择 **[!UICONTROL 放大镜]** 图标，以打开下拉列表。
1. 在下拉列表中，选择一个选项，该选项描述希望搜索范围是多窄，多宽。 您可以选择 **[!UICONTROL 在所有文件和文件夹中]**， **[!UICONTROL 在选定的文件夹中]**，或 **[!UICONTROL 在选定的文件夹和子文件夹中]**.
1. 在搜索字段中，输入搜索词。
1. 在搜索字段的右侧，选择 **[!UICONTROL 开始]** 或按 **[!UICONTROL 输入]**.

   搜索结果将显示在右侧的“浏览”面板中。

<!-- Does not appear to be working anymore >[!NOTE]
>
>Adobe Dynamic Media Classic tracks searches. To run a search a second time, select **[!UICONTROL Search]** and choose the name of a search at the bottom of the Search menu. -->

## 执行高级搜索 {#conducting-an-advanced-search}

在资产库中的搜索字段正下方，选择 **[!UICONTROL 高级搜索]** 使用多个条件（包括元数据字段中的值）进行搜索。

在高级搜索中指定以下任一条件：

* **按资源类型筛选**：将搜索范围缩小到仅一种资源类型。 在菜单中选择一种资产类型。

* **文件和文件夹**：选择要搜索的位置： **[!UICONTROL 在所有文件和文件夹中]**， **[!UICONTROL 在选定的文件夹中]**，或 **[!UICONTROL 在选定的文件夹和子文件夹中]**.

* **所有发布状态**：搜索标记为准备发布的文件、未标记为准备发布的文件或所有文件。

* **条件**：如果为搜索指定元数据标准，请选择搜索是必须匹配所有条件（ALL搜索）还是任何条件（OR搜索）。

* **搜索条件**：创建一个或多个搜索字段以搜索元数据。 要创建检索字段：

   1. 在“高级搜索”中的 **[!UICONTROL 搜索条件]** 标题，并在 **[!UICONTROL 添加字段]** 菜单)，选择向下三角形箭头图标以打开下拉列表。 选择元数据视图。 您可以选择 **[!UICONTROL 具有值的所有属性]**， **[!UICONTROL 紧凑视图]**， **[!UICONTROL IPTC]**， **[!UICONTROL 元数据服务器发布字段]**，或 **[!UICONTROL XMP]**.
   1. 选择 **[!UICONTROL 添加字段]** 下拉菜单，然后选择字段名称。
   1. 选择 **[!UICONTROL 包含]** 选项： **[!UICONTROL 包含]**， **[!UICONTROL 不包含]**， **[!UICONTROL 开头为]**， **[!UICONTROL 结尾为]**，或 **[!UICONTROL 等于]**.
   1. 对于数字字段，选择一个值或输入一个自定义日期范围。
   1. （可选）重复步骤 1-4 创建更多个搜索字段。

选择 **[!UICONTROL 删除搜索字段]** 图标（内部带有“X”的圆形），因此删除搜索字段。

在高级搜索面板的右下角，选择 **[!UICONTROL Search]** 开始您的搜索。 搜索结果将显示在右侧的“浏览”面板中。 您可以更改任何搜索条件并选择 **[!UICONTROL Search]** 再次运行搜索。

选择 **[!UICONTROL 清除]** 如果要清除搜索条件并开始新搜索，请执行以下操作。 选择 **[!UICONTROL 关闭]** 完成搜索以关闭“搜索”面板时。

## 使用元数据过滤资源 {#filter-assets-using-metadata}

过滤资源库“过滤器”选项卡中的资源。要过滤资源，可使用元数据值作为条件。选择要过滤的元数据字段后，“过滤器”选项卡会列出在所选字段中输入的所有元数据值。 它还列出了为每个值分配的资源数。 例如，在对 **[!UICONTROL 创建者]** 元数据字段， **[!UICONTROL 过滤器]** 选项卡列出了在 **[!UICONTROL 创建者]** 不同资源的元数据字段。 它还列出了每个名称的名称以及分配给该名称的资产数量。 然后，选择一个元数据值以查看分配了该值的所有资源。 在本例中，选择 `Prairie Cat` 元数据值，用于查看名称为的所有资源 `Prairie Cat` 输入于 **[!UICONTROL 创建者]** 元数据字段。 可以使用多个元数据字段作为过滤条件进行过滤。

您可以保存过滤器操作以多次运行它们。

>[!NOTE]
>
>仅默认元数据视图中的元数据字段可用于过滤器操作。“元数据视图”页显示默认元数据视图的名称。

请参阅[元数据视图](application-setup.md#metadata_views)。

### 运行筛选器操作 {#running-a-filter-operation}

请按照以下步骤操作，以便您可以通过使用资产的元数据值进行筛选来查找资产：

1. 在资产库中，选择 **[!UICONTROL 过滤器]** 选项卡。

   上一个过滤器操作的条件将显示在“过滤器”窗格中。“过滤器”窗格分成几个面板，每个面板各显示一个元数据字段。可使用面板来选择要作为过滤条件的元数据字段，在每个字段内，选择一个要用于过滤器操作的元数据值。

   要运行已创建和保存的筛选器操作，请选择 **[!UICONTROL 选择预设]**，然后在菜单中选择操作的名称。

   请参阅 [保存、重复和删除筛选器操作](searching-assets.md#saving_repeating_and_deleting_filter_operations).

1. 单击 **[!UICONTROL 字段]** 然后，在面板上按照以下说明操作，以便您可以显示筛选菜单并构建筛选操作：

   * **选择元数据字段**：在筛选菜单中选择字段的名称。

     >[!NOTE]
     >
     >过滤菜单中仅显示默认元数据视图中的元数据字段的名称。

     请参阅[元数据视图](application-setup.md#metadata_views)。

   * **添加元数据字段**：选择 **[!UICONTROL 添加面板]**. 该面板出现在“筛选器”窗格上后，选择其 **[!UICONTROL 字段]** 按钮，然后在筛选菜单中选择元数据字段的名称。

   * **删除元数据字段**：选择 **[!UICONTROL 删除此面板]** 在筛选菜单中。

   选择元数据字段时，其面板会列出以下内容：

   * 所有元数据值都输入到字段中。
   * 对于每个元数据值，分配有此值的资源的数目。

1. 根据需要多次重复执行第 2 步以列出面板上用于过滤器操作的所有元数据字段。
1. 在每个面板中，选择一个要作为过滤条件的元数据值。不能在每个面板中选择多个元数据值。

   与您选择的所有值匹配的资源将显示在“浏览”面板中。

   >[!NOTE]
   >
   >通过单击从筛选操作中临时删除字段 **[!UICONTROL 取消全选]**. 此选项位于每个面板的顶部，在元数据值上方。

1. （可选）要保存筛选操作以便以后运行，请选择 **[!UICONTROL 选择预设]** > **[!UICONTROL 将当前预设另存为新预设]**，然后在 **[!UICONTROL 保存]** 对话框。

### 保存、重复和删除筛选器操作 {#saving-repeating-and-deleting-filter-operations}

按照过滤器选项卡中的以下说明进行操作，以便保存、重复和删除过滤器操作：

* **保存筛选器操作**：转到 **[!UICONTROL 选择预设]** > **[!UICONTROL 将当前预设另存为新预设]**，然后在 **[!UICONTROL 保存]** 对话框。

* **重复筛选器操作**：选择 **[!UICONTROL 选择预设]** 并在菜单中选择过滤器操作的名称。 菜单将列出您所保存的过滤器操作。

* **从选择预设菜单删除滤镜操作**：运行过滤器操作。 然后，转到 **[!UICONTROL 选择预设]** > **[!UICONTROL 删除预设]** 在菜单上。

## 使用元数据服务器 {#using-the-metadata-server}

元数据服务器是一个公共API，可用于通过http请求按元数据搜索资源。

要配置元数据服务器，请转到 **[!UICONTROL 设置]** > **[!UICONTROL 应用程序设置]** > **[!UICONTROL 发布设置]** > **[!UICONTROL 元数据服务器]**.

元数据服务器发布页面可让您设置以下选项：

* **[!UICONTROL 即时发布]**：在更改元数据时自动推送这些更改，包括新资源、关键词更改等。

* **[!UICONTROL XMP数据包]**：发布XMP数据包。 此数据包不用于搜索，但提供最新的XMP。

* **[!UICONTROL 关键字]**：将关键字发布到元数据服务器以用于搜索。

* **[!UICONTROL 元数据服务器发布字段]**：选择要包含在元数据中的字段。 通过此选项，可决定公众可以使用的资产信息量。 这些字段也显示在元数据视图中，但只能在元数据服务器中进行更改。

选择 **[!UICONTROL 立即发布]** 以启动作业。 此时会出现一条确认消息，通知您作业已启动。

>[!MORELIKETHIS]
>
>* [导航基础知识](navigation-basics.md#navigation_basics)
>* [查看、添加和导出元数据](viewing-adding-exporting-metadata.md#viewing_adding_and_exporting_metadata)
