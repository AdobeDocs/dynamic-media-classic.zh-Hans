---
title: 设置eCatalog查看器预设
description: 了解如何在Adobe Dynamic Media Classic中设置eCatalog查看器预设。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic,Viewers,Viewer Presets,eCatalog
role: User
exl-id: 4357e6b8-fbc5-4e93-9476-db92a7dc7464
topic: Integrations, Development
level: Experienced
source-git-commit: 61665faba1e6bb711aae5becf0150d1ebe3105c0
workflow-type: tm+mt
source-wordcount: '482'
ht-degree: 25%

---

# 设置eCatalog查看器预设{#setting-up-ecatalog-viewer-presets}

eCatalog 查看器预设决定了 eCatalog 查看器的样式、行为和外观。Adobe Dynamic Media Classic提供了eCatalog查看器预设，如果您是管理员，则可以创建自己的eCatalog查看器预设。

要创建预设，您可以从头开始或从Adobe Dynamic Media Classic提供的eCatalog查看器预设开始，然后以新名称保存预设。 可以创建自己的 eCatalog 查看器预设，以使用公司颜色来显示印刷材料并设置色调。

eCatalog查看器预设提供了许多设置，可用于在页面之间切换、缩放、搜索和选择“外观”。 这些控件的外观和查看器的显示方式取决于您选择的eCatalog查看器预设。

请按照以下步骤操作，以创建eCatalog查看器预设（您必须是管理员）：

1. 在全局导航栏上，转到&#x200B;**[!UICONTROL 设置]** > **[!UICONTROL 查看器预设]**。
1. 在“查看器预设”屏幕上，重新开始或从现有的 eCatalog 查看器预设开始创建 eCatalog 查看器预设：

   * **创建eCatalog查看器预设**：选择&#x200B;**[!UICONTROL 添加]**。 在“添加查看器预设”对话框中，选择一个平台，选择eCatalog查看器，然后选择&#x200B;**[!UICONTROL 添加]**。

   * **编辑eCatalog查看器预设**：选择eCatalog查看器预设，然后选择&#x200B;**[!UICONTROL 编辑]**。 完成预设创建后，选择&#x200B;**[!UICONTROL 另存为]**。

1. 在`Configure Viewer`页面上，输入eCatalog查看器预设的名称。
1. 在`Configure Viewer`页面上，设置所需的选项。

   如果要阅读其描述，请选择选项旁边的&#x200B;**[!UICONTROL 信息提示]**&#x200B;图标。

   当您更新和更改设置时，“预览”页面将显示查看器。

1. （可选）在&#x200B;**[!UICONTROL 信息面板设置]**&#x200B;中，**[!UICONTROL 信息服务器URL]**&#x200B;选项可以包含以下特殊令牌，查看器将替换这些令牌：

   | 令牌 | 代替为 | 说明 |
   | --- | --- | --- |
   | `$1$` | rollover_key 值 | 映射的`<area>`元素中的项标识符。 |
   | `$2$` | frame | 图像集中当前显示的帧的序号。 |
   | `$3$` | 图像根 | 在图像命令中指定的第一个物品的第一个路径元素（通常为指定图像集的目录条目的图像目录 ID）。 |

1. （可选）在&#x200B;**[!UICONTROL 信息面板设置]**&#x200B;的&#x200B;**[!UICONTROL 响应模板]**&#x200B;框中，键入当Adobe Dynamic Media Classic在检索图像映射信息时遇到错误时要显示的文本。 例如，如果系统收到公司名称和 eCatalog 名称，但是没有变换标识符，则将为用户显示该消息。

>[!NOTE]
>
>若要使用此响应模板而不是eCatalog本身中定义的模板，请将`fmt=1`添加到信息服务器URL的末尾。 例如： `https://.../$3$/$4$/$1$/?FMT=1`。

1. 选择&#x200B;**[!UICONTROL 保存]**。
1. 选择&#x200B;**[!UICONTROL 默认]**，以便您创建的eCatalog查看器预设是用于在网页上显示eCatalog的预设。

要删除eCatalog查看器预设，请在“查看器预设”屏幕上选择该预设，然后选择&#x200B;**[!UICONTROL 删除]**。

>[!MORELIKETHIS]
>
>* [Viewer Presets](application-setup.md#viewer_presets)
