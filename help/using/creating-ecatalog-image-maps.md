---
title: 创建eCatalog图像映射
description: 了解如何在Adobe Dynamic Media Classic中创建eCatalog图像映射。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: 5e7f39a5-36a6-40df-8752-064a582c9346
topic: Integrations, Development
level: Experienced
autotag-review: '2026-05-13T17:43:26.837Z'
TQID: 'https://experienceleague.adobe.com/E1qnvzD2WIqVHt0UAtIq7bZfYlPZbfG9Ye6F9ntX5Q4'
product_v2: id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2: id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
source-git-commit: 23257d3c04ec0d662f382ffb55fd6c26454d39a2
workflow-type: tm+mt
source-wordcount: 1496
ht-degree: 18%

---

# 创建eCatalog图像映射{#creating-ecatalog-image-maps}

“图像映射”是eCatalog页面上的一个区域，您可以通过鼠标在该区域上滚动，或选择它来触发各种操作。 例如，当您将指针移到“图像映射”上时，您会看到项目的变换文本描述。 选择图像映射时，将启动另一个操作。 例如，您可以打开一个网页，以便查看者了解有关某个项目的更多信息或购买该项目，或者您可以启动视频以查看正在使用的项目。

## 绘制eCatalog图像映射 {#drawing-ecatalog-image-maps}

对于 eCatalog，可以在 eCatalog 屏幕的“映射页面”选项卡上绘制图像映射。 该屏幕包括显示 eCatalog 页面的图像映射区域，右侧显示“图像映射”列表。 在创建图像映射时，其名称会输入到“图像映射”列表中。

1. 选择eCatalog的变换&#x200B;**[!UICONTROL 编辑]**&#x200B;按钮。
1. 选择&#x200B;**[!UICONTROL 映射页面]**。
1. 在“映射页面”屏幕的左侧，选择所需页面。
1. 在“图像映射”区域中，绘制一个矩形或多边形（多个边）图像映射：

   * **矩形映射**：选择“矩形图像映射”工具并在页面上拖动以创建矩形。

   * **多边形映射**：选择“多边形图像映射”工具，然后根据需要多次选择图像周边区域。 选择后，Adobe Dynamic Media Classic将绘制图像映射的边框。

     绘制图像映射后，Adobe Dynamic Media Classic会在“图像映射”列表中为其指定一个名称。 为了形成名称，Adobe Dynamic Media Classic会在您正在使用的eCatalog页面的名称后附加一个序列号。

1. （可选）在“图像映射”列表的[!UICONTROL 名称]列中，您可以为图像映射输入新名称。 输入的名称中不能包含空格。
1. 您可以让查看者在选择“图像映射”时打开一个新网页。 在“图像映射”列表面板的“URL”列中，输入网页的URL。

   要简化输入URL（HREF模板）的过程，请选择&#x200B;**[!UICONTROL 编辑]**&#x200B;并输入模板。

