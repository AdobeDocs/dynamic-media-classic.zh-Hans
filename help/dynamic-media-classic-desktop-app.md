---
title: Adobe Dynamic Media Classic桌面应用程序 — 现已推出
description: 进一步了解Adobe Dynamic Media Classic桌面应用程序。
contentOwner: rbrough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/introducing_adobe_dynamic_media_classic
feature: Dynamic Media Classic
role: Admin,User
exl-id: 604b4630-4704-4254-84b5-91b33bb19d58
source-git-commit: 3345861b5d65f46071578a81913e6b0a4eeb6b8d
workflow-type: tm+mt
source-wordcount: '2026'
ht-degree: 1%

---

# 现已推出：Adobe Dynamic Media Classic桌面应用程序 {#dynamic-media-classic-desktop-app}

Adobe Dynamic Media Classic用户现在可以访问新的桌面应用程序体验，该体验不再依赖于浏览器中的AdobeFlash技术。

此新应用程序现在可用于Windows®和macOS。

>[!IMPORTANT]
>
>Adobe建议您在2020年10月1日之前安装新的Adobe Dynamic Media Classic桌面应用程序。 这样做可确保在2020年12月31日弃用AdobeFlash Player之前实现顺利过渡。 在该日期之后，您将无法登录到浏览器版本的Adobe Dynamic Media Classic用户界面，该用户界面在产品中标记为Adobe Dynamic Media Classic。

请参阅 [新的Adobe Dynamic Media Classic登录体验现已可用。](/help/new-ui-2020.md)

## Adobe Dynamic Media Classic桌面应用程序的系统要求 {#system-requirements-dmc-app}

Adobe Dynamic Media Classic桌面应用程序与以下操作系统兼容：

* macOS 10.10或更高版本。
* Windows® 7或更高版本。

请参阅 [Adobe Dynamic Media Classic桌面应用程序的系统要求](/help/system-requirements.md).

不会在Adobe Dynamic Media Classic桌面应用程序中为 *次要* 版本。 从次要版本中的修复中受益的客户可以进行升级。

## 已在最新版本(20.22.2)中修复，仅限macOS {#release-feb2022}

* macOS Monterey — 文件上传页面在后续上传时冻结。 <!-- https://jira.corp.adobe.com/browse/ASSETS-7948 -->

## 最新版本中的修复(20.22.1) {#release-jan2022}

* 图像编辑 **[!UICONTROL 保存]** 按钮无法正常工作。
* 在Set编辑器中， **[!UICONTROL 关闭]**, **[!UICONTROL 保存]**&#x200B;和 **[!UICONTROL 另存为]** 在中滚动资产后，按钮会被禁用 **[!UICONTROL 添加资产]** 的上界。
* **[!UICONTROL 播放]** 按钮不起作用。
* 无法输入 `d` 和 `e` in **[!UICONTROL 用户名]** 和 **[!UICONTROL 密码]** 运行macOS蒙特利时的字段。
* 已将剩余的Analytics API移至版本2.0。

## 版本20.21.3中的修复 {#release-sept2021}

