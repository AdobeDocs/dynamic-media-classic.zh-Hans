---
title: AdobeDynamic Media Classic桌面应用程序 — 现已推出
description: 了解有关Dynamic Media Classic桌面应用程序的更多信息。
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/introducing_adobe_dynamic_media_classic
feature: Dynamic Media Classic
role: Administrator,Business Practitioner
exl-id: 604b4630-4704-4254-84b5-91b33bb19d58
source-git-commit: c4e2b8b42b56420269087d0d4f262490464270c0
workflow-type: tm+mt
source-wordcount: '1850'
ht-degree: 1%

---

# 现已推出：AdobeDynamic Media Classic桌面应用程序 {#dynamic-media-classic-desktop-app}

Dynamic Media Classic用户现在可以访问新的桌面应用程序体验，而不再依赖浏览器中的AdobeFlash技术。

此新应用程序现已在Windows®和macOS中可用。

>[!IMPORTANT]
>
>Adobe建议您在2020年10月1日之前安装新的AdobeDynamic Media Classic桌面应用程序。 这样做可确保在2020年12月31日弃用AdobeFlash Player之前实现顺利过渡。 在该日期之后，您将无法登录到AdobeDynamic Media Classic用户界面的浏览器版本，该版本在产品中标记为Dynamic Media Classic。

有关[新Dynamic Media Classic登录体验的常见问题解答，请参阅。](/help/new-ui-2020.md)

## AdobeDynamic Media Classic桌面应用程序的系统要求 {#system-requirements-dmc-app}

AdobeDynamic Media Classic桌面应用程序与以下操作系统兼容：

* macOS 10.10或更高版本。
* Windows® 7或更高版本。

>[!NOTE]
>
>对于&#x200B;*次要*&#x200B;版本，不会在Dynamic Media Classic桌面应用程序中生成升级通知。 从次要版本中的修复中受益的客户可以进行升级。

## 次要版本(20.21.2)中的修复 {#minor-release}

* 已知的“服务器”下拉列表20.21.1中的限制为空。
* 在&#x200B;**[!UICONTROL 上传作业选项]**&#x200B;中，位于&#x200B;**[!UICONTROL Photoshop选项]**&#x200B;下的层命名默认值现在为&#x200B;**[!UICONTROL Photoshop和层名称]**。 PSD 文件中的图层以单独图像形式上载。
   * 早期默认的&#x200B;**[!UICONTROL 图层名称]**，在PSD文件中将图像命名为其图层名称或图层编号。 如果PSD文件中的层名称是缺省的Photoshop层名称，则使用层编号。
   * 新的默认值&#x200B;**[!UICONTROL Photoshop和图层名称]**&#x200B;将图像命名为PSD文件之后的图像，然后是图层名称或图层编号。 如果 PSD 文件中的图层名称是默认的 Photoshop 图层名称，则将使用图层编号。
   * 鉴于Dynamic Media Classic中的图层图像现在具有唯一的名称，因此不会对现有PSD或模板（原始PSD文件中共享的图层名称）进行任何更新。
* 资产的缩略图损坏。

## 最新版本的修复(20.21.1) {#latest-fixes-desktop-app}

* 由于超时导致出现登录问题，导致出现以下消息：*未经权限，可将此用户分配给组或组。 请与管理员联系。*
* 查看器预设重复，每次密码尝试都不正确。
* 由于根文件夹中的许多资产，桌面应用程序变得无响应。 (已在Windows®上修复；在macOS中按需要工作。)

## 以前版本(20.20.2)中的修复 {#previous-version-fixes-desktop-app}

* 对于可通过适用于macOS和Windows®的桌面应用程序用户界面上传的文件数量没有限制。
* 无需注销桌面应用程序即可在公司之间进行切换。
* 现在，Ctrl+V可在Windows®上执行粘贴操作。
* 将来，当桌面应用程序的新版本发布时，用户将在桌面应用程序内收到通知。

## 在macOS或Windows®上下载并安装最新的AdobeDynamic Media Classic桌面应用程序 {#installation-dmc-app}

另请参阅:

