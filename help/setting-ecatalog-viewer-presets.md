---
title: 设置 eCatalog 查看器预设
seo-title: 设置 eCatalog 查看器预设
description: 'null'
seo-description: 了解如何设置eCatalog查看器预设。
uuid: aca66bc5-8491-4d81-9a06-1d3531860a14
contentOwner: admin
content-type: 引用
products: SG_ EXPERIENCE MANAGER/Dynamic-Media-Scene-7
discoiquuid: 6c123f85-3bc4-4392-a7 fb-55618127c65 e
translation-type: tm+mt
source-git-commit: a1722c15d3c049f05959d895e85297d47d730872

---


# 设置 eCatalog 查看器预设{#setting-up-ecatalog-viewer-presets}

eCatalog 查看器预设决定了 eCatalog 查看器的样式、行为和外观。Dynamic Media Classic提供eCatalog查看器预设，如果您是管理员，还可以创建自己的电子目录查看器预设。

要创建新预设，您可以从头开始，或从Dynamic Media经典提供的eCatalog查看器预设开始，并根据新名称保存它。可以创建自己的 eCatalog 查看器预设，以使用公司颜色来显示印刷材料并设置色调。

eCatalog 查看器预设提供很多设置，包括页间跳转、缩放、搜索及选择“外观”。这些控件的外观及查看器本身的外观取决于所选的 eCatalog 查看器预设。

按照以下步骤创建 eCatalog 查看器预设（必须是管理员）：

1. 单击“**设置**”&gt;“**查看器预设**”。
1. 在“查看器预设”屏幕上，重新开始或从现有的 eCatalog 查看器预设开始创建 eCatalog 查看器预设：

   **创建电子目录查看器预设** 单击添加。In the Add Viewer Preset dialog box, choose a platform, choose eCatalog Viewer, then click **Add**.

   **编辑电子目录查看器预设** 选择一个电子目录查看器预设，然后单击编辑。Click **Save As** after you finish creating the preset.

1. 在“配置查看器”屏幕上，输入 eCatalog 查看器预设的名称。
1. 在“配置查看器”屏幕上，设置所需选项。

   单击选项旁边的“信息提示”图标 ，即可查看该选项的说明。

   更新和更改设置时，预览屏幕将显示查看器。

1. （可选）在“信息面板设置”中，“信息服务器 URL”选项可以包括查看器代替的以下特殊令牌：

   | 令牌 | 代替为 | 说明 |
   |--- |--- |--- |
   | `$1$` | rollover_key 值 | The item identifier from the `<area>` element of the map. |
   | `$2$` | frame | 图像集中当前显示的帧的序号。 |
   | `$3$` | imageroot | 在图像命令中指定的第一个物品的第一个路径元素（通常为指定图像集的目录条目的图像目录 ID）。 |

1. (可选)在“信息面板设置”中，在“响应模板”框中键入要在“动态媒体经典”遇到的图像映射检索信息时显示的文本。例如，如果系统收到公司名称和 eCatalog 名称，但是没有变换标识符，则将为用户显示该消息。

>[!NOTE]
>
>要使用该“响应模板”而不是在 eCatalog 本身中定义的模板，将“fmt=1”添加到“信息服务器 URL”的末尾。示例: `https://.../$3$/$4$/$1$/?FMT=1`.

1. 单击“**保存**”。
1. 如果要使用所创建的 eCatalog 查看器预设在网页上显示 eCatalog，单击“默认”。

To delete an eCatalog Viewer Preset, select it on the Viewer Presets screen and click **Delete**.

>[!MORELIKETHIS]
>
>* [Viewer Presets](application-setup.md#viewer_presets)

