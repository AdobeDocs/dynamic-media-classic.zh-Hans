---
title: 个人设置
description: 所有用户都可以更改Dynamic Media Classic的“个人设置”屏幕上的设置。
uuid: 29cb825a-f158-4a1e-9d5f-7636ee411b6e
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/setup
discoiquuid: 6314e7b7-5bde-4fe2-8674-e4fc525d4d1c
feature: Dynamic Media Classic
role: Administrator,Business Practitioner
exl-id: a019f973-7647-466f-8af3-5312e9225e89
translation-type: tm+mt
source-git-commit: c4e2b8b42b56420269087d0d4f262490464270c0
workflow-type: tm+mt
source-wordcount: '819'
ht-degree: 28%

---

# 个人设置 {#personal-setup}

所有用户都可以更改“个人设置”屏幕中的设置。要打开“个人设置”屏幕，请单击“设置”>“个人设置”。

>[!NOTE]
>
>“个人设置”屏幕列表您在Dynamic Media Classic中具有的用户角色：公司管理员、管理员或用户。

“个人设置”设置控制浏览面板的默认行为、您接收电子邮件的方式以及密码设置。在更改这些设置之后，请记住单击“保存”。

## 我的帐户信息

标识您的帐户名称、名称、用户名（电子邮件地址）和指定的用户角色。

## 桌面

* **清除图像缓存**  — 从您的计算机中删除所有Adobe Dynamic Media缓存的图像文件。
* **清除资产缓存**  — 从您的计算机中删除所有Adobe Dynamic Media缓存资产文件。

除了使用桌面应用程序清除图像和资产缓存外，您还可以直接从文件系统手动清除缓存。 根据您的操作系统，导航到以下内容：

* macOS:`~/Library/Application\ Support/com.adobe.DMCDesktop/Local\ Store/`
* Windows®: `C:\Users\YourUserName\AppData\Roaming\com.adobe.DMCDesktop\Local Store`

## Creative Suite Extension

**安装Adobe Dynamic Media Creative Suite扩展：**

1. 在Dynamic Media Classic的工具栏中，单击&#x200B;**[!UICONTROL Setup]** > **[!UICONTROL Personal Setup]**，在“Creative Suite扩展”下，单击&#x200B;**[!UICONTROL Download Now]**&#x200B;以下载`s7csxs.zxp`文件。
1. 单击&#x200B;**[!UICONTROL 安装]**&#x200B;和&#x200B;**[!UICONTROL 系统要求]**&#x200B;链接，以了解有关该扩展的其他信息。

<!--    A readme file is included at the root of the unzipped file to provide you with additional information about the extension.

1. Depending on your installed operating system, do one of the following: -->

<!-- #### Windows

|If you are running|Do this|
|--- |--- |
|Adobe Illustrator 18 in Adobe Creative Cloud 2014|<ul><li>From the root of the unzipped folder, click CC-2014.</li><li>Depending on the bit version of Adobe Illustrator that you are using, click win32 or win64.</li><li>Click libraries > flame, and then copy `aflame.dll` to Adobe Illustrator's executable folder. For example, `C:\Program Files\Adobe\Adobe Illustrator CC 2014\Support Files\Contents\Windows`. </li></ul><br/>**Note**: This example path is for the 64-bit location; the 32-bit location may fall under Program Files (x86) instead. <br/><ul><li>Return to the same libraries folder, click flamingo, and then copy `aflamingo.dll` to the same Adobe Illustrator executable folder that you used in the previous step. </li><li>Return to the win32 or win64 folder that you selected in step 2, and then copy `AdobeS7FXGFileFormat.aip` to Adobe Illustrator's plug-ins folder. For example, `C:\Program Files\Adobe\Adobe Illustrator CC 2014\Plug-ins\Illustrator Formats`. </li></ul> <br/>**Note**: This example path is for the 64-bit location; the 32-bit location may fall under Program Files (x86) instead.|
|Adobe Illustrator 17 in Adobe Creative Cloud|<ul><li>From the root of the unzipped folder, click CC. </li><li>Depending on the bit version of Adobe Illustrator that you are using, click win32 or win64.</li><li> Copy `AdobeS7FXGFileFormat.aip` to Adobe Illustrator's plug-ins folder. For example, `C:\Program Files\Adobe\Adobe Illustrator CC (64 Bit)\Plug-ins\Illustrator Formats`.</li></ul><br/>**Note**: This example path is for the 64-bit location; the 32-bit location may fall under Program Files (x86) instead.|
|Adobe Illustrator 16 in Adobe Creative Suite 6|<ul><li>From the root of the unzipped folder, click 6.0. </li><li>Depending on the bit version of Adobe Illustrator that you are using, click win32 or win64. </li><li>Copy AdobeS7FXGFileFormat.aip to Adobe Illustrator's plug-ins folder. For example, `C:\Program Files\Adobe\Adobe Illustrator CS6 (64 Bit)\Plug-ins\Illustrator Formats`.</li></ul><br/>**Note**: This example path is for the 64-bit location; the 32-bit location may fall under Program Files (x86) instead.|

#### Mac

