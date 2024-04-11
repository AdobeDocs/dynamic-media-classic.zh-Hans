---
title: 删除上传的光栅图像资产
description: 了解如何在Adobe Dynamic Media Classic中删除已上传的资源。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic
role: User
exl-id: d845bcb2-f914-4727-8df2-049dc172f266
topic: Content Management
level: Intermediate
source-git-commit: 5b5dcd1199bd51ec987b5673fce75bc86baad55b
workflow-type: tm+mt
source-wordcount: '136'
ht-degree: 34%

---

# 删除上传的资源{#deleting-an-uploaded-asset}

您可以使用 `delete` 参数以删除资产：

```as3
https://s7ugc1.scene7.com/ugc/image?op=delete&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif
```

下面是删除图像资源时的响应示例：

```as3
<?xml version="1.0" encoding="UTF-8" standalone="no" ?> 
<scene7> 
    <user_generated_content> 
        <response> 
            <serviceName>User Generated Content - Images</serviceName> 
            <version>1.0.0</version> 
            <operationName>delete</operationName> 
            <serviceStatus>SUCCESS</serviceStatus> 
            <title>Delete request for1442564.tif</title> 
            <message>Your file was successfully deleted</message> 
        </response> 
    </user_generated_content> 
</scene7>
```

您可以在 URL 查询字符串中使用以下字段来删除资源：

| URL 参数 | 必需/可选 | 值 |
| --- | --- | --- |
| `op` | 必需 | 刪除 |
| `shared_secret` | 必需 | 公司的共享密钥。 |
| `image_name` | 必需 | 要删除的资源的名称。 |

<!-- <li>For Vector:fxg_name</li> -->

>[!IMPORTANT]
>
>从2023年5月1日开始，Dynamic Media中的UGC资源最多可在上传日期起60天内使用。 60天后，将删除资源。

>[!NOTE]
>
>对Adobe Dynamic Media Classic中新增或现有UGC矢量图像资源的支持已于2021年9月30日终止。

**示例图像 URL：**

`https://s7ugc1.scene7.com/ugc/image?op=delete&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif`

<!-- **Sample vector URL:**

`https://s7ugc1.scene7.com/ugc/vector?op=delete&shared_secret=2160a8fa-cec6-45ba-8d59- ca595f6d2b47& &fxg_name=8875744.fxg` -->
