---
title: 管理设置
description: 了解如何设置Dynamic Media Classic的管理区域。
uuid: 16ba9fed-b5c6-4991-83b3-8d7d7129013a
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 3c9ee4ec-dd37-498d-98d6-1339b80177ff
feature: Dynamic Media Classic
role: Admin
exl-id: 14e3d8be-f265-4cec-aa8e-19ef71526b68
source-git-commit: 1d30c98b76ebe78ff60bae87bd112de7a577182d
workflow-type: tm+mt
source-wordcount: '1948'
ht-degree: 37%

---

<!-- UPDATE TOPIC AFTER DECEMBER 31, 2020!!!! -->

# 管理设置{#administration-setup}

“管理设置”屏幕用于管理Dynamic Media Classic用户。 使用这些屏幕，用户可以在Dynamic Media Classic中工作，并通过电子邮件与用户通信。

1. 要访问“管理设置”选项，请转到&#x200B;**设置** > **个人设置** > **管理设置**。

## 用户管理 {#user-administration}

所有Dynamic Media Classic用户都将分配一个角色，以确定其权限和对Dynamic Media Classic中各项功能的访问权限。 管理员会为自己负责的公司确定不同角色和职责。

通常，Dynamic Media Classic会配置第一组公司并分配公司管理员。 然后，公司管理员可以设置并管理Dynamic Media Classic用户。

Dynamic Media Classic支持多个用户角色。 这些角色可以访问为Dynamic Media Classic设置的公司：

<!-- **Adobe Dynamic Media Classic Administrator** Can view and administer all features in Dynamic Media Classic, as well as set up companies and add administrators and users. -->

**AdobeDynamic Media** Classic UserCan访问他们分配到的公司；不能履行管理职责。

**AdobeDynamic Media Classic公司管** 理员只能查看和管理自己的公司。公司管理员还可以执行所有管理功能，包括添加管理员和用户。公司管理员可以将用户添加到DMC公司管理员帐户。 （该角色是默认用户角色。）

添加用户后，Dynamic Media Classic会向该用户发送一封欢迎电子邮件。 该消息包含密码和Dynamic Media Classic URL。

### 添加用户或管理员 {#adding-a-user-or-administrator}

1. 转到&#x200B;**[!UICONTROL 设置]** > **[!UICONTROL 应用程序设置]** > **[!UICONTROL 管理设置]** > **[!UICONTROL 用户管理]**。
1. 选择&#x200B;**[!UICONTROL Add]**。
1. 输入要添加的用户或管理员的姓名和电子邮件地址，然后选择&#x200B;**[!UICONTROL Next]**。

   >[!NOTE]
   >
   >电子邮件地址中不允许使用撇号字符(`‘`)。

