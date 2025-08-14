---
title: 上传栅格图像资产
description: 了解如何将光栅图像资产上传到Adobe Dynamic Media Classic。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic
role: User
exl-id: 2ef78fe6-1e7c-4f48-86da-137ddaa55bbf
topic: Content Management
level: Intermediate
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '1014'
ht-degree: 52%

---

# 上传栅格图像资产 {#uploading-an-image-asset-or-a-vector-asset}

在上载图像资源之前，必须先请求一个共享密钥。可以使用该共享密钥检索上载令牌。然后，使用上传令牌上传光栅图像资产。

>[!IMPORTANT]
>
>从2023年5月1日开始，Dynamic Media中的UGC资产最多可在上传日期起60天内使用。 60天后，将删除资源。

>[!NOTE]
>
>对Adobe Dynamic Media Classic中新增或现有UGC矢量资源的支持已于2021年9月30日终止。

## 请求共享密钥 {#requesting-a-shared-secret-key}

由&#x200B;*使用Admin Console请求*&#x200B;共享密钥[以创建支持案例。](https://helpx.adobe.com/enterprise/using/support-for-experience-cloud.html)在技术支持案例中，请求共享密钥。

在电子邮件中，请提供要用于上载图像资源的公司名称。从Adobe Dynamic Media Classic收到密钥后，请将其本地保存以供将来使用。

## 检索上传令牌 {#retrieving-the-upload-token}

*上载令牌*&#x200B;可确保他人不能使用相同的共享密钥来上载资源。它可确保上载合法且来自信任的来源。

上载令牌是字母数字字符串，只能在特定时间段内使用。使用以下URL替换您的共享密钥，以便您可以检索上载令牌。

* 栅格图像
  `https://s7ugc1.scene7.com/ugc/image?op=get_uploadtoken&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602`在此示例中，共享密钥为`fece4b21-87ee-47fc-9b99-2e29b78b602`

<!-- * Vector
  `https://s7ugc1.scene7.com/ugc/vector?op=get_uploadtoken&shared_secret=2d19f60e-890a-4e79-a1a5-9ac2875429b9`In this example, the shared-secret key is `2d19f60e-890a-4e79-a1a5-9ac2875429b9` -->

默认情况下，上载令牌在您检索到它之后 5 分钟（300 秒）便到期。若要请求更多时间，请在URL中包含`expires`，并指定您需要的时间（以秒为单位）。 例如，以下示例图像 URL 检索有效期为 1800 秒的上载令牌：

```as3
https://s7ugc1.scene7.com/ugc/image?op=get_uploadtoken&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&expires=1800
```

图像的成功响应类似于以下内容：

```as3
<?xml version="1.0" encoding="UTF-8" standalone="no" ?> 
<scene7> 
    <user_generated_content> 
        <response> 
        <serviceName>User Generated Content: Images</serviceName> 
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
| --- | --- | --- |
| 操作 | 必需 | get_uploadtoken |
| 共享密钥 | 必需 | 正在进行上载的公司的共享密钥。 |
| 过期 | 可选 | 上载令牌有效的秒数。如果未指定，则默认为300秒。 |

**光栅图像URL示例：**

`https://s7ugc1.scene7.com/ugc/image?op=get_uploadtoken&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&expires=600`

<!-- **Sample vector URL:**

`https://s7ugc1.scene7.com/ugc/vector?op=get_uploadtoken&shared_secret=2d19f60e-890a-4e79-a1a5-9ac2875429b9&expires=5000` -->

**允许的HTTP方法：**
`GET`和`POST`

您现在可以上载图像资源。

