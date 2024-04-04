---
title: 管理设置
description: 了解如何设置Adobe Dynamic Media Classic的管理区域。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic
role: Admin
exl-id: 14e3d8be-f265-4cec-aa8e-19ef71526b68
topic: Administration
level: Intermediate
source-git-commit: f054057d383b26e9088582f418f62504c3f327d8
workflow-type: tm+mt
source-wordcount: '1971'
ht-degree: 33%

---

<!-- UPDATE TOPIC AFTER DECEMBER 31, 2020!!!! -->

# 管理设置{#administration-setup}

“管理设置”屏幕用于管理Adobe Dynamic Media Classic用户。 使用这些屏幕使用户能够在Adobe Dynamic Media Classic中工作并通过电子邮件与用户通信。

1. 要访问管理设置选项，请转到 **设置** > **个人设置** > **管理设置**.

## 用户管理 {#user-administration}

将为所有Adobe Dynamic Media Classic用户分配一个角色，该角色可确定用户对Adobe Dynamic Media Classic中各项功能的权限和访问权限。 管理员会为自己负责的公司确定不同角色和职责。

通常，Adobe Dynamic Media Classic会配置第一组公司并分配公司管理员。 然后，公司管理员将设置和管理Adobe Dynamic Media Classic用户。

Adobe Dynamic Media Classic支持多个用户角色。 这些角色可以访问为Adobe Dynamic Media Classic设置的公司：

<!-- **Adobe Dynamic Media Classic Administrator** Can view and administer all features in Adobe Dynamic Media Classic, as well as set up companies and add administrators and users. -->

**Adobe Dynamic Media Classic用户** 可以访问已向其分配他们的公司；无法执行任何管理职责。

**Adobe Dynamic Media Classic公司管理员** 只能查看和管理自己的公司。 公司管理员还可以执行所有管理功能，包括添加管理员和用户。公司管理员可以将用户添加到DMC公司管理员帐户。 （该角色是默认用户角色。）

添加用户后，Adobe Dynamic Media Classic会向用户发送欢迎电子邮件。 该消息包含密码和Adobe Dynamic Media Classic URL。

### 添加用户或管理员 {#adding-a-user-or-administrator}

1. 转到 **[!UICONTROL 设置]** > **[!UICONTROL 应用程序设置]** > **[!UICONTROL 管理设置]** > **[!UICONTROL 用户管理]**.
1. 选择 **[!UICONTROL 添加]**.
1. 输入要添加的用户或管理员的名称和电子邮件地址，然后选择 **[!UICONTROL 下一个]**.

   >[!NOTE]
   >
   >撇号字符(`'`)不允许在电子邮件地址中使用。

