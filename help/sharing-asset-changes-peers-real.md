---
title: 與同儕即時共用資產變更
description: 瞭解如何在Adobe Dynamic Media Classic中即時與同業共用資產變更。
uuid: 13fa4f6e-66bf-4682-96a9-0e7040706f53
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: ca7c8a7f-76f4-4a25-8c36-617a029e55be
feature: Dynamic Media Classic,Asset Management,Collaboration
role: Admin,User
exl-id: d74b4966-fe43-4349-bbe1-3a379c49bf1f
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '279'
ht-degree: 44%

---

# 與同儕即時共用資產變更{#sharing-asset-changes-with-peers-in-real-time}

在同一公司的多部電腦上執行多個Adobe Dynamic Media Classic復本時，所有Adobe Dynamic Media Classic使用者端的下列動作都會即時更新至所有對等使用者端：

* 編輯資產（產生器、影像編輯器等）
* 重命名资源
* 删除资源
* 移动资源
* 上载一个或多个资源（桌面版和 FTP）
* 创建、删除或重命名文件夹

在原始使用者端中進行變更後，所有登入同一公司的對等使用者端都會更新變更。 系统会更改对等客户端而事先不发出通知，除非对等客户端正在任何图像编辑器或生成器中编辑发生更改的资源。

登入時，系統會提示您允許或拒絕對等更新。 可以“记住”选择，以便只得到一次提示。要清除选择，请从“全局设置”的“对等辅助网络”面板中删除相应站点。

如果正在编辑对等客户端所更改的资源，则系统会提示您在生成器或编辑器中采纳更改。如果您選擇 **[!UICONTROL 是]**，然後產生器或編輯器會捨棄對資產所做的任何變更並匯入更新的資產。 如果您選擇 **[!UICONTROL 否]**，資產在產生器或編輯器中不會變更，而您所做的任何變更會保留在該工作階段中。

保存资源时，系统会通知您存在更新的版本，并询问您是否要用更改覆盖该资源。