|If you are running|Do this|
|--- |--- |
|Adobe Illustrator 18 in Adobe Creative Cloud 2014|<ul><li>From the root of the unzipped folder, click CC-2014 > mac64.</li><li>Click libraries > flame, and then copy the `aflame.framework` folder to Adobe Illustrator package contents folder. For example, `/Applications/Adobe Illustrator CC 2014/ Illustrator.app/Contents/Frameworks/`. (To open Adobe Illustrator’s package contents folder, right-click on the Adobe illustrator CC 2014 icon and click Show Package Contents from context menu).</li><li>Return to the same libraries folder, click `flamingo`, and then copy the `aflamingo.framework` folder to the same Adobe Illustrator package contents folder that you used in the previous step.</li><li>Return to the mac64 folder that you selected in step 1, and then copy the `AdobeS7FXGFileFormat.aip` folder to Adobe Illustrator’s plug-in folder. For example, `/Applications/Adobe Illustrator CC 2014/Plug-ins/Illustrator Formats/`.</li></ul><br/>|
|Adobe Illustrator 17 in Adobe Creative Cloud|<ul><li>From the root of the unzipped folder, click CC > mac64</li><li>Copy the `AdobeS7FXGFileFormat.aip` folder to Adobe Illustrator’s plug-in folder. For example, `/Applications/Adobe Illustrator CC/Plug-ins/Illustrator Formats/`.</li></ul><br/>|
|Adobe Illustrator 16 in Adobe Creative Suite 6|<ul><li>From the root of the unzipped folder, click 6.0 > mac64</li><li>Copy the `AdobeS7FXGFileFormat.aip` folder to Adobe Illustrator’s plug-in folder. For example, `/Applications/Adobe Illustrator CS6/Plug-ins/Illustrator Formats/`.</li></ul>|

The plug-in is now available for you to use in Adobe Illustrator. -->

## 浏览器

* **缩览图大小**  — 在浏览面板的网格视图中确定缩览图图像的默认大小。
* **默认资源库视图**  — 确定构建集的资源库中的资源是显示为缩略图还是按名称显示。如果要处理资源库中的大量资源，可以按名称查看资源。例如，如果要使用许多 PDF 文件构建较大的 eCatalog，可以按名称查看资源，以使列表变得简短。
* **默认浏览排序顺序**  — 确定默认情况下资源在浏览面板中的显示顺序。在菜单中选择排序条件，并选择是升序排序还是降序排序。
* **默认浏览位置**  — 允许您将浏览位置设置为默认位置、最后浏览的文件夹或您导航到并标识的特定位置。还可以将浏览位置设置为按升序或降序排序文件和文件夹。
* **默认浏览视图**  — 确定首次打开“浏览”面板时显示的默认视图是“网格视图”还是“列表视图”。
* **初始屏幕显示**  — 确定是否看到任何初始屏幕，包括欢迎初始屏幕。
* **显示工具提示**  — 确定将指针移到按钮、菜单和导航链接上时是否显示工具提示。工具提示描述屏幕上的用户界面项。
* **棋盘背景**  — 在图像后面显示一个棋盘图层，使您能够轻松查看具有Alpha渠道的图像的透明区域。
* **显示文件大小**  — 在您浏览时显示资产的文件大小。
* **在搜索中包括UDF**  — 要提高您运行的大多数元数据搜索的系统性能，请取消选择（默认）。

   如果包括用户定义的字段对于您的大部分元数据搜索有帮助，您可以选择此选项以将其打开。或者可以使用高级搜索，与包括用户定义的字段相比，这种方式可以提供更直接、更快速的搜索体验。

   请参阅[实施高级搜索](searching-assets.md#conducting_an_advanced_search)。

   另请参阅[用户定义的字段](application-setup.md#user_defined_fields)。

* **基本搜索类型**  — 您可以从以下两个选项中进行选择： **[!UICONTROL 容]** 器搜索指定值的完整字符串； **[!UICONTROL Starts]** With从字符串的开头搜索，并返回比Contains更快的 **[!UICONTROL 结果]**。任一选项都将覆盖管理员在&#x200B;**[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Application General Settings]**&#x200B;中设置的默认值。
* **显示命令反馈**  — 选择此项可开启显示命令请求至服务器；取消选择可关闭。
* **导出期间显示** 对话框 — 选择此选项可在导出期间显示弹出对话框。如果取消选择（关闭）此选项，您仍可转到“作业”页以检索导出结果。

## 电子邮件

* **电子邮件选项**  — 选择您希望Dynamic Media Classic在上载和发布作业完成时通过电子邮件通知您的方式。可以选择仅当发生警告或错误时接收作业完成通知。
* **电子邮件范围**  — 确定您是接收公司的所有作业电子邮件，还是仅接收有关您启动的上载和发布作业的电子邮件。
* **电子邮件类型**  — 确定在上载作业和发布作业完成时是否已通知您。

## 语言

* **首选语言**  — 确定要用于该界面的语言。

## 密码

* **当前密码**  — 输入您当前密码的密码。
* **新密码**  — 输入新的有效密码。您的密码必须满足以下要求：
   * 长度为8-25个字符。
   * 至少包含一个小写字母。
   * 至少包含一个大写字母。
   * 至少包含一个数字。
   * 至少包含下列特殊字符之一：`# $ & - _ : { }`
* **重新键入密码**  — 重新输入新密码以确认输入正确。
* **密码过期**  — 确定密码在72天后是否过期作为安全措施。如果选择“是”，则会在 72 天之后要求您创建新密码。
