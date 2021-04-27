---
title: Adobe Dynamic Media Classic桌面应用程序 — 现已推出
description: 进一步了解Dynamic Media Classic桌面应用程序。
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/introducing_adobe_dynamic_media_classic
feature: Dynamic Media Classic
role: Administrator,Business Practitioner
exl-id: 604b4630-4704-4254-84b5-91b33bb19d58
translation-type: tm+mt
source-git-commit: c4e2b8b42b56420269087d0d4f262490464270c0
workflow-type: tm+mt
source-wordcount: '1850'
ht-degree: 1%

---

# 现已推出：Adobe Dynamic Media Classic桌面应用程序{#dynamic-media-classic-desktop-app}

Dynamic Media Classic用户现在可以访问新的桌面应用程序体验，而不再依赖浏览器中的AdobeFlash技术。

此新应用程序现在可用于Windows®和macOS。

>[!IMPORTANT]
>
>Adobe建议您在2020年10月1日之前安装新的Adobe Dynamic Media Classic桌面应用程序。 这样做将确保在2020年12月31日弃用AdobeFlash Player之前，您拥有一个流畅的过渡。 在该日期之后，您无法登录到浏览器版Adobe Dynamic Media Classic用户界面，产品中标记为Dynamic Media Classic。

有关[现已推出的新Dynamic Media经典登录体验，请参阅常见问题解答。](/help/new-ui-2020.md)

## Adobe Dynamic Media Classic桌面应用程序{#system-requirements-dmc-app}的系统要求

Adobe Dynamic Media Classic桌面应用程序与以下操作系统兼容：

* macOS 10.10或更高版本。
* Windows® 7或更高版本。

>[!NOTE]
>
>对于&#x200B;*次要*&#x200B;版本，不会为Dynamic Media Classic桌面应用程序内的升级通知生成。 从次要版本中的修复中受益的客户可以进行升级。

## 修复了次要版本(20.21.2){#minor-release}中的问题

* 20.21.1中服务器下拉列表的已知限制为空。
* 在&#x200B;**[!UICONTROL 上传作业选项]**&#x200B;中，**[!UICONTROL Photoshop选项]**&#x200B;下的图层命名默认值现在为&#x200B;**[!UICONTROL Photoshop和图层名称]**。 PSD 文件中的图层以单独图像形式上载。
   * 早期的&#x200B;**[!UICONTROL 图层名称]**&#x200B;默认值，在PSD文件中将图像命名为图层名称或图层编号。 如果PSD文件中的图层名称是默认的Photoshop图层名称，则使用图层编号。
   * 新的默认值&#x200B;**[!UICONTROL Photoshop和图层名称]**&#x200B;将图像命名在PSD文件后面，后面是图层名称或图层编号。 如果 PSD 文件中的图层名称是默认的 Photoshop 图层名称，则将使用图层编号。
   * 由于Dynamic Media Classic中的图层图像现在具有唯一的名称，因此不会更新现有PSD或模板（原始PSD文件中共享的图层名称）。
* 资源的缩略图已损坏。

## 最新版本(20.21.1){#latest-fixes-desktop-app}中的修复

* 由于超时导致的登录问题导致以下消息：*未经许可，可将此用户分配给组或组。 与管理员联系。*
* 查看器预设与每次错误的密码尝试重复。
* 由于根文件夹中的许多资源，桌面应用程序变得不响应。 (在Windows®上修复；在macOS上按需工作。)

## 修复了先前版本(20.20.2){#previous-version-fixes-desktop-app}

* 无限制可通过macOS和Windows®的桌面应用程序用户界面上传的文件数。
* 无需注销桌面应用程序即可在公司之间切换。
* 现在，Ctrl+V可在Windows®上进行粘贴操作。
* 将来，当发布新版本的桌面应用程序时，用户将在桌面应用程序内收到通知。

## 在macOS或Windows® {#installation-dmc-app}上下载并安装最新的Adobe Dynamic Media Classic桌面应用程序

另请参阅:

