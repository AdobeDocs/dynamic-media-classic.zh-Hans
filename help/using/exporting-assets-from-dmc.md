---
title: 从Adobe Dynamic Media Classic导出资源
description: 了解如何从Adobe Dynamic Media Classic导出资源。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 5e3b0002-5ae2-4437-862f-caa098b04362
topic: Content Management
level: Intermediate
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 38%

---

# 从Adobe Dynamic Media Classic导出资源{#exporting-assets-from-dmc}

您可以将在Adobe Dynamic Media Classic中编辑的资源保存到本地网络驱动器。 导出的资源会打包成一个 Zip 文件，供下载或通过电子邮件发送。

可用于导出作业的 Zip 压缩文件的最大文件大小为 1 GB。此外，每个导出作业最多允许500个总资产。

Adobe Dynamic Media Classic会保留“作业”屏幕中导出作业的记录。

**要从Adobe Dynamic Media Classic导出资源：**

1. 选择要导出的资源，然后转到&#x200B;**[!UICONTROL 文件]** > **[!UICONTROL 导出]**。
1. 在“导出所选资源”窗口中，单击“**[!UICONTROL 图像选项]**”，然后指定以下任一选项（管理员可确定哪些选项对用户可用）：

   * **[!UICONTROL 预设]**： （可选）选择图像预设，以便在导出资产时设置资产的格式。 如果选择了图像预设，其他格式选项将不可用，因为资源会采用由图像预设定义的格式。

   * **[!UICONTROL 转换]**：转换资源文件或原始图像。

   * **[!UICONTROL 大小]**：您可以选择标准大小。 或者，您可以从&#x200B;**[!UICONTROL 大小]**&#x200B;下拉列表中选择&#x200B;**[!UICONTROL 其他]**，选择所需的度量单位，然后指定宽度和高度。

     另请参阅[指定Media Portal用户可用的导出选项](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users)。

   * **[!UICONTROL 格式]**：选择图像格式。

   * **[!UICONTROL 颜色]**：选择RGB、CMYK或灰色。

   * **[!UICONTROL 分辨率]**：选择72 ppi、150 ppi或300 ppi。

   * **[!UICONTROL 作业名称]**：您可以为导出分配作业名称。

   * **[!UICONTROL 将电子邮件发送至]**：可选。 如果打算通过电子邮件发送资产，请输入电子邮件地址。 电子邮件会列出收件人可从中下载资源的 URL。

1. 选择&#x200B;**[!UICONTROL 导出]**。

系统支持以下三种基本导出操作：

* 原始文件（导出资源的原始文件）
* 使用预设进行转换（使用图像预设设置资产的格式）
* 无预设转换（使用导出对话框来指定图像修饰符）

无法导出下列资源类型。其他所有规则均生成导出。

* 图像集
* 渲染集
* 旋转集
* 媒体集
* 多比特率集
* eCatalog

此外，模板不能导出为“原始文件”。

可以使用转换导出以下资源类型：

* 图像
* 模板
* 已调整图像
* PDF（生成转换的页面）
* PostScript®

当大量各种各样的资源类型进入导出程序时，会出现以下行为结果：

* 在作业提交之前，将从列表中删除所有无法导出的资源类型
* 如果请求转换，则所有可转换的类型都将被导出，所有其他类型都将导出为原始类型
