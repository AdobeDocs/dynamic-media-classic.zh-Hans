---
title: 上载文件
description: 了解如何在AdobeDynamic Media Classic中上传文件。
uuid: b3025f84-4f28-4276-bc9c-f0c0c2a26e12
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: b2bc3bf9-e313-481a-8670-c3bedde21b1a
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 8dfcfb3f-6472-4efd-bc87-d5111eee45ce
source-git-commit: 44045daa35052f01a26c67e0b2a0fb1405c53292
workflow-type: tm+mt
source-wordcount: '3866'
ht-degree: 34%

---

# 上载文件{#uploading-files}

在将资产文件上传到Dynamic Media Classic之前，请确保资产文件的名称正确，并且文件夹结构的设置和组织方式符合您的需要。 您可以从AdobeDynamic Media Classic提供的FTP站点上传文件，也可以直接从您的计算机或网络上传文件。 AdobeDynamic Media Classic提供了在上传文件时优化文件的选项。 如果您安装了AdobeDynamic Media Classic桌面应用程序，则可以通过直接从桌面拖动文件和文件夹来上传它们。 请参阅[应用程序常规设置](application-setup.md#general_settings)。

## 准备要上传的资产和文件夹 {#preparing-your-assets-and-folders-for-uploading}

在将资产上传到AdobeDynamic Media Classic之前，请确保资产的格式和大小均正确。 您还必须遵守AdobeDynamic Media Classic资产命名规则。 通过设置文件的文件夹组织和结构，可确保可以轻松定位及处理文件。

### 支持的资源文件格式 {#supported-asset-file-formats}

此表列出了AdobeDynamic Media Classic支持的资产文件格式。 有关支持的Camera Raw文件的信息，请参阅[https://helpx.adobe.com/camera-raw/using/supported-cameras.html](https://helpx.adobe.com/camera-raw/using/supported-cameras.html)。

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
| AdobeDynamic Media Classic图像创作 | VNC、VNT、VNW |
| SVG | SVG、SVGX |
| TAR | TAR |
| 视频 | 3GP、AVI、M2P、M2T、M2TS、M2V、M4V、MOV、MP4、MPEG、MPG、MTS、OGV、TS、VOB、WMV/ASF |
| XML | XML |
| ZIP | ZIP |

TAR 和 ZIP 上载支持包括一个复选框，用于选择是否要解压缩文件。

### Dynamic Media中不支持的图像格式 {#unsupported-image-formats-dynamic-media}

下表描述了Dynamic Media中支持的&#x200B;*not*&#x200B;光栅图像文件格式的子类型。

另请参阅[检测不支持的Dynamic Media](https://helpx.adobe.com/experience-manager/kb/detect-unsupported-assets-for-dynamic-media.html)文件格式。

* IDAT区块大于100 MB的PNG文件。
* PSB文件。
* 不支持具有非CMYK、RGB、灰度或位图的色彩空间的PSD文件。 不支持DuoTone、Lab和索引色彩空间。
* 位深度大于16的PSD文件。
* 具有浮点数据的TIFF文件。
* 具有Lab色彩空间的TIFF文件。

### 资源类型 {#asset-types}

要通过AdobeDynamic Media Classic程序获得最佳结果，请务必使用推荐的文件格式和大小。 下表列出了资源类型，其中一些资源类型列有常用资源的推荐格式和文件大小。

| 资源类型 | 说明/推荐 |
| --- | --- |
| 音频 | 输入音频资源格式，其中包括 AAC、HE-AAC、AC3、WAV、WMA、AIFF、MP3。可以将音频转码为以下格式：MP3、AAC 和 HE-AAC。 |
| 图像（用于调整图像大小、缩放、图像集、旋转集） | 图像的最大尺寸必须至少为2000像素；典型图像大小在1500到2500像素之间，最长大小。 推荐使用无损图像格式，包括 TIFF 和 PNG 文件。如果使用 JPEG 图像，请使用最高质量设置。Animate GIF文件的处理方式与其他静态内容类似。 |
| eCatalog | 使用在 Adobe® Acrobat® 或 Creative Suite 应用程序中创建并保存为“印刷就绪”的高分辨率 PDF 文件。PDF 包括所有需要的字体、图像、蒙版以及引用的图形元素，采用单页、两页跨页或多页格式。通过按字母数字顺序为文件命名来排列页面顺序。将 eCatalog 类型的所有 PDF 文件放于一个文件夹中，以便于上载。您可以在上载时选择裁切选项，以便从 PDF 中删除修剪区域，包括裁切标记、对齐目标或颜色条。多数印刷就绪的 PDF 文件采用 CMYK 颜色空间，因此务必要获得用于 PDF 文件的 CMYK ICC 颜色配置文件。 |
| 模板 | 分层图像或布局设计，可以包括文本、图像和图层。可以将图层、文本字符串和属性（如颜色和大小）参数化，从而可以自定义变量数据。在模板中使用时的图像要求与其他图像相同。在 Photoshop 或其他图像编辑程序中准备图形。采用 TIFF 或 PNG 格式将每个图形保存为平面化透明文件。确保图像分辨率适合所要求的用途。打印图像为300 ppi。 |
| 视频 | AdobeDynamic Media Classic支持以OGV和MP4格式保存的视频文件。 您可以在上载时将文件转码为 MP4 格式。请参阅[支持的资源文件格式](#supported-static-file-formats)。 |
| 字体 | 上传了TrueType、Type1(仅限Windows®)、OpenType®字体和PhotoFonts。 |
| 图像 | 图像和分层图像文件。 |
| 图像集和样本集 | 可以显示在查看器中的一组相关图像。 |
| ICC 配置文件 | 颜色配置文件，可以用来将上载的图像从源颜色空间转换为其他颜色空间。 |
| 晕影 | 使用“图像创作”程序创作的图像以及相关文件。 |
| 内容文件 | Adobe InDesign、Illustrator 或 Photoshop 内容文件。 |
| FXG 文件 | 与分辨率无关的图形格式文件；可用于创建可自定义的模板，以输出到打印、网络、电子邮件、桌面和设备。 |
| SVG 文件 | 图像服务服务器可以渲染的可缩放矢量图形文件。 |
| XML 文件 | 定义用于修改请求的路径和查询部分的预处理规则的文件。 |
| 级联样式表文件。 | 上载用于自定义 HTML5 查看器的 CSS 外观。 |
| JavaScript 文件 | JavaScript文件用于查看器工具以保存帐户信息。 Adobe安全建议，仅对于在交付时使用单独域的客户帐户，才应使用此资产类型（以避免跨站点脚本）。 |

>[!NOTE]
>
>在将图像文件和PDF上传到AdobeDynamic Media Classic时，系统会将这些源文件转换为P-TIFF(Pyramid TIFF)文件。 这些P-TIFF是稍后发布到Dynamic Media图像服务器的文件。 AdobeDynamic Media Classic使用Pyramid Tiff文件格式，因为它包含各种缩放比率，当使用AdobeDynamic Media Classic缩放查看器查看时，这些比率允许快速缩放。

### 支持静态文件格式 {#supported-static-file-formats}

AdobeDynamic Media Classic支持多种静态文件格式。 静态内容是指按“原样”发布的任何资产，例如CSS、PDF、SVG和XML。

可以发布以下文件类型：

* GIF 动画
* 音频文件
* CSS
* JavaScript（为公司配置自己的域时）
* 主视频
* PDF（当PDF在上传后标记为发布时，为了避免交付现有eCatalog/PDF工作流的所有PDF）
* PrX 视频
* SVG
* XML
* ZIP

AdobeDynamic Media Classic不提供用于生成静态内容的预览URL的选项。

### 文件名要求 {#filename-requirements}

由于在文件上载过程中将去除文件名中的扩展名，因此系统不允许文件使用相同的根名称。在AdobeDynamic Media Classic系统中，资产文件名减去文件扩展名会变为资产的资产ID。 因此，两个资源不能同名。

确保贵公司的所有用户都了解以下文件命名规则：

* 系统中不允许存在名称完全相同的资源 ID。
* 资产ID名称区分大小写。
* 最佳做法是确保资源 ID 不包含空格（例如 black jacket.tif 和 blue jacket.jpg）。AdobeDynamic Media Classic ASCII在使用资产名称构建URL字符串时，会对资产名称中的空格进行编码。 这些 ASCII 编码不易理解，从而使 URL 更难理解。
* 文件名中允许特定语言字符。但是，文件名中不能出现以下字符：

   \ ;/ ? :@ &amp; = + $ , * &quot; &lt; > | ` { } %

   如果文件名包含一个或多个上述字符，将会在上载时删除这些字符。

通常，资产文件名可以与其项目号、产品SKU或其他名称相同，如下所示：

| 商品 | 文件名 | 资源 ID |
|--- |--- |--- |
| 896649 | 896649.jpg | 896649 |
| 48A3_2X | 48A3_2X.tif | 48A3_2X |

### 文件夹组织和结构 {#folder-organization-and-structure}

在将内容上传到系统之前，请先在Dynamic Media Classic中为您的内容组织和Adobe文件夹及子文件夹。 采用这种方式提前进行规划主要有两个好处：

* 在通过FTP将内容上传到Dynamic Media Classic时，您可以告知系统在上传期间复制您的文件夹结构。 这样，您的内容就会组织在Dynamic Media ClassicAdobe中与您的计算机或网络上相同的文件夹和子文件夹中。 (要在Dynamic Media Classic中复制您的文件夹结构，请在您通过FTP上传Adobe时选择包含子文件夹选项。)
* 与在开始就使用经过仔细计划的文件夹结构相比，在文件上载之后重新对系统内的文件夹进行组织要困难得多。

在Dynamic Media ClassicAdobe上存储内容时选择的文件夹命名方法和结构取决于贵组织的需求。 以下是一些文件夹结构示例：

**基于SKU的**  — 文件夹的命名依据是SKU或项目编号。例如，为所有以 0、20、30 开头的编号序列分别创建单独的文件夹。

**基于品牌**  — 对于具有多个品牌线的制造商和营销其他品牌的零售商，请将文件分隔到为不同品牌命名的产品文件夹中。

**基于项目**  — 根据转出/删除日期或项目名称组织文件夹。主要生成 eCatalog 的客户喜欢使用这种方法。

**网站文件夹层次结构的镜像**  — 此文件夹结构反映网站的文件夹结构，例如，产品类别的文件夹名为。

## 关于上传文件 {#uploading-your-files}

可以从桌面上载单个文件或通过 FTP 上载文件夹。如果要上传超过100 MB的文件或上传整个文件夹和子文件夹，请选择&#x200B;**VIA FTP**&#x200B;选项卡。

AdobeDynamic Media Classic会向您发送一封电子邮件，以确认上传作业何时开始和结束，并通知您任何问题。

在大型上传作业期间（或紧接着），某些新项目可能会显示“图像尚未优化”消息。 出现此消息是因为文件尚未完全处理并添加到AdobeDynamic Media Classic。 您可以稍后优化这些文件。请参阅[优化文件](application-setup.md#optimize_files)。

### 使用“从桌面”选项卡上传文件 {#upload-files-using-sps-desktop-application}

AdobeDynamic Media Classic桌面应用程序允许您通过拖动上传文件和文件夹。

1. 在AdobeDynamic Media Classic桌面应用程序的全局导航栏上，选择&#x200B;**[!UICONTROL Upload]**。
1. 在“上载”页面上，选择&#x200B;**[!UICONTROL 从Desktop]**&#x200B;选项卡。
1. 在“上传”页面左侧的&#x200B;**[!UICONTROL 选择要上传的文件]**&#x200B;区域中，选择&#x200B;**[!UICONTROL Browse]**&#x200B;以选择要上传的文件或文件夹，然后选择&#x200B;**[!UICONTROL Open]**。
1. 在“上传”页面右侧的&#x200B;**选择文件夹目标**&#x200B;区域中，导航到要在其中添加已上传文件或文件夹的目标文件夹。
1. （可选）在“上传”页面底部附近的“作业名称”文本字段中，输入上传作业的新名称。 或者，您也只需使用Dynamic Media Classic提供的默认系统生成名称即可。 将在“作业”页中记录此作业和其他上载和发布作业，可以在此页中检查作业的状态。请参阅[检查作业文件](checking-job-files.md#checking_job_files)。
1. （可选）如果要自动发布上传的资产，请在上传页面底部附近选择&#x200B;**[!UICONTROL 上传后发布]**。
在发布文件时，文件将发送到实时服务器。然后，可以在外部网站和应用程序中使用这些文件的 URL。“作业选项”(Job Options)对话框中也提供此选项。
1. （可选）在“上传”页面底部附近，选择&#x200B;**[!UICONTROL 覆盖任意文件夹中相同的基本资产名称（无论扩展名]**）（如果希望上传的文件替换具有相同名称的现有文件）。 “作业选项”(Job Options)对话框中也提供此选项。
此选项的名称可能不同，具体取决于**[!UICONTROL 应用程序设置]** > **[!UICONTROL 常规设置]** > **[!UICONTROL 上传到应用程序]** > **[!UICONTROL 覆盖图像]**&#x200B;中的设置。
1. 在“上载”页的右下角附近，选择&#x200B;**[!UICONTROL 作业选项]**，然后指定所需的选项。

   请参阅[上载选项](uploading-files.md#upload_options)。

1. 在上传作业选项对话框中，选择&#x200B;**[!UICONTROL 保存]**。
1. 在上传页面的右下角，选择&#x200B;**[!UICONTROL 提交上传]**。
要查看上传进度，请在全局导航栏上选择**[!UICONTROL 作业]**。 您可以继续在Adobe Dynamic Media Classic中工作，并随时返回到“作业”页面以查看正在进行的作业。 要取消正在进行的上载作业，请选择“持续时间”旁边的“**[!UICONTROL 取消]**”。

### 使用“通过FTP”选项卡上传文件 {#upload-files-using-via-ftp}

1. 登录到特定于您的特定区域的AdobeDynamic Media Classic FTP站点。 使用您从管理员那里收到的 FTP 用户名和密码。
1. 在AdobeDynamic Media Classic的全局导航栏上，选择&#x200B;**[!UICONTROL Upload]**。
1. 在“上传”页面上，选择&#x200B;**[!UICONTROL VIA FTP]**&#x200B;选项卡。
1. 在“上传”页面左侧的&#x200B;**[!UICONTROL 选择要上传的FTP文件夹]**&#x200B;区域，选择要从中上传文件的FTP文件夹。
1. 在“上传”页面右侧的&#x200B;**[!UICONTROL 选择AdobeDynamic Media文件夹目标]**&#x200B;区域中，在AdobeDynamic Media Classic中选择一个目标文件夹。
1. （可选）在“上传”页面底部附近的“作业名称”文本字段中，输入上传作业的新名称。 或者，您也只需使用Dynamic Media Classic提供的默认系统生成名称即可。 将在“作业”页中记录此作业和其他上载和发布作业，可以在此页中检查作业的状态。请参阅[检查作业文件](checking-job-files.md#checking_job_files)。
1. （可选）如果要自动发布上传的资产，请在上传页面底部附近选择&#x200B;**[!UICONTROL 上传后发布]**。
在发布文件时，文件将发送到实时服务器。然后，可以在外部网站和应用程序中使用这些文件的 URL。“作业选项”(Job Options)对话框中也提供此选项。
1. （可选）在“上传”页面底部附近，选择&#x200B;**[!UICONTROL 覆盖任意文件夹中相同的基本资产名称（无论扩展名]**）（如果希望上传的文件替换具有相同名称的现有文件）。 “作业选项”(Job Options)对话框中也提供此选项。
此选项的名称可能不同，具体取决于**[!UICONTROL 设置]** > **[!UICONTROL 应用程序设置]** > **[!UICONTROL 常规设置]** > **[!UICONTROL 上传到应用程序]** > **[!UICONTROL 覆盖图像]**&#x200B;中的设置。
1. 可选；仅当您单击&#x200B;**[!UICONTROL VIA FTP]**&#x200B;选项卡时才可用。 如果要自动从上传的ZIP或TAR文件中提取所有文件，请在“上传”页面底部附近选择&#x200B;**[!UICONTROL Uncompress Zip或Tar Files on Upload]**。 “作业选项”(Job Options)对话框中也提供此选项。
1. 在“上载”页的右下角附近，选择&#x200B;**[!UICONTROL 作业选项]**，然后指定所需的选项。

   请参阅[上载选项](uploading-files.md#upload_options)。

1. 在上传作业选项对话框中，选择&#x200B;**[!UICONTROL 保存]**。
1. 在上传页面的右下角，选择&#x200B;**[!UICONTROL 提交上传]**。

   要查看上传进度，请在全局导航栏上选择&#x200B;**[!UICONTROL 作业]**。 “作业”页将显示上载进度。您可以继续在Adobe Dynamic Media Classic中工作，并随时返回到“作业”页面以查看正在进行的作业。

要取消正在进行的上载作业，请选择“持续时间”旁边的“**[!UICONTROL 取消]**”。

## “上载作业选项”对话框 {#upload-options}

上传文件时，您可以在“上传作业选项”对话框中从以下选项中进行选择：

* **作业**  — 选择作 **** 业以选择影响整个上载作业的选项。

   您还可以使用“常规设置”中的&#x200B;**[!UICONTROL 默认上传选项]**&#x200B;对话框，选择&#x200B;*默认*&#x200B;选项以上传作业。 转到&#x200B;**[!UICONTROL 设置]** > **[!UICONTROL 应用程序设置]** > **[!UICONTROL 常规设置]** > **[!UICONTROL 默认上传选项]**，然后设置所需的默认选项。

   * **[!UICONTROL 当]**  — 仅当您选择“通过FTP”选项卡时，此选 **[!UICONTROL 项]** 才可用。
      * **[!UICONTROL 一次性]**  — 指定运行一次的上传作业。选项包括：
         * **[!UICONTROL 现在]**  — 在选择保存上传作业选项对话框后立即 **** 运行上传作业，然后在上传页 **[!UICONTROL 面选]** 择提交上传。
         * **[!UICONTROL 安排稍后执行]**  — 选择您希望上传作业运行的年、月、日和时间（以15分钟的增量为单位）。
      * **[!UICONTROL 定期]**  — 指定每日、每周或每月运行的上传作业。或者，根据您自己的规范自定义上传作业。
         * **[!UICONTROL 每日]**  — 设置您希望作业每天运行的时间。如果希望作业仅在星期一到星期五运行，请选择&#x200B;**[!UICONTROL 仅限工作日]**。
         * **[!UICONTROL 每周]**  — 选择您希望该作业运行的特定日期和时间。
         * **[!UICONTROL 每月]**  — 选择您希望该作业运行的月份或一周中某天的特定日期（包括开始时间）。
         * **[!UICONTROL 自定义]**  — 根据您自己的规范自定义上传或发布作业时间间隔。请参阅[创建自定义上传或发布作业时间间隔](checking-job-files.md#creating-a-custom-upload-or-publish-job-time-interval)。
   * **[!UICONTROL 上传后发布]**  — 如果您选择了“来自桌面”选 **[!UICONTROL 项]** 卡或“通过 **[!UICONTROL FTP”选]** 项卡，则可用。选择此选项以自动发布上载的资源。在发布文件时，文件将发送到实时服务器。然后，可以在外部网站和应用程序中使用这些文件的 URL。“上载”页中也提供了该选项。

   * **[!UICONTROL 无论是否扩展名，都会覆盖任何文件夹中相同的基本资产名称]**  — 如果您选择了“来自桌面”选项卡或“通过FTP”选 **[!UICONTROL 项]** 卡，则 **[!UICONTROL 将]** 可用。如果要使上载的文件替换现有同名文件，请选中此选项。“上载”页中也提供了该选项。此选项的名称可能不同，具体取决于&#x200B;**[!UICONTROL 设置]** > **[!UICONTROL 应用程序设置]** > **[!UICONTROL 常规设置]** > **[!UICONTROL 上传到应用程序]** > **[!UICONTROL 覆盖图像]**&#x200B;中的设置。

   * **[!UICONTROL 上传时解压缩Zip或Tar文件]**  — 如果您选择了“来自桌面”选项卡或“通 **[!UICONTROL 过]** FTP”选 **[!UICONTROL 项卡，则]** 可用。如果要自动从上传的ZIP或TAR文件中提取所有文件，请选择此选项。 “作业选项”(Job Options)对话框中也提供此选项。

   * **[!UICONTROL 包含子文件夹]**  — 仅当您选择“通过FTP”选项卡时 **[!UICONTROL 才]** 可用。如果要上载文件夹的子文件夹，请选中此选项。您上传的文件夹及其子文件夹的名称会自动输入到AdobeDynamic Media Classic中。

   * **[!UICONTROL 处理元数据文件]**  — 仅当您选择“通过FTP”选项卡时 **[!UICONTROL 才]** 可用。如果要上载制表符分隔的文件或 XML 文件以将元数据添加到多个资源中，可以选择该选项。请参阅[导入元数据（通过 FTP）](viewing-adding-exporting-metadata.md#import-metadata)。


* **裁剪OPTIONS**  — 要自动从图像裁剪空格像素，请打开 **** 裁剪菜单，选择 **[!UICONTROL 手动]**，然后在“顶部”、“右”、“底部”和“左”文本字段中输入像素测量，以从侧边裁剪。您还可以在“裁剪”菜单中选择&#x200B;**[!UICONTROL Trim]**&#x200B;并选择以下选项：

   * **[!UICONTROL 根据]** 裁切掉 — 选择是根据颜色还是透明度进行裁剪：
      * **[!UICONTROL 颜色]**  — 选择“颜色”选项。然后选择“角”菜单，并选择所具有的颜色能最好地表示您想要裁切的空白颜色的图像角。基于颜色修剪：指定 0 则仅当像素与您在图像的角中选择的颜色完全匹配时才会裁切像素。数字越接近 1，允许的色差越大。
      * **[!UICONTROL 透明度]**  — 选择“透明 **** 度”选项。基于透明度进行裁切：指定0，以仅在像素透明时裁剪像素；接近1的数字使透明度更高。
      * **[!UICONTROL 容差]**  — 拖动滑块以指定从0到1的容差。

* **颜色配置文件OPTIONS**  — 在创建用于AdobeDynamic Media Classic动态交付的优化文件时，选择颜色转换：

   * **[!UICONTROL 默认颜色保留]**  — 当图像包含色彩空间信息时，保留源图像的颜色；没有颜色转换。几乎目前的所有图像都嵌入了相应的颜色配置文件。不过，如果 CMYK 源图像不包含嵌入的颜色配置文件，则会将颜色转换为 sRGB（标准红绿蓝）色彩空间。在网页上显示图像时，推荐使用 sRGB 颜色空间。
   * **[!UICONTROL 保留原始色彩空间]**  — 在摄取到Dynamic Media Classic时，不进行任何颜色转换，即可保留原始Adobe。对于没有嵌入颜色配置文件的图像，使用“发布”设置中配置的默认颜色配置文件完成处理图像请求所需的任何颜色转换。 这些颜色配置文件并不总是与使用此选项创建的文件中的颜色保持一致。 因此，建议您使用“默认护色”选项。
   * **[!UICONTROL 自定义自]**  >  **[!UICONTROL 至]**  — 打开菜单，以便您可以选择“转换自” **[!UICONTROL 和“]** 转换 **[!UICONTROL 为]** 颜色空间”。此高级选项覆盖在源文件中嵌入的任何颜色信息。仅当您要提交的所有图像都包含不正确或缺少的颜色配置文件数据时，才选择此选项。

* **图像编辑选项**  — 您可以在图像中保留剪 &lt;> 贴蒙版，并选择颜色配置文件。请参阅上传](image-editing-options-upload.md#image-editing-options-at-upload)时的[图像微调选项。

* **PostScript®选项**  — 您可以栅格化PostScript®文件、裁剪文件、维护透明背景、选择分辨率和选择色彩空间。请参阅[使用PostScript和Illustrator文件](postscript-illustrator-files.md#working_with_postscript_and_illustrator_files)。

* **Photoshop选项**  — 您可以从Adobe® Photoshop®文件创建模板、维护图层、指定图层的命名方式、提取文本，以及指定图像如何定位到模板中。请参阅[PSD 上载选项](psd-files.md#psd_upload_options)。

* **PDF选项**  — 您可以栅格化文件、提取搜索词和链接、自动生成eCatalog、设置分辨率和选择色彩空间。请参阅[PDF 上载选项](pdfs.md#pdf_upload_options)。

* **Illustrator选项**  — 您可以栅格化Adobe Illustrator®文件、维护透明背景、选择分辨率和选择色彩空间。请参阅[使用PostScript和Illustrator文件](postscript-illustrator-files.md#working_with_postscript_and_illustrator_files)。

* **EVIDEO选项**  — 您可以通过选择视频预设对视频文件进行转码。请参阅[使用视频编码预设](uploading-encoding-videos.md#working_with_video_encoding_presets)。

* **其他元数据**  — 输入描述要上传文件的关键字。用逗号分隔关键字。关键字简化了资源搜索。请参阅[执行高级搜索](searching-assets.md#conducting_an_advanced_search)。

* **批集预设**  — 如果要从上传的文件中创建图像集、旋转集或样本集，请为要使 **** 用的预设选择活动列。可以选择多个预设。您可以在“应用程序设置/批量集预设”页中创建预设。请参阅[批量级预设](application-setup.md#batch_set_presets)。

* **高级**  — 请参阅 [在上载其他作业后](uploading-files.md#follow-an-upload-with-another-job)。

## 上载后执行其他作业 {#follow-an-upload-with-another-job}

使用FTP上传项目时，您可以安排在上传完成后开始后续作业。 如果其他作业已计划开始，则您在此处计划的作业将在它们之后排入队列。

新作业将向您指定的地址发送一条通知，以触发该位置的代码。该后续发布作业所使用的名称与上载作业相同，但在开头加有文本 *Pub_*。

**上载后执行其他作业:**

1. 选择&#x200B;**[!UICONTROL Upload]**，然后选择&#x200B;**[!UICONTROL VIA FTP]**&#x200B;选项卡。
1. 在“上载”页的右下角，选择&#x200B;**[!UICONTROL 作业选项]**。
1. 在上传作业选项对话框中，展开&#x200B;**[!UICONTROL ADVANCED]**&#x200B;部分。
1. 从&#x200B;**[!UICONTROL Follow Upload with another job]**&#x200B;下拉列表中选择以下选项之一：

   * 无
   * HTTP 请求
   * 图像服务发布
   * 图像渲染发布
   * 视频发布

1. 指定 HTTP 地址。
1. 指定是否仅在上传文件时才运行。
1. 指出是要在每次完成该作业时运行该请求，还是仅在发布文件时运行该请求。

   >[!NOTE]
   >
   >定期计划的作业有时不会导致任何文件发布。

>[!MORELIKETHIS]
>
>* [使用资产文件夹](asset-folders.md#working_with_asset_folders)
>* [处理定期上传和发布作业](checking-job-files.md#handling_recurring_upload_and_publish_jobs)
>* [使用上传或发布作业作为触发器](checking-job-files.md#using_an_upload_or_publish_job_as_a_trigger)

