---
title: 创建eCatalog图像映射
description: 了解如何在Adobe Dynamic Media Classic中创建eCatalog图像映射。
uuid: 943ad3f7-a885-4bc2-88cb-77083384bdf8
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
discoiquuid: 4cf63359-63b5-4da7-9498-335d91b4776c
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: 5e7f39a5-36a6-40df-8752-064a582c9346
source-git-commit: 65e3b69bdcbd651a5f9ab100592217e61a8c05ef
workflow-type: tm+mt
source-wordcount: '1492'
ht-degree: 40%

---

# 创建eCatalog图像映射{#creating-ecatalog-image-maps}

图像映射是eCatalog页面上的一个区域，您可以通过鼠标将其翻转或选择以触发各种操作。 例如，当您将指针移到“图像映射”上时，您将看到项目的变换文本描述。 当您选择图像映射时，将启动另一个操作。 例如，您可以打开网页，以便查看器可以更多地了解一个项目或购买它，您还可以启动视频来查看使用中的项目。

## 绘制eCatalog图像映射 {#drawing-ecatalog-image-maps}

对于 eCatalog，可以在 eCatalog 屏幕的“映射页面”选项卡上绘制图像映射。该屏幕包括显示 eCatalog 页面的图像映射区域，右侧显示“图像映射”列表。创建图像映射时，其名称会输入到“图像映射”列表中。

1. 选择eCatalog的变换 **[!UICONTROL 编辑]** 按钮。
1. 选择 **[!UICONTROL 映射页面]**.
1. 在“映射页面”屏幕的左侧，选择所需页面。
1. 在“图像映射”区域中，绘制一个矩形或多边形（多个边）图像映射：

   * **矩形地图**  — 选择“矩形图像映射”工具并在页面上拖动以创建矩形。

   * **多边形地图**  — 选择“多边形图像映射”工具，然后根据需要多次选择图像的周长。 选择后，Adobe Dynamic Media Classic将绘制图像映射的边框。

      绘制图像映射后，Adobe Dynamic Media Classic会在“图像映射”列表中为其指定一个名称。 为了形成名称，Adobe Dynamic Media Classic会在您正在使用的eCatalog页面的名称后附加一个序列号。

1. （可选）从“图像映射”列表中，位于 [!UICONTROL 名称] 列中，您可以为图像映射输入新名称。 输入的名称中不能包含空格。
1. 您可以让查看者在选择“图像映射”时打开一个新网页。 在“图像映射”列表面板中的“URL”列中输入网页的 URL。

   要更轻松地输入URL（Href模板），请选择 **[!UICONTROL 编辑]** 并输入模板。

