---
title: 获取磁盘使用情况信息
description: 了解如何获取磁盘使用信息。
uuid: 01361693-53d0-4072-b7c3-f284631d28cf
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 6763546d-83c4-42dc-879f-6bbfc8b56482
feature: Dynamic Media Classic
role: Administrator,Business Practitioner
exl-id: 337a4681-ac9a-40d9-82e8-1999bbed980c
source-git-commit: 217e5bf81cc2108e4bf283f585dfd83d319ff7c9
workflow-type: tm+mt
source-wordcount: '88'
ht-degree: 88%

---

# 获取磁盘使用情况信息 {#getting-disk-usage-information}

您可使用 `disk_info` 参数检索关于公司磁盘空间使用情况的信息，如以下示例中所示：

```as3
https://s7ugc1.scene7.com/ugc/image?op=disk_info&shared_secret=d03b7e0b-c9dc-4c6c-af0b-419beeea1c63
```

示例响应如下所示：

```as3
<?xml version="1.0" encoding="UTF-8" standalone="no" ?> 
<scene7> 
    <user_generated_content> 
        <response> 
            <serviceName>User Generated Content - Images</serviceName> 
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
|--- |--- |--- |
| op | 必需 | disk_info |
| shared_secret | 必需 | 公司的共享密钥 |

下面的示例代码将获取 000Company 的磁盘信息：

```as3
https://s7ugc1.scene7.com/ugc/image?op=disk_info&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b9602
```
