---
title: 与对等客户端实时共享资源更改
description: 了解如何与同行实时共享资产更改。
uuid: 13fa4f6e-66bf-4682-96a9-0e7040706f53
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: ca7c8a7f-76f4-4a25-8c36-617a029e55be
feature: Dynamic Media Classic,Asset Management,Collaboration
role: Administrator,Business Practitioner
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '279'
ht-degree: 68%

---


# 与对等客户端实时共享资源更改{#sharing-asset-changes-with-peers-in-real-time}

在同一公司的一台或多台计算机上运行多个Dynamic Media Classic副本时，来自任何Dynamic Media Classic客户端的以下操作将与所有对等客户端实时更新：

* 编辑资源（生成器、图像编辑器等。）
* 重命名资源
* 删除资源
* 移动资源
* 上载一个或多个资源（桌面版和 FTP）
* 创建、删除或重命名文件夹

在原始客户端中进行更改后，所有登录到同一公司的对等客户端都会用更改进行更新。 系统会更改对等客户端而事先不发出通知，除非对等客户端正在任何图像编辑器或生成器中编辑发生更改的资源。

登录时，系统会提示您允许或拒绝对等更新。 可以“记住”选择，以便只得到一次提示。要清除选择，请从“全局设置”的“对等辅助网络”面板中删除相应站点。

如果正在编辑对等客户端所更改的资源，则系统会提示您在生成器或编辑器中采纳更改。如果选择“是”，则生成器或编辑器会放弃对资源所做的任何更改并导入更新的资源。如果选择“否”，则资源在生成器或编辑器中不会发生更改，您在该会话中所做的任何更改都会保留下来。

保存资源时，系统会通知您存在更新的版本，并询问您是否要用更改覆盖该资源。