* [下载并静默安装Mac上最新的Adobe Dynamic Media Classic桌面应用程序](#install-silent-mac-dmc-app)
* [在Windows®上下载并静默安装最新的Adobe Dynamic Media Classic桌面应用程序](#install-silent-windows-dmc-app)

1. 在您的系统上卸载任何旧版Dynamic Media Classic桌面应用程序。

1. 下载Adobe Dynamic Media Classic桌面应用程序的最新安装程序。

   * 最新版本(20.21.2)可在以下位置获得：

      * [macOS(.DMG) — 下载](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.dmg)
      * [Windows®(.EXE) — 下载](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.exe)
   * 以前版本(20.21.1)可在以下位置获得：

      * [macOS(.DMG) — 下载](https://download.macromedia.com/dynamic-media-classic/20.21.1/adobe-dynamic-media-classic-20.21.1.dmg)
      * [Windows®(.EXE) — 下载](https://download.macromedia.com/dynamic-media-classic/20.21.1/adobe-dynamic-media-classic-20.21.1.exe)


<!--         * [macOS (.DMG) - Download.](https://download.macromedia.com/dynamic-media-classic/20.20.2/adobe-dynamic-media-classic-20.20.2.dmg)
        * [Windows (.EXE) - Download.](https://download.macromedia.com/dynamic-media-classic/20.20.2/adobe-dynamic-media-classic-20.20.2.exe) -->


1. 根据您下载的安装程序执行下列操作之一。

   * **对于macOS**  — 在“拖放 **[!UICONTROL 到安装”对]** 话框中，拖放 **[!UICONTROL Adobe Dynamic Media]** 类并将其放 **[!UICONTROL 到Applications]**&#x200B;上。

      ![在macOS上拖放安装](/help/assets/dragondrop-install1.png)

   * 在&#x200B;**[!UICONTROL Applications]**&#x200B;文件夹中，点按Adobe Dynamic Media Classic图标。
   * 在对话框中，点按&#x200B;**[!UICONTROL 打开]**&#x200B;以打开Adobe Dynamic Media Classic桌面应用程序。

      ![打开下载的应用程序](/help/assets/open-dmclassicapp1.png)

   * **对于Windows**  — 运行安装程序二进制文件，然后按照屏幕上的说明安装桌面应用程序。

1. 打开应用程序时，将显示新的Adobe Dynamic Media经典登录页面：

   ![Dynamic Media Classic登录](/help/assets/dmclassic-login1.png)

1. 要登录Adobe Dynamic Media Classic桌面应用程序，请使用您在浏览器中登录Dynamic Media Classic时所用的相同凭据。

   要使用&#x200B;**[!UICONTROL Server]**，请参阅生产环境的以下映射：

   | 浏览器URL | 桌面应用程序服务器名称 |
   |---|---|
   | https://s7sps1.scene7.com/ | NA（北美）生产 |
   | https://s7sps3.scene7.com/ | EMEA（欧洲、中东和非洲）生产 |
   | https://s7sps5.scene7.com/ | 亚太（亚太）生产 |

1. 登录后，请注意熟悉的浏览器用户界面体验。 您可以像往常一样在桌面应用程序上继续使用Dynamic Media Classic活动。

## 下载并&#x200B;*silent*&#x200B;在macOS {#install-silent-mac-dmc-app}上安装最新的Adobe Dynamic Media Classic桌面应用程序

另请参阅:

* [在Mac或Windows®上下载并安装最新的Adobe Dynamic Media Classic桌面应用程序](#installation-dmc-app)
* [在Windows®上下载并静默安装最新的Adobe Dynamic Media Classic桌面应用程序](#install-silent-windows-dmc-app)

要下载并&#x200B;*silent*&#x200B;安装macOS上最新版Adobe Dynamic Media Classic桌面应用程序，请执行以下操作：

1. 在您的系统上卸载任何旧版Dynamic Media Classic桌面应用程序。

1. 下载适用于macOS的Adobe Dynamic Media Classic桌面应用程序的最新安装程序。

   * [macOS(.DMG) — 下载](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.dmg)

1. 使用以下命令将下载的磁盘映像(.DMG)装载到安装点位置：

   `hdiutil attach adobe-dynamic-media-classic-20.21.2.dmg -mountpoint <mount_point_path>`

1. 使用以下命令将.APP文件复制到&#x200B;**[!UICONTROL Applications]**:

   `rsync -a <mount_point_path>/Adobe\ Dynamic\ Media\ Classic.app /Applications/
Unmount DMG - hdiutil detach <mount_point_path>`

1. 打开应用程序时，将显示新的Adobe Dynamic Media经典登录页面：

   ![Dynamic Media Classic登录](/help/assets/dmclassic-login1.png)

1. 要登录Adobe Dynamic Media Classic桌面应用程序，请使用您在浏览器中登录Dynamic Media Classic时所用的相同凭据。

   要使用&#x200B;**[!UICONTROL Server]**，请参阅生产环境的以下映射：

   | 浏览器URL | 桌面应用程序服务器名称 |
   |---|---|
   | https://s7sps1.scene7.com/ | NA（北美）生产 |
   | https://s7sps3.scene7.com/ | EMEA（欧洲、中东和非洲）生产 |
   | https://s7sps5.scene7.com/ | 亚太（亚太）生产 |

## 下载并&#x200B;*silent*&#x200B;安装Windows® {#install-silent-windows-dmc-app}上最新的Adobe Dynamic Media Classic桌面应用程序

您使用的命令用于基本的MSI静默安装。 但是，Dynamic Media Classic桌面应用程序安装程序是使用InstallShield创建的InstallScript MSI安装程序。 在记录模式下运行安装程序时，任何用户交互都会记录在响应文件中。 然后，此响应文件用于静默安装，如[在静默模式下运行安装中所述。](https://docs.revenera.com/installshield19helplib/helplibrary/SilentInstall.htm)

另请参阅:

* [在Mac或Windows®上下载并安装最新的Adobe Dynamic Media Classic桌面应用程序](#installation-dmc-app)
* [在macOS上下载并静默安装最新的Adobe Dynamic Media Classic桌面应用程序](#install-silent-mac-dmc-app)

要下载并&#x200B;*silent*&#x200B;安装Windows®上最新版Adobe Dynamic Media Classic桌面应用程序，请执行以下操作：

1. 在您的系统上卸载任何旧版Dynamic Media Classic桌面应用程序。

1. 下载Adobe Dynamic Media Classic桌面应用程序的最新安装程序。

   * [Windows®(.EXE) — 下载](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.exe)

1. 使用以下命令在记录模式下运行安装程序：

   `adobe-dynamic-media-classic-20.21.2.exe /r /f1"C:\Setup.iss"`

1. 在GUI安装程序窗口中，按照安装步骤进行安装，以便在`Setup.iss`文件中记录交互/输入（如安装位置）。

1. 将创建的`Setup.iss`文件和`adobe-dynamic-media-classic-20.21.2.exe`复制到其他计算机。

1. 对静默安装运行以下命令：

   `adobe-dynamic-media-classic-20.21.2.exe /s /f1"C:\Setup.iss"`

   有关命令行参数的详细信息，请访问[Setup.exe和Update.exe命令行参数。](https://docs.revenera.com/installshield19helplib/helplibrary/IHelpSetup_EXECmdLine.htm)

1. 打开应用程序时，将显示新的Adobe Dynamic Media经典登录页面：

   ![Dynamic Media Classic登录](/help/assets/dmclassic-login1.png)

1. 要登录Adobe Dynamic Media Classic桌面应用程序，请使用您在浏览器中登录Dynamic Media Classic时所用的相同凭据。

   要使用&#x200B;**[!UICONTROL Server]**，请参阅生产环境的以下映射：

   | 浏览器URL | 桌面应用程序服务器名称 |
   |---|---|
   | https://s7sps1.scene7.com/ | NA（北美）生产 |
   | https://s7sps3.scene7.com/ | EMEA（欧洲、中东和非洲）生产 |
   | https://s7sps5.scene7.com/ | 亚太（亚太）生产 |


## 使用Dynamic Media Classic桌面应用程序{#dmc-app-video-walk-through}的视频浏览

观看使用Dynamic Media Classic桌面应用程序](https://experienceleague.adobe.com/docs/experience-manager-learn/assets/dynamic-media/dynamic-media-classic-desktop-application.html#dynamic-media)的视频浏览(长度：2分36秒)。[

## 使用桌面应用程序{#clear-cache}清除您计算机上的图像缓存和资产缓存

1. 在Dynamic Media Classic桌面应用程序的右上角附近，点按&#x200B;**[!UICONTROL 设置]** > **[!UICONTROL 个人设置]**。
1. 在&#x200B;**[!UICONTROL 个人设置]**&#x200B;页面的&#x200B;**[!UICONTROL 桌面]**&#x200B;标题下，执行下列任一操作：
   * 要从您的计算机中删除所有Adobe Dynamic Media缓存的图像文件，请点按&#x200B;**[!UICONTROL 清除图像缓存]**，然后点按&#x200B;**[!UICONTROL 确定]**。
   * 要从您的计算机中删除所有Adobe Dynamic Media缓存的资产文件，请点按&#x200B;**[!UICONTROL 清除资产缓存]**，然后点按&#x200B;**[!UICONTROL 确定]**。
1. 在页面的右下角，点按&#x200B;**[!UICONTROL 关闭]**。

### 手动清除图像缓存和资产缓存

除了使用桌面应用程序清除图像和资产缓存外，您还可以直接从文件系统手动清除缓存。

1. 根据您的操作系统，导航到以下内容：

   * macOS:`~/Library/Application\ Support/com.adobe.DMCDesktop/Local\ Store/`
   * Windows®: `C:\Users\YourUserName\AppData\Roaming\com.adobe.DMCDesktop\Local Store`

## Dynamic Media Classic 20.21.1中的已知限制

* **[!UICONTROL Server]**&#x200B;下拉列表在更新到Dynamic Media Classic桌面应用程序20.21.1后为空 — 方案：您将安装并登录Dynamic Media Classic 20.20.1或20.20.2，然后关闭应用程序。 然后更新到Dynamic Media Classic 20.21.1。尝试登录时，**[!UICONTROL 登录到帐户]**&#x200B;对话框中的&#x200B;**[!UICONTROL Server]**&#x200B;下拉列表为空。 要解决此问题，您必须[手动清除缓存](#clear-cache)（请参阅上面的步骤）。

## Dynamic Media Classic 20.20.1中的已知限制（在20.20.2中修复）

**_仅适用于Windows® — 是否对可通过桌面应用程序UI上载的文件数有限制？_**<br>是，通过桌面应用程序UI，一次最多可上载150个文件。

**_适用于Windows®和macOS — 如何在公司之间切换？_**<br>要在公司之间切换，请执行以下操作：

* 在Dynamic Media Classic应用程序中，从公司下拉列表中选择新公司。
* 出现弹出窗口时，点按&#x200B;**[!UICONTROL 确定]**&#x200B;以注销并关闭应用程序。

   ![要使用新公司，请重新启动应用程序](/help/assets/dmclassic-new-company1.png)

* 重新启动Dynamic Media Classic，然后照常登录以使用新公司。

## 提示与技巧

**_我无法在Dynamic Media Classic的登陆页上看到“Media Cart（媒体购物车）”面板。_**<br>在Dynamic Media Classic中，点按**[!UICONTROL 设置>个人设置&#x200B;]**。在“浏览器”部分，确保选中了**[!UICONTROL “显示MediaPortal功能&#x200B;]**”（已选中）。 点按**[!UICONTROL 保存>关闭&#x200B;]**。

**_资产的发布状态（绿色指示符）反映不正确。_**<br>在浏览器用户界面中，需要重新登录UI才能查看资产的正确发布状态。在桌面应用程序中，Adobe在工具栏中的**[!UICONTROL 选择无&#x200B;]**按钮右侧引入了**[!UICONTROL 刷新&#x200B;]**图标。 点按**[!UICONTROL 刷新&#x200B;]**图标，以查看给定页面上所有资产的最新状态。 无需重新登录，就像浏览器UI一样。

![“刷新”](/help/assets/refresh-icon1.png)
*图标“刷新”图标*

**_我看不到批集预设在桌面应用程序中工作。_**<br>点按**[!UICONTROL 上传>作业选项>批集预设&#x200B;]**。确保已启用相关的**[!UICONTROL 批集预设&#x200B;]**。 单击**[!UICONTROL 保存并提交上载&#x200B;]**。
