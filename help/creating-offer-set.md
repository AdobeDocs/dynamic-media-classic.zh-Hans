---
title: 创建选件集
description: 了解如何在Adobe Dynamic Media Classic中创建优惠集。
uuid: 6d6a4af9-70c0-4cfa-9a8f-855d6adfcc8f
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
discoiquuid: 59b6437d-c21e-4929-9291-3032dbb34565
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 05f2cce0-72bf-4933-87ab-c9003c848e35
source-git-commit: 352b1c383195fa03294ad3501207d63f3cfe3e42
workflow-type: tm+mt
source-wordcount: '1293'
ht-degree: 35%

---

# 创建选件集 {#creating-an-offer-set}

您可以创建以下任意类型的优惠套餐：

* 视频
* 参数化模板
* 图像

对于模板，选择&#x200B;**[!UICONTROL 添加和预览]**，然后设置您选择的参数。 其他选件集类型不包含参数，但您仍可以通过选择&#x200B;**[!UICONTROL 预览]**&#x200B;并更改可用的预设来自定义它们。

Adobe Dynamic Media Classic提供了用于编辑和创建选件集的工具。

>[!NOTE]
>
>在创建选件集之前，请确保发布要用于该集的所有资产，以将其设置为Adobe Dynamic Media Classic。 请参阅[手动发布资源](publishing-files.md#manually_publishing_assets)和[手动取消发布资源](publishing-files.md#manually_unpublishing_assets)。

## 优惠套餐的类型 {#types-of-offer-sets}

从以下类型的优惠套餐创建一种优惠套餐：

* **图像**  — 您可以为选件集组合图像。每个图像在集中包含一个不同的选件。

* **图像模板**  — 您可以使用“生成”>“模板基础知识”命 **[!UICONTROL 令在Adobe Dynamic Media Classic中]** 参数化图像模板。通过参数，可换出及自定义模板的各组成部分（文本框架中的文本、不同的图像）。对于优惠套餐，举例来说，您可以使用模板参数在优惠套餐中的同一图像上创建变型。有关创建图像模板并对其进行参数化的信息，请参阅[创建模板参数](creating-template-parameters.md#creating_template_parameters)。

另请参阅[模板基础知识](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/553_Template%20Basics_converted%20renamed_Dynamic%20Banners-AVS)培训视频。

* **视频**  — 您可以为选件集组合视频。每个视频是套餐中的一个不同优惠。

## 使用参数化模板创建选件集 {#creating-an-offer-set-with-a-parameterized-template}

在创建优惠套餐时，“**[!UICONTROL 保存后发布]**”选项按以下方式影响集和集成员：

| **[!UICONTROL 在保存前]** 选择保存后发布选项？ | 保存后的集状态 | 保存后的集成员状态 |
| --- | --- | --- |
| 是 | 已发布 | 已发布 |
| 否 | 未发布 | 集成员保持其已发布或未发布状态。 |

另请参阅[手动发布资源](publishing-files.md#manually_publishing_assets)和[手动取消发布资源](publishing-files.md#manually_unpublishing_assets)。

**要使用参数化模板创建选件集，请执行以下操作：**

1. 选择模板或横幅。
1. 转到&#x200B;**[!UICONTROL Build]** > **[!UICONTROL Test&amp;Target选件集]**。

   “Test&amp;Target选件集”页列出了选件集中的选件。 列表中的第一项是对象。

1. 选择对象，然后选择&#x200B;**[!UICONTROL 添加并预览]**。

   此页面的左侧将列出模板中的参数和参数值。

1. 更改参数值以创建优惠。例如，在文本字段中输入不同文本、更改图层大小、用一个图像交换另一个图像或者选择不同的查看器预设。
1. 选择&#x200B;**[!UICONTROL 保存]**&#x200B;或&#x200B;**[!UICONTROL 另存为**]**&#x200B;以将选件保存为选件集的一部分。

   “Test&amp;Target选件集”页面列出了您创建的选件。

1. 重复步骤 3 到 5 为套餐创建更多优惠。
1. 完成后，在页面右下角附近，确保选中&#x200B;**[!UICONTROL 保存后发布*]**（默认）。
1. 选择&#x200B;**[!UICONTROL 关闭]**，输入选件集的名称，然后选择&#x200B;**[!UICONTROL 保存]**。

在关闭Test&amp;Target选件集页面之前，请先将该选件集推送到Adobe Target Standard/Premium。 请参阅[将优惠套餐推送到 Test&amp;Target](pushing-offer-sets-target.md#pushing_offer_sets_to_target)。

## 创建包含图像或视频的选件集 {#creating-an-offer-set-with-images-or-videos}

在创建优惠套餐时，“**[!UICONTROL 保存后发布]**”选项按以下方式影响集和集成员：

| **[!UICONTROL 在保存前]** 选择保存后发布选项？ | 保存后的集状态 | 保存后的集成员状态 |
| --- | --- | --- |
| 是 | 已发布 | 已发布 |
| 否 | 未发布 | 集成员保持其已发布或未发布状态。 |

另请参阅[手动发布资源](publishing-files.md#manually_publishing_assets)和[手动取消发布资源](publishing-files.md#manually_unpublishing_assets)。

**使用图像或视频创建优惠套餐:**

1. 组合选件集的图像或视频。 从Test&amp;Target选件集屏幕或网格视图或列表视图开始，然后使用以下方法之一：

   * **Test&amp;Target选件集屏幕**  — 转到 **[!UICONTROL 内部版本]**  >  **[!UICONTROL Test&amp;Target选件集]**。将图像或视频拖到屏幕上。要创建大小不同的视频或图像，请拖入图像或视频的多个副本，然后逐个设置每个大小。

   * **网格视图或列表视图**  — 选择图像或视频，然后转到 **[!UICONTROL 构建]**  >  **[!UICONTROL Test&amp;Target选件集]**。

1. 或者，选择图像或视频，然后选择&#x200B;**[!UICONTROL 预览]**。 在“预览选件”页面上，您可以更改所选图像或视频的大小和外观。 或者，您也可以更改选件集中的所有图像或视频。

   * 选择预设以更改图像或视频的外观和大小。
   * 要将您选择的预设应用于选件集中的所有选件，请选中&#x200B;**[!UICONTROL 选择全部预设]**&#x200B;复选框。

   选择&#x200B;**[!UICONTROL Save]**&#x200B;以保存对图像或视频选件所做的更改。 然后选择&#x200B;**[!UICONTROL 关闭]**&#x200B;以返回到Test&amp;Target选件集页面。

1. 完成为选件集创建选件并为不同图像选择图像预设后，请确保选中&#x200B;**[!UICONTROL 保存后发布]**（默认）。
1. 选择&#x200B;**[!UICONTROL Save]**&#x200B;并输入选件集的名称，然后选择&#x200B;**[!UICONTROL Save]**。

在关闭Test&amp;Target选件集页面之前，请将该选件集推送到Adobe Target Standard/Premium。 请参阅[将选件集推送到Test&amp;Target](pushing-offer-sets-target.md#pushing_offer_sets_to_target)。

## 编辑选件集 {#editing-an-offer-set}

无论您是编辑已发布的集还是未发布的集，**[!UICONTROL 保存后发布]**&#x200B;选项都会通过以下方式影响集和集成员：

| 是否已发布集？ | **[!UICONTROL 在保存您]** 的编辑之前选择保存选项后发布？ | 保存后的集状态 | 保存后的集成员状态 |
| --- | --- | --- | --- |
| 是 | 是 | 已发布 | 已发布 |
| 是 | 否 | 已发布 | 现有的集成员保持其已发布状态。在编辑期间添加的任何新的集成员保持其已发布或未发布状态。 |
| 否 | 是 | 已发布 | 已发布 |
| 否 | 否 | 未发布 | 现有的集成员以及在编辑期间添加的任何新的集成员保持其已发布或未发布状态。 |

另请参阅[手动发布资源](publishing-files.md#manually_publishing_assets)和[手动取消发布资源](publishing-files.md#manually_unpublishing_assets)。

**要编辑选件集，请执行以下操作：**

1. 要编辑选件集，请在网格视图或列表视图中显示选件集，然后选择其&#x200B;**[!UICONTROL 编辑]**&#x200B;滚动按钮。
1. 在Test&amp;Target选件集页面中，执行以下任一操作：

   * **删除选件**  — 选择选件，然后选择“删除” **** 以从选件集中删除选件。
   * **添加选件**  — 添加选件的方式取决于您正在使用的选件集类型：
      * **模板**  — 选择 **[!UICONTROL 添加和预览]**，然后在“添加和预览选件”页面上，创建另一个选件。
      * **图像和视频**  — 将图像或视频拖动到Test&amp;Target选件集页面。

   >[!NOTE]
   >
   >您无法删除与某个活动相关联的优惠套餐。要删除与促销活动关联的选件集，请登录到Adobe Target Standard/Premium，然后先删除促销活动关联。 即使与促销活动取消关联后，资产也只能从Adobe Dynamic Media Classic中删除，这需要登录到Adobe Target Standard/Premium，而不能从Adobe Target Standard/Premium中登录。

1. 完成编辑后，在页面右下角附近，确保选中&#x200B;**[!UICONTROL 保存后发布]**（默认）。
1. 选择&#x200B;**[!UICONTROL Save]**，选择存储文件夹，输入集的名称，然后选择&#x200B;**[!UICONTROL Save]**。

## 删除选件集 {#deleting-an-offer-set}

在删除优惠套餐时，套餐本身将移到垃圾桶中。不过，集中的成员（或“子项”）不受影响；它们分别保持现有的已发布或未发布状态。

另请参阅[手动发布资源](publishing-files.md#manually_publishing_assets)和[手动取消发布资源](publishing-files.md#manually_unpublishing_assets)。

**要删除选件集，请执行以下操作：**

1. 在“网格视图”、“列表视图”或“详细信息视图”中，选择一个或多个选件集。
1. 在全局导航栏上，转到&#x200B;**[!UICONTROL 文件]** > **[!UICONTROL 删除]** > **删除**。

>[!MORELIKETHIS]
>
>* [创建模板参数](creating-template-parameters.md#creating_template_parameters)

