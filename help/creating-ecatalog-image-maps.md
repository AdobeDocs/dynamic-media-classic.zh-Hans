---
title: 创建 eCatalog 图像映射
seo-title: 创建 eCatalog 图像映射
description: 'null'
seo-description: 了解如何创建电子目录图像映射。
uuid: 943ad3f7-a885-4bc2-88cb-7708384bdf8
contentOwner: admin
content-type: 引用
products: SG_ EXPERIENCE MANAGER/Dynamic-Media-Scene-7
geptopics: SG_ SCENESELEFERENDER_ PK/categories/ecatalloc
discoiquuid: cf63359-63b5-4da7-9498-335d91b4776c
translation-type: tm+mt
source-git-commit: d5bf894d56687561c93ef08762bc19d3597225e6

---


# 创建 eCatalog 图像映射{#creating-ecatalog-image-maps}

图像映射是 eCatalog 页面上的一个区域，您可以在该区域内滚动鼠标或单击鼠标，以触发各种操作。例如，将鼠标指针移动到“图像映射”上时，您会看到某个物品的变换文本说明。单击“图像映射”时，将启动其他操作。例如，您可以打开网页，以便查看器可以更多地了解一个项目或购买它，您还可以启动视频来查看使用中的项目。

## 绘制 eCatalog 图像映射 {#drawing-ecatalog-image-maps}

对于 eCatalog，可以在 eCatalog 屏幕的“映射页面”选项卡上绘制图像映射。该屏幕包括显示 eCatalog 页面的图像映射区域，右侧显示“图像映射”列表。创建图像映射时，其名称会输入到“图像映射”列表中。

1. 单击 eCatalog 的变换“编辑”按钮。
1. Click **Map Pages**.
1. 在“映射页面”屏幕的左侧，选择所需页面。
1. 在“图像映射”区域中，绘制一个矩形或多边形（多个边）图像映射：

   **矩形映射** 选择矩形图像映射工具并在页面上拖动以创建矩形。

   **多边形映射** 选择多边形图像映射工具，并在图像的周长周围单击任意多次。单击时，Dynamic Media经典将绘制图像映射的边框。

   绘制图像映射后，Dynamic Media经典在图像映射列表中为其分配名称。要构成该名称，Dynamic Media经典将一个序号附加到您工作的电子目录页面的名称。

