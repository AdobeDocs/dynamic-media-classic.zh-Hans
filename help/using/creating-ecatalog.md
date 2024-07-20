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

创建eCatalog时，保存&#x200B;]**之后的**[!UICONTROL  Publish选项会以下列方式影响该集和设置成员：

| 保存前已选择“保存后的Publish”选项？ | 保存后的集状态 | 保存后的集成员状态 |
| --- | --- | --- |
| 是 | 已发布 | 已发布 |
| 否 | 未发布 | 集成员保持其已发布或未发布状态。 |

另请参阅[手动发布资源](publishing-files.md#manually_publishing_assets)和[手动取消发布资源](publishing-files.md#manually_unpublishing_assets)。

**创建eCatalog：**

1. 采用以下方法之一开始创建 eCatalog：

   * **首先选择文件**：在“浏览”面板中，选择文件，然后转到&#x200B;**[!UICONTROL 生成]** > **[!UICONTROL 电子目录]**。

   * **从eCatalog屏幕开始**：转到&#x200B;**[!UICONTROL 生成]** > **[!UICONTROL eCatalogs]**。 在资产库中选择一个文件夹。 将文件从文件夹拖到eCatalog页的“订单页”选项卡中。

     >[!NOTE]
     >
     >要按照名称而不是缩略图查看资源库中的物品，在“个人设置”的“默认资源库”视图中选择“名称”选项。

1. 为 eCatalog 选择整体布局。为单页选择&#x200B;**[!UICONTROL 1 Up]**，为双页跨页选择&#x200B;**[!UICONTROL 2 Up]**，或为超过两页的页面跨页选择&#x200B;**[!UICONTROL 自定义]**。 在&#x200B;**[!UICONTROL 更改eCatalog布局]**&#x200B;对话框中，选择&#x200B;**[!UICONTROL 所有跨页]**&#x200B;选项，然后选择&#x200B;**[!UICONTROL 确定]**。
1. （可选）更改单个页面或跨页布局，方法是选择这些页面或跨页，然后选择&#x200B;**[!UICONTROL 1 Up]**、**[!UICONTROL 2 Up]**&#x200B;或&#x200B;**[!UICONTROL 自定义]**&#x200B;按钮。 在&#x200B;**[!UICONTROL 更改eCatalog布局]**&#x200B;对话框中，选择&#x200B;**[!UICONTROL 选定跨页]**&#x200B;选项，然后选择&#x200B;**[!UICONTROL 确定]**。
1. 根据需要采用以下方法之一重新排序页面：

   * **正在拖动**：将页面或跨页拖到新位置。 垂直栏显示要移动的页面的位置。

   * **移动至按钮**：选择页面或跨页，选择&#x200B;**[!UICONTROL 移动至]**，然后在您希望页面显示之前的菜单中选择该页面。

   * **序列号**：在列表视图中，在序列号#字段中输入页码。

1. 完成后，在页面的右下角附近，确保选中了&#x200B;**[!UICONTROL 保存Publish]**（默认）。
1. 选择&#x200B;**[!UICONTROL 保存]**。
1. 在“保存”对话框中，选择一个文件夹以存储您的 eCatalog。在“文件名”字段中，输入旋转集名称。
1. 选择&#x200B;**[!UICONTROL 保存]**。

   在保存eCatalog后，您可以通过选择&#x200B;**[!UICONTROL 预览]**&#x200B;来预览它。

## 编辑eCatalog {#editing-an-ecatalog}

无论您是编辑已发布的集还是未发布的集，**[!UICONTROL 保存]**&#x200B;后的Publish选项都将通过以下方式影响该集和集成员：

| 是否已发布集？ | 在保存编辑之前，是否已选择“保存后的Publish”选项？ | 保存后的集状态 | 保存后的集成员状态 |
| --- | --- | --- | --- |
| 是 | 是 | 已发布 | 已发布 |
| 是 | 否 | 已发布 | 现有集成员将保留其已发布状态。 在编辑期间添加的任何新的集成员保持其已发布或未发布状态。 |
| 否 | 是 | 已发布 | 已发布 |
| 否 | 否 | 未发布 | 现有的集成员以及在编辑期间添加的任何新的集成员保持其已发布或未发布状态。 |

另请参阅[手动发布资源](publishing-files.md#manually_publishing_assets)和[手动取消发布资源](publishing-files.md#manually_unpublishing_assets)。

**要编辑eCatalog：**

1. 选择eCatalog的变换&#x200B;**[!UICONTROL 编辑]**&#x200B;按钮。
1. 根据需要，进行相应的更改。
1. 完成编辑后，在页面的右下角附近，请确保选中了&#x200B;**[!UICONTROL 保存]**&#x200B;后的Publish（默认）。
1. 选择&#x200B;**[!UICONTROL 保存]**，选择一个存储文件夹，输入该集的名称，然后选择&#x200B;**[!UICONTROL 保存]**。

## 删除eCatalog

在删除集时，集本身将移到垃圾桶中。但是，该集中的成员（或“子项”）不受影响；相反，它们各自保留其现有的已发布或未发布状态。

另请参阅[手动发布资源](publishing-files.md#manually_publishing_assets)和[手动取消发布资源](publishing-files.md#manually_unpublishing_assets)。

**删除eCatalog：**

1. 在网格视图、列表视图或详细信息视图中，选择一个或多个 Catalog。
1. 在全局导航栏上，转到&#x200B;**[!UICONTROL 文件]** > **[!UICONTROL 删除]** > **[!UICONTROL 删除]**。

## 自定义目录（目录） {#customizing-the-table-of-contents-toc}

Adobe Dynamic Media Classic在eCatalog屏幕的“订单页面”选项卡上，为您的eCatalog提供默认页码。 要自定义页面名称，可以更改构成目录 (TOC) 的页标签。推荐重命名封面和封底。例如，封面页可以阅读“封面”而不是“第0-1页”。

您可以手动为eCatalog创建自定义目录(TOC)。 或者，您也可以从CSV(仅限Mac)或XML文件导入页面名称。

>[!NOTE]
>
>要恢复默认页面标题，请在&#x200B;**[!UICONTROL 订购页面]**&#x200B;选项卡上选择&#x200B;**[!UICONTROL 目录标签]**，然后选择&#x200B;**[!UICONTROL 恢复默认页面（全部）]**。

### 手动输入页面名称 {#manually-entering-page-names}

转到eCatalog屏幕的“排序页面”选项卡，逐个手动输入页面名称。 然后，在页码字段中，为每个要命名的页面输入一个名称。

### 导入页面名称 {#importing-page-names}

如果处理包含很多页面的 eCatalog，则推荐使用导入页面名称的方法。可以从制表符分隔的文件或 XML 文件导入名称。

目录标签存储在图像的用户数据字段中；将此数据格式化为`name=<value>` ` pairs separated by two question marks "??" `的列表。 例如，要为名为`tocEN`的目录字段设置一个标签，请将图像的用户数据设置为：

`tocEN=&lt;EN_page_label>`

要为名为`tocEN`和`tocFR`的目录字段设置单独的标签：

`tocEN=&lt;EN_page_label>??tocFR=&lt;FR_page_label>`

要在以制表符分隔的文件中导入“用户数据”字段，请包括字段用户数据：

| IPSID | 用户数据 |
| --- | --- |
| `<image_IPS_ID>` | `tocEN=<EN_page_label>??tocFR=<FR_page_label>` |

要在XML文件中导入“用户数据”字段，请包含属性`vc_userdata`：

```as3
<ips> 
<ghw_object vc_objectname="<image_IPS_ID>" … vc_userdata=" tocEN=<EN_page_label>??tocFR=<FR_page_label>" … /> 
</ips>
```

若要从制表符分隔文件或XML文件导入页面名称，请选择&#x200B;**[!UICONTROL 目录标签]**&#x200B;按钮，然后选择&#x200B;**[!UICONTROL 导入]**。 在“上载元数据”对话框中，选择&#x200B;**[!UICONTROL 浏览]**，然后导入CSV文件(仅限Mac)或将每个页面与页面名称相关联的XML文件。
