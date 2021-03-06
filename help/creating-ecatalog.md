---
title: 创建eCatalog
description: 了解如何在AdobeDynamic Media Classic中创建eCatalog。
uuid: 2aff05c2-7052-426c-b61d-7f9091f7ace8
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
discoiquuid: 28889c60-596a-40d2-85d4-f48a4f86b932
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: 51d411b2-b4bc-4cf6-afca-dd0ed0d219a1
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '967'
ht-degree: 57%

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

   * **首先选择文件**  — 在浏览面板中，选择文件，然后转到 **[!UICONTROL Build]**  >  **[!UICONTROL eCatalogs]**。

   * **从eCatalog屏幕开始**  — 转到 **[!UICONTROL Build]**  >  **[!UICONTROL eCatalogs]**。在资源库中选择一个文件夹，将该文件夹中的文件拖到 eCatalog 页面的“排序页面”选项卡中。

      >[!NOTE]
      >
      >要按照名称而不是缩略图查看资源库中的物品，在“个人设置”的“默认资源库”视图中选择“名称”选项。

1. 为 eCatalog 选择整体布局。为单页选择&#x200B;**[!UICONTROL 1向上]**，为双页跨页选择&#x200B;**[!UICONTROL 2向上]**，或为超过两页跨页选择&#x200B;**[!UICONTROL 自定义]**。 在&#x200B;**[!UICONTROL 更改eCatalog布局]**&#x200B;对话框中，选择&#x200B;**[!UICONTROL 所有跨页]**&#x200B;选项，然后选择&#x200B;**[!UICONTROL 确定]**。
1. 或者，选择单个页面或页面跨页，然后选择&#x200B;**[!UICONTROL 1向上]**、**[!UICONTROL 2向上]**&#x200B;或&#x200B;**[!UICONTROL 自定义]**&#x200B;按钮，以更改其布局。 在&#x200B;**[!UICONTROL 更改eCatalog布局]**&#x200B;对话框中，选择&#x200B;**[!UICONTROL 选定的跨页]**&#x200B;选项，然后选择&#x200B;**[!UICONTROL 确定]**。
1. 根据需要采用以下方法之一重新排序页面：

   * **拖动**  — 将页面或页面跨页拖动到新位置。垂直栏显示要移动的页面的位置。

   * **“移动到”按钮**  — 选择一个页面或页面跨页，选择 **[!UICONTROL 移动到]**，然后在您希望页面显示之前的菜单中选择该页面。

   * **序列** 号 — 在列表视图中，在序列号字段中输入页码。

1. 完成后，确保在页面右下角附近选择了“**[!UICONTROL 保存后发布]**”（默认）。
1. 选择&#x200B;**[!UICONTROL Save]**。
1. 在“保存”对话框中，选择一个文件夹以存储您的 eCatalog。在“文件名”字段中，输入旋转集名称。
1. 选择&#x200B;**[!UICONTROL Save]**。

   在保存eCatalog后，可以通过选择&#x200B;**[!UICONTROL 预览]**&#x200B;来预览eCatalog。

## 编辑eCatalog {#editing-an-ecatalog}

无论您是编辑已发布的集还是未发布的集，**[!UICONTROL 保存后发布]**&#x200B;选项都会通过以下方式影响集和集成员：

| 是否已发布集？ | 是否在保存编辑内容之前选择了“保存后发布”选项？ | 保存后的集状态 | 保存后的集成员状态 |
| --- | --- | --- | --- |
| 是 | 是 | 已发布 | 已发布 |
| 是 | 否 | 已发布 | 现有的集成员保持其已发布状态。在编辑期间添加的任何新的集成员保持其已发布或未发布状态。 |
| 否 | 是 | 已发布 | 已发布 |
| 否 | 否 | 未发布 | 现有的集成员以及在编辑期间添加的任何新的集成员保持其已发布或未发布状态。 |