* 桌面应用程序上一段时间不活动后看到的资产缩略图损坏。
* 桌面应用程序通常在设置操作后停止响应。
* 在 **[!UICONTROL 测试图像提供]**.

   请参阅 [测试安全测试服务](/help/testing-assets-making-them-public.md#testing-the-secure-testing-service).

* 更新了Adobe Analytics的身份验证机制。 与新集成相关，或者是否必须从Dynamic Media Classic桌面应用程序中更新某些Analytics变量。

   请参阅 [登录Adobe Analytics](/help/log-analytics.md) 以了解更新的步骤。

## 版本20.21.2中的修复 {#minor-release}

* 20.21.1中的已知限制：the **[!UICONTROL 服务器]** 登录屏幕上的下拉列表为空。
* 在 **[!UICONTROL 上载作业选项]**，图层命名默认值位于 **[!UICONTROL Photoshop选项]**，现在 **[!UICONTROL Photoshop和层名称]**. PSD 文件中的图层以单独图像形式上载。
   * 早期的 **[!UICONTROL 层名称]**，在图像的层名称或层号后命名PSD文件。 如果PSD文件中的层名称是默认的Photoshop层名称，则使用层编号。
   * 的新默认值 **[!UICONTROL Photoshop和层名称]**，在PSD文件后面命名图像，后跟图层名称或图层编号。 如果 PSD 文件中的图层名称是默认的 Photoshop 图层名称，则将使用图层编号。
   * 鉴于Adobe Dynamic Media Classic中的层图像现在具有唯一的名称，将不会更新现有PSD或模板(原始PSD文件中共享的层名称)。
* 资产的缩略图损坏。

## 版本20.21.1中的修复 {#latest-fixes-desktop-app}

* 由于超时导致出现登录问题，导致出现以下消息： *未经权限，可以将此用户分配给组或组。 请联系您的管理员。*
* 查看器预设重复，每次密码尝试都不正确。
* 由于根文件夹中的许多资产，桌面应用程序变得无响应。 (已在Windows®上修复；根据需要在macOS上工作。)

## 版本20.20.2中的修复 {#previous-version-fixes-desktop-app}

* 对于可通过桌面应用程序用户界面上传的文件数量，无限制，适用于macOS和Windows®。
* 无需注销桌面应用程序即可在公司之间进行切换。
* 现在，Ctrl+V可在Windows®上执行粘贴操作。
* 将来，当桌面应用程序的新版本发布时，用户将在桌面应用程序内收到通知。

## 在macOS或Windows®上下载并安装最新的Adobe Dynamic Media Classic桌面应用程序 {#installation-dmc-app}

另请参阅:

* [在Mac上下载并静默安装最新的Adobe Dynamic Media Classic桌面应用程序](#install-silent-mac-dmc-app)
* [在Windows®上下载并静默安装最新的Adobe Dynamic Media Classic桌面应用程序](#install-silent-windows-dmc-app)

1. 在您的系统上卸载任何旧版Adobe Dynamic Media Classic桌面应用程序版本。

1. 下载最新的Adobe Dynamic Media Classic桌面应用程序安装程序。

   * 最新版本可在以下位置获取：

      * [macOS(.DMG) — 下载](https://download.macromedia.com/dynamic-media-classic/20.22.2/adobe-dynamic-media-classic-20.22.2.dmg)
      * [Windows(.EXE) — 下载](https://download.macromedia.com/dynamic-media-classic/20.22.1/adobe-dynamic-media-classic-20.22.1.exe)
   * 以前的版本可在以下位置使用：

      * [macOS(.DMG) — 下载](https://download.macromedia.com/dynamic-media-classic/20.22.1/adobe-dynamic-media-classic-20.22.1.dmg)
      * [Windows®(.EXE) — 下载](https://download.macromedia.com/dynamic-media-classic/20.21.3/adobe-dynamic-media-classic-20.21.3.exe)


<!--         * [macOS (.DMG) - Download](https://download.macromedia.com/dynamic-media-classic/20.21.3/adobe-dynamic-media-classic-20.21.3.dmg) -->

<!--    * [macOS (.DMG) - Download](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.dmg)
        * [Windows® (.EXE) - Download](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.exe) -->

<!--    * [macOS (.DMG) - Download.](https://download.macromedia.com/dynamic-media-classic/20.20.2/adobe-dynamic-media-classic-20.20.2.dmg)
        * [Windows (.EXE) - Download.](https://download.macromedia.com/dynamic-media-classic/20.20.2/adobe-dynamic-media-classic-20.20.2.exe) -->


1. 根据您下载的安装程序执行下列操作之一。

   * **macOS**  — 在 **[!UICONTROL 拖放以安装]** 对话框，拖动 **[!UICONTROL Adobe Dynamic Media Classic]** 然后放到 **[!UICONTROL 应用程序]**.

      ![在macOS上拖放安装](/help/assets/dragondrop-install1.png)

   * 在 **[!UICONTROL 应用程序]** 文件夹中，点按Adobe Dynamic Media Classic图标。
   * 在对话框中，点按 **[!UICONTROL 打开]** 打开Adobe Dynamic Media Classic桌面应用程序。

      ![打开下载的应用程序](/help/assets/open-dmclassicapp1.png)

   * **Windows**  — 运行安装程序二进制文件，并按照屏幕上的说明安装桌面应用程序。

1. 打开应用程序时，将显示新的Adobe Dynamic Media Classic登录页面：

   ![Adobe Dynamic Media Classic登录](/help/assets/dmclassic-login1.png)

1. 要登录到Adobe Dynamic Media Classic桌面应用程序，请使用与您在浏览器中登录Adobe Dynamic Media Classic时所用的凭据相同的凭据。

   对于 **[!UICONTROL 服务器]** 要使用，请参阅生产环境的以下映射：

   | 服务器 | 浏览器URL |
   | --- | --- |
   | NA Production（北美） | https://s7sps1.scene7.com/ |
   | EMEA生产（欧洲、中东和非洲） | https://s7sps3.scene7.com/ |
   | APAC生产（亚太地区） | https://s7sps5.scene7.com/ |

1. 登录后，请注意熟悉的浏览器用户界面体验。 您可以像往常一样，在桌面应用程序上继续日常的Adobe Dynamic Media Classic活动。

## 下载和 *沉默* 在macOS上安装最新的Adobe Dynamic Media Classic桌面应用程序 {#install-silent-mac-dmc-app}

另请参阅:

* [在Mac或Windows®上下载并安装最新的Adobe Dynamic Media Classic桌面应用程序](#installation-dmc-app)
* [在Windows®上下载并静默安装最新的Adobe Dynamic Media Classic桌面应用程序](#install-silent-windows-dmc-app)

下载和 *沉默* 在macOS上安装最新版本的Adobe Dynamic Media Classic桌面应用程序：

1. 在您的系统上卸载任何旧版Adobe Dynamic Media Classic桌面应用程序版本。

1. 下载适用于macOS的Adobe Dynamic Media Classic桌面应用程序的最新安装程序。

   * [macOS(.DMG) — 下载](https://download.macromedia.com/dynamic-media-classic/20.22.2/adobe-dynamic-media-classic-20.22.2.dmg)

1. 使用以下命令将下载的磁盘映像(.DMG)装载到安装点位置：

   `hdiutil attach adobe-dynamic-media-classic-20.22.2.dmg -mountpoint <mount_point_path>`

1. 将.APP文件复制到 **[!UICONTROL 应用程序]** 使用以下命令：

   ```
   rsync -a <mount_point_path>/Adobe\ Dynamic\ Media\ Classic.app /Applications/
   Unmount DMG - hdiutil detach <mount_point_path>
   ```

1. 打开应用程序时，将显示新的Adobe Dynamic Media Classic登录页面：

   ![Adobe Dynamic Media Classic登录](/help/assets/dmclassic-login1.png)

1. 要登录到Adobe Dynamic Media Classic桌面应用程序，请使用与您在浏览器中登录Adobe Dynamic Media Classic时所用的凭据相同的凭据。

   对于 **[!UICONTROL 服务器]** 要使用，请参阅生产环境的以下映射：

   | 服务器 | 浏览器URL |
   | --- | --- |
   | NA Production（北美） | https://s7sps1.scene7.com/ |
   | EMEA生产（欧洲、中东和非洲） | https://s7sps3.scene7.com/ |
   | APAC生产（亚太地区） | https://s7sps5.scene7.com/ |

## 下载和 *沉默* 在Windows®上安装最新的Adobe Dynamic Media Classic桌面应用程序 {#install-silent-windows-dmc-app}

您使用的命令用于基本的MSI静默安装。 但是，Adobe Dynamic Media Classic桌面应用程序安装程序是使用InstallShield创建的InstallScript MSI安装程序。 在记录模式下运行安装程序时，任何用户交互都会记录在响应文件中。 然后，将此响应文件用于静默安装，如 [在静默模式下运行安装。](https://docs.revenera.com/installshield19helplib/helplibrary/SilentInstall.htm)

另请参阅:

* [在Mac或Windows®上下载并安装最新的Adobe Dynamic Media Classic桌面应用程序](#installation-dmc-app)
* [在macOS上下载并静默安装最新的Adobe Dynamic Media Classic桌面应用程序](#install-silent-mac-dmc-app)

下载和 *沉默* 在Windows®上安装最新版本的Adobe Dynamic Media Classic桌面应用程序：

1. 在您的系统上卸载任何旧版Adobe Dynamic Media Classic桌面应用程序版本。

1. 下载最新的Adobe Dynamic Media Classic桌面应用程序安装程序。

   * [Windows®(.EXE) — 下载](https://download.macromedia.com/dynamic-media-classic/20.22.1/adobe-dynamic-media-classic-20.22.1.exe)

1. 使用以下命令在记录模式下运行安装程序：

   `adobe-dynamic-media-classic-20.22.1.exe /r /f1"C:\Setup.iss"`

1. 在GUI安装程序窗口中，按照要安装的步骤进行安装，以便将交互/输入（如安装位置）记录在 `Setup.iss` 文件。

1. 复制已创建的 `Setup.iss` 文件和 `adobe-dynamic-media-classic-20.22.1.exe` 到其他计算机。

1. 为静默安装运行以下命令：

   `adobe-dynamic-media-classic-20.22.1.exe /s /f1"C:\Setup.iss"`

   有关命令行参数的详细信息，请访问 [Setup.exe和Update.exe命令行参数。](https://docs.revenera.com/installshield19helplib/helplibrary/IHelpSetup_EXECmdLine.htm)

1. 打开应用程序时，将显示新的Adobe Dynamic Media Classic登录页面：

   ![Adobe Dynamic Media Classic登录](/help/assets/dmclassic-login1.png)

1. 要登录到Adobe Dynamic Media Classic桌面应用程序，请使用与您在浏览器中登录Adobe Dynamic Media Classic时所用的凭据相同的凭据。

   对于 **[!UICONTROL 服务器]** 要使用，请参阅生产环境的以下映射：

   | 服务器 | 浏览器URL |
   | --- | --- |
   | NA Production（北美） | https://s7sps1.scene7.com/ |
   | EMEA生产（欧洲、中东和非洲） | https://s7sps3.scene7.com/ |
   | APAC生产（亚太地区） | https://s7sps5.scene7.com/ |

## 使用Adobe Dynamic Media Classic桌面应用程序的视频演示 {#dmc-app-video-walk-through}

观看 [使用Adobe Dynamic Media Classic桌面应用程序的视频演示](https://experienceleague.adobe.com/docs/experience-manager-learn/assets/dynamic-media/dynamic-media-classic-desktop-application.html#dynamic-media) (长度：2分36秒)。

## 使用桌面应用程序清除计算机上的图像缓存和资产缓存 {#clear-cache}

1. 在Adobe Dynamic Media Classic桌面应用程序的右上角附近，点按 **[!UICONTROL 设置]** > **[!UICONTROL 个人设置]**.
1. 在 **[!UICONTROL 个人设置]** 页面下 **[!UICONTROL 桌面]** 标题中，执行以下任一操作：
   * 要从您的计算机中删除所有AdobeDynamic Media缓存的图像文件，请点按 **[!UICONTROL 清除图像缓存]**，然后点按 **[!UICONTROL 确定]**.
   * 要从您的计算机中删除所有AdobeDynamic Media缓存的资产文件，请点按 **[!UICONTROL 清除资产缓存]**，然后点按 **[!UICONTROL 确定]**.
1. 在页面的右下角，点按 **[!UICONTROL 关闭]**.

### 手动清除图像缓存和资产缓存

除了使用桌面应用程序清除图像和资产缓存之外，您还可以直接从文件系统手动清除缓存。

1. 根据您的操作系统，导航到以下内容：

   * macOS: `~/Library/Application\ Support/com.adobe.DMCDesktop/Local\ Store/`
   * Windows®: `C:\Users\YourUserName\AppData\Roaming\com.adobe.DMCDesktop\Local Store`

## Adobe Dynamic Media Classic中的已知限制20.21.1

* 的 **[!UICONTROL 服务器]** 更新到Adobe Dynamic Media Classic桌面应用程序20.21.1后，下拉列表为空 — 方案：安装并登录到Adobe Dynamic Media Classic 20.20.1或20.20.2，然后关闭应用程序。 然后更新到Adobe Dynamic Media Classic 20.21.1。当您尝试登录时， **[!UICONTROL 服务器]** 下拉列表 **[!UICONTROL 登录到您的帐户]** 对话框为空。 要解决此问题，您必须 [手动清除缓存](#clear-cache) （请参阅上述步骤）。

## Adobe Dynamic Media Classic 20.20.1的已知限制(已在20.20.2中修复)

**_仅适用于Windows® — 是否对可通过桌面应用程序用户界面上传的文件数量存在限制？_**<br>是，一次最多可通过桌面应用程序UI上传150个文件。

**_适用于Windows®和macOS — 如何在公司之间切换？_**<br>要在公司之间切换，请执行以下操作：

* 在Adobe Dynamic Media Classic应用程序中，从公司下拉列表中选择新公司。
* 出现弹出窗口时，点按 **[!UICONTROL 确定]** 注销并关闭应用程序。

   ![要使用新公司，请重新启动应用程序](/help/assets/dmclassic-new-company1.png)

* 重新启动Adobe Dynamic Media Classic，然后照常登录以与新公司合作。

## 提示和技巧

**_我在Adobe Dynamic Media Classic的登陆页面上看不到“媒体购物车”面板。_**<br>在Adobe Dynamic Media Classic中，点按**[!UICONTROL 设置>个人设置&#x200B;]**. 在浏览器部分，确保**[!UICONTROL 显示媒体门户功能&#x200B;]**已选择（选中）。 点按**[!UICONTROL 保存>关闭&#x200B;]**.

**_资产的发布状态（绿色指示器）未正确反映。_**<br>在浏览器用户界面中，需要重新登录UI才能查看正确的资产发布状态。 在桌面应用程序中，Adobe引入了**[!UICONTROL 刷新&#x200B;]**图标**[!UICONTROL 选择无&#x200B;]**按钮。 点按**[!UICONTROL 刷新&#x200B;]**图标，以查看给定页面上所有资产的最新状态。 与使用浏览器UI时一样，无需重新登录。

![“刷新”图标](/help/assets/refresh-icon1.png)
*“刷新”图标*

**_我看不到批量集预设在桌面应用程序中工作。_**<br>点按**[!UICONTROL 上传>作业选项>批集预设&#x200B;]**. 确保**[!UICONTROL 批集预设&#x200B;]**启用。 单击**[!UICONTROL 保存并提交上传&#x200B;]**.
