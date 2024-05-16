---
title: 设置混合媒体集查看器预设
description: 了解如何在Adobe Dynamic Media Classic中设置混合媒体集查看器预设。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/mixed_media_sets
feature: Dynamic Media Classic,Viewers,Mixed Media Sets
role: User
exl-id: d41b30e7-994a-43f3-8698-7dbfc36305ae
topic: Content Management
level: Intermediate
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '614'
ht-degree: 27%

---

# 设置混合媒体集查看器预设{#setting-up-a-mixed-media-set-viewer-preset}

混合媒体集查看器预设决定着主查看器的样式、行为和外观。配置预设时，指定要在混合媒体查看器内显示的其他查看器。例如，如果您在混合媒体集中包含图像集，请为混合媒体集查看器指定图像集查看器预设。

可以选择在混合媒体集查看器中包含全部或部分社区功能。嵌入功能会添加指向查看器的链接，以便用户复制在外部页面（如博客、网站或社交网站）中显示查看器所需的代码。 “链接”功能提供查看器的 URL，以便用户可以链接回该查看器。访问功能提供指向您指定的网站的链接。

1. 在全局导航栏上，转到 **[!UICONTROL 设置]** > **[!UICONTROL 查看器预设]**.
1. 在“查看器预设”页面上，执行下列操作之一：

   * 要创建预设，请选择 **[!UICONTROL 添加]**. 在“添加查看器预设”对话框中，选择一个平台，然后选择 **[!UICONTROL 混合媒体集查看器]**，然后选择 **[!UICONTROL 添加]**.
   * 要编辑混合媒体集查看器预设，请选择它，然后选择 **[!UICONTROL 编辑]**.

1. 在配置查看器页面上，在混合媒体集查看器预设的预设名称框中键入名称。
1. 指定 **[!UICONTROL 选项卡]** 或 **[!UICONTROL 无选项卡]**. 制表符按类型（如视频、样本和旋转集）分隔项目。未指定制表符时，所有项目都会显示在“预览”窗口下的行中。
1. 在 **[!UICONTROL 名称]** 框中，键入要添加查看器的名称。

   例如，如果要向混合媒体集添加色板集，请键入 `Swatch Set A`.

1. 从“查看器”菜单中选择要查看的资源的类型，如样本集。
1. 从“预设”菜单中为所选资源类型选择预设。

   例如，如果要添加样本集，请选择 **[!UICONTROL 样本集1 — 颜色]**.

1. 选择 **[!UICONTROL 添加]**.

   新的查看器预设显示在列表中。

1. 对要添加的所有查看器预设重复步骤6:9。
1. 要编辑预设列表，执行以下任意操作：

   * 要从列表中删除预设，请选择该预设，然后选择 **[!UICONTROL 删除]**.
   * 要重新排序列表中的预设，请选择预设，然后选择蓝色 **[!UICONTROL 向上]** 或 **[!UICONTROL 向下]** 箭头。

1. 要将社区功能（“嵌入”、“链接”、“访问”）添加到查看器中，请指定以下任何设置的选项：

   * **电子邮件**：选择 **[!UICONTROL 开启]** 在查看器中启用电子邮件按钮。 当用户选择电子邮件按钮查看集合时，将打开包含集合链接的电子邮件。

   * **嵌入**：选择 **[!UICONTROL 实时]**. 在“嵌入按钮标签”框中，键入要在查看器中显示的“嵌入”按钮的名称。如果需要，请选择 **[!UICONTROL 浏览]** 以定位和选择按钮的自定义外观。

   * **链接**：选择 **[!UICONTROL 实时]**. 在“链接按钮标签”框中，键入要在查看器中显示的“链接”按钮的名称。 如果需要，请选择 **[!UICONTROL 浏览]** 以定位和选择按钮的自定义外观。

   * **访问**：选择 **[!UICONTROL 实时]**. 在访问按钮标签框中，键入要在查看器中显示的访问按钮名称。 在访问URL框中，键入要在选择链接时打开的网站URL。

1. 根据需要指定其他选项。要查看选项的描述，请选择选项旁边的“信息提示”图标。

   当您更新和更改设置时，“预览”页面将显示查看器。

1. 选择 **[!UICONTROL 保存]**.

>[!MORELIKETHIS]
>
>* [创建和编辑查看器预设](application-setup.md#adding_and_editing_viewer_presets)
