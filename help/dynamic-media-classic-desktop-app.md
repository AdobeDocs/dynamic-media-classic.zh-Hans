---
title: AdobeDynamic Media Classic桌面应用程序——现已推出
seo-title: AdobeDynamic Media Classic桌面应用程序——现已推出
description: 'null'
seo-description: 进一步了解Dynamic Media Classic桌面应用程序。
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/introducing_adobe_dynamic_media_classic
translation-type: tm+mt
source-git-commit: 477a8fd6ffee00cd586d91f6eeda8e676753a90f
workflow-type: tm+mt
source-wordcount: '1244'
ht-degree: 0%

---


# 现已推出：AdobeDynamic Media Classic桌面应用程序 {#dynamic-media-classic-desktop-app}

Dynamic Media Classic用户现在可以获得新的桌面应用程序体验，该体验不再依赖浏览器中的AdobeFlash技术。

此新应用程序现在可用于Windows和macOS。

>[!IMPORTANT]
>
>我们建议您在2020年10月1日之前安装新的AdobeDynamic Media Classic桌面应用程序。 这样做将确保在2020年12月31日弃用AdobeFlash Player之前，您拥有一个流畅的过渡。 在该日期，您将无法再登录到AdobeDynamic Media Classic用户界面的浏览器版本，产品中标为Dynamic Media Classic。

请参阅新增的Dynamic [Media Classic登录体验的常见问题解答。](/help/new-ui-2020.md)

## AdobeDynamic Media Classic桌面应用程序的系统要求 {#system-requirements-dmc-app}

AdobeDynamic Media Classic桌面应用程序与以下操作系统兼容：
* macOS X 10.10或更高版本。
* Windows 7或更高版本。

## 在macOS或Windows上下载和安装AdobeDynamic Media Classic桌面应用程序 {#installation-dmc-app}

另请参阅:

