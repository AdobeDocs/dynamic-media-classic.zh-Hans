---
title: Adobe Dynamic Media Classic桌面
description: 进一步了解现在可用的Adobe Dynamic Media Classic桌面应用程序。
contentOwner: rbrough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/introducing_adobe_dynamic_media_classic
feature: Dynamic Media Classic
role: Admin,User
exl-id: 604b4630-4704-4254-84b5-91b33bb19d58
topic: Administration
level: Intermediate
source-git-commit: afc347201b13c3b91ec5e1bd3ac5304442772f8d
workflow-type: tm+mt
source-wordcount: '1994'
ht-degree: 0%

---

# 现已推出：Adobe Dynamic Media Classic桌面应用程序 {#dynamic-media-classic-desktop-app}

Adobe Dynamic Media Classic用户现在可以访问新的桌面应用程序体验，不再需要依赖浏览器中的AdobeFlash技术。

此新应用程序现在可用于Windows®和macOS。

>[!IMPORTANT]
>
>Adobe建议您在2020年10月1日之前安装新的Adobe Dynamic Media Classic桌面应用程序。 这样做将确保在2020年12月31日弃用AdobeFlash Player之前实现顺利过渡。 在该日期之后，您将无法登录到产品中标记为Adobe Dynamic Media Classic的Adobe Dynamic Media Classic用户界面的浏览器版本。

查看[新Adobe Dynamic Media Classic登录的常见问题解答。](/help/using/new-ui-2020.md)

## Adobe Dynamic Media Classic桌面应用程序的系统要求 {#system-requirements-dmc-app}

Adobe Dynamic Media Classic桌面应用程序与以下操作系统兼容：

* macOS 10.10或更高版本。
* Windows® 7或更高版本。

请参阅[Adobe Dynamic Media Classic桌面应用程序的系统要求](/help/using/system-requirements.md)上的完整系统要求。

没有为&#x200B;*次要*&#x200B;版本生成Adobe Dynamic Media Classic桌面应用程序中的升级通知。 从次要版本中的修复中获益的客户可以升级。

## 仅在最新版本(20.22.2)的macOS中修复 {#release-feb2022}

* macOS Montery：文件上传页面在后续上传时冻结。<!-- https://jira.corp.adobe.com/browse/ASSETS-7948 -->

## 最新版本(20.22.1)中的修复 {#release-jan2022}

* 编辑图像时，**[!UICONTROL 保存]**&#x200B;按钮不起作用。
* 在“集”编辑器中，滚动&#x200B;**[!UICONTROL 添加Assets]**&#x200B;面板中的资源后，**[!UICONTROL 关闭]**、**[!UICONTROL 保存]**&#x200B;和&#x200B;**[!UICONTROL 另存为]**&#x200B;按钮将被禁用。
* “视频详细信息”视图中的&#x200B;**[!UICONTROL 播放]**&#x200B;按钮不起作用。
* 运行macOS Monterey时，无法在&#x200B;**[!UICONTROL 用户名]**&#x200B;和&#x200B;**[!UICONTROL 密码]**&#x200B;字段中输入`d`和`e`。
* 已将剩余的Analytics API移至版本2.0。

## 20.21.3版中的修复 {#release-sept2021}