另请参阅[手动发布资源](publishing-files.md#manually_publishing_assets)和[手动取消发布资源](publishing-files.md#manually_unpublishing_assets)。

**编辑 eCatalog:**

1. 选择eCatalog的滚动&#x200B;**[!UICONTROL 编辑]**&#x200B;按钮。
1. 根据需要，进行相应的更改。
1. 在完成编辑后，确保在页面右下角附近选择了“**[!UICONTROL 保存后发布]**”（默认）。
1. 选择&#x200B;**[!UICONTROL Save]**，选择存储文件夹，输入集的名称，然后选择&#x200B;**[!UICONTROL Save]**。

## 删除eCatalog {#deleting-an-ecatalog}

在删除集时，集本身将移到垃圾桶中。不过，集中的成员（或“子项”）不受影响；它们分别保持现有的已发布或未发布状态。

另请参阅[手动发布资源](publishing-files.md#manually_publishing_assets)和[手动取消发布资源](publishing-files.md#manually_unpublishing_assets)。

**删除 eCatalog:**

1. 在网格视图、列表视图或详细信息视图中，选择一个或多个 Catalog。
1. 在全局导航栏上，转到&#x200B;**[!UICONTROL 文件]** > **[!UICONTROL 删除]** > **[!UICONTROL 删除]**。

## 自定义目录（目录） {#customizing-the-table-of-contents-toc}

AdobeDynamic Media Classic在eCatalog屏幕的“订单页面”选项卡上提供eCatalog中的默认页码。 要自定义页面名称，可以更改构成目录 (TOC) 的页标签。推荐重命名封面和封底。例如，封面可以是“封面”，而不是“第0-1页”。

可以采用手动方式或通过从 CSV（仅 Mac）或 XML 文件导入页面名称来为 eCatalog 创建自定义目录 (TOC)。

>[!NOTE]
>
>要恢复默认页面标题，请在&#x200B;**[!UICONTROL 排序页面]**&#x200B;选项卡中，选择&#x200B;**[!UICONTROL 目录标签]**，然后选择&#x200B;**[!UICONTROL 还原默认值（全部）]**。

### 手动输入页面名称 {#manually-entering-page-names}

要逐个手动输入页面名称，转至 eCatalog 屏幕的“排序页面”选项卡。然后，在页码字段中，输入要命名的每个页面的名称。

### 导入页面名称 {#importing-page-names}

如果处理包含很多页面的 eCatalog，则推荐使用导入页面名称的方法。可以从制表符分隔的文件或 XML 文件导入名称。

TOC标签存储在图像的“用户数据”字段中；将此数据格式化为`name=<value>` ` pairs separated by two question marks “??” `的列表。 例如，要为名为 `tocEN` 的 TOC 字段设置一个标签，可以将图像的“用户数据”设置为：

`tocEN=&lt;EN_page_label>`

要为名为`tocEN`和`tocFR`的目录字段设置单独的标签，请执行以下操作：

`tocEN=&lt;EN_page_label>??tocFR=&lt;FR_page_label>`

要在以制表符分隔的文件中导入“用户数据”字段，请包括该字段的用户数据：

| IPSID | 用户数据 |
| --- | --- |
| `<image_IPS_ID>` | `tocEN=<EN_page_label>??tocFR=<FR_page_label>` |

要用 XML 文件导入“用户数据”字段，应包含 `vc_userdata` 属性：

```as3
<ips> 
<ghw_object vc_objectname="<image_IPS_ID>" … vc_userdata=" tocEN=<EN_page_label>??tocFR=<FR_page_label>" … /> 
</ips>
```

要从制表符分隔或XML文件导入页面名称，请选择&#x200B;**[!UICONTROL 目录标签]**&#x200B;按钮，然后选择&#x200B;**[!UICONTROL 导入]**。 在“上传元数据”对话框中，选择&#x200B;**[!UICONTROL 浏览]**，然后导入CSV文件（仅限Mac）或将每个页面与页面名称关联的XML文件。
