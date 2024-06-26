---
title: 创建eCatalog
description: 了解如何在Adobe Dynamic Media Classic中创建eCatalog。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: 51d411b2-b4bc-4cf6-afca-dd0ed0d219a1
topic: Integrations, Development
level: Experienced
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '984'
ht-degree: 30%

---

# 创建 eCatalog {#creating-an-ecatalog}

创建eCatalog需要对页面进行排序，选择页面布局，并通过绘制图像映射来链接页面。 它还需要输入变换图像和超文本链接数据。 也可以选择自定义目录，以使观众能够在 eCatalog 查看器中看到页面名称而不是页码。

## 创建eCatalog {#create}

您可以在eCatalog中包含图像文件和PDF文件。

创建eCatalog时， **[!UICONTROL 保存后发布]** 选项会以下列方式影响集和集成员：

| 保存前选择了“保存后发布”选项？ | 保存后的集状态 | 保存后的集成员状态 |
| --- | --- | --- |
| 是 | 已发布 | 已发布 |
| 否 | 未发布 | 集成员保持其已发布或未发布状态。 |

另请参阅[手动发布资源](publishing-files.md#manually_publishing_assets)和[手动取消发布资源](publishing-files.md#manually_unpublishing_assets)。

**要创建eCatalog，请执行以下操作：**

1. 采用以下方法之一开始创建 eCatalog：

   * **首先选择文件**：在“浏览”面板中，选择文件，然后转到 **[!UICONTROL 生成]** > **[!UICONTROL eCatalogs]**.

   * **从eCatalog屏幕开始**：转到 **[!UICONTROL 生成]** > **[!UICONTROL eCatalogs]**. 在资产库中选择一个文件夹。 将文件从文件夹拖到eCatalog页的“订单页”选项卡中。

     >[!NOTE]
     >
     >要按照名称而不是缩略图查看资源库中的物品，在“个人设置”的“默认资源库”视图中选择“名称”选项。

1. 为 eCatalog 选择整体布局。选择 **[!UICONTROL 单页]** 对于单页面， **[!UICONTROL 2页]** 对于双页跨页，或者 **[!UICONTROL 自定义]** 跨页超过两页的页面。 在 **[!UICONTROL 更改eCatalog布局]** 对话框中，选择 **[!UICONTROL 所有跨页]** 选项并选择 **[!UICONTROL 确定]**.
1. （可选）通过选择单个页面或跨页并选择它们来更改其布局 **[!UICONTROL 单页]**， **[!UICONTROL 2页]**，或 **[!UICONTROL 自定义]** 按钮。 在 **[!UICONTROL 更改eCatalog布局]** 对话框中，选择 **[!UICONTROL 选定的跨页]** 选项并选择 **[!UICONTROL 确定]**.
1. 根据需要采用以下方法之一重新排序页面：

   * **拖动**：将页面或跨页拖动到新位置。 垂直栏显示要移动的页面的位置。

   * **“移至”按钮**：选择页面或跨页，选择 **[!UICONTROL 移动到]**，然后在菜单中选择您希望页面在前面显示的页面。

   * **序列号**：在列表视图中，在序号字段中输入页码。

1. 完成后，在页面的右下角附近，请确保 **[!UICONTROL 保存后发布]** 处于选中状态（默认）。
1. 选择 **[!UICONTROL 保存]**.
1. 在“保存”对话框中，选择一个文件夹以存储您的 eCatalog。在“文件名”字段中，输入旋转集名称。
1. 选择 **[!UICONTROL 保存]**.

   保存eCatalog后，您可以通过选择 **[!UICONTROL 预览]**.

## 编辑eCatalog {#editing-an-ecatalog}

无论您编辑的是已发布的集还是未发布的集，您都可以 **[!UICONTROL 保存后发布]** 选项会以下列方式影响集和集成员：

| 是否已发布集？ | 在保存编辑之前，是否选择了“保存后发布”选项？ | 保存后的集状态 | 保存后的集成员状态 |
| --- | --- | --- | --- |
| 是 | 是 | 已发布 | 已发布 |
| 是 | 否 | 已发布 | 现有集成员将保留其已发布状态。 在编辑期间添加的任何新的集成员保持其已发布或未发布状态。 |
| 否 | 是 | 已发布 | 已发布 |
| 否 | 否 | 未发布 | 现有的集成员以及在编辑期间添加的任何新的集成员保持其已发布或未发布状态。 |

另请参阅[手动发布资源](publishing-files.md#manually_publishing_assets)和[手动取消发布资源](publishing-files.md#manually_unpublishing_assets)。

**要编辑eCatalog，请执行以下操作：**

1. 选择eCatalog的变换 **[!UICONTROL 编辑]** 按钮。
1. 根据需要，进行相应的更改。
1. 完成编辑后，在页面的右下角附近，请确保 **[!UICONTROL 保存后发布]** 处于选中状态（默认）。
1. 选择 **[!UICONTROL 保存]**，选择一个存储文件夹，输入集的名称，然后选择 **[!UICONTROL 保存]**.

## 删除eCatalog

在删除集时，集本身将移到垃圾桶中。但是，该集中的成员（或“子项”）不受影响；相反，它们各自保留其现有的已发布或未发布状态。

另请参阅[手动发布资源](publishing-files.md#manually_publishing_assets)和[手动取消发布资源](publishing-files.md#manually_unpublishing_assets)。

**要删除eCatalog，请执行以下操作：**

1. 在网格视图、列表视图或详细信息视图中，选择一个或多个 Catalog。
1. 在全局导航栏上，转到 **[!UICONTROL 文件]** > **[!UICONTROL 删除]** > **[!UICONTROL 删除]**.

## 自定义目录（目录） {#customizing-the-table-of-contents-toc}

Adobe Dynamic Media Classic在eCatalog屏幕的“订单页面”选项卡上，为您的eCatalog提供默认页码。 要自定义页面名称，可以更改构成目录 (TOC) 的页标签。推荐重命名封面和封底。例如，封面页可以阅读“封面”而不是“第0-1页”。

您可以手动为eCatalog创建自定义目录(TOC)。 或者，您也可以从CSV(仅限Mac)或XML文件导入页面名称。

>[!NOTE]
>
>要恢复默认页面标题，请在 **[!UICONTROL 排序页面]** 选项卡，选择 **[!UICONTROL TOC标签]**，然后选择 **[!UICONTROL 恢复默认值（全部）]**.

### 手动输入页面名称 {#manually-entering-page-names}

转到eCatalog屏幕的“排序页面”选项卡，逐个手动输入页面名称。 然后，在页码字段中，为每个要命名的页面输入一个名称。

### 导入页面名称 {#importing-page-names}

如果处理包含很多页面的 eCatalog，则推荐使用导入页面名称的方法。可以从制表符分隔的文件或 XML 文件导入名称。

目录标签存储在图像的用户数据字段中；请将此数据格式化为列表 `name=<value>` ` pairs separated by two question marks "??" `. 例如，为名为的目录字段设置一个标签 `tocEN`，将图像的用户数据设置为：

`tocEN=&lt;EN_page_label>`

要为命名的目录字段设置单独的标签 `tocEN` 和 `tocFR`：

`tocEN=&lt;EN_page_label>??tocFR=&lt;FR_page_label>`

要在以制表符分隔的文件中导入“用户数据”字段，请包括字段用户数据：

| IPSID | 用户数据 |
| --- | --- |
| `<image_IPS_ID>` | `tocEN=<EN_page_label>??tocFR=<FR_page_label>` |

要在XML文件中导入“用户数据”字段，请包含属性 `vc_userdata`：

```as3
<ips> 
<ghw_object vc_objectname="<image_IPS_ID>" … vc_userdata=" tocEN=<EN_page_label>??tocFR=<FR_page_label>" … /> 
</ips>
```

要从制表符分隔文件或XML文件导入页名，请选择 **[!UICONTROL TOC标签]** 按钮并选择 **[!UICONTROL 导入]**. 在上载元数据对话框中，选择 **[!UICONTROL 浏览]**，然后导入用于关联每个页面与页面名称的CSV文件(仅限Mac)或XML文件。
