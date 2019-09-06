---
title: 删除上载的资源
seo-title: 删除上载的资源
description: 'null'
seo-description: 了解如何删除已上传的资产。
uuid: edd2b688-c377-4be1-ba16-d2 dd2 e6 f716 d
contentOwner: admin
content-type: 引用
products: SG_ EXPERIENCE MANAGER/Dynamic-Media-Scene-7
discoiquuid: dd338c-06c6-44d5-8493-dc2087 eeffb
translation-type: tm+mt
source-git-commit: 75f006fd81b0fe2dad5479cdd98e45eaada46b2a

---


# 删除上载的资源{#deleting-an-uploaded-asset}

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
|--- |--- |--- |
| op | 必需 | 刪除 |
| shared_secret | 必需 | 公司的共享密钥。 |
| <ul><li>对于图像：image_name</li><li>对于矢量：fxg_name</li></ul> | 必需 | 要删除的资源的名称。 |

**示例图像 URL：**

`https://s7ugc1.scene7.com/ugc/image?op=delete&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif`

**示例矢量 URL：**

`https://s7ugc1.scene7.com/ugc/vector?op=delete&shared_secret=2160a8fa-cec6-45ba-8d59- ca595f6d2b47& &fxg_name=8875744.fxg`
