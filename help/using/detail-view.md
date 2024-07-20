---
title: 在“详细信息”视图中工作
description: 了解如何在Adobe Dynamic Media Classic的“详细信息”视图中工作。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 618ae6a4-6f60-4a80-b197-a9d35b3c47af
topic: Content Management
level: Intermediate
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '621'
ht-degree: 20%

---

# 在“详细信息”视图中工作{#working-in-detail-view}

您可以通过在“详细信息”视图中打开资产来使用和了解资产。 在“详细信息”视图中，您可以看到资产大小、属性、派生项和元数据。 您还可以查看资产是否发布以及何时发布，并可获取已发布资产的URL。 根据资源类型，您可以按不同大小预览资源，将其放大，并执行锐化、裁切以及其他格式设置操作。

<!-- 

Comment Type: remark
Last Modified By: Rick Brough (rbrough@adobe.com)
Last Modified Date: 2018-06-14T13:52:46.623-0400

<p>as_detail_view_popup.png found in Downloads on local in folder "scene7-images"</p>

 -->

![详细信息视图](/help/using/assets/image_0.img.png)
*详细信息视图（左侧隐藏资产库面板）。*

>[!NOTE]
>
>要打开存储资产的文件夹，可以选择信息面板顶部的文件夹路径。

## 在“详细信息”视图中打开资产 {#open-an-asset-in-detail-view}

您可以在“详细信息”视图中显示资源，以便仔细检查、预览或处理该资源。

1. 在“浏览”面板中，执行以下任一操作：

   * 选择资源。 在Adobe Dynamic Media Classic的右上角附近，选择&#x200B;**[!UICONTROL 详细信息视图]**&#x200B;图标。
   * 双击资源。
   * 选择资源，然后转到&#x200B;**[!UICONTROL 文件]** > **[!UICONTROL 详细信息]**。

>[!NOTE]
>
>在“详细信息”视图中，您可以在同一文件夹中从一个资产页面转到另一个资产。 只需单击&#x200B;**[!UICONTROL 上一个资源]**&#x200B;或&#x200B;**[!UICONTROL 下一个资源]**。 这些按钮位于“详细视图”的右上角。

## 在“详细信息”视图中获取信息 {#getting-information-in-detail-view}

“详细信息视图”提供有关资产或文件的信息。 显示有关项目的以下信息：存储项目的文件夹、其文件名、将项目上传到Adobe Dynamic Media Classic的日期及其发布历史记录。 您还可以查看和编辑元数据，并在详细信息视图中为资源添加关键字。

您可以在详细信息视图中获取资产URL；但是，在发布资产之前，该URL处于不活动状态。 对于图像，“详细信息视图”还提供构建和派生资源及元数据的列表，例如缩放目标和图像集。

## 在“详细信息”视图中使用资产 {#working-with-assets-in-detail-view}

“详细信息视图”提供了用于处理所打开资产的工具。 可用的工具取决于您使用的资源类型，但“详细信息视图”始终提供以下功能：

* 发布&#x200B;**的**&#x200B;项目：选择名称左侧的&#x200B;**[!UICONTROL `Publish`]**&#x200B;图标，或转到&#x200B;**[!UICONTROL 文件]** > **[!UICONTROL Publish]**&#x200B;或&#x200B;**[!UICONTROL 文件]** > **[!UICONTROL 取消发布]**。

* **重命名资源**：选择名称并输入新名称。

* **编辑并添加元数据**：选择“元数据”面板，然后根据需要进行更改。 请参阅[查看、添加和导出元数据](/help/using/viewing-adding-exporting-metadata.md)。

* **编辑并添加关键字**：选择关键字，并根据需要添加或删除关键字。 请参阅[添加或编辑关键字](/help/using/viewing-adding-exporting-metadata.md)。

* **删除资源**：转到&#x200B;**[!UICONTROL 文件]** > **[!UICONTROL 删除]**。

对于离散文件（例如图像、图像集和字体），您可以在“详细视图”中查看发布和编辑历史记录，并检查作业详细信息。

此表显示了“详细信息视图”中不同类型的资源可用的其他选项。

| 资源类型 | 编辑/调整 | 预览 |
| --- | --- | --- |
| 图像 | 添加图像映射<br>添加缩放目标<br>裁切<br>锐化<br>创建调整后的视图 | 是；缩放和图像预设 |
| CAB 和窗饰图像 | 否 | 缩略图 |
| eCatalog | 编辑 | 是<br>信息面板也可用 |
| 字体 | 编辑字体信息 | 否 |
| FXG 文件 | 编辑 | 是 |
| ICC 配置文件 | 编辑配置文件信息 | 否 |
| Illustrator 文件 | 否（除非转换为 FXG） | 否 |
| 图像集 | 编辑 | 是 |
| InDesign 文件 | 否（除非转换为 FXG） | 否 |
| PDF 文件 | 否 | 否 |
| PSD 文件 | 对于个别图层可用 | 对于个别图层可用 |
| 旋转集 | 编辑 | 是 |
| SVG 文件 | 否 | 否 |
| 模板 | 编辑 | 是 |
| 视频 | 否 | 是 |
| 晕影和渲染的晕影 | 否 | 显示图像<br>您可以以XML格式查看晕影的可渲染元素的内容和结构 |
| XML 文件 | 否 | 显示内容 |
| ZIP 文件 | 否 | 内容未显示 |

>[!MORELIKETHIS]
>
>* [查看、添加和导出元数据](viewing-adding-exporting-metadata.md#viewing_adding_and_exporting_metadata)
