---
title: 个人设置
description: 所有用户都可以在Adobe Dynamic Media Classic的“个人设置”屏幕上更改设置。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/setup
feature: Dynamic Media Classic
role: Admin,User
exl-id: a019f973-7647-466f-8af3-5312e9225e89
topic: Administration, Collaboration
level: Intermediate
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '830'
ht-degree: 19%

---

# 个人设置 {#personal-setup}

所有用户都可以更改“个人设置”屏幕中的设置。要打开“个人设置”屏幕，请转到&#x200B;**[!UICONTROL 设置]** > **[!UICONTROL 个人设置]**。

>[!NOTE]
>
>“个人设置”屏幕列出您在Adobe Dynamic Media Classic中的用户角色：公司管理员、管理员或用户。

“个人设置”设置控制“浏览”面板的默认行为、接收电子邮件的方式和密码设置。 更改这些设置后，请记得选择&#x200B;**[!UICONTROL 保存]**。

## 我的帐户信息

标识您的帐户名称、名称、用户名（电子邮件地址）和指定的用户角色。

## 桌面

* **清除图像缓存**：从您的计算机中删除所有Adobe Dynamic Media缓存的图像文件。
* **清除资源缓存**：从您的计算机中删除所有Adobe Dynamic Media缓存资源文件。

除了使用桌面应用程序清除图像和资产缓存之外，您还可以直接从文件系统手动清除缓存。 根据您的操作系统，导航至以下内容：

* macOS： `~/Library/Application\ Support/com.adobe.DMCDesktop/Local\ Store/`
* Windows®： `C:\Users\YourUserName\AppData\Roaming\com.adobe.DMCDesktop\Local Store`

## Creative Suite Extension

**要安装Adobe Dynamic Media Creative Suite扩展，请执行以下操作：**

1. 在Adobe Dynamic Media Classic的工具栏上，转到&#x200B;**[!UICONTROL 设置]** > **[!UICONTROL 个人设置]**，在Creative Suite Extension下，选择&#x200B;**[!UICONTROL 立即下载]**&#x200B;以下载`s7csxs.zxp`文件。
1. 选择&#x200B;**[!UICONTROL 安装]**&#x200B;和&#x200B;**[!UICONTROL 系统要求]**&#x200B;链接以获取有关扩展的其他信息。

<!--    A readme file is included at the root of the unzipped file to provide you with additional information about the extension.

1. Depending on your installed operating system, do one of the following: -->

<!-- #### Windows

|If you are running|Do this|
|--- |--- |
|Adobe Illustrator 18 in Adobe Creative Cloud 2014|<ul><li>From the root of the unzipped folder, select CC-2014.</li><li>Depending on the bit version of Adobe Illustrator that you are using, select win32 or win64.</li><li>Select libraries > flame, and then copy `aflame.dll` to Adobe Illustrator's executable folder. For example, `C:\Program Files\Adobe\Adobe Illustrator CC 2014\Support Files\Contents\Windows`. </li></ul><br/>**Note**: This example path is for the 64-bit location; the 32-bit location may fall under Program Files (x86) instead. <br/><ul><li>Return to the same libraries folder, select flamingo, and then copy `aflamingo.dll` to the same Adobe Illustrator executable folder that you used in the previous step. </li><li>Return to the win32 or win64 folder that you selected in step 2, and then copy `AdobeS7FXGFileFormat.aip` to Adobe Illustrator's plug-ins folder. For example, `C:\Program Files\Adobe\Adobe Illustrator CC 2014\Plug-ins\Illustrator Formats`. </li></ul> <br/>**Note**: This example path is for the 64-bit location; the 32-bit location may fall under Program Files (x86) instead.|
|Adobe Illustrator 17 in Adobe Creative Cloud|<ul><li>From the root of the unzipped folder, select CC. </li><li>Depending on the bit version of Adobe Illustrator that you are using, select win32 or win64.</li><li> Copy `AdobeS7FXGFileFormat.aip` to Adobe Illustrator's plug-ins folder. For example, `C:\Program Files\Adobe\Adobe Illustrator CC (64 Bit)\Plug-ins\Illustrator Formats`.</li></ul><br/>**Note**: This example path is for the 64-bit location; the 32-bit location may fall under Program Files (x86) instead.|
|Adobe Illustrator 16 in Adobe Creative Suite 6|<ul><li>From the root of the unzipped folder, select 6.0. </li><li>Depending on the bit version of Adobe Illustrator that you are using, select win32 or win64. </li><li>Copy AdobeS7FXGFileFormat.aip to Adobe Illustrator's plug-ins folder. For example, `C:\Program Files\Adobe\Adobe Illustrator CS6 (64 Bit)\Plug-ins\Illustrator Formats`.</li></ul><br/>**Note**: This example path is for the 64-bit location; the 32-bit location may fall under Program Files (x86) instead.|

#### Mac

