---
title: 「快速入門：Media Portal」
description: Media Portal簡介和快速入門，可幫助您在Adobe Dynamic Media Classic中快速啟動和執行Media Portal技術和管理。
uuid: 0dbd6146-b392-4e03-955b-0b323b654b9f
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
discoiquuid: 1385a092-0b2c-4e05-ad1e-ce3685022300
feature: Dynamic Media Classic,Collaboration,Asset Management
role: Admin,User
exl-id: bff613c8-a93b-4cca-94db-8cad1cc36296
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '872'
ht-degree: 49%

---

# 快速入門： Media Portal{#quick-start-media-portal}

Media Portal可讓公司輕鬆取得、控制資產，並將核准的資產分發給外部合作夥伴和管道，以及公司的內部使用者。 這個以瀏覽器為基礎的「自助式」環境為Media Portal使用者提供管理員控制的Adobe Dynamic Media Classic資產「檢視」，可輕鬆存取、瀏覽、搜尋、預覽和匯出企業核准格式的資產。

作为管理员，您可以控制用户在 Media Portal 中查看、访问和使用资源的方式。此外，您可以自定义 Media Portal 界面，使其匹配您的网站和品牌。您可以在Media Portal介面中指定字型、字型顏色、字型大小，以及合併商標元素（例如標誌）。

請參閱下列訓練影片：

* [Media Portal概觀](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/544_mp_overview1_converted%20renamed_Done-AVS)

* [Media Portal導覽1](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/545_mp_tour1_user_converted%20renamed_Done-AVS)

* [Media Portal導覽2](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/546_mp_tour2_admin_converted%20renamed_Done-AVS)

以下快速入門旨在讓您快速上手並執行Media Portal管理。 在每個步驟結束時，選取主題連結以瞭解更多資訊。

## 1. 了解 Media Portal 用户角色

Media Portal 用户分为三个角色，即用户、参与者和用户参与者。每个角色可以执行一组不同的任务。例如，参与者可以重命名和删除文件和文件夹，但是用户不能执行这些任务。了解不同的角色，以便在添加用户时，了解为他们赋予哪些职责。

请参阅[Media Portal 用户角色](media-portal-user-roles.md#media_portal_user_roles)。

## 2. 创建用于管理用户的组

组决定了用户有权访问的文件夹和文件、用户可以在这些文件夹和文件中执行的操作以及可以使用的图像预设。作为管理员，您的首要任务是创建组。对于每个组，决定组成员可以访问哪些文件夹、文件和图像预设。此外，向组成员授予读取、写入和删除权限。这些权限决定了成员是否可以浏览、编辑、重命名和删除他们可以访问的文件夹和文件。

另請參閱 [建立和管理Media Portal群組](creating-media-portal-groups.md#creating_and_managing_media_portal_groups).

## 3. 添加用户

添加用户时，为用户指定一个角色（用户、参与者或用户参与者）。还要将该用户指定给一个或多个组。要加快添加用户的过程，您可以 CSV 文件形式上载用户列表。新用户会收到用于登录 Media Portal 的欢迎电子邮件和说明。

另請參閱 [新增和管理Media Portal使用者](adding-media-portal-users.md#adding_and_managing_media_portal_users).

## 4. 管理 FTP 帐户

您可以有與Media Portal相關聯並對應至Adobe Dynamic Media Classic帳戶中特定資料夾的個別FTP帳戶。 这种功能意味着，您可以允许用户使用单独的 FTP 帐户将数字资源上载到您的帐户中。

另請參閱 [管理FTP](ftp-accounts.md#managing_ftp_accounts).

>[!NOTE]
>
>只有 Media Portal 管理员可以管理这些 FTP 帐户。此外，只有具有 Media Portal 参与者用户或 Media Portal 参与者角色的用户可以上载文件。

请参阅[Media Portal 用户角色](media-portal-user-roles.md#media_portal_user_roles)。

## 5. 指定导出选项

Media Portal使用者匯出檔案時，可以重新格式化檔案並匯出原始主要檔案（如果您授予他們執行此作業的許可權）。 作为管理员，您可以决定用户如何导出文件。

另請參閱 [指定Media Portal使用者可用的匯出選項](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users).

## 6. 创建图像预设

图像预设是一组预定义的设置，用于更改图像在导出时的外观大小、图像质量、格式、分辨率以及其他方面。您可以创建图像预设，以便控制用户在导出图像时如何重设这些图像的格式。

另請參閱 [建立和啟用影像預設集](creating-enabling-image-presets.md#creating_and_enabling_image_presets).

## 7. 创建元数据预设和用户定义的元数据字段

元数据描述和标识了一个文件；它用于搜索和组织资源。为确保正确输入了元数据并且需要数据的元数据字段都已填充，可以创建元数据预设。元数据预设是一组预定义的元数据条目。您还可以创建元数据字段来唯一地描述您所处理的文件。

请参阅[更有效地利用元数据](making-efficient-metadata.md#making_more_efficient_use_of_metadata)。

## 8.自訂媒體入口網站頁面

Media Portal樣式設定可讓您使用公司標誌和顏色來為Media Portal頁面命名。 使用樣式設定將您的公司品牌放在Media Portal上。

另請參閱 [自訂Media Portal](customizing-media-portal-screen.md#customizing_the_media_portal_screen).
