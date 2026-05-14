---
title: 与同行实时共享资产更改
description: 了解如何在Adobe Dynamic Media Classic中与同行实时共享资源更改。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
feature: Dynamic Media Classic,Asset Management,Collaboration
role: Admin,User
exl-id: d74b4966-fe43-4349-bbe1-3a379c49bf1f
topic: Administration, Collaboration
level: Intermediate
autotag-review: '2026-05-13T20:12:54.992Z'
TQID: 'https://experienceleague.adobe.com/Yn5GsnQ4cM3Byk18iEB8Z4uGsTt9FjEZOBP17Yt-K8M'
product_v2: id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 81e92d0e8963cccb5b058328cb7601925f7ace4f
workflow-type: tm+mt
source-wordcount: 281
ht-degree: 26%

---

# 与同行实时共享资产更改{#sharing-asset-changes-with-peers-in-real-time}

假设您在同一公司的计算机上运行有多个Adobe Dynamic Media Classic副本。 在此类场景中，来自任何Dynamic Media Classic客户端的以下操作会实时更新到所有对等客户端：

* 编辑资产（生成器、图像编辑器等）
* 重命名资源
* 删除资源
* 移动资源
* 上载一个或多个资源（桌面版和 FTP）
* 创建、删除或重命名文件夹

在原始客户端中进行更改后，登录到同一公司的所有对等客户端都会随该更改而更新。 系统会更改对等客户端而事先不发出通知，除非对等客户端正在任何图像编辑器或生成器中编辑发生更改的资源。

登录时，系统会提示您允许或拒绝对等更新。 可以“记住”选择，以便只得到一次提示。 要清除选择，请从“全局设置”的“对等辅助网络”面板中删除相应站点。

如果您正在编辑由同事更改的资产，则系统会提示您将该更改摄取到生成器或编辑器中。 如果选择&#x200B;**[!UICONTROL 是]**，则生成器或编辑器将放弃对该资产所做的任何更改并导入更新的资产。 如果选择&#x200B;**[!UICONTROL 否]**，则资产在生成器或编辑器中保持不变，并且您所做的任何更改将保留在该会话中。

在保存资源时，系统会通知您存在较新版本，并询问您是否要用更改覆盖资源。
