---
title: 调整图像
description: 了解如何在Adobe Dynamic Media Classic中调整图像。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 880ee6d0-cb0a-4d53-9056-f0b8b292136e
topic: Content Management
level: Intermediate
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '571'
ht-degree: 41%

---

# 调整图像{#adjusting-an-image}

Adobe Dynamic Media Classic提供了多种用于调整图像外观的命令。 您可以翻转、旋转、模糊、更改颜色平衡和为图像着色。 在使用这些命令进行试验时，您可以在正在处理的图像上看到命令效果。

另请参阅[创建映像的别名](adjusting-image.md#creating_an_alias_for_an_image)。

**要调整图像：**

1. 选择图像的变换“编辑”按钮并选择“调整”，或者在“浏览”面板中双击该图像，使其在“详细信息视图”中打开。
1. 选择大小和图像预设（在窗口的底部）。
1. 使用`Adjust Editor`窗口右侧的命令，以便调整图像：

   * 使用“翻转”选项水平或竖直翻转图像。
   * 使用“旋转”滑块来旋转图像。您可以在“旋转”字段中输入值来旋转图像。正值顺时针旋转图像；负值逆时针旋转图像。
   * 使用“模糊”滑块或其相应的框模糊处理图像。值越高，图像越模糊。
   * 使用“对比度”、“亮度”、“饱和度”、“色相”以及“颜色平衡”选项来调整颜色和亮度。这些效果将累积。例如，对洋红色/绿色设置所做的更改将添加到对色相设置所做的更改。
   * 使用`Colorize`选项对图像进行彩色化，同时保留阴影和高光。 对“彩色化”选项所做的更改也是累积的。从“亮度”菜单中，选择&#x200B;**[!UICONTROL 无补偿]**，以便禁用自动亮度补偿。 将对比度值设置为 0 保持原始图像的对比度范围，或者指定值大于 0 的对比度范围。值 100 将使对比度最大化。典型值介于 30 到 70 之间。

1. 在完成图像调整后，执行以下操作之一：

   * 选择&#x200B;**[!UICONTROL 保存]**。

   * 要替换图像的原始图像，请选择&#x200B;**[!UICONTROL 另存为]**。

     在下拉列表中，选择&#x200B;**[!UICONTROL 替换原始]**，然后选择&#x200B;**[!UICONTROL 保存]**。

   * 要将图像另存为新主图像，请选择&#x200B;**[!UICONTROL 另存为]**。

     在下拉列表中，选择&#x200B;**[!UICONTROL 另存为新主节点]**。
在&#x200B;**[!UICONTROL 文件夹名称]**&#x200B;列表框中，选择要保存新主映像的文件夹。
选择&#x200B;**[!UICONTROL 保存]**。

   * 将图像另存为主图像的另一个视图。 您可以为其创建别名。选择&#x200B;**[!UICONTROL 另存为]**。

     从&#x200B;**[!UICONTROL 另存为]**&#x200B;对话框的下拉列表中，选择&#x200B;**[!UICONTROL 另存为主视图]**。
在&#x200B;**[!UICONTROL 文件夹名称]**&#x200B;列表框中，选择要保存新主映像的文件夹。
选择&#x200B;**[!UICONTROL 保存]**。

## 创建图像的别名 {#creating-an-alias-for-an-image}

调整图像后，可将其另存为主图像的另一个视图。 为此，您可以使用&#x200B;**[!UICONTROL 另存为主]**&#x200B;功能的另一个视图来创建图像的别名。

**为图像创建别名：**

1. 在网格视图或列表视图中，在要创建别名的图像旁边的&#x200B;**[!UICONTROL 编辑]**&#x200B;下拉列表中，选择&#x200B;**[!UICONTROL 调整]**。
1. 在页面的右下角，选择&#x200B;**[!UICONTROL 另存为]**。
1. 从&#x200B;**[!UICONTROL 另存为]**&#x200B;对话框的下拉列表中，选择&#x200B;**[!UICONTROL 另存为主视图]**。
1. 在“**[!UICONTROL 文件夹名称]**”列表框中，选择要保存已创建别名的图像的文件夹。
1. 在“**[!UICONTROL 文件名]**”字段中，键入要用作别名的名称。
1. 选择&#x200B;**[!UICONTROL 保存]**。
