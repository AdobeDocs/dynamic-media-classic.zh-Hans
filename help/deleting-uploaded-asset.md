---
title: 删除上传的栅格图像资产
description: 了解如何在Adobe Dynamic Media Classic中删除已上传的资产。
uuid: edd2b688-c377-4be1-ba16-d2dd2e6f716d
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: dd338c8c-06c6-44d5-8493-dc2087eeeafb
feature: Dynamic Media Classic
role: User
exl-id: d845bcb2-f914-4727-8df2-049dc172f266
source-git-commit: e235cdf331a1366ea81bd609e4e264c0c2cd8264
workflow-type: tm+mt
source-wordcount: '133'
ht-degree: 48%

---

# 删除上传的资产{#deleting-an-uploaded-asset}

您可以按照以下格式使用 `delete` 参数删除某个资源：

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
>从2023年5月1日开始，Dynamic Media Classic中的UGC光栅资产将可自上传之日起最多使用60天。 60天后，资产将被删除。

>[!NOTE]
>
>2021年9月30日终止对Adobe Dynamic Media Classic中新的或现有的UGC矢量图像资产的支持。

**示例图像 URL：**

`https://s7ugc1.scene7.com/ugc/image?op=delete&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif`

<!-- **Sample vector URL:**

`https://s7ugc1.scene7.com/ugc/vector?op=delete&shared_secret=2160a8fa-cec6-45ba-8d59- ca595f6d2b47& &fxg_name=8875744.fxg` -->