请参阅[上传图像资产](uploading-image-asset-or-vector.md#uploading_an_image_asset)。

## 上传栅格图像资产 {#uploading-an-image-asset}

您检索到在特定时间内有效的上载令牌后，即可上载图像资源。以 multipart/form post 形式上载资源，而值的其余部分以 URL 查询字符串形式发送，如以下示例中所示：

```as3
https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d-312094e0ef20_18000&company_name=000Company
```

`upload_token`和`company_name`字段为必填项。

请参阅[检索上载令牌](uploading-image-asset-or-vector.md#retrieving_the_upload_token)。

请参阅[检索共享密钥](uploading-image-asset-or-vector.md#requesting_a_shared_secret_key)。

您还能以 URL 查询字符串的形式发送其他可选值，如以下示例所示：

```as3
https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d-312094e0ef20_18000&company_name=000Company&file_limit=2000000&file_exts=jpg,gif
```

`file_limit`参数以字节为单位指定文件大小限制。 `file_exts`参数指定允许上传的文件扩展名。 这两个值都是可选的。

对于允许的文件大小限制和文件扩展名，在应用程序中设置全局限制。如果您在请求中发送的内容是全局限制的子集，则表示同意。 全局限制如下所示：

| 全局限制 | 值 |
| --- | --- |
| 所有客户端的文件大小 | 20 MB |
| 用于上载的支持的图像文件格式 | BMP、GIF、JPG、PNG、PSD、TIFF |

用户可通过下面的 HTML 表单上载资源。表单要求用户输入以下信息：

* 公司名称。
* 上载令牌。
* 文件大小限制。
* 文件扩展名的列表。
* 是否保留与资源关联的颜色配置文件和文件名。
* 是否使用挖空背景。 如果启用“挖空背景”，请设置“拐角”、“公差”和“填充方法”。
在上传[处查看](image-editing-options-upload.md#image-editing-options-at-upload)图像微调选项中的“挖空背景”。
* 要上传的文件的名称。

您可以通过选择[https://s7ugc1.scene7.com/ugc/upload.html](https://s7ugc1.scene7.com/ugc/upload.html)来查看与上述表单关联的HTML源代码

在Firefox中，右键单击浏览器窗口，然后选择&#x200B;**[!UICONTROL 查看页面Source]**。 代码显示相应的URL查询字符串以及在用户选择&#x200B;**[!UICONTROL Submit]**&#x200B;时运行的POST方法。

若要在Internet Explorer中查看XML响应，请转到&#x200B;**[!UICONTROL 查看]** > **[!UICONTROL Source]**。 若要在Firefox中查看XML响应，请转到&#x200B;**[!UICONTROL 工具]** > **[!UICONTROL 浏览器工具]** > **[!UICONTROL Web开发人员工具]**。 建议使用 Firefox 查看 XML 响应。

下面是成功上载的示例响应：

```as3
<?xml version="1.0" encoding="UTF-8" standalone="no" ?> 
<scene7> 
    <user_generated_content> 
        <response> 
            <serviceName>User Generated Content: Images</serviceName> 
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

该资源类似于任何其他的图像服务资源；您可以对其应用处理查询。例如，以下URL请求已拉伸到指定宽度和高度的资产。

```as3
https://s7w2p1.scene7.com/is/image/S7WebUGC/ugc/9536356.tif?&wid=800&hei=100&fit=stretch
```

以 multipart/form post 形式发送要上载的资源，而值的其余部分以 URL 查询字符串形式发送。您可以在 URL 查询字符串中使用以下字段来上载资源：

| URL 参数 | 必需或可选 | 值 |
| --- | --- | --- |
| `op` | 必需 | 上载 |
| `upload_token` | 必需 | 上载与公司关联的共享密钥的令牌。 |
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

您可以使用`image_info`检索您上传的资源的元数据，如以下示例所示：

```as3
https://s7ugc1.scene7.com/ugc/image?op=image_info&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif
```

成功响应的示例如下所示：

```as3
<?xml version="1.0" encoding="UTF-8" standalone="no" ?> 
<scene7> 
    <user_generated_content> 
        <response> 
            <serviceName>User Generated Content: Images</serviceName> 
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
| --- | --- | --- |
| `op` | 必需 | image_info |
| `shared_secret` | 必需 | 公司的共享密钥。 |
| `image_name` | 必需 | 图像的名称。 |

**示例 URL：**

`https://s7ugc1.scene7.com/ugc/image?op=image_info&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif`

**允许的 HTTP 方法：**

GET 和 POST

<!-- ## Upload a vector asset {#uploading-a-vector-asset}

>[!IMPORTANT]
>
>Support for new or existing UGC vector image assets in Adobe Dynamic Media Classic end on September 30, 2021.

After you retrieve an upload token that is valid for a specific amount of time, you can upload a vector asset. You upload the asset as a multipart/form post while sending the rest of the values as a URL query string, as shown in this example:

```as3
https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d- 312094e0ef20_18000&company_name=000Company
```

The `upload_token` and `company_name` fields are required.

See [Retrieve the upload token](uploading-image-asset-or-vector.md#retrieving_the_upload_token).

See [Retrieve a shared-secret key](uploading-image-asset-or-vector.md#requesting_a_shared_secret_key).

You can also send other optional values as URL query strings, as in this example:

```as3
https://s7ugc1.scene7.com/ugc/vector?op=upload&upload_token=aa2a378a-cd25-4c80-994d- 312094e0ef20_18000&company_name=000Company&file_limit=2000000&file_exts=ai,pdf
```

The `file_limit` parameter specifies the file-size limit in bytes. The `file_exts` parameter specifies the filename extensions that are allowed for upload. Both of these values are optional.

A global limit is set in the application for the file size limit and the filename extensions allowed. If what you send in the request is a subset of the global limits, it is honored. The global limits are the following:

| Global limit | Value |
| --- | --- |
| File size for all clients | 20 MB |
| Supported vector file formats for upload | AI, EPS, PDF (only when the PDF is previously opened and saved in Adobe Illustrator CS6) |

The following HTML form lets a user upload an asset. The form asks the user to enter the following information:

* A company name.
* An upload token.
* A file size limit.
* A list of filename extensions.
* Whether to preserve the color profile and file name associated with the asset.
* Whether to use Knockout Background. If you enable Knockout Background, set the Corner, Tolerance, and Fill Method.
See Knockout Background in [Image fine-tuning options at upload](image-editing-options-upload.md#image-editing-options-at-upload).
* The name of the file to upload.

The following HTML code is displayed when you right-click in the browser window, and then select **[!UICONTROL View Source]** for the form shown in the example. The code shows the corresponding URL query string and the POST method that are run when the user selects **[!UICONTROL Submit]**.

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
<td><strong>Select Submit to upload your Vector: </strong></td> 
<td><input type="submit" value="Submit"></td> 
</tr> 
</table> 
</form> 
</body>
```

To view the XML response in Internet Explorer, go to **[!UICONTROL View]** > **[!UICONTROL Source]**. To view XML response in Firefox, go to **[!UICONTROL Tools]** > **[!UICONTROL Browser Tools]** > **[!UICONTROL Page Source]**. Firefox is recommended for viewing XML responses.

The following is a sample response from a successful upload:

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
>The uploaded asset (AI, EPS, PDF so on) is converted to the FXG format and the response sends a direct link to that FXG asset.

The asset is like any other Web-to-print resource; you apply processing queries to it. For example, the following URL converts an FXG resource into a 500x500 png image.

```as3
https://s7w2p1.scene7.com/is/agm/W2PTest/ugc/8875744.fxg?fmt=png&wid=500&hei=500
```

Send the asset to upload as a multipart/form post while sending the rest of the values as a URL query string. You can use the following fields in the URL query string to upload an asset:

| URL Parameter | Required or Optional | Value |
| --- | --- | --- |
| `op` | Required | upload |
| `upload_token` | Required | Upload token for the shared-secret key associated with the company. |
| `company_name` | Required | Name of the company performing the upload. |
| `file_limit` | Optional | File size limit, in bytes, for the asset. |
| `file_exts` | Optional | List of allowable extensions for the asset file. |

>[!NOTE]
>
>You are required to send the asset to be uploaded as the only field in a multipart POST request.

**Sample URL:**

`https://s7ugc1.scene7.com/ugc/vector?op=upload&upload_to ken=aa2a378a-cd25-4c80-994d- 312094e0ef20_18000&company_name=000Company`

**Allowed HTTP method:**

POST
 -->