---
title: 设置图像预设
description: 了解如何在Adobe Dynamic Media Classic中设置图像预设。
uuid: 90530948-dee9-41bd-b39e-684140446abc
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
discoiquuid: 1ec39fe5-7b2a-4034-9570-6b5595f97052
feature: Dynamic Media Classic,Image Presets
role: User
exl-id: 336802cc-b032-49b2-b2e6-d699bc997ee5
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '659'
ht-degree: 50%

---

# 设置图像预设{#setting-up-image-presets}

像宏一样，图像预设是用某个名称保存的一组预定义大小和格式命令。要了解图像预设的工作方式，请假设您的网站要求每个产品图像以两种不同的大小显示：500 x 500像素和150 x 150像素。 您创建了两个图像预设，一个称为“放大”，以 500 x 500 像素显示图像，另一个称为“缩略图”，以 150 x 150 像素显示图像。为了投放大小为“放大”和“缩略图”的图像，Dynamic Media图像服务器查找放大图像预设和缩略图图像预设的定义。 然后，服务器按每个图像预设的大小和格式规范动态生成图像。

Adobe Dynamic Media Classic附带了几个“最佳实践”图像预设，这些预设已设置好供您使用。 管理员也可以创建图像预设。 要创建图像预设，您可以从头开始，也可以使用现有的图像预设进行创建，然后用新名称进行保存。

从服务器动态传送图像时，对于大小有所缩减的图像，其清晰度和细节可能会有些损失。因此，每个图像预设都包含格式控制，用于优化以特定大小进行传送的图像。这些控制可确保传送至网站或应用程序的图像清晰可辨。

## 创建图像预设 {#creating-an-image-preset}

如果您是公司的管理员，则可以创建自己的图像预设。您可以创建图像预设，也可以从Adobe Dynamic Media Classic提供的默认图像预设开始，对其进行编辑并以新名称保存。

**创建图像预设:**

1. 转到 **[!UICONTROL 设置]** > **[!UICONTROL 图像预设]**.

   可以在该屏幕上浏览至一个图像预设名称来预览现有的图像预设。在选择图像预设名称时，预览窗口中示例图像的大小和外观会发生更改。

1. 执行以下任一操作：

   * **创建图像预设**  — 选择 **[!UICONTROL 添加]**.
   * **编辑图像预设**  — 浏览到与要创建的图像预设最相似的图像预设，然后选择 **[!UICONTROL 编辑]**.

1. 输入图像预设的名称。
1. 输入宽和高的像素数。这些数字确定了所传送图像的大小。
1. 填写“添加预设”或“编辑预设”屏幕。有关详细信息，请参阅[图像预设选项](application-setup.md#image_preset_options)。

   Adobe Dynamic Media Classic建议从以下“最佳实践”选项开始：

   * **[!UICONTROL 格式]**  — 选择JPEG或其它符合您要求的格式。 所有 Web 浏览器都支持 JPEG 图像格式；这种格式在小文件大小与图像质量之间取得了良好平衡。然而，JPEG 格式图像使用了有损压缩模式，如果压缩设置过低，可能会产生多余的图像伪影。因此，Adobe Dynamic Media Classic建议将压缩质量（在滑块上）设置为75。 该设置在图像质量与小文件大小之间取得了良好平衡。

   * **[!UICONTROL 锐化]**  — 请勿选择锐化(此锐化滤镜提供的控制力低于 **[!UICONTROL 钝化蒙版]** 设置)。

   * **[!UICONTROL 重新采样模式]**  — 选择 **[!UICONTROL 双三次]**.

   * **[!UICONTROL 钝化蒙版]** (USM) — 输入以下设置：

   | 预设类型 | 大小 | USM：数量 | USM：半径 | USM：阈值 |
   | --- | --- | --- | --- | --- |
   | 交叉销售（微型缩略图） | 75 x 75 | 1.5 | 0.8 | 5 |
   | 缩略图 | 150 x 150 | 1.1 | 1 | 5 |
   | 主图像 | 350 x 350 | 1 | 1 | 6 |
   | 放大 | 500 x 500 | 1.2 | 1.2 | 5 |

1. 选择 **[!UICONTROL 保存]**.

此处列出的用于创建图像预设的Adobe Dynamic Media Classic“最佳实践”选项是一般建议；锐化操作具有高度主观性。 这些“最佳实践”设置基于2000 x 2000主映像；较大或较小的主文件的设置可能不同。 如果要调整“钝化蒙版”设置，Adobe Dynamic Media Classic建议使用这些范围：

* **[!UICONTROL 金额]**  — 介于。8和1.5之间。

* **[!UICONTROL 半径]**  — 介于。6和2之间。

* **[!UICONTROL 阈值]**  — 从1到6。

要删除图像预设，请在“图像预设”屏幕上选择它，然后选择 **[!UICONTROL 删除]**.

>[!MORELIKETHIS]
>
>* [创建并编辑图像预设](application-setup.md#creating_and_editing_image_presets)
>* [图像预设选项](application-setup.md#image_preset_options)
>* [预览基于其图像预设的图像资源](previewing-asset.md#previewing_an_image_asset_based_on_its_image_preset)