* [在Mac上下载并静默安装最新的AdobeDynamic Media Classic桌面应用程序](#install-silent-mac-dmc-app)
* [在Windows®上下载并静默安装最新的AdobeDynamic Media Classic桌面应用程序](#install-silent-windows-dmc-app)

1. 在您的系统上卸载任何旧版Dynamic Media Classic桌面应用程序版本。

1. 下载AdobeDynamic Media Classic桌面应用程序的最新安装程序。

   * 以下版本提供了最新版本(20.21.2):

      * [macOS(.DMG) — 下载](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.dmg)
      * [Windows®(.EXE) — 下载](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.exe)
   * 以前的版本(20.21.1)可在以下位置使用：

      * [macOS(.DMG) — 下载](https://download.macromedia.com/dynamic-media-classic/20.21.1/adobe-dynamic-media-classic-20.21.1.dmg)
      * [Windows®(.EXE) — 下载](https://download.macromedia.com/dynamic-media-classic/20.21.1/adobe-dynamic-media-classic-20.21.1.exe)


<!--         * [macOS (.DMG) - Download.](https://download.macromedia.com/dynamic-media-classic/20.20.2/adobe-dynamic-media-classic-20.20.2.dmg)
        * [Windows (.EXE) - Download.](https://download.macromedia.com/dynamic-media-classic/20.20.2/adobe-dynamic-media-classic-20.20.2.exe) -->


1. 根据您下载的安装程序执行下列操作之一。

   * **对于macOS**  — 在拖放到 **[!UICONTROL 安装对话]** 框中，将 **[!UICONTROL AdobeDynamic Media]** 类拖放到应用程 **[!UICONTROL 序]**&#x200B;中。

      ![在macOS上拖放安装](/help/assets/dragondrop-install1.png)

   * 在&#x200B;**[!UICONTROL Applications]**&#x200B;文件夹中，点按AdobeDynamic Media Classic图标。
   * 在对话框中，点按&#x200B;**[!UICONTROL 打开]**&#x200B;以打开AdobeDynamic Media Classic桌面应用程序。

      ![打开下载的应用程序](/help/assets/open-dmclassicapp1.png)

   * **对于Windows**  — 运行安装程序二进制文件，并按照屏幕上的说明安装桌面应用程序。

1. 打开应用程序时，将显示新的AdobeDynamic Media Classic登录页面：

   ![Dynamic Media Classic登录](/help/assets/dmclassic-login1.png)

1. 要登录到AdobeDynamic Media Classic桌面应用程序，请使用与在浏览器中登录Dynamic Media Classic时所用的凭据相同的凭据。

   要使用&#x200B;**[!UICONTROL Server]**，请参阅生产环境的以下映射：

   | 浏览器URL | 桌面应用程序服务器名称 |
   |---|---|
   | https://s7sps1.scene7.com/ | NA（北美）生产 |
   | https://s7sps3.scene7.com/ | EMEA（欧洲、中东和非洲）生产 |
   | https://s7sps5.scene7.com/ | APAC（亚太地区）生产 |

1. 登录后，请注意熟悉的浏览器用户界面体验。 您可以像往常一样，在桌面应用程序上继续日常的Dynamic Media Classic活动。

## 在macOS上下载并&#x200B;*silent*&#x200B;安装最新的AdobeDynamic Media Classic桌面应用程序 {#install-silent-mac-dmc-app}

另请参阅:

* [在Mac或Windows®上下载并安装最新的AdobeDynamic Media Classic桌面应用程序](#installation-dmc-app)
* [在Windows®上下载并静默安装最新的AdobeDynamic Media Classic桌面应用程序](#install-silent-windows-dmc-app)

要在macOS上下载并&#x200B;*silent*&#x200B;安装最新版的AdobeDynamic Media Classic桌面应用程序，请执行以下操作：

1. 在您的系统上卸载任何旧版Dynamic Media Classic桌面应用程序版本。

1. 下载适用于macOS的AdobeDynamic Media Classic桌面应用程序的最新安装程序。

   * [macOS(.DMG) — 下载](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.dmg)

1. 使用以下命令将下载的磁盘映像(.DMG)装载到安装点位置：

   `hdiutil attach adobe-dynamic-media-classic-20.21.2.dmg -mountpoint <mount_point_path>`

1. 使用以下命令将.APP文件复制到&#x200B;**[!UICONTROL Applications]**:

   `rsync -a <mount_point_path>/Adobe\ Dynamic\ Media\ Classic.app /Applications/
Unmount DMG - hdiutil detach <mount_point_path>`

1. 打开应用程序时，将显示新的AdobeDynamic Media Classic登录页面：

   ![Dynamic Media Classic登录](/help/assets/dmclassic-login1.png)

1. 要登录到AdobeDynamic Media Classic桌面应用程序，请使用与在浏览器中登录Dynamic Media Classic时所用的凭据相同的凭据。

   要使用&#x200B;**[!UICONTROL Server]**，请参阅生产环境的以下映射：

   | 浏览器URL | 桌面应用程序服务器名称 |
   |---|---|
   | https://s7sps1.scene7.com/ | NA（北美）生产 |
   | https://s7sps3.scene7.com/ | EMEA（欧洲、中东和非洲）生产 |
   | https://s7sps5.scene7.com/ | APAC（亚太地区）生产 |

## 在Windows®上下载并&#x200B;*silent*&#x200B;安装最新的AdobeDynamic Media Classic桌面应用程序 {#install-silent-windows-dmc-app}

您使用的命令用于基本的MSI静默安装。 但是，Dynamic Media Classic桌面应用程序安装程序是使用InstallShield创建的InstallScript MSI安装程序。 在记录模式下运行安装程序时，任何用户交互都会记录在响应文件中。 然后，此响应文件将用于静默安装，如[在静默模式下运行安装中所述。](https://docs.revenera.com/installshield19helplib/helplibrary/SilentInstall.htm)

另请参阅:

* [在Mac或Windows®上下载并安装最新的AdobeDynamic Media Classic桌面应用程序](#installation-dmc-app)
* [在macOS上下载并静默安装最新的AdobeDynamic Media Classic桌面应用程序](#install-silent-mac-dmc-app)

要下载并&#x200B;*silent*&#x200B;在Windows®上安装最新版本的AdobeDynamic Media Classic桌面应用程序，请执行以下操作：

1. 在您的系统上卸载任何旧版Dynamic Media Classic桌面应用程序版本。

1. 下载AdobeDynamic Media Classic桌面应用程序的最新安装程序。

   * [Windows®(.EXE) — 下载](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.exe)

1. 使用以下命令在记录模式下运行安装程序：

   `adobe-dynamic-media-classic-20.21.2.exe /r /f1"C:\Setup.iss"`

1. 在GUI安装程序窗口中，按照要安装的步骤进行安装，以便交互/输入（如安装位置）记录在`Setup.iss`文件中。

1. 将创建的`Setup.iss`文件和`adobe-dynamic-media-classic-20.21.2.exe`复制到其他计算机。

1. 为静默安装运行以下命令：

   `adobe-dynamic-media-classic-20.21.2.exe /s /f1"C:\Setup.iss"`

   有关命令行参数的详细信息，请参见[Setup.exe和Update.exe命令行参数。](https://docs.revenera.com/installshield19helplib/helplibrary/IHelpSetup_EXECmdLine.htm)

1. 打开应用程序时，将显示新的AdobeDynamic Media Classic登录页面：

   ![Dynamic Media Classic登录](/help/assets/dmclassic-login1.png)

1. 要登录到AdobeDynamic Media Classic桌面应用程序，请使用与在浏览器中登录Dynamic Media Classic时所用的凭据相同的凭据。

   要使用&#x200B;**[!UICONTROL Server]**，请参阅生产环境的以下映射：

   | 浏览器URL | 桌面应用程序服务器名称 |
   |---|---|
   | https://s7sps1.scene7.com/ | NA（北美）生产 |
   | https://s7sps3.scene7.com/ | EMEA（欧洲、中东和非洲）生产 |
   | https://s7sps5.scene7.com/ | APAC（亚太地区）生产 |


## 有关使用Dynamic Media Classic桌面应用程序的视频演示 {#dmc-app-video-walk-through}

观看有关使用Dynamic Media Classic桌面应用程序的[视频演练](https://experienceleague.adobe.com/docs/experience-manager-learn/assets/dynamic-media/dynamic-media-classic-desktop-application.html#dynamic-media)(长度：2分36秒)。

## 使用桌面应用程序清除计算机上的图像缓存和资产缓存 {#clear-cache}

1. 在Dynamic Media Classic桌面应用程序的右上角附近，点按&#x200B;**[!UICONTROL 设置]** > **[!UICONTROL 个人设置]**。
1. 在&#x200B;**[!UICONTROL 个人设置]**&#x200B;页面的&#x200B;**[!UICONTROL Desktop]**&#x200B;标题下，执行以下任一操作：
   * 要从您的计算机中删除所有AdobeDynamic Media缓存的图像文件，请点按&#x200B;**[!UICONTROL 清除图像缓存]**，然后点按&#x200B;**[!UICONTROL 确定]**。
   * 要从您的计算机中删除所有AdobeDynamic Media缓存的资产文件，请点按&#x200B;**[!UICONTROL 清除资产缓存]**，然后点按&#x200B;**[!UICONTROL 确定]**。
1. 在页面的右下角，点按&#x200B;**[!UICONTROL 关闭]**。

### 手动清除图像缓存和资产缓存

除了使用桌面应用程序清除图像和资产缓存之外，您还可以直接从文件系统手动清除缓存。

1. 根据您的操作系统，导航到以下内容：

   * macOS:`~/Library/Application\ Support/com.adobe.DMCDesktop/Local\ Store/`
   * Windows®: `C:\Users\YourUserName\AppData\Roaming\com.adobe.DMCDesktop\Local Store`

## Dynamic Media Classic 20.21.1中的已知限制

* **[!UICONTROL Server]**&#x200B;下拉列表在更新到Dynamic Media Classic桌面应用程序20.21.1后为空 — 方案：安装并登录到Dynamic Media Classic 20.20.1或20.20.2，然后关闭应用程序。 然后更新到Dynamic Media Classic 20.21.1。当您尝试登录时，**[!UICONTROL 登录帐户]**&#x200B;对话框中的&#x200B;**[!UICONTROL Server]**&#x200B;下拉列表为空。 要解决此问题，您必须[手动清除缓存](#clear-cache)（请参阅上面的步骤）。

## Dynamic Media Classic 20.20.1的已知限制(已在20.20.2中修复)

**_仅适用于Windows® — 是否对可通过桌面应用程序用户界面上传的文件数量存在限制？_**<br>是，一次最多可通过桌面应用程序UI上传150个文件。

**_适用于Windows®和macOS — 如何在公司之间切换？_**<br>要在公司之间切换，请执行以下操作：

* 在Dynamic Media Classic应用程序中，从公司下拉列表中选择新公司。
* 出现弹出窗口时，点按&#x200B;**[!UICONTROL 确定]**&#x200B;以注销并关闭应用程序。

   ![要使用新公司，请重新启动应用程序](/help/assets/dmclassic-new-company1.png)

* 重新启动Dynamic Media Classic，然后照常登录以与新公司合作。

## 提示和技巧

**_我在Dynamic Media Classic的登陆页上看不到“媒体车”面板。_**<br>在Dynamic Media Classic中，点按**[!UICONTROL 设置>个人设置&#x200B;]**。在“浏览器”部分中，确保选中**[!UICONTROL 显示MediaPortal功能&#x200B;]**（选中）。 点按**[!UICONTROL 保存>关闭&#x200B;]**。

**_资产的发布状态（绿色指示器）未正确反映。_**<br>在浏览器用户界面中，需要重新登录UI才能查看正确的资产发布状态。在桌面应用程序中，Adobe在**[!UICONTROL 选择无&#x200B;]**按钮右侧的工具栏中引入了**[!UICONTROL 刷新&#x200B;]**图标。 点按**[!UICONTROL 刷新&#x200B;]**图标，以查看给定页面上所有资产的最新状态。 与使用浏览器UI时一样，无需重新登录。

![“刷新”](/help/assets/refresh-icon1.png)
*图标“刷新”图标*

**_我看不到批量集预设在桌面应用程序中工作。_**<br>点按**[!UICONTROL 上传>作业选项>批集预设&#x200B;]**。确保已启用相关的**[!UICONTROL 批集预设&#x200B;]**。 单击**[!UICONTROL 保存并提交上载&#x200B;]**。