1. 要为用户分配角色，请选择角色选项。

   请参阅[Dynamic Media Classic用户角色和权限](administration-setup.md#user_administration)。

1. 要将用户添加到公司，请选择公司名称。
1. 如果要将用户添加到群组（如果要添加Media Portal用户或参与者），请选择&#x200B;**[!UICONTROL Next]**&#x200B;并添加该用户。
1. 选择&#x200B;**[!UICONTROL Save]**&#x200B;以完成用户设置。

   保存之后，系统将提示您是否要将用户添加到其他公司。如果要将用户添加到公司，请选择&#x200B;**[!UICONTROL Add]**。

   给所有新用户随机生成的密码；用户首次登录Dynamic Media Classic桌面应用程序时，需要更改密码。

   在您添加新用户后，会向他们发送欢迎电子邮件。该电子邮件提供了临时密码，并说明了如何登录到Dynamic Media Classic。

   如果用户未收到欢迎电子邮件，请让他们转到Dynamic Media Classic登录页面(https://s7sps1.scene7.com)，然后选择&#x200B;**[!UICONTROL 忘记密码]**。 将重置密码并发送新的电子邮件。如果用户未收到电子邮件，并且该电子邮件不在“垃圾邮件”文件夹中，请联系技术支持人员。

   添加新的Media Portal用户时，您还可以转到&#x200B;**[!UICONTROL 设置]** > **[!UICONTROL 应用程序设置]** > **[!UICONTROL 用户管理]**，然后选择&#x200B;**[!UICONTROL 上传用户列表]**&#x200B;并选择一个不超过500个用户的.csv文件。

### 删除用户 {#deleting-a-user}

您可以通过将用户设为无效，从Dynamic Media Classic中删除这些用户。 无效用户会从系统和所有帐户中被删除。

1. 转到&#x200B;**[!UICONTROL 设置]** > **[!UICONTROL 应用程序设置]** > **[!UICONTROL 管理设置]** > **[!UICONTROL 用户管理]**。
1. 从列表中选择用户，然后选择&#x200B;**[!UICONTROL 编辑]**。
1. 取消选择“有效”。
1. 选择&#x200B;**[!UICONTROL Save]**。

### 激活或停用用户 {#activating-or-deactivating-users}

已被停用的用户不再具有进入在“选择要访问的帐户”菜单的顶部列出的帐户的权限。

1. 转到&#x200B;**[!UICONTROL 设置]** > **[!UICONTROL 应用程序设置]** > **[!UICONTROL 管理设置]** > **[!UICONTROL 用户管理]**。
1. 在用户列表中，选择或取消选择用户名旁边的&#x200B;**[!UICONTROL 活动]**&#x200B;选项。

### 编辑用户信息 {#editing-user-information}

您可以编辑的用户信息取决于您的管理员角色以及要编辑其信息的用户被指定的角色。变暗（不可用）的选项不可编辑。

1. 转到&#x200B;**[!UICONTROL 设置]** > **[!UICONTROL 应用程序设置]** > **[!UICONTROL 管理设置]** > **[!UICONTROL 用户管理]**。
1. 从列表中选择用户，然后选择&#x200B;**[!UICONTROL 编辑]**。
1. 选择表中显示您尝试修改其权限或访问权限的公司的条目，然后选择&#x200B;**[!UICONTROL 管理公司]**。
1. 选择用户角色。
1. 如果要更改用户的群组成员资格（如果正在编辑或添加Media Portal用户或参与者），请选择&#x200B;**[!UICONTROL 下一步]**&#x200B;并编辑群组成员资格。
1. 选择&#x200B;**[!UICONTROL Save]**。

### 对用户列表进行过滤和排序 {#filtering-and-sorting-the-user-list}

您可以通过过滤和排序用户列表来找到用户。无论在“选择要访问的帐户”菜单中选择哪个帐户，您管理的所有帐户中的所有用户都会显示在“用户”列表中。

您可以使用以下用户列表过滤技术：

* **按组过滤**  — 选择按 **[!UICONTROL 组]** 菜单，然后选择一个选项以将列表缩小到组中的用户。

* **按用户角色过滤**  — 选择按用 **[!UICONTROL 户]** 角色菜单，然后选择一个选项以将列表范围缩小到不同类型的用户或管理员。

* **按字段名称过滤**  — 选择“ **[!UICONTROL 启用按字段过滤]**”。然后选择&#x200B;**[!UICONTROL 按字段名称]**&#x200B;菜单，选择列以过滤列表，然后选择“过滤字符”菜单并选择字母。 按您所选的字母在其中一列上过滤列表。要查看完整列表，请取消选择&#x200B;**[!UICONTROL 按字段启用过滤器]**&#x200B;选项。

* **过滤掉无效用户**  — 取消选 **[!UICONTROL 择包括无效]**。搜索结果只显示系统中的用户。已从系统和您管理的帐户删除了无效用户。

* **按列标题排序**  — 选择一个标题，按用户的状态（按名字、姓氏或电子邮件的字母顺序）、用户角色或有效/无效状态对所有用户进行排序。

如果您有许多用户，可以通过选择“最大列表大小”菜单并选择一个数值来限制列表的大小。

<!-- CQDOC-16690 TOPIC REMOVED AS PER JIRA TICKET INSTRUCTIONS ### Linking an IMS user identity to a Dynamic Media Classic IPS user account {#linking-an-ims-user-identity-to-a-scene-ips-user-account}

You can link an Adobe IMS user identity to a Dynamic Media Classic IPS user account so you can use SSO (Single Sign On) to log on and launch Scene7 Publishing System from within Adobe Marketing Cloud.

1. Adobe should already have setup your account with an Adobe Marketing Cloud organization and linked it to your Scene7 Publishing System product context. If this setup is not yet done or you are unsure if it has been done, contact Adobe Customer Care.

   When the setup is complete, you can can log on to Adobe Marketing Cloud and link your Adobe Marketing Cloud identity to your Dynamic Media Classic user account by doing the following.

1. In Adobe Marketing Cloud, navigate to your account settings.
1. Select **Manage Organizations**.
1. Select **Link Account** or **Get Access**.
1. Select **Experience Manager**, and then type your credentials.

   Your credentials include your IPS company region, email address, and password.

1. Select **Link**.
1. When the link is set, you can launch Scene7 Publishing System from within Adobe Marketing Cloud, or you can launch it directly.

   Do one of the following:

    * To launch Dynamic Media Classic from within Adobe Marketing Cloud, in the left rail of Adobe Marketing Cloud, select **Solutions** > **Experience Manager**. Under the Dynamic Media Classic card, select **Launch**.
    * To log on to Scene7 Publishing System directly using your IMS credentials, use the following website:

      https://s7spsN.scene7.com/IpsWeb?ims=1

      Replace “N” in the above path with the number for your IPS company region. That is, N = 1 for North America; 3 for EMEA; or 5 for JAPAC.
 -->

## 带宽和存储 {#bandwidth-storage}

Dynamic Media Classic管理员可以为其管理的公司生成带宽、存储和其他类型的报表。 这些报表可在“带宽和存储”页面上找到。

要打开此页，请转到&#x200B;**[!UICONTROL Setup]** > **[!UICONTROL Personal Setup]**。 展开&#x200B;**[!UICONTROL 管理设置]**，然后选择&#x200B;**[!UICONTROL 带宽和存储]**。

### 报告类型 {#types-of-reports}

下表介绍了可从“带宽和存储”页面生成的报表：

| 报告 | 信息 | 用途 |
|:--- |:--- |:--- |
| 带宽 | 公司的带宽使用情况 | 跟踪公司在特定日期范围内的带宽使用量，以确定流量模式。 |
| 存储 | 存储使用情况 | 跟踪公司上载的数据量。 |
| 图像内容 | 按类型划分的图像请求数目 | 跟踪不同图像类型的请求数量和容量。 |
| 域 | 按域划分的 URL 请求数目 | 根据特定公司的图像请求的域，跟踪图像使用情况。(Dynamic Media Classic每个帐户可以提供多个域。 有关更多信息，请联系技术支持。） |
| 视频流 | 流视频的带宽使用情况 | 跟踪公司在特定日期范围内的流视频使用情况，以确定流量模式。 |
| 视频内容 | 不同视频的播放时间 | 确定哪些是最常观看和最少观看的视频。 |

“图像内容”报告提供了对以下图像类型所发出的请求的信息：

* **图像请求**  — 图像请求。

* **缩略图请求**  — 在查看器中请求色板或替代图像。

* **蒙版请求**  — 对返回灰度级掩码的图像的请求。

* **查看器拼贴请求**  — 查看器加载的图像请求。

* **Vnt对象请求**  — 图像渲染请求，用于返回在请求的晕影中具有指定对象的图像。

* **Vnt信息请求**  — 返回有关所请求晕影的信息的图像渲染请求。

>[!NOTE]
>
>“视频流”报告仅应用于流视频。它不跟踪对渐进式视频的观看情况。

### 生成报表 {#generating-a-report}

生成带宽、存储、图像内容、域、视频流或视频内容报告：

1. 转到&#x200B;**[!UICONTROL Setup]** > **[!UICONTROL Personal Setup]**。
1. 展开“管理设置”，然后选择“带宽和存储”]**。**[!UICONTROL 
1. 选择选项卡：**[!UICONTROL 带宽]**、**[!UICONTROL 存储]**、**[!UICONTROL 图像内容]**、**[!UICONTROL 域]**、**[!UICONTROL 视频流]**&#x200B;或&#x200B;**[!UICONTROL 视频内容]**。

   请参阅[报告类型](administration-setup.md#types_of_reports)。

### 以不同方式查看数据 {#viewing-data-in-different-ways}

在“带宽与存储”页面上生成报告后，您可以选择用于查看信息的选项。您可以选择如何显示信息，如何在图表或数据网格中查看信息，以及指定用于捕获信息的时间段。在“数据”视图中，您还可以排序信息并重新排列各个列。

* **在图表或数据网格中查看数据**  — 选择“图表” **[!UICONTROL 查]** 看图表中的数据；选择 **[!UICONTROL 数据]** 查看数据网格中的数据。

* **选择报表演示类型**  — 在“报表类型”菜单上，选择 **[!UICONTROL 摘要]**、 **[!UICONTROL 每日]**&#x200B;或 **** 月份，以摘要形式、按日或按月组织数据。并非所有报告都提供该选项。

* **指定时间段**  — 选择选项以定义报表的时间段，然后在定 **** 义时间段后选择更新：

* **预定义时间段**  — 在“预定义报表”菜单中，选择一个选项。例如，选择“上月”以捕获上月的数据。

* **自定义时间段**  — 在“预定义报表”菜单上，选择“自 **[!UICONTROL 定义]**”。然后，在&#x200B;**[!UICONTROL 开始月份]**（或&#x200B;**[!UICONTROL 开始日期]**）菜单上选择日期，在月数（或天数）菜单上选择日期。 对于域报告和视频内容报告，您可以为捕获报告信息选择特定的开始和结束日期。

* **对数据排序（仅限数据视图）**  — 要对列的信息进行排序，请选择列的标题。再次选择以按降序排序。

* **重新排列列（仅限数据视图）**  — 要将列移动到数据网格上的其他位置，请拖动其标题。

### 导出和打印报表 {#exporting-and-printing-reports}

在生成报告后，您可以导出其数据，在电子表格和其他应用程序中使用。您还可以打印报告。

* **导出报表数据**  — 在“数据”视图中，根据需要对数据进行排序和排列。然后打开&#x200B;**[!UICONTROL Export]**&#x200B;菜单并选择格式：**[!UICONTROL 制表符分隔]**、**[!UICONTROL 逗号分隔]**&#x200B;或&#x200B;**[!UICONTROL 格式化的HTML]**。 按您所选的格式将数据复制到剪贴板。现在，您可以将数据粘贴到电子表格或应用程序中。

* **打印报表**  — 选择 **[!UICONTROL 打印]**，在“打印”对话框中选择所需的选项，然后选择“ **[!UICONTROL 确定]**”。

## 图像错误 {#image-errors}

Dynamic Media Classic管理员可以生成图像错误报表。 “图像错误”报告针对您当前登录的公司，提供了过去 24 小时内 20 个最常见的图像错误。要生成“图像错误”报告，请执行以下操作：

1. 转到&#x200B;**[!UICONTROL Setup]** > **[!UICONTROL Personal Setup]**。
1. 展开“管理设置”，然后选择“**[!UICONTROL 图像错误]**”。
1. （可选）请执行下列操作之一：

   * 要按标题信息对错误进行排序，请选择一个标题。 默认情况下，按发生次数，从最高到最低排序错误。
   * 将光标移动到错误的“响应”字段上，可查看具体的错误消息。
   * 要查看指向图像或反向链接网页的链接，请将光标移到URL字段或反向链接字段上。
   * 要将链接复制到实际图像，请选择&#x200B;**[!UICONTROL URL复制URL]**。 您可以在浏览器窗口中粘贴此链接，以转到该图像并检查错误。
   * 要将链接复制到反向链接网页，请选择&#x200B;**[!UICONTROL 反向链接复制URL]**。

显示的错误适用于您目前登录的公司。每个错误都包括以下信息：

* **图像ID**  — 违规图像的ID。

* **时间**  — 在过去24小时内，第一次报告错误到上次报告错误的时间范围。

* **计数**  — 图像上报告的错误数。

* **响应**  — 特定的错误消息。错误是 4xx 或者 5xx。

* **URL**  — 列出指向Dynamic Media Classic上图像的URL。

* **反向链接**  — 指定初始请求来自的网站的URL。引用网站可以是具有指向图像的链接的任何网站。

“URL”和“引用网站”列都有与之相关的“复制 URL”以简化测试。
