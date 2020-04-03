---
title: 个人设置
seo-title: 个人设置
description: 'null'
seo-description: 所有用户都可以更改Dynamic Media Classic的“个人设置”屏幕上的设置。
uuid: 29cb825a-f158-4a1e-9d5f-7636ee411b6e
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/setup
discoiquuid: 6314e7b7-5bde-4fe2-8674-e4fc525d4d1c
translation-type: tm+mt
source-git-commit: a1722c15d3c049f05959d895e85297d47d730872

---


# 个人设置 {#personal-setup}

所有用户都可以更改“个人设置”屏幕中的设置。要打开“个人设置”屏幕，请单击“设置”>“个人设置”。

>[!NOTE]
>
>“个人设置”屏幕会列出您在 Scene7 Publishing System 中有哪些用户角色：“公司管理员”、“管理员”或“用户”。

“个人设置”设置控制浏览面板的默认行为、您接收电子邮件的方式以及密码设置。在更改这些设置之后，请记住单击“保存”。

## 我的帐户信息

标识您的帐户名称、名称、用户名（电子邮件地址）和指定的用户角色。

### 桌面版

单击“立即安装”，将 Scene7 Publishing System 的桌面版本安装在您的本地硬盘上。或者，单击“立即重新安装”，再次安装桌面版本。

### 用于 Web-to-Print 的 Illustator 插件

在运行 Windows 7 或 8 的计算机上，您必须具有管理员权限并在 Windows 中以管理员身份登录以安装用于 Web-to-Print 的 Illustator 插件。安装后，可以在 Adobe Illustrator 中使用该插件。

以下 Adobe Illustrator 版本支持该插件:

* Adobe Creative Cloud 2014 中的 Adobe Illustrator 18。
* Adobe Creative Cloud 中的 Adobe Illustrator 17。
* Adobe Creative Suite 6 中的 Adobe Illustrator 16。

支持的 Adobe Illustrator 平台包括：

* Apple Mac OS X 10.7 或更高版本。
* Windows 8，32 位和 64 位。
* Windows 7，32 位和 64 位。
* Windows XP，32 位和 64 位（仅适用于 Adobe Creative Suite 6 中的 Adobe Illustrator 16）。

另请参阅[模板发布](quick-start-template-publishing.md)。

## 在本地硬盘中安装插件

1. 在 Scene7 Publishing System 的“个人设置”页中的“用于 Web-to-Print 的 Illustrator 插件”下面，单击“**立即下载**”以下载 **Illustrator Plug-in for Web-to-Print.zip** 文件。
1. 将该 ZIP 文件解压缩到一个临时文件夹中。

   在解压缩的文件的根目录中包含一个自述文件以提供有关该插件的其他信息。

1. 根据安装的操作系统，执行以下操作之一：

### Windows

| 如果运行 | 执行的操作 |
|--- |--- |
| Adobe Creative Cloud 2014 中的 Adobe Illustrator 18 | <ul><li>从解压缩的文件夹的根目录中，单击“CC-2014”。</li><li>根据使用的 Adobe Illustrator 版本，单击“win32”或“win64”。</li><li>单击“libraries”>“flame”，然后将 `aflame.dll` 复制到可执行文件夹中。例如，`C:\Program Files\Adobe\Adobe Illustrator CC 2014\Support Files\Contents\Windows`。 </li></ul><br/>**注意&#x200B;**:此示例路径用于64位位置；32位位置可能会变为位于项目文件(x86)下。<br/><ul><li>返回到相同的 libraries 文件夹，单击“flamingo”，然后将 `aflamingo.dll` 复制到上一步中使用的相同 Adobe Illustrator 可执行文件夹中。 </li><li>返回到在步骤 2 中选择的 win32 或 win64 文件夹，然后将 `AdobeS7FXGFileFormat.aip` 复制到 Adobe Illustrator 的插件文件夹中。例如，`C:\Program Files\Adobe\Adobe Illustrator CC 2014\Plug-ins\Illustrator Formats`。 </li></ul> <br/>**注意&#x200B;**:此示例路径用于64位位置；32位位置可能会变为位于项目文件(x86)下。 |
| Adobe Creative Cloud 中的 Adobe Illustrator 17 | <ul><li>从解压缩的文件夹的根目录中，单击“CC”。 </li><li>根据使用的 Adobe Illustrator 版本，单击“win32”或“win64”。</li><li> Copy `AdobeS7FXGFileFormat.aip` to Adobe Illustrator&#39;s plug-ins folder. 例如，`C:\Program Files\Adobe\Adobe Illustrator CC (64 Bit)\Plug-ins\Illustrator Formats`。</li></ul><br/>**注意&#x200B;**:此示例路径用于64位位置；32位位置可能会变为位于项目文件(x86)下。 |
| Adobe Creative Suite 6 中的 Adobe Illustrator 16 | <ul><li>从解压缩的文件夹的根目录中，单击“6.0”。 </li><li>根据使用的 Adobe Illustrator 版本，单击“win32”或“win64”。 </li><li>将 AdobeS7FXGFileFormat.aip 复制到 Adobe Illustrator 的插件文件夹中。例如，`C:\Program Files\Adobe\Adobe Illustrator CS6 (64 Bit)\Plug-ins\Illustrator Formats`。</li></ul><br/>**注意&#x200B;**:此示例路径用于64位位置；32位位置可能会变为位于项目文件(x86)下。 |

### Mac

