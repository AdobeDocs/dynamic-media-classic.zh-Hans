---
title: 快速入门： Media Portal
description: Media Portal简介和快速入门，可帮助您在Adobe Dynamic Media Classic中快速启动和运行Media Portal技术和管理。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
feature: Dynamic Media Classic,Collaboration,Asset Management
role: Admin,User
exl-id: bff613c8-a93b-4cca-94db-8cad1cc36296
topic: Collaboration, Content Management
level: Beginner
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '725'
ht-degree: 45%

---

# 快速入门： Media Portal{#quick-start-media-portal}

Media Portal使公司能够轻松获取、控制已批准的资产，并将其分发给公司的外部合作伙伴和渠道以及内部用户。 这个基于浏览器的“自助”环境为Media Portal用户提供了对Adobe Dynamic Media Classic资源的管理员控制的“视图”，以便轻松访问、浏览、搜索、预览和导出企业批准的格式的资源。

作为管理员，您可以控制用户在 Media Portal 中查看、访问和使用资源的方式。此外，您可以自定义Media Portal界面以匹配您的网站和品牌。 您可以在Media Portal界面中指定字体、字体颜色、字体大小并合并品牌元素，如徽标。

请观看以下培训视频：

* [Media Portal概述](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/544_mp_overview1_converted%20renamed_Done-AVS)

* [Media Portal导览1](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/545_mp_tour1_user_converted%20renamed_Done-AVS)

* [Media Portal导览2](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/546_mp_tour2_admin_converted%20renamed_Done-AVS)

以下快速入门旨在帮助您快速启动并运行Media Portal管理。 在每个步骤结束时，选择主题链接以了解详情。

## &#x200B;1. 了解 Media Portal 用户角色

Media Portal用户分为三个角色：用户、参与者以及用户参与者。 每个角色可以执行一组不同的任务。例如，参与者可以重命名和删除文件和文件夹，但是用户不能执行这些任务。了解不同的角色，以便在添加用户时，了解为他们赋予哪些职责。

请参阅[Media Portal 用户角色](media-portal-user-roles.md#media_portal_user_roles)。

## &#x200B;2. 创建用于管理用户的组

组决定了用户有权访问的文件夹和文件、用户可以在这些文件夹和文件中执行的操作以及可以使用的图像预设。作为管理员，您的首要任务是创建组。对于每个组，决定组成员可以访问哪些文件夹、文件和图像预设。此外，向组成员授予读取、写入和删除权限。这些权限决定了成员是否可以浏览、编辑、重命名和删除他们可以访问的文件夹和文件。

请参阅[创建和管理Media Portal组](creating-media-portal-groups.md#creating_and_managing_media_portal_groups)。

## &#x200B;3. 添加用户

添加用户时，为用户指定一个角色（用户、参与者或用户参与者）。您还可以将用户分配给一个或多个组。 要加快添加用户的过程，您可以 CSV 文件形式上载用户列表。新用户会收到用于登录 Media Portal 的欢迎电子邮件和说明。

请参阅[添加和管理Media Portal用户](adding-media-portal-users.md#adding_and_managing_media_portal_users)。

## &#x200B;4. 管理 FTP 帐户

您可以拥有与Media Portal关联的独立FTP帐户。 它们可以映射到您Adobe Dynamic Media Classic帐户中的特定文件夹。 这种功能意味着，您可以允许用户使用单独的 FTP 帐户将数字资源上载到您的帐户中。

请参阅[管理FTP帐户](ftp-accounts.md#managing_ftp_accounts)。

>[!NOTE]
>
>只有Media Portal管理员可以管理这些FTP帐户。 此外，只有具有 Media Portal 参与者用户或 Media Portal 参与者角色的用户可以上载文件。

请参阅[Media Portal 用户角色](media-portal-user-roles.md#media_portal_user_roles)。

## &#x200B;5. 指定导出选项

Media Portal用户在导出文件时，可以重新格式化文件并导出原始主文件 — 如果您授予他们执行此操作的权限。 作为管理员，您可以决定用户如何导出文件。

请参阅[指定Media Portal用户可用的导出选项](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users)。

## &#x200B;6. 创建图像预设

图像预设是预定义设置的集合。 这些设置可以在导出图像时更改图像的外观大小、图像质量、格式、分辨率和其他方面。 您可以创建图像预设，以便控制用户在导出图像时如何重设这些图像的格式。

请参阅[创建和启用图像预设](creating-enabling-image-presets.md#creating_and_enabling_image_presets)。

## &#x200B;7. 创建元数据预设和用户定义的元数据字段

元数据描述并标识文件。 用于搜索和组织资源。 您可以创建元数据预设，以确保正确输入元数据，并填写任何需要数据的元数据字段。 元数据预设是一组预定义的元数据条目。您还可以创建元数据字段来唯一地描述您所处理的文件。

请参阅[更有效地利用元数据](making-efficient-metadata.md#making_more_efficient_use_of_metadata)。

## 8.自定义Media Portal页面

Media Portal样式设置允许您使用公司徽标和颜色来标记Media Portal页面。 使用样式设置将您的公司品牌置于Media Portal上。

请参阅[自定义Media Portal页面](customizing-media-portal-screen.md#customizing_the_media_portal_screen)。
