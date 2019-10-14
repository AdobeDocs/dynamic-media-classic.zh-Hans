---
title: 为引导式缩放创建缩放目标
seo-title: 为引导式缩放创建缩放目标
description: 'null'
seo-description: 了解如何为向导式缩放创建缩放目标。
uuid: 501ea37b-adc5-4290-87eb-52a3501e5d26
contentOwner: admin
content-type: 引用
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEEVENTONDEMAND_PK/categories/zoom
discoiquuid: e7b4673c-8681-4741-912e-9a31cf106449
translation-type: tm+mt
source-git-commit: 6fff3699f8a08af433df3f3a7790a11bf9d05b00

---


# 为引导式缩放创建缩放目标{#creating-zoom-targets-for-guided-zoom}

缩放目标会将查看者引导到图像的特定部分。除了随意缩放之外，查看者也可以单击缩放目标缩略图，缩放到图像的重点部分。通过缩放目标，可突出显示图像的有趣或诱人之处。

![Creating zoom targets for Guided Zoom](/help/assets/zo_guided_zoom.png)

## 关于缩放目标 {#about-zoom-targets}

缩放目标的最大缩放百分比是 100%。根据查看器大小和图像大小的不同组合，最小缩放百分比也会有所不同，如下表所示：

| 图像大小 | 查看器大小 | 缩放百分比 |
|--- |--- |--- |
| 大 | 较小 | 最小缩放百分比较小 |
| 小 | 较大 | 最小缩放百分比较大 |

您可以更改缩放查看器大小，使之与网页上使用的大小相匹配。要永久更改此设置，可以在“设置”屏幕上更改查看器大小（如果您是管理员）。请参阅[设置缩放查看器预设](setting-zoom-viewer-presets.md#setting_up_zoom_viewer_presets)。

## 创建并编辑缩放目标 {#creating-and-editing-zoom-targets}

在“缩放目标编辑器”屏幕上创建并编辑缩放目标。要打开该屏幕，请选择一个图像并执行以下任一操作：

* Click the rollover **[!UICONTROL Edit]** button and choose Zoom Targets.
* In the Browse Panel, display the image in **[!UICONTROL Detail View]**, then click **[!UICONTROL Zoom Targets]**.

On the Zoom Target Editor screen, click **[!UICONTROL Select Target]** button (arrow) to select a target before changing its size or position. Click **[!UICONTROL Add Targets]** (rectangle) to create a zoom target on the image. “缩放目标编辑器”屏幕上也提供了用于删除、复制和命名缩放目标的工具。

### 创建缩放目标 {#creating-a-zoom-target}

打开“缩放目标编辑器”屏幕，并按照以下步骤创建缩放目标：

1. Click **[!UICONTROL Add Targets]** (rectangle), move the pointer over the image, and click where you want to the zoom target to be.

   缩放目标的缩略图图像显示在屏幕右侧的面板中。

1. Click **[!UICONTROL Select Target]** (arrow), click to select the zoom target you created, and adjust the size and position of the target.

   * **调整大**&#x200B;小将指针移到缩放目标的一角上，然后拖动以放大或缩小目标。

   * **定位**&#x200B;将指针移到缩放目标上，然后将其拖动到其他位置。

1. 在“名称”框中输入缩放目标名称。

   >[!NOTE]
   >
   >在“名称”框中输入的不仅仅是名称。用户在缩放目标上移动指针时，将会看到您在“名称”框中输入的内容。在“名称”框中输入对缩放目标的简要描述，以便用户了解其可以缩放的内容。

1. 可以视情况在“用户数据”字段中输入用户数据。该字段可供网站设计人员向缩放目标中添加信息。
1. Click **[!UICONTROL Save]**.

   即可保存缩放目标的坐标和缩放级别。带有您输入的名称的缩放目标缩略图显示在屏幕右侧。

>[!NOTE]
>
>要查看缩放目标在缩放查看器中的显示效果，请单击“缩放目标编辑器”屏幕的“预览”按钮，并在“预览”屏幕中选择缩放查看器。有关该屏幕的信息，请参阅[使用不同缩放查看器预览图像](previewing-image-assets-different-zoom.md#previewing_image_assets_with_different_zoom_viewers)。

### 编辑缩放目标 {#editing-zoom-targets}

使用“缩放目标编辑器”屏幕上的这些技术编辑缩放目标：

* **重新**&#x200B;定位使用“选择目标”按钮（箭头），单击目标以选择它。 然后，将目标拖动到其他位置。

* **调整**&#x200B;大小使用“选择目标”按钮（箭头），单击目标以选择它。 然后，将指针移动到缩放目标的一角，并拖动指针以放大或缩小目标。

* **删除**&#x200B;单击屏幕右侧目标的缩略图图像。 然后单击 **[!UICONTROL 删除目标]**。

* **重命**&#x200B;名单击屏幕右侧目标的缩略图图像。 Then enter a name in the **[!UICONTROL Name]** text field and click **[!UICONTROL Save]**.

### 复制缩放目标 {#copying-zoom-targets}

可以将缩放目标从一个图像复制到另一个图像。如果两个图像的内容相似且缩放目标位于同一位置，则可复制目标。请按照以下步骤将缩放目标复制到其他图像：

1. 在“缩放目标编辑器”屏幕中打开带有要复制的缩放目标的图像。
1. 单击 **[!UICONTROL 将目标复制到]**。
1. In the Select Images dialog box, select an image and click **[!UICONTROL Select]**.

