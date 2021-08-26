---
title: 上载图像资源或矢量资源
description: 了解如何上传图像资产或矢量资产。
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic
role: User
exl-id: 2ef78fe6-1e7c-4f48-86da-137ddaa55bbf
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '1495'
ht-degree: 78%

---

# 上载图像资源或矢量资源{#uploading-an-image-asset-or-a-vector-asset}

在上载图像资源之前，必须先请求一个共享密钥。可以使用该共享密钥检索上载令牌。然后，可以使用上载令牌上载图像资源或矢量资源。

## 请求共享密钥 {#requesting-a-shared-secret-key}

通过[使用Admin Console请求&#x200B;*共享密钥*&#x200B;以创建支持案例。](https://helpx.adobe.com/enterprise/admin-guide.html/enterprise/using/support-for-experience-cloud.ug.html) 在您的支持案例中，请求共享密钥。

在电子邮件中，请提供要用于上载图像资源的公司名称。从AdobeDynamic Media Classic收到密钥后，请将其保存在本地，以供将来使用。

## 检索上载令牌 {#retrieving-the-upload-token}

*上载令牌*&#x200B;可确保他人不能使用相同的共享密钥来上载资源。它可确保上载合法且来自信任的来源。

上载令牌是字母数字字符串，只能在特定时间段内使用。使用以下URL替换您的共享密钥，以便您可以检索上传令牌。

* 图像
   `https://s7ugc1.scene7.com/ugc/image?op=get_uploadtoken&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602`在此示例中，共享密钥为  `fece4b21-87ee-47fc-9b99-2e29b78b602`

* 矢量
   `https://s7ugc1.scene7.com/ugc/vector?op=get_uploadtoken&shared_secret=2d19f60e-890a-4e79-a1a5-9ac2875429b9`在此示例中，共享密钥为  `2d19f60e-890a-4e79-a1a5-9ac2875429b9`

默认情况下，上载令牌在您检索到它之后 5 分钟（300 秒）便到期。要请求更多时间，请在 URL 中添加 `expires` 和要需要的时间量（以秒为单位）。例如，以下示例图像 URL 检索有效期为 1800 秒的上载令牌：

```as3
https://s7ugc1.scene7.com/ugc/image?op=get_uploadtoken&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&expires=1800
```

图像的成功响应类似于以下内容：

```as3
<?xml version="1.0" encoding="UTF-8" standalone="no" ?> 
<scene7> 
    <user_generated_content> 
        <response> 
        <serviceName>User Generated Content - Images</serviceName> 
        <version>1.0.0</version> 
        <operationName>get_uploadtoken</operationName> 
        <serviceStatus>SUCCESS</serviceStatus> 
        <title>Upload Token for fece4b21-87ee-47fc-9b99-2e29b78b602</title> 
        <message> 
            <uploadtoken>aa2a378a-cd25-4c80-994d-312094e0ef20_1800</uploadtoken> 
            <expiration_in_seconds>1800</expiration_in_seconds> 
        </message> 
        </response> 
    </user_generated_content> 
</scene7>
```

将上载令牌保存到本地，以备以后请求时使用。

您可以在查询 URL 字符串中使用以下字段来检索上载令牌：

| URL 参数 | 必需或可选 | 值 |
|--- |--- |--- |
| op | 必需 | get_uploadtoken |
| shared_secret | 必需 | 正在进行上载的公司的共享密钥。 |
| expires | 可选 | 上载令牌有效的秒数。如果不指定，则默认为 300 秒。 |

**示例图像 URL：**

`https://s7ugc1.scene7.com/ugc/image?op=get_uploadtoken&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&expires=600`

**示例矢量 URL：**

`https://s7ugc1.scene7.com/ugc/vector?op=get_uploadtoken&shared_secret=2d19f60e-890a-4e79-a1a5-9ac2875429b9&expires=5000`

**允许的HTTP方法：**
`GET` 和  `POST`

您现在可以上载图像资源。

请参阅[上载图像资源](uploading-image-asset-or-vector.md#uploading_an_image_asset)。

## 上载图像资源 {#uploading-an-image-asset}

您检索到在特定时间内有效的上载令牌后，即可上载图像资源。以 multipart/form post 形式上载资源，而值的其余部分以 URL 查询字符串形式发送，如以下示例中所示：

```as3
https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d-312094e0ef20_18000&company_name=000Company
```

`upload_token`和`company_name`字段为必填字段。

请参阅[检索上载令牌](uploading-image-asset-or-vector.md#retrieving_the_upload_token)。

请参阅[检索共享密钥](uploading-image-asset-or-vector.md#requesting_a_shared_secret_key)。

您还能以 URL 查询字符串的形式发送其他可选值，如以下示例所示：

```as3
https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d-312094e0ef20_18000&company_name=000Company&file_limit=2000000&file_exts=jpg,gif
```

`file_limit`参数指定文件大小限制（以字节为单位）。 `file_exts` 参数指定允许上载的文件扩展名。这两个值都是可选的。

对于允许的文件大小限制和文件扩展名，在应用程序中设置全局限制。如果请求中所发送的内容是全局限制的子集，则允许这一发送。全局限制如下所示：

| 全局限制 | 值 |
|--- |--- |
| 所有客户端的文件大小 | 20 MB |
| 用于上载的支持的图像文件格式 | BMP、GIF、JPG、PNG、PSD |

用户可通过下面的 HTML 表单上载资源。表单要求用户输入以下信息：

* 公司名。
* 上载令牌.
* 文件大小限制.
* 文件扩展名的列表.
* 是否保留与资产关联的颜色配置文件和文件名。
* 是否使用“挖空背景”。 如果启用“挖空背景”，请设置“拐角”、“公差”和“填充方法”。
请参阅上传时的[图像编辑选项中的“挖空背景”](image-editing-options-upload.md#image-editing-options-at-upload)。
* 待上载文件的名称.

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>Art Spec: If not leaving art spec, delete only the first of the 2 &lt;draft-comment> elements under &lt;adobefig>.</p>

 -->

您可以通过单击[https://s7ugc1.scene7.com/ugc/upload.html](https://s7ugc1.scene7.com/ugc/upload.html)查看与上述表单关联的HTML源代码

在Firefox的浏览器窗口中，右键单击，然后单击&#x200B;**[!UICONTROL 查看页面源]**。 该代码将显示当用户单击“**[!UICONTROL 提交]**”时运行的相应 URL 查询字符串和 POST 方法。

要在 Internet Explorer 中查看 XML 响应，请单击“**[!UICONTROL 查看]**”>“**[!UICONTROL 源文件]**”。要在Firefox中查看XML响应，请单击&#x200B;**[!UICONTROL 工具]** > **[!UICONTROL 浏览器工具]** > **[!UICONTROL Web开发人员工具]**。 建议使用 Firefox 查看 XML 响应。

下面是成功上载的示例响应：

```as3
<?xml version="1.0" encoding="UTF-8" standalone="no" ?> 
<scene7> 
    <user_generated_content> 
        <response> 
            <serviceName>User Generated Content - Images</serviceName> 
            <version>1.0.0</version> 
            <operationName>upload</operationName> 
            <serviceStatus>SUCCESS</serviceStatus> 
            <title>Your file has been uploaded Successfully.</title> 
            <message> 
            <url>https://s7w2p1.scene7.com/is/image/ </url> 
            <path>000Company/ugc/1442564.tif</path> 
            <fullurl>https://s7w2p1.scene7.com/is/image/000Company/ugc/1442564.tif </fullurl> 
            </message> 
        </response> 
    </user_generated_content> 
</scene7>
```

>[!NOTE]
>
>上载的资源（JPG、GIF 等）转换为 PTIFF 格式，响应向该 PTIFF 资源发送直接链接。

该资源类似于任何其他的图像服务资源；您可以对其应用处理查询。例如，以下 URL 请求拉伸到指定宽度和高度的资源。

```as3
https://s7w2p1.scene7.com/is/image/S7WebUGC/ugc/9536356.tif?&wid=800&hei=100&fit=stretch
```

以 multipart/form post 形式发送要上载的资源，而值的其余部分以 URL 查询字符串形式发送。您可以在 URL 查询字符串中使用以下字段来上载资源：

| URL 参数 | 必需或可选 | 值 |
|--- |--- |--- |
| `op` | 必需 | 上载 |
| `upload_token` | 必需 | 与公司关联的共享密钥的上载令牌。 |
| `company_name` | 必需 | 执行上载的公司的名称。 |
| `file_limit` | 可选 | 资源的文件大小限制（以字节为单位）。 |
| `file_exts` | 可选 | 图像资源文件容许扩展名的列表。 |
| `preserve_colorprofile` | 可选 | 用于在将上载文件转换成 PTIFF 格式时保留任何嵌入的颜色配置文件。可能的值为 true 或 false。默认值为 false。 |
| `preserve_filename` | 可选 | 保留所上载资源的文件名。可能的值为 true 或 false。默认值为 false。 |

>[!NOTE]
>
>须将待上载资源作为 multipart POST 请求中的唯一字段发送。

**示例 URL：**

`https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d-312094e0ef20_18000&company_name=000Company`

**允许的 HTTP 方法：**

POST

### 获取图像的资源元数据 {#getting-asset-metadata-for-images}

您可以使用 `image_info` 检索所上载资源的元数据，如以下示例中所示：

```as3
https://s7ugc1.scene7.com/ugc/image?op=image_info&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif
```

成功响应的示例如下所示：

```as3
<?xml version="1.0" encoding="UTF-8" standalone="no" ?> 
<scene7> 
    <user_generated_content> 
        <response> 
            <serviceName>User Generated Content - Images</serviceName> 
            <version>1.0.0</version> 
            <operationName>image_info</operationName> 
            <serviceStatus>SUCCESS</serviceStatus> 
            <title>More information on 1442564.tif</title> 
            <message> 
            File created on Tue Sep 08 19:02:04 CDT 2009, File Size = 243494 bytes 
            <imageFormat>Tiff</imageFormat> 
            <colorSpace>Rgb</colorSpace> 
            <width>686</width> 
            <height>457</height> 
            </message> 
        </response> 
    </user_generated_content> 
</scene7>
```

您可以在 URL 查询字符串中使用以下字段请求有关资源的信息：

| URL 参数 | 必需或可选 | 值 |
|--- |--- |--- |
| `op` | 必需 | image_info |
| `shared_secret` | 必需 | 公司的共享密钥。 |
| `image_name` | 必需 | 图像的名称。 |

**示例 URL：**

`https://s7ugc1.scene7.com/ugc/image?op=image_info&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif`

**允许的 HTTP 方法：**

GET 和 POST

## 上载矢量资源 {#uploading-a-vector-asset}

检索到在特定时间内有效的上载令牌后，即可以上载矢量资源。以 multipart/form post 形式上载资源，而值的其余部分以 URL 查询字符串形式发送，如以下示例中所示：

```as3
https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d- 312094e0ef20_18000&company_name=000Company
```

`upload_token`和`company_name`字段为必填字段。

请参阅[检索上载令牌](uploading-image-asset-or-vector.md#retrieving_the_upload_token)。

请参阅[检索共享密钥](uploading-image-asset-or-vector.md#requesting_a_shared_secret_key)。

您还能以 URL 查询字符串的形式发送其他可选值，如以下示例所示：

```as3
https://s7ugc1.scene7.com/ugc/vector?op=upload&upload_token=aa2a378a-cd25-4c80-994d- 312094e0ef20_18000&company_name=000Company&file_limit=2000000&file_exts=ai,pdf
```

`file_limit`参数指定文件大小限制（以字节为单位）。 `file_exts` 参数指定允许上载的文件扩展名。这两个值都是可选的。

对于允许的文件大小限制和文件扩展名，在应用程序中设置全局限制。如果请求中所发送的内容是全局限制的子集，则允许这一发送。全局限制如下所示：

| 全局限制 | 值 |
|--- |--- |
| 所有客户端的文件大小 | 20 MB |
| 支持的可上载矢量文件格式 | AI、EPS、PDF（仅当 PDF 之前已在 Adobe Illustrator CS6 打开并保存时） |

用户可通过下面的 HTML 表单上载资源。表单要求用户输入以下信息：

* 公司名。
* 上载令牌.
* 文件大小限制.
* 文件扩展名的列表.
* 是否保留与资产关联的颜色配置文件和文件名。
* 是否使用“挖空背景”。 如果启用“挖空背景”，请设置“拐角”、“公差”和“填充方法”。
请参阅上传时的[图像编辑选项中的“挖空背景”](image-editing-options-upload.md#image-editing-options-at-upload)。
* 待上载文件的名称.

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>Art Spec: If not leaving art spec, delete only the first of the 2 &lt;draft-comment> elements under &lt;adobefig>.</p>

 -->

当您在浏览器窗口中右键单击，然后单击示例中显示的表单的&#x200B;**[!UICONTROL 查看源]**&#x200B;时，将显示以下HTML代码。 该代码将显示当用户单击“**[!UICONTROL 提交]**”时运行的相应 URL 查询字符串和 POST 方法。

```as3
<body> 
<script language="javascript"> 
function uploadImage() 
{ 
document.image_upload.action="vector?op=upload&company_name="+document.image_upload.company_name.value+"&upload_token="+document.image_upload.upload_token.value+"&file_limit="+document.image_upload.file_limit.value+"&file_exts="+document.image_upload.file_exts.value; 
return true; 
} 
</script> 
<form method="POST" enctype="multipart/form-data" name="image_upload" id="image_upload" onSubmit="return uploadImage();"> 
<table> 
<tr><td colspan="2"><strong> UGC Vector Upload Test Page: </strong></td></tr> 
<tr><td colspan="2"></td></tr> 
<tr><td><strong> Company Name</strong></td><td><input type="text" size="40" name="company_name"></td></tr> 
<tr><td><strong> Upload Token </strong></td><td><input type="text" size="40" name="upload_token"></td></tr> 
<tr><td><strong> File Size Limit (in bytes) </strong></td><td><input type="text" size="40" name="file_limit"> bytes</td></tr> 
<tr><td><strong> File Extensions allowed </strong></td><td><input type="text" size="40" name="file_exts"></td></tr> 
<tr><td colspan="2"></td></tr> 
<tr> 
<td><strong>File to upload: : </strong></td> 
<td><input name="filename" type="file" id="filename" size="58" maxlength="1024" /></td> 
</tr> 
<tr><td colspan="2"></td></tr> 
<tr> 
<td><strong>Click Submit to upload your Vector: </strong></td> 
<td><input type="submit" value="Submit"></td> 
</tr> 
</table> 
</form> 
</body>
```

要在 Internet Explorer 中查看 XML 响应，请单击“**[!UICONTROL 查看]**”>“**[!UICONTROL 源文件]**”。要在Firefox中查看XML响应，请单击&#x200B;**[!UICONTROL 工具]** > **[!UICONTROL 浏览器工具]** > **[!UICONTROL 页面源]**。 建议使用 Firefox 查看 XML 响应。

下面是成功上载的示例响应：

```as3
<?xml version="1.0" encoding="UTF-8" standalone="no" ?> 
    <scene7> 
    <user_generated_content> 
    <response> 
    <serviceName>User Generated Content -Vector</serviceName> 
    <version>1.0.0</version> 
    <operationName>upload</operationName> 
    <serviceStatus>SUCCESS</serviceStatus> 
    <title>Your file has been uploaded Successfully.</title> 
    <message> 
    <url>https://s7w2p1.scene7.com/is/agm</url> 
    <path>W2PTest/ugc/8875744.fxg</path> 
    <fullurl> 
        https://s7w2p1.scene7.com/is/agm/W2PTest/ugc/8875744.fxg 
    </fullurl> 
</message> 
</response> 
</user_generated_content> 
</scene7>
```

>[!NOTE]
>
>上载的资源（AI、EPS、PDF 等）将转换为 FXG 格式，且响应将发送指向该 FXG 资源的直接链接。

该资产与任何其他Web-to-print资源一样；您可以将处理查询应用到该查询。 例如，以下 URL 可将 FXG 资源转换为 500x500 png 图像。

```as3
https://s7w2p1.scene7.com/is/agm/W2PTest/ugc/8875744.fxg?fmt=png&wid=500&hei=500
```

以 multipart/form post 形式发送要上载的资源，而值的其余部分以 URL 查询字符串形式发送。您可以在 URL 查询字符串中使用以下字段来上载资源：

| URL 参数 | 必需或可选 | 值 |
|--- |--- |--- |
| `op` | 必需 | 上载 |
| `upload_token` | 必需 | 与公司关联的共享密钥的上载令牌。 |
| `company_name` | 必需 | 执行上载的公司的名称。 |
| `file_limit` | 可选 | 资源的文件大小限制（以字节为单位）。 |
| `file_exts` | 可选 | 资源文件允许的扩展名列表。 |

>[!NOTE]
>
>须将待上载资源作为 multipart POST 请求中的唯一字段发送。

**示例 URL：**

`https://s7ugc1.scene7.com/ugc/vector?op=upload&upload_to ken=aa2a378a-cd25-4c80-994d- 312094e0ef20_18000&company_name=000Company`

**允许的 HTTP 方法：**

POST
