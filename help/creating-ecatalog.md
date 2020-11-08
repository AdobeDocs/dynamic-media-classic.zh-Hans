---
title: 创建 eCatalog
seo-title: 创建 eCatalog
description: 'null'
seo-description: 了解如何创建电子目录。
uuid: 2aff05c2-7052-426c-b61d-7f9091f7ace8
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
discoiquuid: 28889c60-596a-40d2-85d4-f48a4f86b932
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '1005'
ht-degree: 78%

---


# 创建 eCatalog{#creating-an-ecatalog}

创建 eCatalog 需要对页面排序、选择页面布局、通过绘制图像映射链接页面以及输入变换和超文本数据。也可以选择自定义目录，以使观众能够在 eCatalog 查看器中看到页面名称而不是页码。

## 创建 eCatalog {#create}

可以在 eCatalog 中包含图像文件以及 PDF 文件。

在创建 eCatalog 时，“**保存后发布**”选项按以下方式影响集和集成员：

| 是否在保存之前选择了“保存后发布”选项？ | 保存后的集状态 | 保存后的集成员状态 |
|--- |--- |--- |
| 是 | 已发布 | 已发布 |
| 否 | 未发布 | 集成员保持其已发布或未发布状态。 |

另请参阅[手动发布资源](publishing-files.md#manually_publishing_assets)和[手动取消发布资源](publishing-files.md#manually_unpublishing_assets)。

**创建 eCatalog**

1. 采用以下方法之一开始创建 eCatalog：

   **首先选择文件** 。在浏览面板中，选择文件，然后单击“构建”>“电子目录”。

   **开始从电子目录屏幕** ，单击“构建”>“电子目录”。 在资源库中选择一个文件夹，将该文件夹中的文件拖到 eCatalog 页面的“排序页面”选项卡中。

   ***note**: To view the items in the Asset Library by name instead of thumbnail, select the Name option for Default Asset Library View in Personal Setup. *

1. 为 eCatalog 选择整体布局。如果是单页，单击“单页”按钮 ，如果是双页跨页，单击“双页”按钮 ，如果是多页跨页，则单击“自定义”按钮 。“更改 eCatalog 布局”对话框随即显示。Select the All Spreads options and click **OK**.
1. 也可以单击各个页面或页面跨页，然后选择“单页”按钮、“双页”按钮或“自定义”按钮，来更改其布局（可选）。“更改 eCatalog 布局”对话框随即显示。Select the Selected Spreads options and click **OK**.
1. 根据需要采用以下方法之一重新排序页面：

   **拖动** 将页面或跨页拖动到新位置。 垂直栏显示要移动的页面的位置。

   **“移到”按钮** 选择一个页面或页面跨页，单击“移到”按钮，然后在菜单上选择您希望之前显示页面的页面。

   **序列** #在列表视图中，在序列#字段中输入页码。

1. 完成后，确保在页面右下角附近选择了“**保存后发布**”（默认）。
1. 单击“**保存**”。
1. 在“保存”对话框中，选择一个文件夹以存储您的 eCatalog。在“文件名”字段中，输入旋转集名称。
1. 单击“**保存**”。

   在保存 eCatalog 后，可以单击“**预览**”以进行预览。

## 编辑 eCatalog {#editing-an-ecatalog}

根据是编辑已发布的集还是未发布的集，“**保存后发布**”选项按以下方式影响集和集成员：

| 是否已发布集？ | 是否在保存编辑内容之前选择了“保存后发布”选项？ | 保存后的集状态 | 保存后的集成员状态 |
|--- |--- |--- |--- |
| 是 | 是 | 已发布 | 已发布 |
| 是 | 否 | 已发布 | 现有集成员将保留其已发布状态。您在编辑过程中添加的任何新集成员将保留其已发布或未发布状态。 |
| 否 | 是 | 已发布 | 已发布 |
| 否 | 否 | 未发布 | 现有的集成员以及在编辑期间添加的任何新的集成员保持其已发布或未发布状态。 |

另请参阅[手动发布资源](publishing-files.md#manually_publishing_assets)和[手动取消发布资源](publishing-files.md#manually_unpublishing_assets)。

**编辑 eCatalog**

1. 单击 eCatalog 的变换“**编辑**”按钮。
1. 根据需要，进行相应的更改。
1. 在完成编辑后，确保在页面右下角附近选择了“**保存后发布**”（默认）。
1. 单击“**保存**”，选择一个存储文件夹，输入该集的名称，然后单击“**保存**”。

## 删除 Catalog {#deleting-an-ecatalog}

在删除集时，集本身将移到垃圾桶中。不过，集中的成员（或“子项”）不受影响；它们分别保持现有的已发布或未发布状态。

另请参阅[手动发布资源](publishing-files.md#manually_publishing_assets)和[手动取消发布资源](publishing-files.md#manually_unpublishing_assets)。

**删除 eCatalog**

1. 在网格视图、列表视图或详细信息视图中，选择一个或多个 Catalog。
1. 在全局导航栏上，单击“**文件**”>“**删除**”>“**删除**”。

## 自定义目录 (TOC) {#customizing-the-table-of-contents-toc}

Dynamic Media Classic在电子目录屏幕的“订单页面”选项卡上提供电子目录中的默认页码。 要自定义页面名称，可以更改构成目录 (TOC) 的页标签。推荐重命名封面和封底。例如，封面可以阅读“封面”而不是“第0-1页”。

可以采用手动方式或通过从 CSV（仅 Mac）或 XML 文件导入页面名称来为 eCatalog 创建自定义目录 (TOC)。

>[!NOTE]
>
>要恢复默认的页面标题，单击“排序页面”选项卡上的“TOC 标签”按钮，然后选择“恢复默认值（全部）”。

### 手动输入页面名称 {#manually-entering-page-names}

要逐个手动输入页面名称，转至 eCatalog 屏幕的“排序页面”选项卡。然后在页码字段中单击，并输入名称。输入要指定给每个页面的名称。

### 导入页面名称 {#importing-page-names}

如果处理包含很多页面的 eCatalog，则推荐使用导入页面名称的方法。可以从制表符分隔的文件或 XML 文件导入名称。

目录标签存储在图像的“用户数据”字段中；将此数据格式化为列表 `name=<value>`` pairs separated by two question marks “??” `。 例如，要为名为tocEN &quot;的目录字段设置一个标签，请将图像的用户数据设置为：

tocEN=&lt;EN_page_label>

要为名为 tocEN 和 tocFR 的 TOC 字段设置单独标签：

tocEN=&lt;EN_page_label>??tocFR=&lt;FR_page_label>

要在制表符分隔的文件中导入“用户数据”字段，应包含 userdata 字段）：

| IPSID | Userdata |
|--- |--- |
| `<image_IPS_ID>` | tocEN=&lt;EN_page_label>??tocFR=&lt;FR_page_label> |

要用 XML 文件导入“用户数据”字段，应包含 `vc_userdata` 属性：

```as3
<ips> 
<ghw_object vc_objectname="<image_IPS_ID>" … vc_userdata=" tocEN=<EN_page_label>??tocFR=<FR_page_label>" … /> 
</ips>
```

要从制表符分隔的文件或 XML 文件导入页面名称，选择“TOC 标签”按钮并选择“导入”。“上载元数据”对话框随即显示。单击“浏览”按钮，并导入将每个页面与页面名称关联的 CSV 文件（仅 Mac）或 XML 文件。
