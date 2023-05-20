---
title: 從Adobe Dynamic Media Classic匯出資產
description: 瞭解如何從Adobe Dynamic Media Classic匯出資產。
uuid: d42b7a73-80c0-4a9a-a04e-7ef53e6fcf22
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: eb850ec7-a669-41ea-b2b0-4c9178e34f95
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 5e3b0002-5ae2-4437-862f-caa098b04362
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '432'
ht-degree: 51%

---

# 從Adobe Dynamic Media Classic匯出資產{#exporting-assets-from-dmc}

您可以將在Adobe Dynamic Media Classic中編輯的資產儲存至本機網路磁碟機。 导出的资源会打包成一个 Zip 文件，供下载或通过电子邮件发送。

可用于导出作业的 Zip 压缩文件的最大文件大小为 1 GB。此外，每個匯出工作最多允許500個總資產。

Adobe Dynamic Media Classic會在「工作」畫面中保留匯出工作的記錄。

**若要從Adobe Dynamic Media Classic匯出資產：**

1. 選取您要匯出的資產，然後前往 **[!UICONTROL 檔案]** > **[!UICONTROL 匯出]**.
1. 在“导出所选资源”窗口中，单击“**[!UICONTROL 图像选项]**”，然后指定以下任一选项（管理员可确定哪些选项对用户可用）：

   * **[!UICONTROL 預設集]**  — 或者，選擇影像預設集，在匯出資產時將其格式化。 如果选择了图像预设，其他格式选项将不可用，因为资源会采用由图像预设定义的格式。

   * **[!UICONTROL 轉換]**  — 轉換資產檔案或原始影像。

   * **[!UICONTROL 大小]**  — 您可以選取標準大小。 或者，您可以選取 **[!UICONTROL 其他]** 從 **[!UICONTROL 大小]** 下拉式清單，選擇所需的測量單位，然後指定寬度和高度。

      另請參閱 [指定Media Portal使用者可用的匯出選項](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users).

   * **[!UICONTROL 格式]**  — 選擇影像格式。

   * **[!UICONTROL 顏色]**  — 選擇「RGB」、「CMYK」或「灰色」。

   * **[!UICONTROL 解析度]**  — 選擇72 ppi、150 ppi或300 ppi。

   * **[!UICONTROL 工作名稱]**  — 您可以為匯出指派工作名稱。

   * **[!UICONTROL 傳送電子郵件至]**  — 如果您打算透過電子郵件傳送資產，可選擇輸入電子郵件地址。 电子邮件会列出收件人可从中下载资源的 URL。

1. 選取 **[!UICONTROL 匯出]**.

系统支持以下三种基本导出操作：

* 原始文件（导出资源的原始文件）
* 使用预设转换（使用图像预调为资源设置格式）
* 无预设转换（使用导出对话框来指定图像修饰符）

无法导出下列资源类型。所有其他會產生匯出。

* 图像集
* 渲染集
* 旋转集
* 媒体集
* 多位元速率集
* eCatalog

此外，也无法作为“原始文件”导出模板。

可以使用转换导出以下资源类型：

* 图像
* 模板
* 已调整图像
* PDF（產生轉換的頁面）
* PostScript®

当大量各种各样的资源类型进入导出程序时，会出现以下行为结果：

* 在提交作业之前会从列表中移除无法导出的所有资源类型
* 如果请求了转换，则能够转换的所有类型以及所有其他类型都按原样导出
