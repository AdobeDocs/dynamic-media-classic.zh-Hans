---
title: 创建eCatalog
description: 了解如何在Adobe Dynamic Media Classic中创建eCatalog。
uuid: 2aff05c2-7052-426c-b61d-7f9091f7ace8
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
discoiquuid: 28889c60-596a-40d2-85d4-f48a4f86b932
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: 51d411b2-b4bc-4cf6-afca-dd0ed0d219a1
topic: Integrations, Development
level: Experienced
source-git-commit: 5d8b7cb8b4616a998346675d7324b568634698fb
workflow-type: tm+mt
source-wordcount: '967'
ht-degree: 56%

---

# 创建 eCatalog {#creating-an-ecatalog}

创建 eCatalog 需要对页面排序、选择页面布局、通过绘制图像映射链接页面以及输入变换和超文本数据。也可以选择自定义目录，以使观众能够在 eCatalog 查看器中看到页面名称而不是页码。

## 创建eCatalog {#create}

您可以在eCatalog中包含图像文件和PDF文件。

在创建 eCatalog 时，“**[!UICONTROL 保存后发布]**”选项按以下方式影响集和集成员：

| 是否在保存之前选择了“保存后发布”选项？ | 保存后的集状态 | 保存后的集成员状态 |
| --- | --- | --- |
| 是 | 已发布 | 已发布 |
| 否 | 未发布 | 集成员保持其已发布或未发布状态。 |

