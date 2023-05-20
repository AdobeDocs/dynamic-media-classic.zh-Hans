---
title: 新增和管理Media Portal使用者
description: 瞭解如何在Adobe Dynamic Media Classic中新增和管理Media Portal使用者。
uuid: 96d4103c-6428-4ce1-b9e4-231599304f27
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
discoiquuid: 5e933045-ce1a-41b9-ba8b-2151c396b7a2
feature: Dynamic Media Classic,Collaboration,Asset Management
role: Admin,User
exl-id: 9590c53c-fd38-4bf2-b723-cd7369702364
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '1017'
ht-degree: 58%

---

# 新增和管理Media Portal使用者{#adding-and-managing-media-portal-users}

作为管理员，您可以添加和管理用户，决定他们是否可以更改密码、编辑用户信息以及上载用户列表。这些任务在“用户管理”屏幕上完成。若要存取此畫面，請瀏覽至 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 管理設定]** > **[!UICONTROL 使用者管理]**.

>[!NOTE]
>
>在添加用户之前，请设置用于管理这些用户的组。Media Portal 不允许仅添加用户而不将该用户指定到一个或多个组。如需詳細資訊，請參閱 [建立和管理Media Portal群組](creating-media-portal-groups.md#creating_and_managing_media_portal_groups).

## 管理Media Portal密碼 {#handling-media-portal-passwords}

在注册时，将向 Media Portal 用户、参与者和参与者用户发送一封包含密码的欢迎电子邮件。管理员可以决定 Media Portal 用户是否可以更改此密码。

1. 導覽至 **[!UICONTROL 設定]** > **[!UICONTROL Media Portal設定]** > **[!UICONTROL 一般設定]**.
1. 在“常规设置”页面上，选择或取消选择“**[!UICONTROL 允许 Media Portal 用户更改密码]**”。
1. 選取 **[!UICONTROL 儲存]**.

>[!NOTE]
>
>允許變更密碼的Media Portal使用者可以透過選取 **[!UICONTROL 設定]** > **[!UICONTROL 個人設定]** 和變更「個人設定」畫面上的密碼。

## 新增Media Portal使用者 {#adding-a-media-portal-user}

1. 導覽至 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 管理設定]** > **[!UICONTROL 使用者管理]**.
1. 在「使用者管理」頁面上，選取 **新增**.
1. 在新增使用者對話方塊的使用者資訊面板中，輸入使用者的名字、姓氏和電子郵件地址，然後選取 **[!UICONTROL 下一個]**.
1. 在“公司/角色”面板的“公司”下拉列表中，选择用户的公司。
1. 在「角色」清單中，選取Media Portal角色，然後選取 **[!UICONTROL 下一個]**.

   请参阅[Media Portal 用户角色](media-portal-user-roles.md#media_portal_user_roles)。

1. 在“访问组”面板中，选择一个或多个组。

   另請參閱 [建立和管理Media Portal群組](creating-media-portal-groups.md#creating_and_managing_media_portal_groups).

1. （選用）選取 **[!UICONTROL 電子郵件設定]** 以選擇與預設設定不同的電子郵件設定。

   请参阅[为 Media Portal 用户设置欢迎电子邮件](adding-media-portal-users.md#setting_up_the_welcome_e_mail_message_for_media_portal_users)。

1. 選取 **[!UICONTROL 新增使用者]**.

在添加用户后，Media Portal 向该用户发送一封欢迎电子邮件。该消息包括一个临时密码和 Media Portal URL。

## 上载 Media Portal 用户列表 {#uploading-a-media-portal-user-list}

如果您要添加多个用户，可以上载一个用户列表。用户便会自动添加到当前所选的帐户中。

以 CSV（逗点分隔值）文件形式创建包含用户信息的用户列表。上载此列表后，此列表中的用户便会自动添加到具有其指定组分配的帐户中。向每个新用户发送一封欢迎电子邮件，其中包括到 Media Portal 的链接和一个临时密码。

### 创建 CSV 文件 {#creating-the-csv-file}

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
| 草原城 | Kat | `prairiek@company.com` | welcome | Media Portal 管理员 | PortalCo/IT、PortalCo/Admin |
| Rick | Brough | `rickb@myco.com` | welcome | Media Portal 用户 | PortalCo/MktgGroup、PortalCo/test |

### 上载 CSV 文件 {#uploading-the-csv-file}

1. 打开“用户管理设置”屏幕。
1. 選取 **[!UICONTROL 上傳使用者清單]**.
1. 在「選取要上傳的檔案」對話方塊中，選取CSV檔案，然後選取 **[!UICONTROL 開啟]**.

列表中的每个用户即会自动添加到指定组中。将向每个用户发送一封欢迎电子邮件。

>[!NOTE]
>
>如果 CSV 文件的格式不正确，会出现以下错误消息：“处理上载的 CSV 文件时出错”。检查文件内容是否为有效数据。此外，如果 CSV 包含现有 IP 或 IPS 用户，则该用户不会添加到“用户列表”中。

## 生成一个可选择的 Media Portal 用户列表 {#generating-a-selectable-list-of-media-portal-users}

您可以在一个弹出窗口中显示 Media Portal 用户的姓名和电子邮件地址。如果您要剪切和粘贴用户名和地址以便在 Media Portal 外部使用，此列表会非常有用。

1. 導覽至 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 管理設定]** > **[!UICONTROL 使用者管理]**.
1. 在 **[!UICONTROL 依使用者角色]** 下拉式清單，選擇Media Portal使用者角色的名稱，然後選取 **[!UICONTROL 重新整理]** 顯示一個Media Portal使用者類別的名稱。
1. 選取 **[!UICONTROL 快顯清單]**. 複製並貼上此清單。

## 为 Media Portal 用户设置欢迎电子邮件消息 {#setting-up-the-welcome-e-mail-message-for-media-portal-users}

添加新 Media Portal 用户、参与者和参与者用户时，您可以发送一封欢迎电子邮件。您可以設定此電子郵件訊息，或告訴Adobe Dynamic Media Classic不要傳送。

1. 導覽至 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 管理設定]** > **[!UICONTROL 使用者管理]**.
1. 在「使用者管理設定」畫面中，選取 **[!UICONTROL 電子郵件設定]**.
1. 在“电子邮件设置”对话框中，指定以下任何设置：

   * **[!UICONTROL 傳送電子郵件]**  — 如果您不想透過電子郵件通知新使用者您已註冊，請取消選取此選項。

   * **[!UICONTROL 預設密碼]**  — 為新使用者輸入臨時密碼，或將該欄位留空以讓Adobe Dynamic Media Classic產生隨機密碼。 使用者第一次登入時，系統會要求他們變更密碼。

   * **[!UICONTROL 替代URL]**  — 如果您的使用者透過其他URL存取Adobe Dynamic Media Classic，請輸入與預設不同的URL。

## 其他用户管理任务 {#other-user-management-tasks}

从“用户管理设置”屏幕开始，您还可以执行以下任务：

* **[!UICONTROL 篩選及排序使用者清單]**  — 篩選Media Portal使用者清單以尋找使用者。

* **[!UICONTROL 刪除使用者]**  — 從清單中移除使用者。

* **[!UICONTROL 啟用和停用使用者]**  — 暫停使用者存取資料夾。

* **[!UICONTROL 編輯使用者資訊]**  — 輸入使用者的最新資訊。

* **[!UICONTROL 建立使用者定義的欄位]**  — 建立自訂、使用者定義的中繼資料欄位，協助您在Adobe Dynamic Media Classic中組織資產。 必要时，也可以激活或停用这些字段。

请参阅[用户定义的字段](application-setup.md#user_defined_fields)。
