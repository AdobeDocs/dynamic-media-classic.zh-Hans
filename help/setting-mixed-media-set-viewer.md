---
title: 设置混合媒体集查看器预设
description: 了解如何在Dynamic Media Classic中设置混合媒体集查看器预设Adobe。
uuid: d5bf1840-e453-445d-bebc-84889b29f3c8
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/mixed_media_sets
discoiquuid: 8029aad8-d696-4d7c-99e2-3b08edb68181
feature: Dynamic Media Classic,Viewers,Mixed Media Sets
role: User
exl-id: d41b30e7-994a-43f3-8698-7dbfc36305ae
source-git-commit: e47c22508230adbb1ece323be0c1413a3f27ad89
workflow-type: tm+mt
source-wordcount: '613'
ht-degree: 44%

---

# 设置混合媒体集查看器预设{#setting-up-a-mixed-media-set-viewer-preset}

混合媒体集查看器预设决定着主查看器的样式、行为和外观。配置预设时，指定要在混合媒体查看器内显示的其他查看器。例如，如果已经在混合媒体集中包含图像集，则为该混合媒体集查看器指定图像集查看器预设。

可以选择在混合媒体集查看器中包含全部或部分社区功能。嵌入功能添加了一个指向查看器的链接，允许用户复制在外部页面（如博客、网站或社交网站）中显示查看器所需的代码。“链接”功能提供查看器的 URL，以便用户可以链接回该查看器。“访问”功能提供指向所指定网站的链接。

1. 在全局导航栏上，转到&#x200B;**[!UICONTROL Setup]** > **[!UICONTROL 查看器预设]**。
1. 在“查看器预设”页面上，执行下列操作之一：

   * 要创建预设，请选择&#x200B;**[!UICONTROL Add]**。 在“添加查看器预设”对话框中，选择平台，选择&#x200B;**[!UICONTROL 混合媒体集查看器]**，然后选择&#x200B;**[!UICONTROL 添加]**。
   * 要编辑混合媒体集查看器预设，请选择该预设，然后选择&#x200B;**[!UICONTROL 编辑]**。

1. 在“配置查看器”页面的“混合媒体集查看器预设的预设名称”框中键入名称。
1. 指定&#x200B;**[!UICONTROL Tabs]**&#x200B;或&#x200B;**[!UICONTROL 无Tabs]**。 制表符按类型（如视频、样本和旋转集）分隔项目。如果未指定制表符，则所有项目都会显示在“预览”窗口下的一行中。
1. 在&#x200B;**[!UICONTROL 名称]**&#x200B;框中，键入要添加的查看器的名称。

   例如，如果要向混合媒体集添加色板集，请键入`Swatch Set A`。

1. 从“查看器”菜单中选择要查看的资源的类型，如样本集。
1. 从“预设”菜单中为所选资源类型选择预设。

   例如，如果要添加色板集，请选择&#x200B;**[!UICONTROL SwatchSet1-Colors]**。

1. 选择&#x200B;**[!UICONTROL Add]**。

   新的查看器预设显示在列表中。

1. 对所有要添加的查看器预设重复步骤 6 - 9。
1. 要编辑预设列表，执行以下任意操作：

   * 要从列表中删除预设，请选择该预设，然后选择&#x200B;**[!UICONTROL 删除]**。
   * 要对列表中的预设重新排序，请选择一个预设，然后选择蓝色的&#x200B;**[!UICONTROL 向上]**&#x200B;或&#x200B;**[!UICONTROL 向下]**&#x200B;箭头。

1. 要将社区功能（“嵌入”、“链接”、“访问”）添加到查看器中，请指定以下任何设置的选项：

   * **电子邮件**  — 在查 **** 看器中选择启用电子邮件按钮。当用户在查看集时选择“电子邮件”按钮时，将打开一封包含该集链接的电子邮件。

   * **嵌入**  — 选择 **[!UICONTROL 实时]**。在“嵌入按钮标签”框中，键入要在查看器中显示的“嵌入”按钮的名称。如果需要，请选择&#x200B;**[!UICONTROL Browse]** ，找到并选择按钮的自定义外观。

   * **链接**  — 选择 **[!UICONTROL 实时]**。在链接按钮标签框中，键入您希望在链接按钮的查看器中显示的名称。 如果需要，请选择&#x200B;**[!UICONTROL Browse]** ，找到并选择按钮的自定义外观。

   * **访问**  — 选择 **[!UICONTROL 实时]**。在“访问按钮标签”框中，键入您希望在“访问”按钮的查看器中显示的名称。 在“访问 URL”框中，键入网站的 URL，该网站是您希望在用户单击链接时打开的网站。

1. 根据需要指定其他选项。要查看选项的描述，请选择选项旁边的信息提示图标。

   在您更新和更改设置时，“预览”页面会显示查看器。

1. 选择&#x200B;**[!UICONTROL Save]**。

>[!MORELIKETHIS]
>
>* [创建和编辑查看器预设](application-setup.md#adding_and_editing_viewer_presets)

