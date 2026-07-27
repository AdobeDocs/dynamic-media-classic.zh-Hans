---
title: 创建样本集
description: 了解如何在Adobe Dynamic Media Classic中创建样本集。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/swatch_sets
feature: Dynamic Media Classic,Viewers
role: User
exl-id: 426b6e6b-daed-4ca6-b095-99bb06604b07
topic: Content Management
level: Intermediate
autotag-review: '2026-05-13T17:44:21.987Z'
TQID: 'https://experienceleague.adobe.com/8nWsAO1rwDZnpj3GkUv7iUEqQR894oeoo81Vtr-uHcs'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
source-git-commit: 1343214cf19c9cfc6153e3f8b90c8ffc260de999
workflow-type: tm+mt
source-wordcount: 709
ht-degree: 42%

---

# 创建样本集{#creating-a-swatch-set}

通过样本集，用户可查看采用不同颜色、图案或结束位置的项目。 要使用颜色样本创建样本集，需要具有要提供给用户的每种不同颜色、模式或光泽度的一个图像。 还需要每种颜色、模式或光泽度的一种颜色、模式或光泽度样本。

例如，假定要使用不同颜色的标记显示大写字母的图像，标记为红色、绿色和蓝色。 在这种情况下，您需要同一顶帽的三个图像。 红色、绿色和蓝色票据都需要一张图片。 您还需要红色、绿色和蓝色色板。 颜色样本用作用户在样本集查看器中选择的缩略图，以查看红色计费、绿色计费或蓝色计费次数上限。

## 创建样本集 {#create}

创建集时，**保存后发布**&#x200B;选项会以下列方式影响该集和集成员：

| 保存前是否选择了&#x200B;**[!UICONTROL 保存后发布]**&#x200B;选项？ | 保存后的集状态 | 保存后的集成员状态 |
| --- | --- | --- |
| 是 | 已发布 | 已发布 |
| 否 | 未发布 | 集成员保持其已发布或未发布状态。 |

另请参阅[手动发布资源](publishing-files.md#manually_publishing_assets)和[手动取消发布资源](publishing-files.md#manually_unpublishing_assets)。

**创建样本集：**

1. 执行以下任一操作：

   * **首先选择图像**：在“浏览”面板中，选择图像，然后转到&#x200B;**[!UICONTROL 生成]** > **[!UICONTROL 样本集]**。

   * **从样本集屏幕开始**：转到&#x200B;**[!UICONTROL 生成]** > **[!UICONTROL 样本集]**。 从资源库中选择一个文件夹，然后将图像拖到“样本集”页面的“视图”部分中。

1. 将样本颜色、模式或光泽度拖到“样本集”页面上的样本占位符框中。

   确保拖到每个占位符里的颜色、模式或光泽度样本表示相邻图像的颜色、模式或光泽度。

1. 要更改样本集中图像的顺序，请将图像拖到新位置。
1. 在页面的右下角附近，确保选中&#x200B;**[!UICONTROL 保存后发布]**（默认）。
1. 选择&#x200B;**[!UICONTROL 保存]**，选择用于存储样本集的文件夹，输入样本集的名称，然后选择&#x200B;**[!UICONTROL 提交]**。
1. 要在样本集查看器中查看您的样本集，请在样本集屏幕上选择&#x200B;**[!UICONTROL 预览]**。 您可以在样本集查看器中选择样本缩略图以查看它们的运行方式。

## 编辑样本集 {#editing-a-swatch-set}

无论您编辑已发布集还是未发布集，**[!UICONTROL Publish after a save]**&#x200B;选项都会通过以下方式影响该集和集成员：

| 是否已发布集？ | 在保存编辑之前，是否选择了&#x200B;**[!UICONTROL 保存后发布]**&#x200B;保存选项？ | 保存后的集状态 | 保存后的集成员状态 |
|--- | --- | --- | --- |
| 是 | 是 | 已发布 | 已发布。 |
| 是 | 否 | 已发布 | 现有的集成员保持其已发布状态。 在编辑期间添加的任何新的集成员保持其已发布或未发布状态。 |
| 否 | 是 | 已发布 | 已发布。 |
| 否 | 否 | 未发布 | 现有的集成员以及在编辑期间添加的任何新的集成员保持其已发布或未发布状态。 |

另请参阅[手动发布资源](publishing-files.md#manually_publishing_assets)和[手动取消发布资源](publishing-files.md#manually_unpublishing_assets)。

**要编辑样本集：**

1. 在网格视图中，浏览到样本集，然后选择图像下方的&#x200B;**[!UICONTROL 编辑]**。
1. 执行以下操作之一：

   * 要添加图像（已发布或已取消发布），请将其从添加Assets中的文件夹拖动到样本集的&#x200B;**[!UICONTROL 视图]**&#x200B;页面。
   * 要删除图像，请选择该图像，然后在工具栏上选择&#x200B;**[!UICONTROL 删除]**。
   * 要将图像重新排序，请将图像拖到新位置。

1. 完成编辑该集时（位于页面的右下角附近），请确保选中&#x200B;**[!UICONTROL 保存]**&#x200B;后发布（默认）。
1. 选择&#x200B;**[!UICONTROL 保存]**，选择一个存储文件夹，输入该集的名称，然后选择&#x200B;**[!UICONTROL 保存]**。

## 删除样本集

删除集合时，集合本身将移到“已删除项”文件夹。 该集中的成员不受影响；它们保持现有的已发布或未发布状态。

另请参阅[手动发布资源](publishing-files.md#manually_publishing_assets)和[手动取消发布资源](publishing-files.md#manually_unpublishing_assets)。

**要删除样本集：**

1. 在网格视图、列表视图或详细信息视图中，选择一个或多个样本集。
1. 在全局导航栏上，转到&#x200B;**[!UICONTROL 文件]** > **[!UICONTROL 删除]** > **[!UICONTROL 删除]**。
