---
title: 添加和管理 Media Portal 用户
description: 了解如何添加和管理Media Portal用户
uuid: 96d4103c-6428-4ce1-b9e4-231599304f27
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
discoiquuid: 5e933045-ce1a-41b9-ba8b-2151c396b7a2
feature: Dynamic Media Classic，协作，资产管理
role: 管理员，业务从业者
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '1034'
ht-degree: 82%

---


# 添加和管理 Media Portal 用户{#adding-and-managing-media-portal-users}

作为管理员，您可以添加和管理用户，决定他们是否可以更改密码、编辑用户信息以及上载用户列表。这些任务在“用户管理”屏幕上完成。要访问该屏幕，请单击“**[!UICONTROL 设置]**”>“**[!UICONTROL 应用程序设置]**”>“**[!UICONTROL 管理设置]**”>“**[!UICONTROL 用户管理]**”。

>[!NOTE]
>
>在添加用户之前，请设置用于管理这些用户的组。Media Portal 不允许仅添加用户而不将该用户指定到一个或多个组。有关更多信息，请参阅[创建和管理 Media Portal 组](creating-media-portal-groups.md#creating_and_managing_media_portal_groups)。

## 处理 Media Portal 密码 {#handling-media-portal-passwords}

在注册时，将向 Media Portal 用户、参与者和参与者用户发送一封包含密码的欢迎电子邮件。管理员可以决定 Media Portal 用户是否可以更改此密码。

1. 单击“**[!UICONTROL 设置”]**>“**[!UICONTROL Media Portal 设置]**”>“**[!UICONTROL 常规设置]**”。
1. 在“常规设置”页面上，选择或取消选择“**[!UICONTROL 允许 Media Portal 用户更改密码]**”。
1. 单击“**[!UICONTROL 保存]**”。

>[!NOTE]
>
>可以更改密码的 Media Portal 用户可以通过单击“**[!UICONTROL 设置]**”>“**[!UICONTROL 个人设置]**”并在“个人设置”屏幕上更改密码来执行此操作。

## 添加 Media Portal 用户  {#adding-a-media-portal-user}

1. 单击“**[!UICONTROL 设置]**”>“**[!UICONTROL 应用程序设置]**”>“**[!UICONTROL 管理设置]**”>“**[!UICONTROL 用户管理]**”。
1. 在“用户管理”页面上，单击“**添加**”。
1. 在“用户信息”面板的“添加用户”对话框中，输入用户的名字、姓氏和电子邮件地址，然后单击“**[!UICONTROL 下一步]**”。
1. 在“公司/角色”面板的“公司”下拉列表中，选择用户的公司。
1. 在“角色”列表中，选择“Media Portal”角色，然后单击“**[!UICONTROL 下一步]**”。

   请参阅[Media Portal 用户角色](media-portal-user-roles.md#media_portal_user_roles)。

1. 在“访问组”面板中，选择一个或多个组。

   请参阅[创建和管理 Media Portal 组](creating-media-portal-groups.md#creating_and_managing_media_portal_groups)。

1. （可选）单击“**[!UICONTROL 电子邮件设置]**”，选择非默认的电子邮件设置。

   请参阅[为 Media Portal 用户设置欢迎电子邮件](adding-media-portal-users.md#setting_up_the_welcome_e_mail_message_for_media_portal_users)。

1. 单击“**[!UICONTROL 添加用户]**”。

在添加用户后，Media Portal 向该用户发送一封欢迎电子邮件。该消息包括一个临时密码和 Media Portal URL。

## 上载 Media Portal 用户列表  {#uploading-a-media-portal-user-list}

如果您要添加多个用户，可以上载一个用户列表。用户便会自动添加到当前所选的帐户中。

以 CSV（逗点分隔值）文件形式创建包含用户信息的用户列表。上载此列表后，此列表中的用户便会自动添加到具有其指定组分配的帐户中。向每个新用户发送一封欢迎电子邮件，其中包括到 Media Portal 的链接和一个临时密码。

### 创建 CSV 文件  {#creating-the-csv-file}

创建一个符合以下格式和字段的 CSV 文件 (filename.csv)。该文件的第一行必须包含此表中列出的列标题；您可以根据需要对这些列进行排序。全部都是必需列。

| 列名称 | 说明 |
|--- |--- |
| 名字 | 名字。 |
| 姓氏 | 姓氏。 |
| 电子邮件 | 有效的电子邮件地址。 |
| 密码 | 区分大小写的密码字符串。 |
| 用户角色 | MediaPortalAdminMediaPortalUserMediaPortalContributorMediaPortalContributorUser |
| 组 | 为每个用户分配的一个或多个帐户组的列表（用逗号分隔）。通过添加账户名称前缀（用正斜线 (/) 分隔）来指定组。例如 PortalCo/IT，其中 PortalCo 为帐户，IT 为 PortalCo 帐户中的组。 |

以下示例电子表格显示了如何设计 CSV 文件：

| 名字 | 姓氏 | 电子邮件 | 密码 | 用户角色 | 组 |
|--- |--- |--- |--- |--- |--- |
| Peter | Peterson | `petep@company.com` | welcome | Media Portal 管理员 | PortalCo/IT、PortalCo/Admin |
| Kevin | Marks | `kevinm@myco.com` | 欢迎 | Media Portal 用户 | PortalCo/MktgGroup、PortalCo/test |


### 上载 CSV 文件  {#uploading-the-csv-file}

1. 打开“用户管理设置”屏幕。
1. 单击“**[!UICONTROL 上载用户列表]**”。
1. 在“选择要上载的文件”对话框中，选择 CSV 文件，然后单击“**[!UICONTROL 打开]**”。

列表中的每个用户即会自动添加到指定组中。将向每个用户发送一封欢迎电子邮件。

>[!NOTE]
>
>如果 CSV 文件的格式不正确，会出现以下错误消息：“处理上载的 CSV 文件时出错”。检查文件内容是否为有效数据。此外，如果 CSV 包含现有 IP 或 IPS 用户，则该用户不会添加到“用户列表”中。

## 生成一个可选择的 Media Portal 用户列表  {#generating-a-selectable-list-of-media-portal-users}

您可以在一个弹出窗口中显示 Media Portal 用户的姓名和电子邮件地址。如果您要剪切和粘贴用户名和地址以便在 Media Portal 外部使用，此列表会非常有用。

1. 单击“**[!UICONTROL 设置]**”>“**[!UICONTROL 应用程序设置]**”>“**[!UICONTROL 管理设置]**”>“**[!UICONTROL 用户管理]**”。
1. 在“**[!UICONTROL 按用户角色]**”下拉列表中，选择 Media Portal 用户角色的名称，然后单击“**[!UICONTROL 刷新]**”以显示一类 Media Portal 用户的名称。
1. 单击“**[!UICONTROL 弹出列表]**”，打开弹出窗口。您可以复制和粘贴该列表。

## 为 Media Portal 用户设置欢迎电子邮件  {#setting-up-the-welcome-e-mail-message-for-media-portal-users}

添加新 Media Portal 用户、参与者和参与者用户时，您可以发送一封欢迎电子邮件。您可以配置此电子邮件或告知Dynamic Media Classic不要发送它。

1. 选择“**[!UICONTROL 设置]**”>“**[!UICONTROL 应用程序设置]**”>“**[!UICONTROL 管理设置]**”>“**[!UICONTROL 用户管理]**”。
1. 在“用户管理设置”屏幕中，单击&#x200B;**[!UICONTROL 电子邮件设置]**。
1. 在“电子邮件设置”对话框中，指定以下任何设置：

   **[!UICONTROL 发送]** 电子邮件如果您不希望通过电子邮件通知新用户您已注册，请取消选择此选项。

   **[!UICONTROL 默认]** 密码为新用户输入临时密码，或将字段留空以使Dynamic Media Classic生成随机密码。用户首次登录时会被要求更改密码。

   **[!UICONTROL 替]** 换URL如果用户通过其他URL访问Dynamic Media Classic，请输入与默认URL不同的URL。

## 其他用户管理任务 {#other-user-management-tasks}

从“用户管理设置”屏幕开始，您还可以执行以下任务：

**[!UICONTROL 筛选和排序用户列]** 表筛选Media Portal用户的列表以查找用户。请参阅过滤和排序用户列表。

**[!UICONTROL 删除]** 用户从列表中删除用户。请参阅删除用户。

**[!UICONTROL 激活和取消激活用]** 户暂停用户访问文件夹。请参阅激活和停用用户。

**[!UICONTROL 编辑用]** 户信息输入有关用户的最新信息。请参阅编辑用户信息。

**[!UICONTROL 创建用户定义字]** 段创建自定义、用户定义的元数据字段，以帮助组织Dynamic Media经典中的资产。必要时，也可以激活或停用这些字段。

请参阅[用户定义的字段](application-setup.md#user_defined_fields)。