* [在macOS上下 *载和静* 默安装AdobeDynamic Media Classic桌面应用程序](#install-silent-mac-dmc-app)
* [在Windows上下 *载和静* 默安装AdobeDynamic Media Classic桌面应用程序](#install-silent-windows-dmc-app)

1. 在您的系统上卸载任何旧版Dynamic Media Classic桌面应用程序。

1. 下载AdobeDynamic Media Classic桌面应用程序的最新安装程序。

   * [macOS(.DMG)-下载。](http://download.macromedia.com/dynamic-media-classic/20.20.1/adobe-dynamic-media-classic-20.20.1.dmg)
   * [Windows(.EXE)-下载。](http://download.macromedia.com/dynamic-media-classic/20.20.1/adobe-dynamic-media-classic-20.20.1.exe)

1. 根据您下载的安装程序执行下列操作之一。

   * **对于macOS** —— 在“ **[!UICONTROL 拖放以安装]** ”对话框中，拖 **[!UICONTROL 动AdobeDynamic Media Classic]** 并将其放入“应 **[!UICONTROL 用程序]**”。

      ![在macOS上拖放安装](/help/assets/dragondrop-install1.png)

   * 在“应用 **[!UICONTROL 程序]** ”文件夹中，点按AdobeDynamic Media Classic图标。
   * 在对话框中，点按打 **[!UICONTROL 开]** ，以打开AdobeDynamic Media Classic桌面应用程序。

      ![打开下载的应用程序](/help/assets/open-dmclassicapp1.png)

   * **对于Windows** —— 运行安装程序二进制文件，按照屏幕上的说明安装桌面应用程序。

1. 打开应用程序时，将显示新的AdobeDynamic Media经典登录页：

   ![Dynamic Media Classic登录](/help/assets/dmclassic-login1.png)

1. 使用与浏览器凭据相同的凭据登录Dynamic Media ClassicAdobe。

   要使 **[!UICONTROL 用服务器]** ，请参阅生产环境的以下映射：

   | 浏览器URL | 桌面应用程序服务器名称 |
   |---|---|
   | https://s7sps1.scene7.com/ | NA（北美）生产 |
   | https://s7sps3.scene7.com/ | EMEA（欧洲、中东和非洲）生产 |
   | https://s7sps5.scene7.com/ | 亚太地区生产 |

1. 登录UI发布后，您会注意到您熟悉的浏览器UI体验。 您现在可以在桌面应用程序UI中像往常一样将日常活动带入您的日常。

## 在macOS上下 *载和静* 默安装AdobeDynamic Media Classic桌面应用程序 {#install-silent-mac-dmc-app}

另请参阅:

* [在Mac或Windows上下载和安装AdobeDynamic Media Classic桌面应用程序](#installation-dmc-app)
* [在Windows上下 *载和静* 默安装AdobeDynamic Media Classic桌面应用程序](#install-silent-windows-dmc-app)

要在macOS上下 *载和静默* 安装AdobeDynamic Media Classic桌面应用程序，请执行以下操作：

1. 在您的系统上卸载任何旧版Dynamic Media Classic桌面应用程序。

1. 下载适用于macOS的AdobeDynamic Media Classic桌面应用程序的最新安装程序。

   * [macOS(.DMG)-下载。](http://download.macromedia.com/dynamic-media-classic/20.20.1/adobe-dynamic-media-classic-20.20.1.dmg)

1. 使用以下命令将下载的磁盘映像(.DMG)装载到装载点位置：

   `hdiutil attach adobe-dynamic-media-classic-20.20.1.dmg -mountpoint <mount_point_path>`

1. 使用以下命令将。 **[!UICONTROL APP文]** 件复制到应用程序：

   `rsync -a <mount_point_path>/Adobe\ Dynamic\ Media\ Classic.app /Applications/
Unmount DMG - hdiutil detach <mount_point_path>`

1. 打开应用程序时，将显示新的AdobeDynamic Media经典登录页：

   ![Dynamic Media Classic登录](/help/assets/dmclassic-login1.png)

1. 使用与浏览器凭据相同的凭据登录Dynamic Media ClassicAdobe。

   要使 **[!UICONTROL 用服务器]** ，请参阅生产环境的以下映射：

   | 浏览器URL | 桌面应用程序服务器名称 |
   |---|---|
   | https://s7sps1.scene7.com/ | NA（北美）生产 |
   | https://s7sps3.scene7.com/ | EMEA（欧洲、中东和非洲）生产 |
   | https://s7sps5.scene7.com/ | 亚太地区生产 |

## 在Windows上下 *载和静* 默安装AdobeDynamic Media Classic桌面应用程序 {#install-silent-windows-dmc-app}

您使用的命令用于基本的MSI静默安装。 但是，Dynamic Media Classic桌面应用程序安装程序是使用InstallShield创建的InstallScript MSI安装程序。 在记录模式下运行安装程序时，任何用户交互都会记录在响应文件中。 然后，此响应文件用于静默安装，如在静默模 [式下运行安装中所述。](https://docs.flexera.com/installshield19helplib/helplibrary/SilentInstall.htm)

另请参阅:

* [在Mac或Windows上下载和安装AdobeDynamic Media Classic桌面应用程序](#installation-dmc-app)
* [在Windows上下 *载和静* 默安装AdobeDynamic Media Classic桌面应用程序](#install-silent-windows-dmc-app)

要在Windows上下 *载和静* 默安装AdobeDynamic Media Classic桌面应用程序，请执行以下操作：

1. 在您的系统上卸载任何旧版Dynamic Media Classic桌面应用程序。

1. 下载AdobeDynamic Media Classic桌面应用程序的最新安装程序。

   * [Windows(.EXE)-下载。](http://download.macromedia.com/dynamic-media-classic/20.20.1/adobe-dynamic-media-classic-20.20.1.exe)

1. 使用以下命令在记录模式下运行安装程序：

   `adobe-dynamic-media-classic-20.20.1.exe /r /f1"C:\Setup.iss"`

1. 在GUI安装程序窗口中，按照安装步骤进行安装，以便交互／输入（如安装位置）记录在文 `Setup.iss` 件中。

1. 将创建的文 `Setup.iss` 件复制 `adobe-dynamic-media-classic-20.20.1.exe` 到其他计算机。

1. 为静默安装运行以下命令：

   `adobe-dynamic-media-classic-20.20.1.exe /s /f1"C:\Setup.iss"`

   有关命令行参数的详细 [信息，请参阅Setup.exe和Update.exe命令行参数。](https://docs.flexera.com/installshield19helplib/helplibrary/IHelpSetup_EXECmdLine.htm)

1. 打开应用程序时，将显示新的AdobeDynamic Media经典登录页：

   ![Dynamic Media Classic登录](/help/assets/dmclassic-login1.png)

1. 使用与浏览器凭据相同的凭据登录Dynamic Media ClassicAdobe。

   要使 **[!UICONTROL 用服务器]** ，请参阅生产环境的以下映射：

   | 浏览器URL | 桌面应用程序服务器名称 |
   |---|---|
   | https://s7sps1.scene7.com/ | NA（北美）生产 |
   | https://s7sps3.scene7.com/ | EMEA（欧洲、中东和非洲）生产 |
   | https://s7sps5.scene7.com/ | 亚太地区生产 |


## 使用Dynamic Media Classic桌面应用程序的视频入门

观看使 [用Dynamic Media Classic桌面应用程序的视频演练](https://docs.adobe.com/content/help/en/experience-manager-learn/assets/dynamic-media/dynamic-media-classic-desktop-application.html) (长度：2分36秒)。

## Dynamic Media Classic的已知限制

**_仅适用于Windows —— 是否对可通过桌面应用程序UI上传的文件数有限制？_**<br>是，通过桌面应用程序UI，一次最多可上传150个文件。

**_适用于Windows和macOS —— 如何在公司之间切换？_**<br>要在公司之间切换，请执行以下操作：
* 在Dynamic Media Classic应用程序中，从“公司”下拉列表中选择新的公司。
* 出现弹出窗口时，点 **[!UICONTROL 击]** “确定”注销并关闭应用程序。

   ![重新启动应用程序以使用新公司](/help/assets/dmclassic-new-company1.png)
* 重新启动Dynamic Media Classic，然后照常登录以使用新公司。

## 提示与技巧

**_我无法在Dynamic Media Classic登陆页上看到“Media Cart（媒体购物车）”面板。_**<br>在Dynamic Media Classic中，点按设**[!UICONTROL 置>个人设置&#x200B;]**。 在“浏览器”部分，确保选**[!UICONTROL 中(已选中&#x200B;]**)“显示媒体门户功能”。 点按**[!UICONTROL 保存>关闭&#x200B;]**。

**_资产的发布状态（绿色指示符）反映不正确。_**<br>在浏览器UI中，需要重新登录UI才能查看资产的正确发布状态。 在桌面应用程序中，我们在工具栏**[!UICONTROL 上&#x200B;]**“选择无”按钮右侧引入了**[!UICONTROL 刷新图标&#x200B;]**。 点按刷**[!UICONTROL 新&#x200B;]**图标，以查看给定页面上所有资产的最新状态。 无需像浏览器UI一样重新登录。

![刷新图标](/help/assets/refresh-icon1.png)*刷新图标*

**_我看不到批集预设在桌面应用程序中工作。_**<br>点按**[!UICONTROL 上传>作业选项>批集预设&#x200B;]**。 确保启用相**[!UICONTROL 关批集预&#x200B;]**设。 单击**[!UICONTROL 保存并提交上传&#x200B;]**。