参见 [使用模板输入JavaScript和URL](creating-image-maps.md#using_a_template_to_enter_javascript_and_urls).

1. （可选）在显示下拉列表中，选择 **[!UICONTROL 变换文本]**，然后输入您希望用户在图像映射上移动指针时在屏幕上看到的文本。
1. （可选）在显示下拉列表中，选择 **[!UICONTROL 其他操作]**，并输入属性，以便在用户将其指针移动到图像映射上方时触发模糊或聚焦操作。

   参见 [定义图像映射的其他操作](creating-image-maps.md#defining_other_actions_for_image_maps).

1. 选择 **[!UICONTROL 保存]**.
1. （可选）选择 **[!UICONTROL 预览]** 以使用默认的eCatalog查看器预设查看eCatalog。

要删除图像映射，请在“图像映射”列表中选择其名称，然后选择 **[!UICONTROL 删除]**. 要在页面中临时禁用图像映射而不删除该图像映射，可以在“图像映射”列表面板上取消选择图像映射的“开”选项。

## 在eCatalog中嵌入富媒体 {#embedding-rich-media-in-an-ecatalog}

可以使用 eCatalog 的富媒体选项向已添加到 eCatalog 的图像映射添加 MP4 格式的视频或旋转集。当用户在eCatalog中选择“图像映射”区域时，将显示关联的旋转集或视频。 如果想要客户查看使用中的项目，或者从不同的角度和透视图查看项目，此功能将特别有用。

此外，当客户将其指针移动到您的图像映射上时，您还可以选择显示工具提示文本，以便他们知道自己选择了什么。

**要在 eCatalog 中嵌入富媒体:**

1. 绘制 eCatalog 图像映射。

   参见 [绘制eCatalog图像映射](creating-ecatalog-image-maps.md#drawing_ecatalog_image_maps).

1. 在显示下拉列表中，选择 **[!UICONTROL 富媒体]**.
1. 在左侧的“添加资源”面板中，导航到要嵌入的旋转集或视频（MP4 格式）资源所在的文件夹。
1. 将资源拖动到图像映射上。
1. （可选）在“图像映射”列表面板中的 **[!UICONTROL 工具提示]** 列标题，输入您希望查看者在屏幕上将指针移动到图像映射上时看到的文本。
1. 选择 **[!UICONTROL 保存]**.

## 编辑 eCatalog 图像映射 {#editing-ecatalog-image-maps}

从 eCatalog 屏幕的“映射页面”选项卡上开始，使用以下方法来编辑 eCatalog 图像映射：

* **调整位置**  — 选择“平移”工具，并将指针移动到地图边框附近，但不会移动到地图边框上。 当指针显示为四向箭头时，将图像映射拖动到新位置。

   参见 [调整图像映射的位置、形状和大小](creating-image-maps.md#adjusting_the_position_shape_and_size_of_image_maps).

* **更改形状和大小**  — 要调整矩形图像映射的大小，请选择平移工具。 然后将指针移动到边框或角上，看到双向箭头图标时进行拖动。要调整多边形图像映射的大小，请拖动正方形选择手柄。要创建选区手柄，请选择“图像映射”的边框并拖动。

   参见 [调整图像映射的位置、形状和大小](creating-image-maps.md#adjusting_the_position_shape_and_size_of_image_maps).

* **删除图像映射**  — 选择“平移”工具，选择“图像映射”以将其选中，然后选择 **[!UICONTROL 删除]**.

   要从eCatalog中删除所有图像映射，请选择 **[!UICONTROL 排序页面]** 选项卡，然后选择 **[!UICONTROL 清除映射]**.

* **处理重叠的图像映射**  — 拖动以更改图像映射在图像映射列表中的顺序。

   参见 [处理重叠的图像映射](creating-image-maps.md#handling_overlapping_image_maps).

* **将图像映射复制到其他页面**  — 选择 **[!UICONTROL 将映射复制到]** （确保您位于“映射页面”选项卡上）。 在选择图像屏幕上，选择要复制图像映射的一个或多个页面，然后选择 **[!UICONTROL 选择]**.

   参见 [将图像映射复制到其他图像](creating-image-maps.md#copying_image_maps).

>[!NOTE]
>
>除了将图像映射复制到eCatalog中的不同页面之外，您还可以将eCatalog中的所有图像映射复制到其他eCatalog。 参见 [在eCatalog之间复制图像映射](creating-ecatalog-image-maps.md#copying_image_maps_between_ecatalogs).

## 查看和导入图像映射数据 {#reviewing-and-importing-image-map-data}

“映射摘要”屏幕提供了关于您的 eCatalog 的元数据。也可以从“映射摘要”屏幕开始为 eCatalog 批量导入图像映射数据。用这种方法导入图像映射数据可以简化图像映射 URL 及变换文本的输入。

要查看“映射摘要”屏幕，请在eCatalog屏幕的“映射页面”选项卡上选择 **[!UICONTROL 摘要]**.

### 检查图像映射数据摘要 {#review-image-map-data-summary}

1. 在映射页面屏幕上，选择 **[!UICONTROL 摘要]**.

   “映射摘要”屏幕显示 eCatalog 中图像映射、URL、变换文本说明以及其他操作的数量。

1. 如果出现变换键错误，请在 **[!UICONTROL Rollover_Key错误]** 列查看电子表格中必须更改哪些内容才能更正错误。 可以选择并复制该消息的文本，并将其粘贴到电子表格中。
1. 选择 **[!UICONTROL 预览]** 因此，您可以在eCatalog查看器中检查页面；选择X以关闭“摘要”屏幕并返回到“映射页面”屏幕，或者选择 **[!UICONTROL 关闭]** 以返回浏览。

### 导入图像映射数据 {#import-image-map-data}

可以将整个 eCatalog 的数据导入到“映射摘要”屏幕中，而不必在每个页面都输入图像映射数据。可以通过制表符分隔的文件或 XML DTD 的形式导入图像映射数据。文件中的字段必须与“映射摘要”屏幕中显示的顺序相同：“名称”、“TOC 标签”、“映射”、“URL”、“变换文本”、“其他操作”和“搜索字符串”。导入图像映射数据可以免去创建每个图像映射时在“图像映射”列表中输入数据的麻烦。

>[!NOTE]
>
>在导入图像映射数据之前，必须已经创建图像映射。

在“映射摘要”屏幕上开始，按照以下步骤为创建的图像映射导入图像映射数据：

1. 选择 **[!UICONTROL 导入映射数据]**.
1. 在导入元数据对话框中，选择 **[!UICONTROL 浏览]**，然后选择制表符分隔或XML DTD文件。
1. 在“作业名称”字段中，键入文件的名称（注意保留其扩展名）。
1. 选择 **[!UICONTROL 上传]**.

## 在eCatalog之间复制图像映射 {#copying-image-maps-between-ecatalogs}

可以将 eCatalog 中的所有图像映射复制到其他 eCatalog 中。这种复制图像映射的方法是在相同的 eCatalog 的外语翻译之间复制图像映射的方便方法。为了成功复制，Adobe Dynamic Media Classic建议在具有相同页数和相同图像的eCatalog之间复制。

>[!NOTE]
>
>如果图像映射所复制到的 eCatalog 已经包含图像映射，复制时将删除原有的图像映射。

要将一个eCatalog中的所有图像映射复制到另一个eCatalog，请执行以下操作：

1. 选择要复制的带有图像映射的eCatalog，然后选择eCatalog的变换图像 **[!UICONTROL 编辑]** 按钮。
1. 在订单页选项卡上，选择 **[!UICONTROL 复制映射]**.
1. 在选择资产对话框中，选择要复制图像映射的eCatalog，然后选择 **[!UICONTROL 选择]**.

如果目标eCatalog（您复制图像映射的eCatalog）的页数或图像大小不同，则Adobe Dynamic Media Classic会显示警告消息。 选择 **[!UICONTROL 继续]** 以复制图像映射，而不管是否出现警告。