另请参阅[手动发布资源](publishing-files.md#manually_publishing_assets)和[手动取消发布资源](publishing-files.md#manually_unpublishing_assets)。

**创建 eCatalog:**

1. 采用以下方法之一开始创建 eCatalog：

   * **首先选择文件**  — 在“浏览”面板中，选择文件，然后转到 **[!UICONTROL 生成]** > **[!UICONTROL eCatalogs]**.

   * **从eCatalog屏幕开始**  — 转到 **[!UICONTROL 生成]** > **[!UICONTROL eCatalogs]**. 在资源库中选择一个文件夹，将该文件夹中的文件拖到 eCatalog 页面的“排序页面”选项卡中。

     >[!NOTE]
     >
     >要按照名称而不是缩略图查看资源库中的物品，在“个人设置”的“默认资源库”视图中选择“名称”选项。

1. 为 eCatalog 选择整体布局。选择 **[!UICONTROL 1栏式]** 对于单页， **[!UICONTROL 2页]** 对于双页跨页，或者 **[!UICONTROL 自定义]** 对于超过两页的页面跨页。 在 **[!UICONTROL 更改eCatalog布局]** 对话框中，选择 **[!UICONTROL 所有跨页]** 选项并选择 **[!UICONTROL 确定]**.
1. （可选）通过选择单个页面或页面跨页，然后选择 **[!UICONTROL 1栏式]**， **[!UICONTROL 2页]**，或 **[!UICONTROL 自定义]** 按钮。 在 **[!UICONTROL 更改eCatalog布局]** 对话框中，选择 **[!UICONTROL 选定的跨页]** 选项并选择 **[!UICONTROL 确定]**.
1. 根据需要采用以下方法之一重新排序页面：

   * **拖动**  — 将页面或跨页拖动到新位置。 垂直栏显示要移动的页面的位置。

   * **“移至”按钮**  — 选择页面或跨页，选择 **[!UICONTROL 移至]**，然后在菜单中选择您希望页面在前面显示的页面。

   * **序列号**  — 在列表视图中，在“序号”字段中输入页码。

1. 完成后，确保在页面右下角附近选择了“**[!UICONTROL 保存后发布]**”（默认）。
1. 选择 **[!UICONTROL 保存]**.
1. 在“保存”对话框中，选择一个文件夹以存储您的 eCatalog。在“文件名”字段中，输入旋转集名称。
1. 选择 **[!UICONTROL 保存]**.

   保存eCatalog后，您可以通过选择 **[!UICONTROL 预览]**.

## 编辑eCatalog {#editing-an-ecatalog}

无论您是编辑已发布集还是未发布集， **[!UICONTROL 保存后发布]** 选项会以下列方式影响集和集成员：

| 是否已发布集？ | 是否在保存编辑内容之前选择了“保存后发布”选项？ | 保存后的集状态 | 保存后的集成员状态 |
| --- | --- | --- | --- |
| 是 | 是 | 已发布 | 已发布 |
| 是 | 否 | 已发布 | 现有的集成员保持其已发布状态。在编辑期间添加的任何新的集成员保持其已发布或未发布状态。 |
| 否 | 是 | 已发布 | 已发布 |
| 否 | 否 | 未发布 | 现有的集成员以及在编辑期间添加的任何新的集成员保持其已发布或未发布状态。 |

另请参阅[手动发布资源](publishing-files.md#manually_publishing_assets)和[手动取消发布资源](publishing-files.md#manually_unpublishing_assets)。

**编辑 eCatalog:**

1. 选择eCatalog的变换 **[!UICONTROL 编辑]** 按钮。
1. 根据需要，进行相应的更改。
1. 在完成编辑后，确保在页面右下角附近选择了“**[!UICONTROL 保存后发布]**”（默认）。
1. 选择 **[!UICONTROL 保存]**，选择一个存储文件夹，输入该集的名称，然后选择 **[!UICONTROL 保存]**.

## 删除eCatalog {#deleting-an-ecatalog}

在删除集时，集本身将移到垃圾桶中。不过，集中的成员（或“子项”）不受影响；它们分别保持现有的已发布或未发布状态。

另请参阅[手动发布资源](publishing-files.md#manually_publishing_assets)和[手动取消发布资源](publishing-files.md#manually_unpublishing_assets)。

**删除 eCatalog:**

1. 在网格视图、列表视图或详细信息视图中，选择一个或多个 Catalog。
1. 在全局导航栏上，转到 **[!UICONTROL 文件]** > **[!UICONTROL 删除]** > **[!UICONTROL 删除]**.

## 自定义目录（目录） {#customizing-the-table-of-contents-toc}

Adobe Dynamic Media Classic在eCatalog屏幕的“订购页面”选项卡上提供eCatalog中的默认页码。 要自定义页面名称，可以更改构成目录 (TOC) 的页标签。推荐重命名封面和封底。例如，前封面可以阅读“封面”而不是“第0-1页”。

可以采用手动方式或通过从 CSV（仅 Mac）或 XML 文件导入页面名称来为 eCatalog 创建自定义目录 (TOC)。

>[!NOTE]
>
>要恢复默认页面标题，请在 **[!UICONTROL 排序页面]** 选项卡，选择 **[!UICONTROL TOC标签]**，然后选择 **[!UICONTROL 恢复默认值（全部）]**.

### 手动输入页面名称 {#manually-entering-page-names}

要逐个手动输入页面名称，转至 eCatalog 屏幕的“排序页面”选项卡。然后，在页码字段中，为要命名的每个页面输入一个名称。

### 导入页面名称 {#importing-page-names}

如果处理包含很多页面的 eCatalog，则推荐使用导入页面名称的方法。可以从制表符分隔的文件或 XML 文件导入名称。

目录标签存储在图像的用户数据字段中；请将此数据格式化为列表 `name=<value>` ` pairs separated by two question marks “??” `. 例如，要为名为 `tocEN` 的 TOC 字段设置一个标签，可以将图像的“用户数据”设置为：

`tocEN=&lt;EN_page_label>`

要为命名的目录字段设置单独的标签 `tocEN` 和 `tocFR`：

`tocEN=&lt;EN_page_label>??tocFR=&lt;FR_page_label>`

要将“用户数据”字段导入以制表符分隔的文件中，请包括字段用户数据：

| IPSID | 用户数据 |
| --- | --- |
| `<image_IPS_ID>` | `tocEN=<EN_page_label>??tocFR=<FR_page_label>` |

要用 XML 文件导入“用户数据”字段，应包含 `vc_userdata` 属性：

```as3
<ips> 
<ghw_object vc_objectname="<image_IPS_ID>" … vc_userdata=" tocEN=<EN_page_label>??tocFR=<FR_page_label>" … /> 
</ips>
```

要从制表符分隔文件或XML文件导入页面名称，请选择 **[!UICONTROL TOC标签]** 按钮并选择 **[!UICONTROL 导入]**. 在上载元数据对话框中，选择 **[!UICONTROL 浏览]**，然后导入CSV文件(仅限Mac)或将每个页面与某个页面名称关联的XML文件。