* 在桌面应用程序上处于非活动状态一段时间后看到的资产的缩略图损坏。
* 桌面应用程序停止响应，通常在Set操作之后。
* 已在&#x200B;**[!UICONTROL 测试图像服务]**&#x200B;下自动启用请求模糊处理和锁定模式。

  请参阅[安全测试服务](/help/using/testing-assets-making-them-public.md#testing-the-secure-testing-service)。

* 更新了Adobe Analytics的身份验证机制。 与新集成或必须从Dynamic Media Classic桌面应用程序中更新某些Analytics变量相关。

  有关更新步骤，请参阅[登录Adobe Analytics](/help/using/log-analytics.md)。

## 20.21.2版中的修复 {#minor-release}

* 20.21.1中的已知限制：“登录”屏幕上的&#x200B;**[!UICONTROL 服务器]**&#x200B;下拉列表为空。
* 在&#x200B;**[!UICONTROL 上载作业选项]**&#x200B;中，**[!UICONTROL Photoshop选项]**&#x200B;下的默认图层名称值现在是&#x200B;**[!UICONTROL Photoshop和图层名称]**。 PSD文件中的图层将作为单独的图像上传。
   * 较早的默认值&#x200B;**[!UICONTROL 图层名称]**&#x200B;在PSD文件中以图层的名称或图层编号命名图像。 如果PSD文件中的图层名称是默认的Photoshop图层名称，则使用图层编号。
   * 新的默认值&#x200B;**[!UICONTROL Photoshop和图层名称]**&#x200B;将图像命名为PSD文件后跟图层名称或图层编号。 如果PSD文件中的图层名称是默认的Photoshop图层名称，则使用图层编号。
   * 考虑到Adobe Dynamic Media Classic中的图层图像现在具有唯一名称，因此不会对现有PSD或模板进行更新(哪些模板与原始PSD文件中的图层名称共享)。
* 资产的缩略图损坏。

## 20.21.1版中的修复 {#latest-fixes-desktop-app}

* 由于超时而导致登录问题导致出现以下消息： *此用户可能被分配给无权限的组。 请与管理员联系。*
* 每次尝试使用错误的密码时，查看器预设都会重复。
* 由于根文件夹中的许多资产，桌面应用程序变得无响应。 (在Windows®上修复；根据需要在macOS上工作。)

## 20.20.2版中的修复 {#previous-version-fixes-desktop-app}

* 对于macOS和Windows®，您可以通过桌面应用程序用户界面上传的文件数量没有限制。
* 无需注销桌面应用程序，即可在公司之间切换。
* 现在，在Windows®上可以按Ctrl+V执行粘贴操作。
* 将来，当桌面应用程序发布新版本时，将会在桌面应用程序本身中通知用户。

## 在macOS或Windows上下载并安装最新的Adobe Dynamic Media Classic桌面应用程序® {#installation-dmc-app}

另请参阅：

* [在Mac上下载并静默安装最新的Adobe Dynamic Media Classic桌面应用程序](#install-silent-mac-dmc-app)
* [在Windows上下载并静默安装最新的Adobe Dynamic Media Classic桌面应用程序](#install-silent-windows-dmc-app)

1. 卸载系统上的任何旧版Adobe Dynamic Media Classic桌面应用程序。

1. 下载Adobe Dynamic Media Classic桌面应用程序的最新安装程序。

   * 最新版本可从以下网站获取：

      * [macOS (.DMG)：下载](https://download.macromedia.com/dynamic-media-classic/20.22.2/adobe-dynamic-media-classic-20.22.2.dmg)
      * [Windows (.EXE)：下载](https://download.macromedia.com/dynamic-media-classic/20.22.1/adobe-dynamic-media-classic-20.22.1.exe)

   * 以前的版本在以下位置提供：

      * [macOS (.DMG)：下载](https://download.macromedia.com/dynamic-media-classic/20.22.1/adobe-dynamic-media-classic-20.22.1.dmg)
      * [Windows® (.EXE)：下载](https://download.macromedia.com/dynamic-media-classic/20.21.3/adobe-dynamic-media-classic-20.21.3.exe)

<!--         * [macOS (.DMG): Download](https://download.macromedia.com/dynamic-media-classic/20.21.3/adobe-dynamic-media-classic-20.21.3.dmg) -->

<!--    * [macOS (.DMG): Download](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.dmg)
        * [Windows&reg; (.EXE): Download](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.exe) -->

<!--    * [macOS (.DMG): Download.](https://download.macromedia.com/dynamic-media-classic/20.20.2/adobe-dynamic-media-classic-20.20.2.dmg)
        * [Windows (.EXE): Download.](https://download.macromedia.com/dynamic-media-classic/20.20.2/adobe-dynamic-media-classic-20.20.2.exe) -->


1. 根据您下载的安装程序执行以下操作之一。

   * **macOS** — 在&#x200B;**[!UICONTROL 拖放以安装]**&#x200B;对话框中，将&#x200B;**[!UICONTROL Adobe Dynamic Media Classic]**&#x200B;拖放到&#x200B;**[!UICONTROL 应用程序]**&#x200B;上。

     ![在macOS上拖放安装](/help/using/assets/dragondrop-install1.png)

   * 在&#x200B;**[!UICONTROL 应用程序]**&#x200B;文件夹中，点按Adobe Dynamic Media Classic图标。
   * 在对话框中，点按&#x200B;**[!UICONTROL 打开]**&#x200B;以打开Adobe Dynamic Media Classic桌面应用程序。

     ![打开下载的应用程序](/help/using/assets/open-dmclassicapp1.png)

   * **Windows** — 运行安装程序二进制文件，并按照屏幕上的说明安装桌面应用程序。

1. 打开应用程序时，会显示新的Adobe Dynamic Media Classic登录页面：

   ![Adobe Dynamic Media Classic登录](/help/using/assets/dmclassic-login1.png)

1. 要登录到Adobe Dynamic Media Classic桌面应用程序，请使用在浏览器中登录到Adobe Dynamic Media Classic的相同凭据。

   对于要使用的&#x200B;**[!UICONTROL 服务器]**，请参阅生产环境的以下映射：

   | 服务器 | 浏览器URL |
   | --- | --- |
   | NA生产（北美） | https://s7sps1.scene7.com/ |
   | EMEA生产（欧洲、中东和非洲） | https://s7sps3.scene7.com/ |
   | APAC生产（亚太） | https://s7sps5.scene7.com/ |

1. 登录后，请注意熟悉的浏览器用户界面体验。 您可以像往常一样，在桌面应用程序上继续您的日常Adobe Dynamic Media Classic活动。

## 在macOS上下载并&#x200B;*静默安装*&#x200B;最新的Adobe Dynamic Media Classic桌面应用程序 {#install-silent-mac-dmc-app}

另请参阅：

* [在Mac或Windows上下载并安装最新的Adobe Dynamic Media Classic桌面应用程序](#installation-dmc-app)
* [在Windows上下载并静默安装最新的Adobe Dynamic Media Classic桌面应用程序](#install-silent-windows-dmc-app)

要在macOS上下载并静默安装&#x200B;*最新版本的Adobe Dynamic Media Classic桌面应用程序，请执行以下操作：*

1. 卸载系统上的任何旧版Adobe Dynamic Media Classic桌面应用程序。

1. 下载适用于macOS的Adobe Dynamic Media Classic桌面应用程序的最新安装程序。

   * [macOS (.DMG)：下载](https://download.macromedia.com/dynamic-media-classic/20.22.2/adobe-dynamic-media-classic-20.22.2.dmg)

1. 使用以下命令将下载的磁盘映像(.DMG)装载到装载点位置：

   `hdiutil attach adobe-dynamic-media-classic-20.22.2.dmg -mountpoint <mount_point_path>`

1. 使用以下命令将.APP文件复制到&#x200B;**[!UICONTROL 应用程序]**：

   ```
   rsync -a <mount_point_path>/Adobe\ Dynamic\ Media\ Classic.app /Applications/
   Unmount DMG: hdiutil detach <mount_point_path>
   ```

1. 打开应用程序时，会显示新的Adobe Dynamic Media Classic登录页面：

   ![Adobe Dynamic Media Classic登录](/help/using/assets/dmclassic-login1.png)

1. 要登录到Adobe Dynamic Media Classic桌面应用程序，请使用在浏览器中登录到Adobe Dynamic Media Classic的相同凭据。

   对于要使用的&#x200B;**[!UICONTROL 服务器]**，请参阅生产环境的以下映射：

   | 服务器 | 浏览器URL |
   | --- | --- |
   | NA生产（北美） | https://s7sps1.scene7.com/ |
   | EMEA生产（欧洲、中东和非洲） | https://s7sps3.scene7.com/ |
   | APAC生产（亚太） | https://s7sps5.scene7.com/ |

## 在Windows®上下载并&#x200B;*静默安装*&#x200B;最新的Adobe Dynamic Media Classic桌面应用 {#install-silent-windows-dmc-app}

您使用的命令用于基本的MSI静默安装。 但是，Adobe Dynamic Media Classic桌面应用程序安装程序是使用InstallShield创建的InstallScript MSI安装程序。 在记录模式下运行安装程序时，任何用户交互都会记录在响应文件中。 然后将此响应文件用于静默安装，如[在静默模式下运行安装](https://docs.revenera.com/installshield25helplib/installshield25helplib.htm#helplibrary/SilentInstall.htm)中所述。

另请参阅：

* [在Mac或Windows上下载并安装最新的Adobe Dynamic Media Classic桌面应用程序](#installation-dmc-app)

* [在macOS上下载并静默安装最新的Adobe Dynamic Media Classic桌面应用程序](#install-silent-mac-dmc-app)

要在Windows®上下载并&#x200B;*静默安装*&#x200B;最新版本的Adobe Dynamic Media Classic桌面应用程序，请执行以下操作：

1. 卸载系统上的任何旧版Adobe Dynamic Media Classic桌面应用程序。

1. 下载Adobe Dynamic Media Classic桌面应用程序的最新安装程序。

   * [Windows® (.EXE)：下载](https://download.macromedia.com/dynamic-media-classic/20.22.1/adobe-dynamic-media-classic-20.22.1.exe)

1. 使用以下命令在记录模式下运行安装程序：

   `adobe-dynamic-media-classic-20.22.1.exe /r /f1"C:\Setup.iss"`

1. 在GUI安装程序窗口中，按照安装步骤进行操作，以便在`Setup.iss`文件中记录交互/输入（如安装位置）。

1. 将创建的`Setup.iss`文件和`adobe-dynamic-media-classic-20.22.1.exe`复制到其他计算机。

1. 为静默安装运行以下命令：

   `adobe-dynamic-media-classic-20.22.1.exe /s /f1"C:\Setup.iss"`

   有关命令行参数的详细信息，请访问[Setup.exe和Update.exe命令行参数](https://docs.revenera.com/installshield25helplib/installshield25helplib.htm#helplibrary/IHelpSetup_EXECmdLine.htm?Highlight=Setup.exe%20and%20Update.exe%20Command-Line%20Parameters)。

1. 打开应用程序时，会显示新的Adobe Dynamic Media Classic登录页面：

   ![Adobe Dynamic Media Classic登录](/help/using/assets/dmclassic-login1.png)

1. 要登录到Adobe Dynamic Media Classic桌面应用程序，请使用在浏览器中登录到Adobe Dynamic Media Classic的相同凭据。

   对于要使用的&#x200B;**[!UICONTROL 服务器]**，请参阅生产环境的以下映射：

   | 服务器 | 浏览器URL |
   | --- | --- |
   | NA生产（北美） | https://s7sps1.scene7.com/ |
   | EMEA生产（欧洲、中东和非洲） | https://s7sps3.scene7.com/ |
   | APAC生产（亚太） | https://s7sps5.scene7.com/ |

## 有关使用Adobe Dynamic Media Classic桌面应用程序的视频演练 {#dmc-app-video-walk-through}

观看使用Adobe Dynamic Media Classic桌面应用程序[&#128279;](https://experienceleague.adobe.com/zh-hans/docs/experience-manager-learn/assets/dynamic-media/dynamic-media-classic-desktop-application#dynamic-media)的视频演练（长度：2分36秒）。

## 使用桌面应用程序清除计算机上的图像缓存和资产缓存 {#clear-cache}

1. 在Adobe Dynamic Media Classic桌面应用程序右上角附近，点按&#x200B;**[!UICONTROL 设置]** > **[!UICONTROL 个人设置]**。
1. 在&#x200B;**[!UICONTROL 个人设置]**&#x200B;页面的&#x200B;**[!UICONTROL 桌面]**&#x200B;标题下，执行以下任一操作：
   * 若要从计算机中删除所有AdobeDynamic Media缓存的图像文件，请点按&#x200B;**[!UICONTROL 清除图像缓存]**，然后点按&#x200B;**[!UICONTROL 确定]**。
   * 若要从计算机中删除所有AdobeDynamic Media缓存的资源文件，请点按&#x200B;**[!UICONTROL 清除资源缓存]**，然后点按&#x200B;**[!UICONTROL 确定]**。
1. 在页面的右下角，点按&#x200B;**[!UICONTROL 关闭]**。

### 手动清除图像缓存和资产缓存

除了使用桌面应用程序清除图像和资产缓存之外，您还可以直接从文件系统手动清除缓存。

1. 根据您的操作系统，导航至以下内容：

   * macOS： `~/Library/Application\ Support/com.adobe.DMCDesktop/Local\ Store/`
   * Windows®： `C:\Users\YourUserName\AppData\Roaming\com.adobe.DMCDesktop\Local Store`

## Adobe Dynamic Media Classic 20.21.1中的已知限制

* 更新到Adobe Dynamic Media Classic桌面应用程序20.21.1后，**[!UICONTROL 服务器]**&#x200B;下拉列表为空：方案：您安装并登录到Adobe Dynamic Media Classic 20.20.1或20.20.2，然后关闭该应用程序。 然后您更新到Adobe Dynamic Media Classic 20.21.1。当您尝试登录时，**[!UICONTROL 登录到您的帐户]**&#x200B;对话框中的&#x200B;**[!UICONTROL 服务器]**&#x200B;下拉列表为空。 要解决此问题，您必须[手动清除缓存](#clear-cache)（请参阅上述步骤）。

## Adobe Dynamic Media Classic 20.20.1中的已知限制（已在20.20.2中修复）

**_仅适用于Windows® — 能否限制通过桌面应用程序UI上传的文件数量？_**<br>是，使用桌面应用程序UI一次最多可以上传150个文件。

**_适用于Windows®和macOS — 如何在公司之间切换？_**<br>要在公司之间切换，请执行以下操作：

* 在Adobe Dynamic Media Classic应用程序中，从公司下拉列表中选择新公司。
* 出现弹出窗口时，点按&#x200B;**[!UICONTROL 确定]**&#x200B;以注销并关闭应用程序。

  ![若要使用新公司，请重新启动应用](/help/using/assets/dmclassic-new-company1.png)

* 重新启动Adobe Dynamic Media Classic，然后照常登录以与新公司合作。

## 提示和技巧

**_我在Adobe Dynamic Media Classic的登录页面上无法看到“媒体购物车”面板。_**<br>在Adobe Dynamic Media Classic中，点按&#x200B;**[!UICONTROL 设置>个人设置&#x200B;]**。 在“浏览器”部分中，确保选中（选中）**[!UICONTROL 显示MediaPortal功能&#x200B;]**。 点按&#x200B;**[!UICONTROL 保存>关闭&#x200B;]**。

资源的&#x200B;**_Publish状态（绿色指示器）未正确反映。_**<br>在浏览器用户界面中，需要重新登录UI才能查看资产的正确发布状态。 在桌面应用程序中，Adobe在&#x200B;**[!UICONTROL 无选择&#x200B;]**&#x200B;按钮右侧的工具栏中引入了&#x200B;**[!UICONTROL 刷新&#x200B;]**&#x200B;图标。 点按&#x200B;**[!UICONTROL 刷新&#x200B;]**&#x200B;图标可查看给定页面上所有资产的最新状态。 与浏览器UI一样，无需重新登录。

![刷新图标](/help/using/assets/refresh-icon1.png)
*刷新图标*

**_我看不到批次集预设在桌面应用程序中工作。_**<br>点按&#x200B;**[!UICONTROL 上传>作业选项>批次集预设&#x200B;]**。 请确保相关&#x200B;**[!UICONTROL 批次集预设&#x200B;]**&#x200B;已启用。 单击&#x200B;**[!UICONTROL 保存并提交上载&#x200B;]**。