| 如果运行 | 执行的操作 |
|--- |--- |
| Adobe Creative Cloud 2014 中的 Adobe Illustrator 18 | <ul><li>从解压缩的文件夹的根目录中，单击“CC-2014”>“mac64”。</li><li>单击“libraries”>“flame”，然后将 `aflame.framework` 文件夹复制到 Adobe Illustrator 包内容文件夹中。示例, `/Applications/Adobe Illustrator CC 2014/ Illustrator.app/Contents/Frameworks/`. （要打开Adobe Illustrator的包内容文件夹，请右键单击Adobe Illustrator CC 2014图标，然后单击上下文菜单中的“显示包内容”。）</li><li>返回到相同的 libraries 文件夹，单击“`flamingo`”，然后将 `aflamingo.framework` 文件夹复制到上一步中使用的相同 Adobe Illustrator 包内容文件夹中。</li><li>返回到在步骤 1 中选择的 mac64 文件夹，然后将 `AdobeS7FXGFileFormat.aip` 文件夹复制到 Adobe Illustrator 的插件文件夹中。例如，`/Applications/Adobe Illustrator CC 2014/Plug-ins/Illustrator Formats/`。</li></ul><br/> |
| Adobe Creative Cloud 中的 Adobe Illustrator 17 | <ul><li>从解压缩文件夹的根目录中，单击“CC”>“mac64”</li><li>Copy the `AdobeS7FXGFileFormat.aip` folder to Adobe Illustrator’s plug-in folder. 例如，`/Applications/Adobe Illustrator CC/Plug-ins/Illustrator Formats/`。</li></ul><br/> |
| Adobe Creative Suite 6 中的 Adobe Illustrator 16 | <ul><li>从解压缩文件夹的根目录中，单击6.0 > mac64</li><li>Copy the `AdobeS7FXGFileFormat.aip` folder to Adobe Illustrator’s plug-in folder. 例如，`/Applications/Adobe Illustrator CS6/Plug-ins/Illustrator Formats/`。</li></ul> |

现在，您可以在 Adobe Illustrator 中使用该插件。

### 浏览器

* **缩略图大小**
   * 确定浏览面板的网格视图中缩略图图像的默认大小。
* **默认资源库视图**
   * 确定“资源库”中用于构建集的资源显示为缩略图还是按名称显示。如果要处理资源库中的大量资源，可以按名称查看资源。例如，如果要使用许多 PDF 文件构建较大的 eCatalog，可以按名称查看资源，以使列表变得简短。
* **默认浏览排序顺序**
   * 确定在浏览面板中显示资源的默认顺序。在菜单中选择排序条件，并选择是升序排序还是降序排序。
* **默认浏览位置**
   * 允许您将浏览位置设置为默认浏览位置、最后浏览的文件夹或者您导航至并标识的特定位置。还可以将浏览位置设置为按升序或降序排序文件和文件夹。
* **默认浏览视图**
   * 确定您在首次打开浏览面板时显示的默认视图是网格视图还是列表视图。
* **启动画面显示**
   * 确定您是否会看到任何启动画面，包括“欢迎”启动画面。
* **显示工具提示**
   * 确定将鼠标指针悬停在按钮、菜单和导航链接上时，是否显示工具提示。工具提示对屏幕上的项目进行说明。
* **灰白格背景**
   * 在图像后显示灰白格图层，使您可以轻松地看到具有 Alpha 通道的图像的透明区域。
* **显示文件大小**
   * 在您浏览时显示资源的文件大小。
* **在退出 SPS 时确认**
   * 在您退出 Scene7 Publishing System 之前，显示确认窗口。
* **在搜索中包括 UDF**
   * 取消选择（默认）可提高您运行的大多数元数据搜索的系统性能。

如果包括用户定义的字段对于您的大部分元数据搜索有帮助，您可以选择此选项以将其打开。或者可以使用高级搜索，与包括用户定义的字段相比，这种方式可以提供更直接、更快速的搜索体验。

请参阅[实施高级搜索](searching-assets.md#conducting_an_advanced_search)。

另请参阅[用户定义的字段](application-setup.md#user_defined_fields)。

* **基本搜索类型**
   * 选择默认的搜索类型，即“包含”或“开头为”。
* **显示 Media Portal 功能**
   * 选择此选项来访问 Media Portal 功能，例如“媒体购物车”。
* **显示命令反馈**
   * 显示对服务器的命令请求。
* **在导出时显示对话框**
   * 执行导出时显示一个对话框。如果取消选择此选项，您仍然可以转到“作业”页面来检索导出的结果。

## 电子邮件

* **电子邮件选项**
   * 选择您希望Dynamic Media Classic在上载和发布作业完成时通过电子邮件通知您的方式。 可以选择仅当发生警告或错误时接收作业完成通知。
* **电子邮件范围**
   * 确定您是接收公司的所有作业电子邮件，还是只接收有关您启动的上载和发布作业的电子邮件。
* **电子邮件类型**
   * 确定在完成上载作业和发布作业时是否通知您。
* **语言**
* **首选语言**
   * 确定界面语言。
* **密码**
* **新密码**
   * 输入新的有效密码。 您的密码必须满足以下要求：
      * 长度在8-25个字符之间
      * 至少包含一个小写字母
      * 至少包含一个大写字母
      * 至少包含一个数字
      * 至少包含下列特殊字符之一：#$&amp;-_:{}

* **重新键入密码**
   * 重新键入新密码以确认您输入了正确的密码。
* **密码过期**
   * 作为一项安全措施，确定您的密码是否在 72 天之后过期。如果选择“是”，会要求您在 72 天之后创建新密码。
