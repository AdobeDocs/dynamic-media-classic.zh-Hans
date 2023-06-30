---
title: 调整图像
description: 了解如何在Adobe Dynamic Media Classic中调整图像。
uuid: c052acd3-e8c1-4134-ad21-b9c41578097f
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 47a23980-2886-4da3-ab2d-6cd50e00d188
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 880ee6d0-cb0a-4d53-9056-f0b8b292136e
topic: Content Management
level: Intermediate
source-git-commit: d82f816553f807b514f4690827dab672a6baf690
workflow-type: tm+mt
source-wordcount: '565'
ht-degree: 52%

---

# 调整图像{#adjusting-an-image}

Adobe Dynamic Media Classic提供了各种用于调整图像外观的命令。 您可以翻转、旋转、模糊处理、更改颜色平衡，以及为图像着色。在使用这些命令进行试验时，您可以在正在处理的图像上看到命令效果。

另请参阅 [为图像创建别名](adjusting-image.md#creating_an_alias_for_an_image).

**要调整图像，请执行以下操作：**

1. 选择图像的变换“编辑”按钮并选择“调整”，或者在“浏览”面板中双击该图像，使其在“详细信息视图”中打开。
1. 选择大小和图像预设（在窗口的底部）。
1. 使用“调整编辑器”窗口右侧的命令来调整图像：

   * 使用“翻转”选项水平或竖直翻转图像。
   * 使用“旋转”滑块来旋转图像。您可以在“旋转”字段中输入值来旋转图像。正值顺时针旋转图像；负值逆时针旋转图像。
   * 使用“模糊”滑块或其相应的框模糊处理图像。值越高，图像越模糊。
   * 使用“对比度”、“亮度”、“饱和度”、“色相”以及“颜色平衡”选项来调整颜色和亮度。这些效果将累积。例如，对洋红色/绿色设置所做的更改将添加到对色相设置所做的更改。
   * 使用“彩色化”选项给图像着色，同时保留阴影和高亮。对“彩色化”选项所做的更改也是累积的。从“亮度”菜单中，选择 **[!UICONTROL 无补偿]** 因此禁用自动亮度补偿。 将对比度值设置为 0 保持原始图像的对比度范围，或者指定值大于 0 的对比度范围。值 100 将使对比度最大化。典型值在30-70范围内。

1. 在完成图像调整后，执行以下操作之一：

   * 选择 **[!UICONTROL 保存]**.

   * 要替换图像的原始图像，请选择 **[!UICONTROL 另存为]**.

     在下拉列表中，选择 **[!UICONTROL 替换原始]**，然后选择 **[!UICONTROL 保存]**.

   * 要将图像另存为新的主控图像，请选择 **[!UICONTROL 另存为]**.

     在下拉列表中，选择“**[!UICONTROL 另存为新的主图像]**”。在 **[!UICONTROL 文件夹名称]** 列表框中，选择要保存新主映像的文件夹。
选择 **[!UICONTROL 保存]**.

   * 将图像另存为主图像的另一个视图。 您可以为其创建别名。选择 **[!UICONTROL 另存为]**.

     在 **[!UICONTROL 另存为]** 对话框中，在下拉列表中选择 **[!UICONTROL 另存为另一个主控视图]**.
在 **[!UICONTROL 文件夹名称]** 列表框中，选择要保存新主映像的文件夹。
选择 **[!UICONTROL 保存]**.

## 为图像创建别名 {#creating-an-alias-for-an-image}

调整图像后，可将其另存为主图像的另一个视图。 为此，您可以为该图像创建别名，方法是使用“**[!UICONTROL 另存为主图像的其他视图]**”功能。

**要为图像创建别名，请执行以下操作：**

1. 在网格视图或列表视图中，在 **[!UICONTROL 编辑]** 要为其创建别名的图像旁边的下拉列表，选择 **[!UICONTROL Adjust]**.
1. 在页面的右下角，选择 **[!UICONTROL 另存为]**.
1. 在 **[!UICONTROL 另存为]** 对话框中，在下拉列表中选择 **[!UICONTROL 另存为主控的附加视图]**.
1. 在“**[!UICONTROL 文件夹名称]**”列表框中，选择要保存已创建别名的图像的文件夹。
1. 在“**[!UICONTROL 文件名]**”字段中，键入要用作别名的名称。
1. 选择 **[!UICONTROL 保存]**.
