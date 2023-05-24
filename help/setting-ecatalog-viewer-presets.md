---
title: 设置eCatalog查看器预设
description: 了解如何在Adobe Dynamic Media Classic中设置eCatalog查看器预设。
uuid: aca66bc5-8491-4d81-9a06-1d3531860a14
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 6c123f85-3bc4-4392-a7fb-55618127c65e
feature: Dynamic Media Classic,Viewers,Viewer Presets,eCatalog
role: User
exl-id: 4357e6b8-fbc5-4e93-9476-db92a7dc7464
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '489'
ht-degree: 34%

---

# 设置eCatalog查看器预设{#setting-up-ecatalog-viewer-presets}

eCatalog 查看器预设决定了 eCatalog 查看器的样式、行为和外观。Adobe Dynamic Media Classic提供了eCatalog查看器预设，如果您是管理员，也可以创建自己的eCatalog查看器预设。

要创建预设，您可以从头开始或从Adobe Dynamic Media Classic提供的eCatalog查看器预设开始，然后以新名称保存。 可以创建自己的 eCatalog 查看器预设，以使用公司颜色来显示印刷材料并设置色调。

eCatalog 查看器预设提供很多设置，包括页间跳转、缩放、搜索及选择“外观”。这些控件的外观和查看器的显示方式取决于您选择的eCatalog查看器预设。

请按照以下步骤操作，以便创建eCatalog查看器预设（您必须是管理员）：

1. 在全局导航栏上，转到 **[!UICONTROL 设置]** > **[!UICONTROL 查看器预设]**.
1. 在“查看器预设”屏幕上，重新开始或从现有的 eCatalog 查看器预设开始创建 eCatalog 查看器预设：

   * **创建eCatalog查看器预设**  — 选择 **[!UICONTROL 添加]**. 在“添加查看器预设”对话框中，选择一个平台，选择eCatalog查看器，然后选择 **[!UICONTROL 添加]**.

   * **编辑eCatalog查看器预设**  — 选择eCatalog查看器预设，然后选择 **[!UICONTROL 编辑]**. 选择 **[!UICONTROL 另存为]** 完成预设创建后。

1. 在“配置查看器”屏幕上，输入 eCatalog 查看器预设的名称。
1. 在“配置查看器”屏幕上，设置所需选项。

   选择 **[!UICONTROL 信息提示]** 图标（如果您要阅读其说明）。

   “预览”页面会在您更新和更改设置时显示查看器。

1. （可选）在 **[!UICONTROL 信息面板设置]**，则 **[!UICONTROL 信息服务器URL]** 选项可以包括查看器替换的以下特殊令牌：

   | 令牌 | 代替为 | 说明 |
   | --- | --- | --- |
   | `$1$` | rollover_key 值 | 来自的项标识符 `<area>` 映射的元素。 |
   | `$2$` | frame | 图像集中当前显示的帧的序号。 |
   | `$3$` | 图像根 | 在图像命令中指定的第一个物品的第一个路径元素（通常为指定图像集的目录条目的图像目录 ID）。 |

1. （可选）在 **[!UICONTROL 信息面板设置]**，在 **[!UICONTROL 响应模板]** 框中，键入在Adobe Dynamic Media Classic检索图像映射信息时遇到错误时要显示的文本。 例如，如果系统收到公司名称和 eCatalog 名称，但是没有变换标识符，则将为用户显示该消息。

>[!NOTE]
>
>要使用此响应模板而不是eCatalog本身中定义的模板，请添加 `fmt=1` 到信息服务器URL的末尾。 示例: `https://.../$3$/$4$/$1$/?FMT=1`.

1. 选择 **[!UICONTROL 保存]**.
1. 选择 **[!UICONTROL 默认]** 如果您希望创建的eCatalog查看器预设是在网页上用于显示eCatalog的预设。

要删除eCatalog查看器预设，请在“查看器预设”屏幕中选择它，然后选择 **[!UICONTROL 删除]**.

>[!MORELIKETHIS]
>
>* [Viewer Presets](application-setup.md#viewer_presets)

