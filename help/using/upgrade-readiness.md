---
title: 升级就绪性
description: 升级准备核对清单 [!DNL Adobe Dynamic Media Classic] 到 [!DNL Dynamic Media] 日期 [!DNL Adobe Experience Manager].
feature: Dynamic Media Classic
role: Admin,User
exl-id: 86537998-b7e9-449c-83eb-6fd04533a00f
topic: Administration, Migration
level: Intermediate
source-git-commit: ae7d0c6d3047d68ed3da4187ef516dc51c95de30
workflow-type: tm+mt
source-wordcount: '224'
ht-degree: 1%

---

# 升级准备清单

使用以下核对清单帮助您了解以下内容并为升级做好准备： [!DNL Dynamic Media Classic] 到 [!DNL Dynamic Media].

|  | 任务 | 说明 |
| :--- | :--- | --- |
| **阶段1：许可** | 运行合同 | 根据流量和存储情况，Adobe客户团队将与您合作，从 [!DNL Dynamic Media Classic] 要在以下日期续订的许可证 [!DNL Dynamic Media] 许可证。 |
| **阶段2：准备** | 验证功能使用情况 | 确认中使用的功能 [!DNL Dynamic Media Classic] 在以下位置提供 [!DNL Dynamic Media]. 请参阅 [功能比较](/help/using/upgrade-feature-comparison.md) 页面。 中尚未提供关键功能 [!DNL Dynamic Media] 包括以下内容：<br>·可视配置器（图像创作、图像渲染）。<br>·图像模板（1:1模板）。<br>· eCatalogs。<br>如果使用上述功能，则升级仍可以进行，前提是这些功能可以通过以下方式访问 [!DNL Dynamic Media Classic]. |
|   | 识别资源 | 查找并准备好要用于升级的资源和预设。 |
| **阶段3：环境** | 升级 [!DNL Adobe Experience Manager] | 的所有实例 [!DNL Adobe Experience Manager] 必须更新到最新版本。 |
|   | 设置 [!DNL Dynamic Media] | Adobe咨询或合作伙伴配置 [!DNL Dynamic Media] 使用您的凭据。 |
| **阶段4：升级** | 复制资产 | 在升级过程中，指定 [!DNL Dynamic Media Classic] 资源将复制到Dynamic Media。 |
| **阶段5：管理设置** | 设置用户和权限 | 创建用户并授予适当的权限。 |
|   | 设置视频编码配置文件 | 创建视频编码配置文件。 |
|   | 设置查看器预设 | 创建查看器预设。 |
|   | 设置图像预设 | 设置图像预设。 |
| **第6阶段：验证** | 确认 | 验证用例、资产、链接和API。 |
