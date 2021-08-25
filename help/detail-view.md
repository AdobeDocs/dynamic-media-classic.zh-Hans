---
title: 在“详细信息”视图中工作
description: 了解如何在Dynamic Media Classic中以详细视图工作。
uuid: cb62f765-9b7f-4a53-8206-99afae2fb80d
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: eaa214ff-d1ef-4691-9148-d01bf243c810
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 618ae6a4-6f60-4a80-b197-a9d35b3c47af
source-git-commit: 47845c30311fb9afb3fffb8502b6e7c534e4bfdb
workflow-type: tm+mt
source-wordcount: '612'
ht-degree: 24%

---

# 在“详细信息”视图中工作{#working-in-detail-view}

您可以通过在详细信息视图中打开资产来处理和了解资产。 在详细信息视图中，您可以看到资产大小、属性、派生项和元数据。 也可以看到资源是否已发布以及是何时发布的，并获得已发布资源的 URL。根据资源类型，您可以按不同大小预览资源，将其放大，并执行锐化、裁切以及其他格式设置操作。

<!-- 

Comment Type: remark
Last Modified By: Rick Brough (rbrough@adobe.com)
Last Modified Date: 2018-06-14T13:52:46.623-0400

<p>as_detail_view_popup.png found in Downloads on local in folder "scene7-images"</p>

 -->

![“资](/help/assets/image_0.img.png)
*产库”面板在左侧的视图中隐藏了“详细信息视图” “详细信息视图”。*

>[!NOTE]
>
>要打开存储资产的文件夹，您可以在“信息”面板顶部选择文件夹路径。

## 在“详细信息”视图中打开资产 {#open-an-asset-in-detail-view}

要仔细检查、预览或处理资产，您可以在详细信息视图中显示资产。

1. 在“浏览”面板中，执行以下任一操作：

   * 选择该资源。在Dynamic Media Classic的右上角附近，选择&#x200B;**[!UICONTROL 详细信息视图]**&#x200B;图标。
   * 双击资源。
   * 选择资产，然后转到&#x200B;**[!UICONTROL 文件]** > **[!UICONTROL 详细信息]**。

>[!NOTE]
>
>在详细信息视图中，您可以通过选择&#x200B;**[!UICONTROL 上一个资产]**&#x200B;或&#x200B;**[!UICONTROL 下一个资产]**，在同一文件夹中从资产页面到资产。 这些按钮位于“详细信息视图”的右上角。

## 在“详细信息”视图中获取信息 {#getting-information-in-detail-view}

详细信息视图提供有关资产或文件的信息。 它显示了有关某个项目的以下信息：存储该内容的文件夹、文件名、项目上传到Dynamic Media Classic的日期及其发布历史记录。 您还可以在详细信息视图中查看和编辑元数据，以及添加资产的关键词。

您可以在详细信息视图中获取资产URL;但是，在发布资产之前，该URL不会处于活动状态。 对于图像，“详细信息视图”还提供了内部版本和派生资产及元数据的列表，例如缩放目标和图像集。

## 在“详细信息”视图中处理资产 {#working-with-assets-in-detail-view}

详细信息视图提供了用于处理您打开的资产的工具。 具体有哪些工具可用取决于您所处理的资产类型，但“详细信息视图”始终提供以下功能：

* **要发布的项目**  — 选择名 **** 称左侧的发布项，或转到 **[!UICONTROL 文件]**  >  **** 发布 **[!UICONTROL 器文件]**  >  **[!UICONTROL 取消发布]**。

* **重命名资产**  — 选择名称并输入新名称。

* **编辑和添加元数据**  — 选择元数据面板，然后根据需要进行更改。请参阅[查看、添加和导出元数据](/help/viewing-adding-exporting-metadata.md)。

* **编辑和添加关键词**  — 选择关键词并根据需要添加或删除关键词。请参阅[添加或编辑关键字](/help/viewing-adding-exporting-metadata.md)。

* **删除资产**  — 转到 **[!UICONTROL 文件]**  >  **[!UICONTROL 删除]**。

对于离散文件（例如图像、图像集和字体），您可以在“详细信息视图”中查看发布和编辑历史记录，并检查作业详细信息。

此表显示了“详细信息视图”中不同类型的资产有哪些其他选项可用。

| 资源类型 | 编辑/调整 | 预览 |
| --- | --- | --- |
| 图像 | 添加图像映射<br>添加缩放目<br><br><br>标裁剪锐化创建调整后的视图 | 是；缩放和图像预设 |
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
| 晕影和渲染的晕影 | 否 | 显示的图像<br>您可以查看XML格式晕影的可渲染元素的内容和结构 |
| XML 文件 | 否 | 显示内容 |
| ZIP 文件 | 否 | 未显示内容 |

>[!MORELIKETHIS]
>
>* [查看、添加和导出元数据](viewing-adding-exporting-metadata.md#viewing_adding_and_exporting_metadata)