1. （可选）在“图像映射”列表面板中的“名称”列下，为图像映射输入新名称。输入的名称中不能包含空格。
1. 可以使查看者在单击“图像映射”时打开新的网页。在“图像映射”列表面板中的“URL”列中输入网页的 URL。

   单击“编辑”并输入模板可使 URL 输入（HREF 模板）更轻松。

   请参阅[使用模板输入 JavaScript 和 URL](creating-image-maps.md#using_a_template_to_enter_javascript_and_urls)。

1. (Optional) In the Show drop-down list, click **Rollover Text**, and then enter the text that you want users to see onscreen when they move their pointers over the Image Map.
1. (Optional) In the Show drop-down list, click **Other Actions**, and enter an attribute to trigger a blur or focus action when users move their pointers over an Image Map.

   请参阅[定义图像映射的其他操作](creating-image-maps.md#defining_other_actions_for_image_maps)。

1. 单击“**保存**”。
1. (Optional) Click **Preview** to view the eCatalog with the default eCatalog Viewer preset.

要删除图像映射，请在“图像映射”列表中选择其名称，然后单击“删除”。要在页面中临时禁用图像映射而不删除该图像映射，可以在“图像映射”列表面板上取消选择图像映射的“开”选项。

## 在 eCatalog 中嵌入富媒体 {#embedding-rich-media-in-an-ecatalog}

可以使用 eCatalog 的富媒体选项向已添加到 eCatalog 的图像映射添加 MP4 格式的视频或旋转集。当用户单击 eCatalog 中的图像映射区域时，关联的视频或旋转集将弹出。如果想要客户查看使用中的项目，或者从不同的角度和透视图查看项目，此功能将特别有用。

您还可以选择当客户将鼠标指针置于图像映射上时显示工具提示文本，以便客户知道他们正在单击的对象。

**要在 eCatalog 中嵌入富媒体**

1. 绘制 eCatalog 图像映射。

   请参阅[绘制 eCatalog 图像映射](creating-ecatalog-image-maps.md#drawing_ecatalog_image_maps)。

1. 在“显示”下拉列表中，选择“富媒体”。
1. 在左侧的“添加资源”面板中，导航到要嵌入的旋转集或视频（MP4 格式）资源所在的文件夹。
1. 将资源拖动到图像映射上。
1. （可选）在“图像映射”列表面板中的“工具提示”列标题下，输入当查看者将鼠标指针置于图像映射上时您想要他们在屏幕上看到的文本。
1. 单击“保存”。

## 编辑 eCatalog 图像映射 {#editing-ecatalog-image-maps}

从 eCatalog 屏幕的“映射页面”选项卡上开始，使用以下方法来编辑 eCatalog 图像映射：

**调整位置** 选择平移工具，并将指针移动到地图的边框附近。当指针显示为四向箭头时，将图像映射拖动到新位置。

请参阅[调整图像映射的位置、形状和大小](creating-image-maps.md#adjusting_the_position_shape_and_size_of_image_maps)。

**更改形状和大小** 要调整矩形图像映射的大小，请选择平移工具。然后将指针移动到边框或角上，看到双向箭头图标时进行拖动。要调整多边形图像映射的大小，请拖动正方形选择手柄。要创建选择手柄，单击图像映射的边框并拖动。

请参阅[调整图像映射的位置、形状和大小](creating-image-maps.md#adjusting_the_position_shape_and_size_of_image_maps)。

**删除图像映射** 选择平移工具，单击图像映射以将其选中，然后单击删除。

要从 eCatalog 中删除所有图像映射，单击“排序页面”选项卡，然后单击“清除映射”。

**处理重叠的图像映射** 拖动以更改图像映射列表上图象映射的顺序。

请参阅[处理重叠的图像映射](creating-image-maps.md#handling_overlapping_image_maps)。

**将图像映射复制到其他页面** 选择将映射映射到按钮(确保您在映射页面选项卡上)。在“选择图像”屏幕上，选择要在其中复制图像映射的一个或多个页面，然后单击“选择”按钮。

请参阅[将图像映射复制到其他图像](creating-image-maps.md#copying_image_maps)。

>[!NOTE]
>
>除了将图像映射复制到 eCatalog 中的其他页面外，您还可以将 eCatalog 中的所有图像映射复制到其他 eCatalog。请参阅[在 eCatalog 之间复制图像映射](creating-ecatalog-image-maps.md#copying_image_maps_between_ecatalogs)。

## 检查并导入图像映射数据 {#reviewing-and-importing-image-map-data}

“映射摘要”屏幕提供了关于您的 eCatalog 的元数据。也可以从“映射摘要”屏幕开始为 eCatalog 批量导入图像映射数据。用这种方法导入图像映射数据可以简化图像映射 URL 及变换文本的输入。

要查看“映射摘要”屏幕，请在 eCatalog 屏幕的“映射页面”选项卡中单击“摘要”。

### 检查图像映射数据摘要 {#review-image-map-data-summary}

1. 在“映射页面”屏幕上，单击“摘要”。

   “映射摘要”屏幕显示 eCatalog 中图像映射、URL、变换文本说明以及其他操作的数量。

1. 如果有变换键错误，单击 Rollover_Key 错误列中的错误，以查看需要在电子表格中进行哪些改动来更正错误。可以选择并复制该消息的文本，并将其粘贴到电子表格中。
1. 在“eCatalog 查看器”中单击“预览”检查页面，单击 X 关闭“摘要”屏幕，并返回到“映射页面”屏幕，或单击“关闭”返回到“浏览”。

### 导入图像映射数据 {#import-image-map-data}

可以将整个 eCatalog 的数据导入到“映射摘要”屏幕中，而不必在每个页面都输入图像映射数据。可以通过制表符分隔的文件或 XML DTD 的形式导入图像映射数据。文件中的字段必须与“映射摘要”屏幕中显示的顺序相同：“名称”、“TOC 标签”、“映射”、“URL”、“变换文本”、“其他操作”和“搜索字符串”。导入图像映射数据可以免去创建每个图像映射时在“图像映射”列表中输入数据的麻烦。

>[!NOTE]
>
>在导入图像映射数据之前，必须已经创建图像映射。

在“映射摘要”屏幕上开始，按照以下步骤为创建的图像映射导入图像映射数据：

1. 单击“导入映射数据”。
1. 在“导入元数据”对话框中，单击“浏览”，然后选择制表符分隔文件或 XML DTD 文件。
1. 在“作业名称”字段中，键入文件的名称（注意保留其扩展名）。
1. 单击“上载”。

## 在 eCatalog 之间复制图像映射 {#copying-image-maps-between-ecatalogs}

可以将 eCatalog 中的所有图像映射复制到其他 eCatalog 中。这种复制图像映射的方法是在相同的 eCatalog 的外语翻译之间复制图像映射的方便方法。为使复制成功，Dynamic Media经典建议在电子目录之间复制相同数量的页面和同一图像。

>[!NOTE]
>
>如果图像映射所复制到的 eCatalog 已经包含图像映射，复制时将删除原有的图像映射。

按照以下步骤将一个 eCatalog 中的所有图像映射复制到其他 eCatalog 中：

1. 选择包含要复制的图像映射的 eCatalog，然后单击 eCatalog 的变换“编辑”按钮。
1. 在“排序页面”选项卡上，单击“复制映射”。
1. 在“选择资源”对话框中，选择要在其中复制图像映射的 eCatalog，然后单击“选择”。

如果目标eCatalog(您复制图象映射的电子目录)具有不同数量的页面或不同大小的图像，则动态媒体经典会显示一条警告消息。可以忽略该警告，单击“继续”来复制图像映射。