|If you are running|Do this|
|--- |--- |
|Adobe Illustrator 18 in Adobe Creative Cloud 2014|<ul><li>From the root of the unzipped folder, select CC-2014 > mac64.</li><li>Select libraries > flame, and then copy the `aflame.framework` folder to Adobe Illustrator package contents folder. For example, `/Applications/Adobe Illustrator CC 2014/ Illustrator.app/Contents/Frameworks/`. (To open Adobe Illustrator's package contents folder, right-select on the Adobe illustrator CC 2014 icon and select Show Package Contents from context menu).</li><li>Return to the same libraries folder, select `flamingo`, and then copy the `aflamingo.framework` folder to the same Adobe Illustrator package contents folder that you used in the previous step.</li><li>Return to the mac64 folder that you selected in step 1, and then copy the `AdobeS7FXGFileFormat.aip` folder to Adobe Illustrator's plug-in folder. For example, `/Applications/Adobe Illustrator CC 2014/Plug-ins/Illustrator Formats/`.</li></ul><br/>|
|Adobe Illustrator 17 in Adobe Creative Cloud|<ul><li>From the root of the unzipped folder, select CC > mac64</li><li>Copy the `AdobeS7FXGFileFormat.aip` folder to Adobe Illustrator's plug-in folder. For example, `/Applications/Adobe Illustrator CC/Plug-ins/Illustrator Formats/`.</li></ul><br/>|
|Adobe Illustrator 16 in Adobe Creative Suite 6|<ul><li>From the root of the unzipped folder, select 6.0 > mac64</li><li>Copy the `AdobeS7FXGFileFormat.aip` folder to Adobe Illustrator's plug-in folder. For example, `/Applications/Adobe Illustrator CS6/Plug-ins/Illustrator Formats/`.</li></ul>|

The plug-in is now available for you to use in Adobe Illustrator. -->

## 浏览器

* **[!UICONTROL 缩略图大小]**：确定“浏览”面板中网格视图的缩略图图像的默认大小。
* **[!UICONTROL 默认资源库视图]**：确定生成集的资源库中的资源是显示为缩略图还是按名称显示。 如果要处理资源库中的大量资源，可以按名称查看资源。例如，如果要使用许多 PDF 文件构建较大的 eCatalog，可以按名称查看资源，以使列表变得简短。
* **[!UICONTROL 默认浏览排序顺序]**：确定资源在浏览面板中的默认显示顺序。 在菜单中选择排序条件，并选择是升序排序还是降序排序。
* **[!UICONTROL 默认浏览位置]**：用于将浏览位置设置为默认位置、上次浏览的文件夹或您导航并识别的特定位置。 还可以将浏览位置设置为按升序或降序排序文件和文件夹。
* **[!UICONTROL 默认浏览视图]**：确定网格视图还是列表视图是您首次打开“浏览”面板时看到的默认视图。
* **[!UICONTROL 启动画面显示]**：确定您是否看到任何启动画面，包括欢迎启动画面。
* **[!UICONTROL 显示工具提示]**：确定在按钮、菜单和导航链接上移动指针时是否显示工具提示。 工具提示描述屏幕上的用户界面项。
* **[!UICONTROL 棋盘格背景]**：在图像后面显示棋盘格图层，以便您轻松查看具有Alpha通道的图像的透明区域。
* **[!UICONTROL 显示文件大小]**：在浏览时显示资源的文件大小。
* **[!UICONTROL 在搜索中包含UDF]**：为了提高您运行的大多数元数据搜索的系统性能，请取消选择（默认）。

  如果包括用户定义的字段对于您的大部分元数据搜索有帮助，您可以选择此选项以将其打开。作为替代方法，使用高级搜索可提供比包含用户定义的字段更直接、更快的搜索体验。

  请参阅[实施高级搜索](searching-assets.md#conducting_an_advanced_search)。

  另请参阅[用户定义的字段](application-setup.md#user_defined_fields)。

* **[!UICONTROL 基本搜索类型]**：您可以从两个选项中进行选择：**[!UICONTROL 包含]**&#x200B;搜索指定值的完整字符串；**[!UICONTROL StartsWith]**&#x200B;从字符串的开头开始搜索并返回比&#x200B;**[!UICONTROL 包含]**&#x200B;更快的结果。 任一选项都会覆盖管理员在&#x200B;**[!UICONTROL 设置]** > **[!UICONTROL 应用程序设置]** > **[!UICONTROL 应用程序常规设置]**&#x200B;中设置的默认值。
* **[!UICONTROL 显示命令反馈]**：选择以打开对服务器的命令请求的显示；取消选择以关闭。
* 导出期间&#x200B;**[!UICONTROL 显示对话框]**：选择此项可在导出期间显示弹出对话框。 如果取消选择（关闭）此选项，您仍可以转到“作业”页面检索导出结果。

## 电子邮件

* **[!UICONTROL 电子邮件选项]**：选择您希望Adobe Dynamic Media Classic在上载和发布作业完成后通过电子邮件通知您的方式。 可以选择仅当发生警告或错误时接收作业完成通知。
* **[!UICONTROL 电子邮件范围]**：确定您是收到公司的所有工作电子邮件，还是只收到有关上载和发布您启动的工作的电子邮件。
* **[!UICONTROL 电子邮件类型]**：确定完成上载作业和发布作业时是否通知您。

## 语言

* **[!UICONTROL 首选语言]**：确定您要用于界面的语言。

## 密码

* **[!UICONTROL 当前密码]**：输入您当前密码的密码。
* **[!UICONTROL 新密码]**：输入新的有效密码。 您的密码必须满足以下要求：
   * 长度必须在8-25个字符之间。
   * 至少包含一个小写字母。
   * 至少包含一个大写字母。
   * 至少包含一个数字。
   * 至少包含下列特殊字符之一： `# $ &: _ : { }`
* **[!UICONTROL 重新键入密码]**：重新输入新密码以确认输入正确。
* **[!UICONTROL 密码过期]**：确定您的密码是否作为安全措施在72天后过期。 如果选择“是”，则会要求您在72天后创建密码。
