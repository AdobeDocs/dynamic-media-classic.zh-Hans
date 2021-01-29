---
title: 从Dynamic Media经典导出资产
description: 了解如何从Dynamic Media经典中导出资产。
uuid: d42b7a73-80c0-4a9a-a04e-7ef53e6fcf22
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: eb850ec7-a669-41ea-b2b0-4c9178e34f95
translation-type: tm+mt
source-git-commit: ca12c96d3a76cfa52fd930d190476cb6fc4f4ac7
workflow-type: tm+mt
source-wordcount: '424'
ht-degree: 70%

---


# 从Dynamic Media经典导出资源{#exporting-assets-from-dmc}

您可以将在Dynamic Media经典中编辑的资源保存到本地网络驱动器。 导出的资源会打包成一个 Zip 文件，供下载或通过电子邮件发送。

可用于导出作业的 Zip 压缩文件的最大文件大小为 1 GB。另外，请注意，每个导出作业最多允许有 500 个总资源。

Dynamic Media·经典在“工作”屏幕中保留了出口工作记录。

**从Dynamic Media经典出口资产**

1. 选择要导出的资源，然后单击“**文件**”>“**导出**”。
1. 在“导出所选资源”窗口中，单击“**图像选项**”，然后指定以下任一选项（管理员可确定哪些选项对用户可用）：

   * **预**
设（可选）在导出资产时，选择图像预设以设置资产的格式。如果选择了图像预设，其他格式选项将不可用，因为资源会采用由图像预设定义的格式。

   * **转**
换转换资产文件或原始图像。

   * **大**
小您可以选择标准大小。您也可以从“大小”下拉列表中单击“其他”，选择所需的度量单位，然后指定宽度和高度。

      另请参见[指定 Media Portal 用户可以使用的导出选项](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users)。

   * **格**
式选择图像格式。

   * **颜**
色选择RGB、CMYK或灰色。

   * **分**
辨率选择72、150或300 ppi。

   * **作业**
名称您可以为导出分配作业名称。

   * **发送电**
子邮件至（可选）输入电子邮件地址，以通过电子邮件发送资产。电子邮件会列出收件人可从中下载资源的 URL。

1. 单击“**导出**”。

系统支持以下三种基本导出操作：

* 原始文件（导出资源的原始文件）
* 使用预设转换（使用图像预调为资源设置格式）
* 无预设转换（使用导出对话框来指定图像修饰符）

无法导出下列资源类型。所有其他类型应该都能生成导出。

* 图像集
* 渲染集
* 旋转集
* 媒体集
* 多比特率集
* eCatalog

此外，也无法作为“原始文件”导出模板。

可以使用转换导出以下资源类型：

* 图像
* 模板
* 已调整图像
* PDF（将生成转换页）
* PostScript

当大量各种各样的资源类型进入导出程序时，会出现以下行为结果：

* 在提交作业之前会从列表中移除无法导出的所有资源类型
* 如果请求了转换，则能够转换的所有类型以及所有其他类型都按原样导出

