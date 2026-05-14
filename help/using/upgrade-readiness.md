---
title: 升级就绪性
description: 升级准备清单，当您想要在 [!DNL Adobe Experience Manager]从 [!DNL Adobe Dynamic Media Classic] 前进到 [!DNL Dynamic Media] 时。
feature: Dynamic Media Classic
role: Admin,User
exl-id: 86537998-b7e9-449c-83eb-6fd04533a00f
topic: Administration, Migration
level: Intermediate
autotag-review: '2026-05-13T20:16:07.073Z'
TQID: 'https://experienceleague.adobe.com/3Kcp3UwvJV8Mkzk6RBRgOJQ7JKF3Ldek-SiOeqS5EKE'
product_v2: id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588id: d378ca77-2da1-4f39-ad92-1917fe974a38
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 81e92d0e8963cccb5b058328cb7601925f7ace4f
workflow-type: tm+mt
source-wordcount: 221
ht-degree: 1%

---

# 升级准备清单

使用以下核对清单帮助您了解并准备从[!DNL Dynamic Media Classic]升级到[!DNL Dynamic Media]。

|  | 任务 | 说明 |
| :--- | :--- | --- |
| **阶段1：许可** | 运行合同 | 根据流量和存储情况，Adobe客户团队将与您合作，从[!DNL Dynamic Media Classic]许可证过渡到[!DNL Dynamic Media]许可证上的续订。 |
| **阶段2：准备** | 验证功能使用情况 | 确认[!DNL Dynamic Media Classic]中使用的功能在[!DNL Dynamic Media]中可用。 请参阅[功能比较](/help/using/upgrade-feature-comparison.md)页面。 [!DNL Dynamic Media]中尚未提供的关键功能包括：<br>·可视配置器（图像作者，图像渲染）。<br>·图像模板（1:1模板）。<br>· eCatalogs。<br>如果正在使用上述功能，则仍可进行升级，并假定可以通过[!DNL Dynamic Media Classic]访问这些功能。 |
|   | 识别资源 | 查找并准备好要用于升级的资源和预设。 |
| **阶段3：环境** | 升级[!DNL Adobe Experience Manager] | 必须将[!DNL Adobe Experience Manager]的所有实例更新到最新版本。 |
|   | 设置[!DNL Dynamic Media] | Adobe Consulting或合作伙伴使用您的凭据配置[!DNL Dynamic Media]。 |
| **阶段4：升级** | 复制资产 | 在升级过程中，将指定的[!DNL Dynamic Media Classic]资产复制到Dynamic Media。 |
| **阶段5：管理设置** | 设置用户和权限 | 创建用户并授予适当的权限。 |
|   | 设置视频编码配置文件 | 创建视频编码配置文件。 |
|   | 设置查看器预设 | 创建查看器预设。 |
|   | 设置图像预设 | 设置图像预设。 |
| **阶段6：验证** | 确认 | 验证用例、资产、链接和API。 |
