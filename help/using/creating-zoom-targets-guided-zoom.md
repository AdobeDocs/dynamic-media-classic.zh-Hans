---
title: 为引导缩放创建缩放目标
description: 了解如何为Adobe Dynamic Media Classic中的引导式缩放创建缩放目标。
uuid: 501ea37b-adc5-4290-87eb-52a3501e5d26
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/zoom
discoiquuid: e7b4673c-8681-4741-912e-9a31cf106449
feature: Dynamic Media Classic,Viewers,Zoom
role: User
exl-id: ffb799ba-1cf1-48e0-91a8-dea758139140
topic: Content Management
level: Intermediate
source-git-commit: d82f816553f807b514f4690827dab672a6baf690
workflow-type: tm+mt
source-wordcount: '729'
ht-degree: 41%

---

# 为引导缩放创建缩放目标{#creating-zoom-targets-for-guided-zoom}

缩放目标会将查看者引导到图像的特定部分。除了自由格式缩放之外，查看者还可以选择缩放目标缩略图，并缩放到您希望他们聚焦的图像部分。 通过缩放目标，可突出显示图像的有趣或诱人之处。

![为引导缩放创建缩放目标](/help/using/assets/zo_guided_zoom.png)

## 关于缩放目标 {#about-zoom-targets}

缩放目标的最大缩放百分比是 100%。根据查看器大小和图像大小的不同组合，最小缩放百分比也会有所不同，如下表所示：

| 图像大小 | 查看器大小 | 缩放百分比 |
| --- | --- | --- |
| 大 | 较小 | 最小缩放百分比较小 |
| 小 | 较大 | 最小缩放百分比较大 |

您可以更改缩放查看器大小，使之与网页上使用的大小相匹配。要永久更改此设置，可以在“设置”屏幕上更改查看器大小（如果您是管理员）。参见 [设置缩放查看器预设](setting-zoom-viewer-presets.md#setting_up_zoom_viewer_presets).

## 创建和编辑缩放目标 {#creating-and-editing-zoom-targets}

在“缩放目标编辑器”屏幕上创建并编辑缩放目标。要打开该屏幕，请选择一个图像并执行以下任一操作：

* 选择变换 **[!UICONTROL 编辑]** 按钮，然后选择“缩放目标”。
* 在“浏览”面板中，将图像显示在 **[!UICONTROL 详细信息视图]**，然后选择 **[!UICONTROL 缩放目标]**.

在缩放目标编辑器屏幕上，选择 **[!UICONTROL 选择目标]** 按钮（箭头）以在更改目标大小或位置之前选择目标。 要在图像上创建缩放目标，请选择 **[!UICONTROL 添加目标]** （矩形）。 “缩放目标编辑器”页还提供了用于删除、复制和命名缩放目标的工具。

### 创建缩放目标 {#creating-a-zoom-target}

要创建缩放目标，请打开“缩放目标编辑器”页面，然后执行以下操作：

1. 选择 **[!UICONTROL 添加目标]** （矩形），将指针移动到图像上，然后选择缩放目标的位置。

   缩放目标的缩略图图像显示在屏幕右侧的面板中。

1. 选取 **[!UICONTROL 选择目标]** （箭头），然后选择您创建的缩放目标，并调整目标的大小和位置。

   * **调整大小**  — 将指针移动到缩放目标的角上并拖动以放大或缩小目标。

   * **位置**  — 将指针移动到缩放目标上并将其拖动到其他位置。

1. 在“名称”框中输入缩放目标名称。

   >[!NOTE]
   >
   >在“名称”框中输入的不仅仅是名称。用户在缩放目标上移动指针时，将会看到您在“名称”框中输入的内容。在“名称”框中输入对缩放目标的简要描述，以便用户了解其可以缩放的内容。

1. 可以视情况在“用户数据”字段中输入用户数据。该字段可供网站设计人员向缩放目标中添加信息。
1. 选择 **[!UICONTROL 保存]**.

   即可保存缩放目标的坐标和缩放级别。带有您输入的名称的缩放目标缩略图显示在屏幕右侧。

>[!NOTE]
>
>要在缩放查看器中查看缩放目标的外观，请选择 **[!UICONTROL 预览]** 按钮，然后在“预览”屏幕中选择一个缩放查看器。 有关此屏幕的信息，请参阅 [使用不同的缩放查看器预览图像](previewing-image-assets-different-zoom.md#previewing_image_assets_with_different_zoom_viewers).

### 编辑缩放目标 {#editing-zoom-targets}

要编辑缩放目标，请在“缩放目标编辑器”页面上使用以下技术：

* **重新定位**  — 使用“选择目标”按钮（箭头），选择目标。 然后，将目标拖动到其他位置。

* **调整大小**  — 使用“选择目标”按钮（箭头），选择目标。 要放大或缩小目标，请将指针移动到缩放目标的一个角上并拖动。

* **删除**  — 选择屏幕右侧的目标缩略图图像。 然后选择 **[!UICONTROL 删除目标]**.

* **重命名**  — 选择屏幕右侧的目标缩略图图像。 然后，在 **[!UICONTROL 名称]** 文本字段并选择 **[!UICONTROL 保存]**.

### 复制缩放目标 {#copying-zoom-targets}

可以将缩放目标从一个图像复制到另一个图像。如果两个图像的内容相似且缩放目标位于同一位置，则可复制目标。要将缩放目标复制到另一个图像，请执行以下操作：

1. 在“缩放目标编辑器”屏幕中打开包含要复制的缩放目标的图像。
1. 选择 **[!UICONTROL 将目标复制到]**.
1. 在“选择图像”对话框中，选择一个图像并选取 **[!UICONTROL 选择]**.