请参阅[使用模板输入JavaScript和URL](creating-image-maps.md#using_a_template_to_enter_javascript_and_urls)。

1. （可选）在“显示”下拉列表中，选择&#x200B;**[!UICONTROL 变换文本]**，然后输入您希望用户在图像映射上移动指针时在屏幕上看到的文本。
1. （可选）在“显示”下拉列表中，选择&#x200B;**[!UICONTROL 其他操作]**，然后输入当用户将其指针移动到图像映射上时触发模糊或聚焦操作的属性。

   请参阅[定义图像映射的其他操作](creating-image-maps.md#defining_other_actions_for_image_maps)。

1. 选择&#x200B;**[!UICONTROL 保存]**。
1. （可选）选择&#x200B;**[!UICONTROL 预览]**&#x200B;以使用默认的eCatalog查看器预设查看eCatalog。

要删除图像映射，请在“图像映射”列表中选择其名称，然后选择&#x200B;**[!UICONTROL 删除]**。 您可以暂时禁用页面上的图像映射，而无需删除图像映射。 在“图像映射”列表面板中选择图像映射选项。

## 在eCatalog中嵌入富媒体 {#embedding-rich-media-in-an-ecatalog}

您可以使用eCatalog的富媒体选项将MP4格式的视频或旋转集添加到已添加到eCatalog的图像映射中。 当用户在eCatalog中选择“图像映射”区域时，将显示关联的旋转集或视频。 如果您希望客户在使用过程中查看项目或从不同角度查看项目，则此功能特别有用。

客户将其指针移动到您的图像映射上时，您还可以选择显示工具提示文本，以便他们知道自己选择的是什么。

**要在eCatalog中嵌入富媒体，请执行以下操作：**

1. 绘制 eCatalog 图像映射。

   查看[绘制eCatalog图像映射](creating-ecatalog-image-maps.md#drawing_ecatalog_image_maps)。

1. 在显示下拉列表中，选择&#x200B;**[!UICONTROL 富媒体]**。
1. 在左侧的“添加Assets”面板中，导航到包含要嵌入的旋转集或视频（MP4格式）资源的文件夹。
1. 将资源拖动到图像映射上。
1. （可选）在“图像映射”列表面板的&#x200B;**[!UICONTROL 工具提示]**&#x200B;列标题下，输入您希望查看者在屏幕上将指针移动到图像映射上时看到的文本。
1. 选择&#x200B;**[!UICONTROL 保存]**。

## 编辑 eCatalog 图像映射 {#editing-ecatalog-image-maps}

从 eCatalog 屏幕的“映射页面”选项卡上开始，使用以下方法来编辑 eCatalog 图像映射：

* **调整位置**：选择“平移”工具，将指针移动到地图边框附近，而不将其放在地图上。 当指针显示方向箭头图标时，将整个“图像映射”拖动到新位置。

  查看[调整图像映射的位置、形状和大小](creating-image-maps.md#adjusting_the_position_shape_and_size_of_image_maps)。

* **更改形状和大小**：要调整矩形图像映射的大小，请选择“平移”工具。 然后将指针移动到边框或角上，看到双向箭头图标时进行拖动。 要调整多边形图像映射的大小，请拖动正方形选择手柄。 要创建选区手柄，请选择“图像映射”的边框并拖动。

  查看[调整图像映射的位置、形状和大小](creating-image-maps.md#adjusting_the_position_shape_and_size_of_image_maps)。

* **删除图像映射**：选择平移工具，选择图像映射以将其选中，然后选择&#x200B;**[!UICONTROL 删除]**。

  要从eCatalog中删除所有图像映射，请选择&#x200B;**[!UICONTROL 排序页面]**&#x200B;选项卡，然后选择&#x200B;**[!UICONTROL 清除映射]**。

* **处理重叠的图像映射**：拖动以更改图像映射在图像映射列表中的顺序。

  查看[处理重叠的图像映射](creating-image-maps.md#handling_overlapping_image_maps)。

* **将图像映射复制到其他页面**：选择&#x200B;**[!UICONTROL 将映射复制到]**（确保您位于“映射页面”选项卡）。 在选择图像屏幕上，选择要复制图像映射的一个或多个页面，然后选择&#x200B;**[!UICONTROL 选择]**。

  查看[将图像映射复制到其他图像](creating-image-maps.md#copying_image_maps)。

>[!NOTE]
>
>将图像映射复制到eCatalog中的不同页面时，还可以将所有图像映射从一个eCatalog复制到另一个。 查看[在eCatalogs](creating-ecatalog-image-maps.md#copying_image_maps_between_ecatalogs)之间复制图像映射。

## 查看和导入图像映射数据 {#reviewing-and-importing-image-map-data}

“映射摘要”屏幕提供了关于您的 eCatalog 的元数据。 也可以从“映射摘要”屏幕开始为 eCatalog 批量导入图像映射数据。 通过这种方式导入图像映射数据，可简化输入图像映射URL和变换文本的过程。

要查看“映射摘要”屏幕，请在eCatalog屏幕的“映射页面”选项卡上选择&#x200B;**[!UICONTROL 摘要]**。

### 检查图像映射数据摘要 {#review-image-map-data-summary}

1. 在“映射页面”屏幕上，选择&#x200B;**[!UICONTROL 摘要]**。

   “映射摘要”屏幕显示eCatalog中的图像映射、URL、变换文本描述和其他操作数。

1. 如果存在变换错误，请在&#x200B;**[!UICONTROL 变换键错误]**&#x200B;列中选择该错误，以查看电子表格中必须更新的内容，以便进行更正。 可以选择并复制该消息的文本，并将其粘贴到电子表格中。
1. 选择&#x200B;**[!UICONTROL 预览]**，以便在eCatalog查看器中检查页面。 选择X以关闭“摘要”屏幕并返回“映射页面”屏幕，或选择&#x200B;**[!UICONTROL 关闭]**&#x200B;以返回“浏览”。

### 导入图像映射数据 {#import-image-map-data}

您可以将整个eCatalog的数据导入“映射摘要”屏幕，而不是在每个页面上输入图像映射数据。 可以通过制表符分隔的文件或 XML DTD 的形式导入图像映射数据。 文件中的字段必须遵循“映射摘要”屏幕上显示的顺序：“名称”、“目录标签”、“映射”、“URL”、“变换文本”、“其他操作”和“搜索字符串”。 导入图像映射数据后，在创建每个图像映射时，无需在“图像映射”列表中输入数据。

>[!NOTE]
>
>在导入图像映射数据之前，必须已经创建图像映射。

在“映射摘要”屏幕上开始，按照以下步骤为创建的图像映射导入图像映射数据：

1. 选择&#x200B;**[!UICONTROL 导入映射数据]**。
1. 在“导入元数据”对话框中，选择&#x200B;**[!UICONTROL 浏览]**，然后选择制表符分隔的文件或XML DTD文件。
1. 在作业名称字段中，键入文件的名称（请确保保留其扩展名）。
1. 选择&#x200B;**[!UICONTROL 上传]**。

## 在eCatalog之间复制图像映射 {#copying-image-maps-between-ecatalogs}

可以将 eCatalog 中的所有图像映射复制到其他 eCatalog 中。 通过此方式复制图像映射是一种在同一eCatalog的本地化版本之间复制图像映射的方法。 为了成功复制，Adobe Dynamic Media Classic建议在具有相同页数和相同图像大小的eCatalog之间复制。

>[!NOTE]
>
>如果图像映射所复制到的 eCatalog 已经包含图像映射，复制时将删除原有的图像映射。

要将一个eCatalog中的所有图像映射复制到另一个eCatalog，请执行以下操作：

1. 选择要复制的图像映射的eCatalog，然后选择eCatalog的变换&#x200B;**[!UICONTROL 编辑]**&#x200B;按钮。
1. 在“排序页面”选项卡上，选择&#x200B;**[!UICONTROL 复制映射]**。
1. 在“选择资源”对话框中，选择要复制图像映射的eCatalog，然后选择&#x200B;**[!UICONTROL 选择]**。

如果您将图像映射复制到的目标eCatalog的页数或图像大小不同，则Adobe Dynamic Media Classic会显示警告消息。 选择&#x200B;**[!UICONTROL 继续]**&#x200B;以复制图像映射，而不考虑警告。
