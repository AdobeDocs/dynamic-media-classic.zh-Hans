---
title: 获取磁盘使用情况信息
description: 了解如何在Adobe Dynamic Media Classic中获取磁盘使用情况信息。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic
role: Admin,User
exl-id: 337a4681-ac9a-40d9-82e8-1999bbed980c
topic: Administration, Content Management
level: Intermediate
autotag-review: '2026-05-13T19:50:49.049Z'
TQID: 'https://experienceleague.adobe.com/g-mRoL2yYGRH-uFr2ACD2qOxBAGUlMMtKKuKtsv2pQk'
product_v2: id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 0d05ca7402db1d8894db1127088905143fb97cff
workflow-type: tm+mt
source-wordcount: 92
ht-degree: 42%

---

# 获取磁盘使用情况信息 {#get-disk-usage-information}

您可以使用`disk_info`参数检索有关公司磁盘空间使用情况的信息，如以下示例所示：

```as3
https://s7ugc1.scene7.com/ugc/image?op=disk_info&shared_secret=d03b7e0b-c9dc-4c6c-af0b-419beeea1c63
```

示例响应如下所示：

```as3
<?xml version="1.0" encoding="UTF-8" standalone="no" ?> 
<scene7> 
    <user_generated_content> 
        <response> 
            <serviceName>User Generated Content: Images</serviceName> 
            <version>1.0.0</version> 
            <operationName>disk_info</operationName> 
            <serviceStatus>SUCCESS</serviceStatus> 
            <title>Disk Information for d03b7e0b-c9dc-4c6c-af0b-419beeea1c63</title> 
            <message>Total Space available = 1395402342400 bytes. Total Space used = 0 bytes.</message> 
        </response> 
    </user_generated_content> 
</scene7>
```

您可以在 URL 查询字符串中使用以下字段来获取磁盘使用情况信息：

| URL 参数 | 必需/可选 | 值 |
| --- | --- | --- |
| 操作 | 必需 | disk_info |
| 共享密钥 | 必需 | 公司的共享密钥 |

下面的示例代码将获取 000Company 的磁盘信息：

```as3
https://s7ugc1.scene7.com/ugc/image?op=disk_info&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b9602
```
