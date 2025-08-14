---
title: 上载文件
description: 了解如何在Adobe Dynamic Media Classic中上传文件。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 8dfcfb3f-6472-4efd-bc87-d5111eee45ce
topic: Content Management
level: Intermediate
source-git-commit: 1cd516119da23f5ef4c0195273025ddd4b3fa789
workflow-type: tm+mt
source-wordcount: '3858'
ht-degree: 26%

---

# 上载文件{#uploading-files}

在将资源文件上传到Adobe Dynamic Media Classic之前，请确保已正确命名资源文件。 另外，请确保已按照所需的方式设置和整理您的文件夹结构。 您可以从Adobe Dynamic Media Classic提供的FTP站点上传文件，也可以直接从您的计算机或网络上传文件。 Adobe Dynamic Media Classic提供可在您上传文件时优化文件的选项。 如果安装了Adobe Dynamic Media Classic桌面应用程序，则可以通过直接从桌面拖动来上传文件和文件夹。 请参阅[应用程序常规设置](application-setup.md#general_settings)。

## 准备资产和文件夹以进行上传 {#preparing-your-assets-and-folders-for-uploading}

在将资源上传到Adobe Dynamic Media Classic之前，请确保它们的格式和大小正确。 您还必须遵守用于命名资源的Adobe Dynamic Media Classic规则。 通过设置文件的文件夹组织和结构，可确保可以轻松定位及处理文件。

### 支持的资源文件格式 {#supported-asset-file-formats}

此表列出了Adobe Dynamic Media Classic支持的资源文件格式。 有关支持的Camera Raw文件的信息，请参阅[https://helpx.adobe.com/camera-raw/using/supported-cameras.html](https://helpx.adobe.com/camera-raw/using/supported-cameras.html)。

| 资源文件格式 | 说明 |
| --- | --- |
| 音频 | AAC、HE-AAC、AC3、WAV、WMA、AIFF、MP3 |
| 级联样式表 | CSS |
| 颜色配置文件 | ICC、ICM |
| 字体 | AFM、OTF、PFB、PFM、PhotoFont、TTC、TTF |
| FXG | FXG |
| Illustrator | AI、FXG |
| 图像 | BMP、FPX、GIF、JPEG、JPG、PNG、PICT(仅限Windows®)、TIF、TIFF |
| InDesign | INDD、INDT |
| MS® Office | DOC、PPT、RTF、XLS |
| PDF | PDF |
| Photoshop | PSD、FXG 和 Camera Raw |
| PostScript | EPS、PS |
| Adobe Dynamic Media Classic图像创作 | VNC、VNT、VNW |
| SVG | SVG、SVGX |
| TAR | TAR |
| 视频 | 3GP、AVI、M2P、M2T、M2TS、M2V、M4V、MOV、MP4、MPEG、MPG、MTS、OGV、TS、VOB、WMV/ASF |
| XML | XML |
| ZIP | ZIP |

TAR 和 ZIP 上载支持包括一个复选框，用于选择是否要解压缩文件。

### Dynamic Media中不支持的图像格式 {#unsupported-image-formats-dynamic-media}

以下列表介绍了Dynamic Media中不支持&#x200B;*的*&#x200B;光栅图像文件格式的子类型。

* IDAT区块大小大于100 MB的PNG文件。
* psb文件。
* 不支持色彩空间不是CMYK、RGB、灰度或位图的PSD文件。 不支持DuoTone、Lab和Indexed色彩空间。
* 位深度大于16的PSD文件。
* 包含浮点数据的TIFF文件。
* 具有Lab色彩空间的TIFF文件。

### 资源类型 {#asset-types}

要通过Adobe Dynamic Media Classic程序获得最佳结果，请务必使用推荐的文件格式和大小。 下表列出了资源类型，其中一些资源类型列有常用资源的推荐格式和文件大小。

| 资源类型 | 说明/推荐 |
| --- | --- |
| 音频 | 输入音频资源格式，其中包括 AAC、HE-AAC、AC3、WAV、WMA、AIFF、MP3。可以将音频转码为以下格式：MP3、AAC 和 HE-AAC。 |
| 图像（用于调整图像大小、缩放、图像集、旋转集） | 图像的最长尺寸必须至少为2000像素；典型图像的最长尺寸范围是1500到2500像素。 推荐使用无损图像格式，包括 TIFF 和 PNG 文件。如果使用 JPEG 图像，请使用最高质量设置。处理动画GIF文件的方式与其他静态内容类似。 |
| eCatalog | 使用在Adobe Acrobat中创建的高分辨率PDF文件或保存为“可按下”的Adobe Creative Suite应用程序。 PDF包括所有需要的字体、图像和蒙版。 并且，以单页、双页跨页或多页格式包含所有所需的引用图形元素。 通过按字母数字顺序为文件命名来排列页面顺序。将 eCatalog 类型的所有 PDF 文件放于一个文件夹中，以便于上载。您可以在上载时选择裁切选项，以便从 PDF 中删除修剪区域，包括裁切标记、对齐目标或颜色条。多数印刷就绪的 PDF 文件采用 CMYK 颜色空间，因此务必要获得用于 PDF 文件的 CMYK ICC 颜色配置文件。 |
| 模板 | 分层图像或布局设计，可以包括文本、图像和图层。可以将图层、文本字符串和属性（如颜色和大小）参数化，从而可以自定义变量数据。在模板中使用时的图像要求与其他图像相同。在 Photoshop 或其他图像编辑程序中准备图形。采用 TIFF 或 PNG 格式将每个图形保存为平面化透明文件。确保图像分辨率适合所要求的用途。打印图像为300 ppi。 |
| 视频 | Adobe Dynamic Media Classic支持以OGV和MP4格式保存的视频文件。 上传时可以将文件转码为MP4格式。 请参阅[支持的资源文件格式](#supported-static-file-formats)。 |
| 字体 | 已上传TrueType、`Type1`(仅限Windows®)、OpenType®字体和PhotoFonts。 |
| 图像 | 图像和分层图像文件。 |
| 图像集和样本集 | 可以显示在查看器中的一组相关图像。 |
| ICC 配置文件 | 一种颜色配置文件，可用于将上传的图像从其源颜色空间转换为不同的颜色空间。 |
| 晕影 | 使用图像创作程序创作的图像和相关文件。 |
| 内容文件 | Adobe InDesign、Illustrator 或 Photoshop 内容文件。 |
| FXG 文件 | 与分辨率无关的图形格式文件；可用于创建可自定义的模板，以输出到打印、网络、电子邮件、桌面和设备。 |
| SVG 文件 | 图像服务服务器可以渲染的可缩放矢量图形文件。 |
| XML 文件 | 定义用于修改请求的路径和查询部分的预处理规则的文件。 |
| 级联样式表文件。 | 上传CSS外观以供HTML5查看器自定义。 |
| JavaScript 文件 | JavaScript文件用于viewer instrumentation保存帐户信息。 Adobe Security建议仅对使用单独域的客户端帐户使用此资源类型，以避免跨站点脚本。 |

>[!NOTE]
>
>在将图像文件和PDF上传到Adobe Dynamic Media Classic时，系统将这些源文件转换为P-TIFF(金字塔TIFF)文件。 这些P-TIFF是稍后发布到Dynamic Media图像服务器的文件。 Adobe Dynamic Media Classic使用金字塔Tiff文件格式，因为它包含各种缩放比率，在使用Adobe Dynamic Media Classic缩放查看器查看时，允许快速缩放。

### 支持静态文件格式 {#supported-static-file-formats}

Adobe Dynamic Media Classic支持多种静态文件格式。 静态内容是“原样”发布的任何资源，如CSS、PDF、SVG和XML。

可以发布以下文件类型：

* GIF 动画
* 音频文件
* CSS
* JavaScript（为公司配置自己的域时）
* 主视频
* PDF (当PDF在上传后标记为发布时，以避免交付现有eCatalog/PDF工作流的所有PDF)
* PrX 视频
* SVG
* XML
* ZIP

Adobe Dynamic Media Classic不提供用于生成静态内容预览URL的选项。

### 文件名要求 {#filename-requirements}

由于在文件上载过程中将去除文件名中的扩展名，因此系统不允许文件使用相同的根名称。在Adobe Dynamic Media Classic系统中，资源文件名减去文件扩展名后，将成为资源的资源ID。 因此，两个资源不能同名。

确保贵公司的所有用户都了解以下命名文件的规则：

* 系统中不允许使用同名的资产ID。
* 资产ID名称区分大小写。
* 最佳做法是确保资源 ID 不包含空格（例如 black jacket.tif 和 blue jacket.jpg）。Adobe Dynamic Media Classic在使用资源名称构建URL字符串时对资源名称中的空格进行ASCII编码。 这些 ASCII 编码不易理解，从而使 URL 更难理解。
* 文件名中允许特定语言字符。但是，文件名中不能出现以下字符：

  `\ ; / ? : @ & = + $ , &#42; " &lt; > | ' { } %`

  如果文件名包含一个或多个上述字符，将会在上载时删除这些字符。

通常，资源文件名可以与其项目编号、产品SKU或其他名称相同，如下所示：

| 商品 | 文件名 | 资源 ID |
| --- | --- | --- |
| 896649 | 896649.jpg | 896649 |
| 48A3_2X | 48A3_2X.tif | 48A3_2X |

### 文件夹组织和结构 {#folder-organization-and-structure}

在将内容上传到系统之前，在Adobe Dynamic Media Classic中组织和构建内容的文件夹和子文件夹。 采用这种方式提前进行规划主要有两个好处：

* 通过FTP将内容上传到Adobe Dynamic Media Classic时，您可以指示系统在上传期间复制您的文件夹结构。 这样，您的内容就会在Adobe Dynamic Media Classic中与您的计算机或网络相同的文件夹和子文件夹中进行组织。 (要在Adobe Dynamic Media Classic中复制文件夹结构，请在通过FTP上传资源时选择包括子文件夹选项。)
* 与在开始就使用经过仔细计划的文件夹结构相比，在文件上载之后重新对系统内的文件夹进行组织要困难得多。

您选择用于在Adobe Dynamic Media Classic上存储内容的文件夹命名方法和结构取决于贵组织的需求。 以下是一些文件夹结构示例：

**基于SKU**：根据SKU或项目编号命名文件夹。 例如，将为所有0、20和30数字系列创建单独的文件夹。

**基于品牌**：对于拥有多个品牌线的制造商和销售其他公司品牌的销售商，请将文件分隔到不同品牌的产品文件夹中。

**基于项目**：根据转出/放置日期或项目名称组织文件夹。 主要生成 eCatalog 的客户喜欢使用这种方法。

**网站文件夹层次结构的镜像**：此文件夹结构镜像网站的文件夹结构，例如，为产品类别使用名为的文件夹。

## 关于上传文件 {#uploading-your-files}

您可以通过FTP从桌面上载单个文件或上载文件夹。 如果要上载超过100 MB的文件或上载整个文件夹和子文件夹，请选择&#x200B;**通过FTP**&#x200B;选项卡。

Adobe Dynamic Media Classic会向您发送一封电子邮件，用于确认上传作业何时开始和结束，并通知您出现任何问题。

在大型上载作业期间（或之后），某些新项目可能会显示“图像尚未优化”消息。 出现此消息是因为文件尚未完全处理并添加到Adobe Dynamic Media Classic。 您可以稍后优化这些文件。请参阅[优化文件](application-setup.md#optimize_files)。

### 使用“从桌面”选项卡上载文件 {#upload-files-using-sps-desktop-application}

Adobe Dynamic Media Classic桌面应用程序允许您通过拖动来上传文件和文件夹。

1. 在Adobe Dynamic Media Classic Desktop应用程序的“全局导航栏”上，选择&#x200B;**[!UICONTROL 上传]**。
1. 在上传页面上，选择&#x200B;**[!UICONTROL 从桌面]**&#x200B;选项卡。
1. 在上传页面的左侧，在&#x200B;**[!UICONTROL 选择要上传的文件]**&#x200B;区域中，选择&#x200B;**[!UICONTROL 浏览]**&#x200B;以选择要上传的文件或文件夹，然后选择&#x200B;**[!UICONTROL 打开]**。
1. 在上传页面的右侧，在选定的&#x200B;**文件夹目标**&#x200B;区域中，导航到要添加已上传文件或文件夹的目标文件夹。
1. （可选）在“上载”页面底部附近的作业名称文本字段中，输入上载作业的新名称。 或者，您只需使用Adobe Dynamic Media Classic提供的系统生成的默认名称即可。 上载和发布作业会记录在“作业”页面上，您可以在该页面上检查作业的状态。 请参阅[检查作业文件](checking-job-files.md#checking_job_files)。
1. （可选）在上传页面底部附近，选择&#x200B;**[!UICONTROL 上传后发布]**，以便您可以自动发布所上传的资产。
在发布文件时，文件将发送到实时服务器。然后，可以在外部网站和应用程序中使用这些文件的 URL。“作业选项”对话框中也提供了相同选项。
1. （可选）如果希望上载的文件替换具有相同名称的现有文件，请选择“上载”页面底部附近的&#x200B;**[!UICONTROL 覆盖任意文件夹中的相同基本资源名称（不论扩展名是什么）]**。 “作业选项”对话框中也提供了相同选项。
此选项的名称可能不同，具体取决于**[!UICONTROL 应用程序设置]** > **[!UICONTROL 常规设置]** > **[!UICONTROL 上载到应用程序]** > **[!UICONTROL 覆盖图像]**&#x200B;中的设置。
1. 在上传页面的右下角附近，选择&#x200B;**[!UICONTROL 作业选项]**，然后指定所需的选项。

   请参阅[上载选项](uploading-files.md#upload_options)。

1. 在“上载作业选项”对话框中，选择&#x200B;**[!UICONTROL 保存]**。
1. 在上传页面的右下角，选择&#x200B;**[!UICONTROL 提交上传]**。
要查看上载进度，请在全局导航栏上选择**[!UICONTROL 作业]**。 您可以继续在Adobe Dynamic Media Classic中工作。 随时返回到“作业”页以查看正在进行的作业。 要取消正在进行的上载作业，请选择“持续时间”旁边的“**[!UICONTROL 取消]**”。

### 使用“通过FTP”选项卡上传文件 {#upload-files-using-via-ftp}

1. 登录到特定于您所在地区的Adobe Dynamic Media Classic FTP站点。 使用您从管理员那里收到的 FTP 用户名和密码。
1. 在Adobe Dynamic Media Classic的全局导航栏上，选择&#x200B;**[!UICONTROL 上传]**。
1. 在上传页面上，选择&#x200B;**[!UICONTROL 通过FTP]**&#x200B;选项卡。
1. 在上传页面的左侧&#x200B;**[!UICONTROL 选择要上载的FTP文件夹]**&#x200B;区域，选择要从中上载文件的FTP文件夹。
1. 在上传页面的右侧，在选定的&#x200B;**[!UICONTROL Adobe Dynamic Media文件夹目标]**&#x200B;区域中，选择Adobe Dynamic Media Classic中的目标文件夹。
1. （可选）在“上载”页面底部附近的作业名称文本字段中，输入上载作业的新名称。 或者，您只需使用Adobe Dynamic Media Classic提供的系统生成的默认名称即可。 上载和发布作业会记录在“作业”页面上，您可以在该页面上检查作业的状态。
请参阅[检查作业文件](checking-job-files.md#checking_job_files)。
1. （可选）在上传页面底部附近，选择&#x200B;**[!UICONTROL 上传后发布]**，以便您可以自动发布所上传的资产。
在发布文件时，文件将发送到实时服务器。然后，可以在外部网站和应用程序中使用这些文件的 URL。“作业选项”对话框中也提供了相同选项。
1. （可选）如果希望上载的文件替换具有相同名称的现有文件，请选择“上载”页面底部附近的&#x200B;**[!UICONTROL 覆盖任意文件夹中的相同基本资源名称（不论扩展名是什么）]**。 “作业选项”对话框中也提供了相同选项。
此选项的名称可能不同，具体取决于**[!UICONTROL 设置]** > **[!UICONTROL 应用程序设置]** > **[!UICONTROL 常规设置]** > **[!UICONTROL 上载到应用程序]** > **[!UICONTROL 覆盖图像]**&#x200B;中的设置。
1. 可选；仅当您选择&#x200B;**[!UICONTROL 通过FTP]**&#x200B;选项卡时可用。 在上传页面底部附近，选择&#x200B;**[!UICONTROL 在上传时解压缩Zip或Tar文件]**，以便您能够自动从上传的ZIP或TAR文件中解压缩所有文件。 “作业选项”对话框中也提供了相同选项。
1. 在上传页面的右下角附近，选择&#x200B;**[!UICONTROL 作业选项]**，然后指定所需的选项。

   请参阅[上载选项](uploading-files.md#upload_options)。

1. 在“上载作业选项”对话框中，选择&#x200B;**[!UICONTROL 保存]**。
1. 在上传页面的右下角，选择&#x200B;**[!UICONTROL 提交上传]**。

   要查看上载进度，请在全局导航栏上选择&#x200B;**[!UICONTROL 作业]**。 “作业”页将显示上载进度。您可以继续在Adobe Dynamic Media Classic中工作。 随时返回到“作业”页以查看正在进行的作业。

要取消正在进行的上载作业，请选择“持续时间”旁边的“**[!UICONTROL 取消]**”。

## “上载作业选项”对话框 {#upload-options}

上载文件时，可以在“上载作业选项”对话框中选择以下选项：

* **作业**：选择&#x200B;**[!UICONTROL 作业]**&#x200B;可选择影响整个上载作业的选项。

  也可以使用“常规设置”中的&#x200B;*默认上载选项*&#x200B;对话框为上载作业选择&#x200B;**[!UICONTROL 默认]**&#x200B;选项。 转到&#x200B;**[!UICONTROL 设置]** > **[!UICONTROL 应用程序设置]** > **[!UICONTROL 常规设置]** > **[!UICONTROL 默认上载选项]**，然后设置所需的默认选项。

   * **[!UICONTROL 时间]**：仅当您选择&#x200B;**[!UICONTROL 通过FTP]**&#x200B;选项卡时，此选项才可用。
      * **[!UICONTROL 一次]**：指定运行一次的上载作业。 选项包括：
         * **[!UICONTROL 现在]**：在“上载作业选项”对话框中选择&#x200B;**[!UICONTROL 保存]**&#x200B;后，立即运行上载作业，然后在“上载”页面上选择&#x200B;**[!UICONTROL 提交上载]**。
         * **[!UICONTROL 安排稍后运行]**：选择您希望上载作业运行的年、月、日和时间（以15分钟为增量）。
      * **[!UICONTROL 定期]**：指定每日、每周或每月运行的上载作业。 或者，根据您自己的规范自定义上载作业。
         * **[!UICONTROL 每日]**：设置您希望作业每天运行的时间。 如果希望作业只在星期一到星期五运行，请选择&#x200B;**[!UICONTROL 仅工作日]**。
         * **[!UICONTROL 每周]**：选择您希望作业在一周中的特定日期和运行时间。
         * **[!UICONTROL 每月]**：选择您希望作业运行的特定日期（一个月或一周中的某一天），包括开始时间。
         * **[!UICONTROL 自定义]**：根据您自己的规范自定义上载或发布作业时间间隔。 请参阅[创建自定义上载或发布作业时间间隔](checking-job-files.md#creating-a-custom-upload-or-publish-job-time-interval)。

   * 上传后发布&#x200B;****：如果选择了通过FTP的&#x200B;**[!UICONTROL 从桌面]**&#x200B;选项卡或&#x200B;**[!UICONTROL 选项卡]**，则可用。 选择此选项可自动发布您上传的资产。 在发布文件时，文件将发送到实时服务器。然后，可以在外部网站和应用程序中使用这些文件的 URL。“上载”页中也提供了该选项。

   * **[!UICONTROL 在任意文件夹内，使用相同的基本资源名称（不论扩展名是什么）进行覆盖]**：如果选择&#x200B;**[!UICONTROL FROM DESKTOP]**&#x200B;选项卡或&#x200B;**[!UICONTROL VIA FTP]**&#x200B;选项卡，则可用。 如果要使上载的文件替换现有同名文件，请选中此选项。“上载”页中也提供了该选项。此选项的名称可能不同，具体取决于&#x200B;**[!UICONTROL 设置]** > **[!UICONTROL 应用程序设置]** > **[!UICONTROL 常规设置]** > **[!UICONTROL 上载到应用程序]** > **[!UICONTROL 覆盖图像]**&#x200B;中的设置。

   * **[!UICONTROL 在上传时解压缩Zip或Tar文件]**：如果选择&#x200B;**[!UICONTROL FROM DESKTOP]**&#x200B;选项卡或&#x200B;**[!UICONTROL VIA FTP]**选项卡，则可用。
选择此选项可自动从上传的ZIP或TAR文件中提取所有文件。 “作业选项”对话框中也提供了相同选项。

   * **[!UICONTROL 包含子文件夹]**：仅当您选择&#x200B;**[!UICONTROL 通过FTP]**选项卡时可用。
如果要上载文件夹的子文件夹，请选中此选项。上传的文件夹及其子文件夹的名称会自动在Adobe Dynamic Media Classic中输入。

   * **[!UICONTROL 处理元数据文件]**：仅当您选择&#x200B;**[!UICONTROL 通过FTP]**选项卡时可用。 如果要上载制表符分隔的文件或XML文件以将元数据添加到多个资源，请选择此选项。
请参阅[导入元数据（通过 FTP）](viewing-adding-exporting-metadata.md#import-metadata)。

* **裁切选项**：自动裁切图像中的空白像素。 打开&#x200B;**[!UICONTROL 裁切]**&#x200B;菜单，选择&#x200B;**[!UICONTROL 手动]**，然后在“顶部”、“右侧”、“底部”和“左侧”文本字段中输入像素度量以从侧面裁切。 您还可以在“裁切”菜单中选择&#x200B;**[!UICONTROL 裁切]**，然后选择以下选项：

   * **[!UICONTROL 裁切依据]**：选择根据颜色还是透明度裁切：
      * **[!UICONTROL 颜色]**：选择“颜色”选项。 然后选择“边角”菜单，然后选择图像的边角，其颜色最能代表要裁切的空白颜色。
基于颜色修剪：指定 0 则仅当像素与您在图像的角中选择的颜色完全匹配时才会裁切像素。数字越接近 1，允许的色差越大。
      * **[!UICONTROL 透明度]**：选择&#x200B;**[!UICONTROL 透明度]**选项。
基于透明度裁剪：指定0表示仅在像素为透明时裁剪像素；数字越接近1则透明度越高。
      * **[!UICONTROL 容差]**：拖动滑块以指定从0到1的容差。

* **颜色配置文件选项**：在创建用于Adobe Dynamic Media Classic动态投放的优化文件时选择颜色转换：

   * **[!UICONTROL 默认保色]**：当图像包含色彩空间信息时，保留源图像颜色；没有颜色转换。 几乎目前的所有图像都嵌入了相应的颜色配置文件。不过，如果 CMYK 源图像不包含嵌入的颜色配置文件，则会将颜色转换为 sRGB（标准红绿蓝）色彩空间。sRGB是在网页上显示图像的推荐颜色空间。
   * **[!UICONTROL 保留原始颜色空间]**：保留原始颜色，在摄取到Adobe Dynamic Media Classic时不会进行任何颜色转换。 对于没有嵌入颜色配置文件的图像，使用在“发布”设置中配置的默认颜色配置文件执行任何处理图像请求所需的颜色转换。 这些颜色配置文件并不总是与使用此选项创建的文件中的颜色一致。 因此，建议您使用“默认护色”选项。
   * **[!UICONTROL 自定义从]** > **[!UICONTROL 到]**：打开菜单，以便选择&#x200B;**[!UICONTROL 转换自]**&#x200B;和&#x200B;**[!UICONTROL 转换至]**&#x200B;色彩空间。 此高级选项覆盖在源文件中嵌入的任何颜色信息。仅当要提交的所有图像包含不正确或缺少颜色配置文件数据时，才选择此选项。

* **图像编辑选项**：您可以保留图像中的剪切&lt;>蒙版，并选择颜色配置文件。
在上传[中查看](image-editing-options-upload.md#image-editing-options-at-upload)映像微调选项。

* **PostScript®选项**：您可以栅格化PostScript®文件、裁切文件、保持透明背景、选择分辨率以及选择色彩空间。
请参阅[处理PostScript和Illustrator文件](postscript-illustrator-files.md#working_with_postscript_and_illustrator_files)。

* **Photoshop选项**：您可以从Adobe® Photoshop®文件创建模板、维护图层、指定图层的命名方式、提取文本以及指定将图像锚定到模板中的方式。
请参阅[PSD 上载选项](psd-files.md#psd_upload_options)。

* **PDF选项**：您可以栅格化文件、提取搜索词和链接、自动生成eCatalog、设置分辨率以及选择颜色空间。
请参阅[PDF 上载选项](pdfs.md#pdf_upload_options)。

* **Illustrator选项**：您可以栅格化Adobe Illustrator®文件、保持透明背景、选择分辨率以及选择色彩空间。
请参阅[处理PostScript和Illustrator文件](postscript-illustrator-files.md#working_with_postscript_and_illustrator_files)。

* **EVIDEO选项**：您可以通过选择视频预设来转码视频文件。
请参阅[使用视频编码预设](uploading-encoding-videos.md#working_with_video_encoding_presets)。

* **更多元数据**：输入描述要上载的文件的关键字。 用逗号分隔关键字。关键字使搜索资源更容易。
请参阅[执行高级搜索](searching-assets.md#conducting_an_advanced_search)。
另请参阅[上传关键字](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/548_upload-keywords_converted%20renamed_Done-AVS)培训视频。

* **批次集预设**：若要从上传的文件创建图像集、旋转集或样本集，请为要使用的预设选择&#x200B;**[!UICONTROL 活动]**列。 可以选择多个预设。您可以在“应用程序设置/批次集预设”页面中创建预设。
请参阅[批量级预设](application-setup.md#batch_set_presets)。

* **高级**：请参阅[使用其他作业执行上载操作](uploading-files.md#follow-an-upload-with-another-job)。

## 上载后执行其他作业 {#follow-an-upload-with-another-job}

使用FTP上传项目时，您可以安排在上传完成后开始后续作业。 如果调度了其他作业以开始，则您在此处调度的作业将在它们之后排队。

新作业会向您指定的地址发送通知，以便触发该位置的代码。 该后续发布作业所使用的名称与上载作业相同，但在开头加有文本 *Pub_*。

**要在上载后执行其他作业：**

1. 选择&#x200B;**[!UICONTROL 上传]**，然后选择&#x200B;**[!UICONTROL 通过FTP]**&#x200B;选项卡。
1. 在上传页面的右下角，选择&#x200B;**[!UICONTROL 作业选项]**。
1. 在“上载作业选项”对话框中，展开&#x200B;**[!UICONTROL 高级]**&#x200B;部分。
1. 从&#x200B;**[!UICONTROL 上载后执行其他作业]**&#x200B;下拉列表中选择以下选项之一：

   * 无
   * HTTP 请求
   * 图像服务发布
   * 图像渲染发布
   * 视频发布

1. 指定 HTTP 地址。
1. 指定是否只在上传文件后运行。
1. 指出是要在每次完成该作业时运行该请求，还是仅在发布文件时运行该请求。

   >[!NOTE]
   >
   >定期计划的作业有时会导致不发布任何文件。

>[!MORELIKETHIS]
>
>* [使用资源文件夹](asset-folders.md#working_with_asset_folders)
>* [处理周期性上载和发布作业](checking-job-files.md#handling_recurring_upload_and_publish_jobs)
>* [使用上载或发布作业作为触发器](checking-job-files.md#using_an_upload_or_publish_job_as_a_trigger)