1. 要向用户分配角色，请选择角色选项。

   请参阅 [Adobe Dynamic Media Classic用户角色和权限](administration-setup.md#user_administration).

1. 要将用户添加到公司，请选择公司名称。
1. 如果要将用户添加到组（如果要添加Media Portal用户或参与者），请选择 **[!UICONTROL 下一个]** 并添加用户。
1. 选择 **[!UICONTROL 保存]** 以完成用户设置。

   保存之后，系统将提示您是否要将用户添加到其他公司。选择 **[!UICONTROL 添加]** 如果要将用户添加到公司。

   所有新用户都将获得随机生成的密码；用户在首次登录到Adobe Dynamic Media Classic桌面应用程序时需要更改密码。

   在您添加新用户后，会向他们发送欢迎电子邮件。电子邮件会提供临时密码并介绍如何登录到Adobe Dynamic Media Classic。

   如果用户没有收到欢迎电子邮件，请让他们转到Adobe Dynamic Media Classic登录页面(https://s7sps1.scene7.com)，然后选择 **[!UICONTROL 忘记我的密码]**. 将重置密码并发送新的电子邮件。如果用户未收到电子邮件，并且该电子邮件不在“垃圾邮件”文件夹中，请联系技术支持人员。

   添加新Media Portal用户时，您还可以转到 **[!UICONTROL 设置]** > **[!UICONTROL 应用程序设置]** > **[!UICONTROL 用户管理]**，然后选择 **[!UICONTROL 上载用户列表]** 并选择一个.csv文件，其中包含的用户的数量不超过500个。

### 删除用户 {#delet-a-user}

您可以通过将用户设为无效来从Adobe Dynamic Media Classic中删除这些用户。 无效用户会从系统和所有帐户中被删除。

1. 转到 **[!UICONTROL 设置]** > **[!UICONTROL 应用程序设置]** > **[!UICONTROL 管理设置]** > **[!UICONTROL 用户管理]**.
1. 从列表中选择用户，然后选择 **[!UICONTROL 编辑]**.
1. 取消选择“有效”。
1. 选择 **[!UICONTROL 保存]**.

### 激活或停用用户 {#activating-or-deactivating-users}

已被停用的用户不再具有进入在“选择要访问的帐户”菜单的顶部列出的帐户的权限。

1. 转到 **[!UICONTROL 设置]** > **[!UICONTROL 应用程序设置]** > **[!UICONTROL 管理设置]** > **[!UICONTROL 用户管理]**.
1. 在用户列表中，选择或取消选择 **[!UICONTROL 活动]** 用户名称旁边的选项。

### 编辑用户信息 {#editing-user-information}

您可以编辑的用户信息取决于您的管理员角色以及要编辑其信息的用户被指定的角色。变暗（不可用）的选项不可编辑。

1. 转到 **[!UICONTROL 设置]** > **[!UICONTROL 应用程序设置]** > **[!UICONTROL 管理设置]** > **[!UICONTROL 用户管理]**.
1. 从列表中选择用户，然后选择 **[!UICONTROL 编辑]**.
1. 选择表中显示您尝试修改其权限或访问权限的公司的条目，然后选择 **[!UICONTROL 管理公司]**.
1. 选择用户角色。
1. 如果要更改用户的组成员资格（如果要编辑或添加Media Portal用户或参与者），请选择 **[!UICONTROL 下一个]** 并编辑组成员资格。
1. 选择 **[!UICONTROL 保存]**.

### 对用户列表进行过滤和排序 {#filtering-and-sorting-the-user-list}

您可以通过过滤和排序用户列表来找到用户。无论在“选择要访问的帐户”菜单中选择哪个帐户，您管理的所有帐户中的所有用户都会显示在“用户”列表中。

您可以使用以下用户列表过滤技术：

* **按组筛选**  — 选择 **[!UICONTROL 按组]** 并选择一个选项以将列表范围缩小到组中的用户。

* **按用户角色筛选**  — 选择 **[!UICONTROL 按用户角色]** 并选择一个选项以将列表范围缩小到不同类型的用户或管理员。

* **按字段名称筛选**  — 选择 **[!UICONTROL 启用按字段筛选]**. 然后选择 **[!UICONTROL 按字段名称]** 菜单，选择用于筛选列表的列，然后选择“筛选字符”菜单并选择字母。 列表会按您选择的字母在某一列上过滤。 要查看完整列表，请取消选择 **[!UICONTROL 启用按字段筛选]** 选项。

* **过滤掉无效用户**  — 取消选择 **[!UICONTROL 包含无效]**. 搜索结果只显示系统中的用户。已从系统和您管理的帐户中删除无效用户。

* **按列标题排序**  — 选择标题以按状态对所有用户进行排序，按名字、姓氏或电子邮件的字母顺序、用户角色或有效/无效状态进行排序。

如果您有许多用户，可以通过选择“最大列表大小”菜单并选择一个数值来限制列表的大小。

<!-- CQDOC-16690 TOPIC REMOVED AS PER JIRA TICKET INSTRUCTIONS ### Linking an IMS user identity to an Adobe Dynamic Media Classic IPS user account {#linking-an-ims-user-identity-to-a-scene-ips-user-account}

You can link an Adobe IMS user identity to an Adobe Dynamic Media Classic IPS user account so you can use SSO (Single Sign On) to log on and launch Scene7 Publishing System from within Adobe Marketing Cloud.

1. Adobe should already have setup your account with an Adobe Marketing Cloud organization and linked it to your Scene7 Publishing System product context. If this setup is not yet done or you are unsure if it has been done, contact Adobe Customer Care.

   When the setup is complete, you can can log on to Adobe Marketing Cloud and link your Adobe Marketing Cloud identity to your Adobe Dynamic Media Classic user account by doing the following.

1. In Adobe Marketing Cloud, navigate to your account settings.
1. Select **Manage Organizations**.
1. Select **Link Account** or **Get Access**.
1. Select **Experience Manager**, and then type your credentials.

   Your credentials include your IPS company region, email address, and password.

1. Select **Link**.
1. When the link is set, you can launch Scene7 Publishing System from within Adobe Marketing Cloud, or you can launch it directly.

   Do one of the following:

    * To launch Adobe Dynamic Media Classic from within Adobe Marketing Cloud, in the left rail of Adobe Marketing Cloud, select **Solutions** > **Experience Manager**. Under the Adobe Dynamic Media Classic card, select **Launch**.
    * To log on to Scene7 Publishing System directly using your IMS credentials, use the following website:

      https://s7spsN.scene7.com/IpsWeb?ims=1

      Replace "N" in the above path with the number for your IPS company region. That is, N = 1 for North America; 3 for EMEA; or 5 for JAPAC.
 -->

## 带宽和存储 {#bandwidth-storage}

Adobe Dynamic Media Classic管理员可以为他们管理的公司生成带宽、存储和其他类型的报告。 这些报告位于“带宽和存储”页面上。

要打开此页面，请转到 **[!UICONTROL 设置]** > **[!UICONTROL 个人设置]**. 展开 **[!UICONTROL 管理设置]**，然后选择 **[!UICONTROL 带宽和存储]**.

### 报告类型 {#types-of-reports}

下表描述了可从“带宽和存储”页生成的报告：

| 报告 | 信息 | 用途 |
|:--- |:--- |:--- |
| 带宽 | 公司的带宽使用情况 | 跟踪公司在特定日期范围内的带宽使用量，以确定流量模式。 |
| 存储 | 存储使用情况 | 跟踪公司上载的数据量。 |
| 图像内容 | 按类型划分的图像请求数目 | 跟踪不同图像类型的请求数量和容量。 |
| 域 | 按域划分的 URL 请求数目 | 根据特定公司的图像请求的域，跟踪图像使用情况。(Adobe Dynamic Media Classic可以为每个帐户提供多个域。 有关更多信息，请联系技术支持。） |
| 视频流 | 流视频的带宽使用情况 | 跟踪公司在特定日期范围内的流视频使用情况，以确定流量模式。 |
| 视频内容 | 不同视频的播放时间 | 确定哪些是最常观看和最少观看的视频。 |

“图像内容”报告提供了对以下图像类型所发出的请求的信息：

* **图像请求**  — 图像请求。

* **缩略图请求**  — 在查看器中请求样本或替代图像。

* **蒙版请求**  — 对返回灰度蒙版的图像的请求。

* **查看器磁贴请求**  — 查看器加载的图像请求。

* **Vnt对象请求**  — 图像渲染请求，用于返回包含所请求晕影中指定的对象的图像。

* **Vnt信息请求**  — 返回有关所请求晕影信息的图像渲染请求。

>[!NOTE]
>
>“视频流”报告仅应用于流视频。它不会跟踪渐进式视频的观看情况。

### 生成报表 {#generating-a-report}

生成带宽、存储、图像内容、域、视频流或视频内容报告：

1. 转到 **[!UICONTROL 设置]** > **[!UICONTROL 个人设置]**.
1. 展开管理设置，然后选择 **[!UICONTROL 带宽和存储]**.
1. 选择一个选项卡： **[!UICONTROL 带宽]**， **[!UICONTROL 存储]**， **[!UICONTROL 图像内容]**， **[!UICONTROL 域]**， **[!UICONTROL 视频流]**，或 **[!UICONTROL 视频内容]**.

   请参阅[报告类型](administration-setup.md#types_of_reports)。

### 以不同方式查看数据 {#viewing-data-in-different-ways}

在“带宽与存储”页面上生成报告后，您可以选择用于查看信息的选项。您可以选择如何显示信息，如何在图表或数据网格中查看信息，以及指定用于捕获信息的时间段。在“数据”视图中，您还可以排序信息并重新排列各个列。

* **在图表或数据网格中查看数据**  — 选择 **[!UICONTROL 图表视图]** 要查看图表中的数据，请选择 **[!UICONTROL 数据视图]** 在数据网格中查看数据。

* **选择报表演示文稿类型**  — 在报表类型菜单中，选择 **[!UICONTROL 摘要]**， **[!UICONTROL 每日]**，或 **[!UICONTROL 每月]** 以汇总形式、按日期或按月组织数据。 并非所有报告都提供该选项。

* **指定时段**  — 选择选项以定义报表的时间期，然后选择 **[!UICONTROL 更新]** 定义时间段后：

* **预定义时间段**  — 在预定义报表菜单中，选择一个选项。 例如，选择“上月”以捕获上月的数据。

* **自定义时间段**  — 在预定义报表菜单上，选择 **[!UICONTROL 自定义]**. 然后，在 **[!UICONTROL 开始月份]** (或 **[!UICONTROL 开始日期]**)菜单和月数（或天或月数）菜单上的日期。 对于域报告和视频内容报告，您可以为捕获报告信息选择特定的开始和结束日期。

* **排序数据（仅限数据视图）**  — 要对列上的信息进行排序，请选择列的标题。 再次选择可按降序排序。

* **重新排列列（仅限数据视图）**  — 要将列移动到数据网格上的其他位置，请拖动其标题。

### 导出和打印报告 {#exporting-and-printing-reports}

在生成报告后，您可以导出其数据，在电子表格和其他应用程序中使用。您还可以打印报告。

* **导出报表数据**  — 在数据视图中，根据需要对数据进行排序和排列。 然后打开 **[!UICONTROL 导出]** 菜单并选择格式： **[!UICONTROL 制表符分隔]**， **[!UICONTROL 逗号分隔]**，或 **[!UICONTROL HTML已格式化]**. 数据会以您选择的格式复制到剪贴板。 现在，您可以将数据粘贴到电子表格或应用程序中。

* **打印报表**  — 选择 **[!UICONTROL 打印]**，在“打印”对话框中选择所需的选项，然后选择 **[!UICONTROL 确定]**.

## 图像错误 {#image-errors}

Adobe Dynamic Media Classic管理员可以生成图像错误报告。 “图像错误”报告针对您当前登录的公司，提供了过去 24 小时内 20 个最常见的图像错误。要生成图像错误报告，请执行以下操作：

1. 转到 **[!UICONTROL 设置]** > **[!UICONTROL 个人设置]**.
1. 展开管理设置，然后选择 **[!UICONTROL 图像错误]**.
1. （可选）请执行下列操作之一：

   * 要按标题信息对错误进行排序，请选择标题。 默认情况下，按发生次数，从最高到最低排序错误。
   * 将光标移动到错误的“响应”字段上，可查看具体的错误消息。
   * 要查看指向图像或反向链接网页的链接，请将光标移动到URL字段或反向链接字段上方。
   * 要复制指向实际图像的链接，请选择 **[!UICONTROL URL复制URL]**. 您可以在浏览器窗口中粘贴此链接，以转到该图像并检查错误。
   * 要复制指向反向链接网页的链接，请选择 **[!UICONTROL 反向链接复制URL]**.

显示的错误适用于您当前登录到的公司。 每个错误都包括以下信息：

* **图像ID**  — 违规图像的ID。

* **时间**  — 在最近24小时内首次报告错误到上次报告错误的时间范围。

* **计数**  — 映像上报告的错误数。

* **响应**  — 特定错误消息。 错误是 4xx 或者 5xx。

* **URL**  — 列出Adobe Dynamic Media Classic上图像的URL。

* **反向链接**  — 指定初始请求来自的网站的URL。 引用网站可以是具有指向图像的链接的任何网站。

“URL”和“引用网站”列都有与之相关的“复制 URL”以简化测试。
