---
title: 上载文件
seo-title: 上载文件
description: 'null'
seo-description: 了解如何上传文件。
uuid: b3025f84-4f28-4276-bc9 c-f0 c0 c2 a26 e12
contentOwner: admin
content-type: 引用
products: SG_ EXPERIENCE MANAGER/Dynamic-Media-Scene-7
discoiquuid: b2bc3bf9-e313-481a-8670-c3 bedde21 b1 a
translation-type: tm+mt
source-git-commit: 684950586bf9b1df897ac46b52d84a21f4cb4120

---


# 上载文件{#uploading-files}

将资源文件上载到 Scene7 Publishing System 之前，确保资源文件命名正确，并且文件夹结构的建立及组织符合要求。您可以从Dynamic Media经典提供的FTP站点或直接从计算机或网络上传文件。动态媒体经典提供了在上传文件时优化文件的选项。如果安装了 Adobe Scene7 Publishing System 桌面应用程序，可以采用直接从桌面拖动的方式来上载文件和文件夹。（请参阅[应用程序常规设置](application-setup.md#general_settings)。）

## 准备将上载的资源和文件夹 {#preparing-your-assets-and-folders-for-uploading}

在将资源上载至 Scene7 Publishing System 之前，确保资源的格式和大小正确。您还必须观察用于命名资产的Dynamic Media经典规则。通过设置文件的文件夹组织和结构，可确保可以轻松定位及处理文件。

### 支持的资源文件格式 {#supported-asset-file-formats}

下表列出 Scene7 Publishing System 支持的资源文件格式。For information on supported Camera Raw files, see [www.adobe.com/go/learn_s7_cameraraw_en](https://www.adobe.com/go/learn_s7_cameraraw_en).

| 资源文件格式 | 说明 |
|--- |--- |
| 音频 | AAC、HE-AAC、AC3、WAV、WMA、AIFF、MP3 |
| 级联样式表 | CSS |
| 颜色配置文件 | ICC、ICM |
| 字体 | AFM、OTF、PFB、PFM、PhotoFont、TTC、TTF |
| FXG | FXG |
| Illustrator | AI、FXG |
| 图像 | BMP、FPX、GIF、JPEG、JPG、PNG、PICT（仅限 Windows）、TIF、TIFF |
| InDesign | INDD、INDT |
| MS Office | DOC、PPT、RTF、XLS |
| PDF | PDF |
| Photoshop | PSD、FXG 和 Camera Raw |
| PostScript | EPS、PS |
| 动态媒体经典图像创作 | VNC、VNT、VNW |
| SVG | SVG、SVGX |
| TAR | TAR |
| 视频 | 3GP、AVI、M2P、M2T、M2TS、M2V、M4V、MOV、MP4、MPEG、MPG、MTS、OGV、TS、VOB、WMV/ASF |
| XML | XML |
| ZIP | ZIP |

TAR 和 ZIP 上载支持包括一个复选框，用于选择是否要解压缩文件。

### 资源类型 {#asset-types}

要使用Dynamic Media经典平台获得最佳效果，请务必使用建议的文件格式和大小。下表列出了资源类型，其中一些资源类型列有常用资源的推荐格式和文件大小。

| 资源类型 | 说明/推荐 |
|--- |--- |
| 音频 | 输入音频资源格式，其中包括 AAC、HE-AAC、AC3、WAV、WMA、AIFF、MP3。可以将音频转码为以下格式：MP3、AAC 和 HE-AAC。 |
| 图像（用于调整图像大小、缩放、图像集、旋转集） | 图像的最大尺寸必须至少为 2000 像素；典型图像大小最大尺寸范围在 1500 到 2500 像素之间。推荐使用无损图像格式，包括 TIFF 和 PNG 文件。如果使用 JPEG 图像，请使用最高质量设置。Animate GIF文件的处理方式与其他静态内容一样。 |
| eCatalog | 使用在 Adobe® Acrobat® 或 Creative Suite 应用程序中创建并保存为“印刷就绪”的高分辨率 PDF 文件。PDF 包括所有需要的字体、图像、蒙版以及引用的图形元素，采用单页、两页跨页或多页格式。通过按字母数字顺序为文件命名来排列页面顺序。将 eCatalog 类型的所有 PDF 文件放于一个文件夹中，以便于上载。您可以在上载时选择裁切选项，以便从 PDF 中删除修剪区域，包括裁切标记、对齐目标或颜色条。多数印刷就绪的 PDF 文件采用 CMYK 颜色空间，因此务必要获得用于 PDF 文件的 CMYK ICC 颜色配置文件。 |
| 模板 | 分层图像或布局设计，可以包括文本、图像和图层。可以将图层、文本字符串和属性（如颜色和大小）参数化，从而可以自定义变量数据。在模板中使用时的图像要求与其他图像相同。在 Photoshop 或其他图像编辑程序中准备图形。采用 TIFF 或 PNG 格式将每个图形保存为平面化透明文件。确保图像分辨率适合所要求的用途。准备打印的图像应为 300 PPI。 |
| 视频 | Dynamic Media Classic支持以OGV和MP格式保存的视频文件。您可以在上传时将文件转码为MP格式。请参阅 [支持的资产文件格式](#supported-static-file-formats)。 |
| 字体 | 已上载的 TrueType、Type1（仅限 Windows）、OpenType 字体以及 PhotoFont |
| 图像 | 图像和分层图像文件。 |
| 图像集和样本集 | 可以显示在查看器中的一组相关图像。 |
| ICC 配置文件 | 颜色配置文件，可以用来将上载的图像从源颜色空间转换为其他颜色空间。 |
| 晕影 | 使用图像创作程序创建的图像及相关文件。 |
| 内容文件 | Adobe InDesign、Illustrator 或 Photoshop 内容文件。 |
| FXG 文件 | 与分辨率无关的图形格式文件；可用于创建可自定义的模板，以输出到打印、网络、电子邮件、桌面和设备。 |
| SVG 文件 | 图像服务服务器可以渲染的可缩放矢量图形文件。 |
| XML 文件 | 定义用于修改请求的路径和查询部分的预处理规则的文件。 |
| 级联样式表文件。 | 上载用于自定义 HTML5 查看器的 CSS 外观。 |
| JavaScript 文件 | 检测查看器时用于保存帐户信息的 Javascript 文件。Adobe Security 建议仅将该文件用于使用单独域进行传送（以避免跨站点编写脚本）的客户端帐户。 |

>[!NOTE]
>
>将图像文件和 PDF 上载至 SPS 时，系统将这些源文件转换为 P-TIFF（金字塔 TIFF）文件。这些P-TIFF是稍后发布到Dynamic Media图像服务器的文件。Dynamic Media经典使用金字塔tiff文件格式，因为它包含各种缩放比率，可在使用Dynamic Media经典缩放查看器查看时实现快速缩放。

### 支持静态文件格式 {#supported-static-file-formats}

Dynamic Media Classic支持多种静态文件格式。静态内容是按“原样”发布的任何资产，如CSS、PDF、SVG、XML等。

可以发布以下文件类型：

* GIF 动画
* 音频文件
* CSS
* JavaScript（为公司配置自己的域时）
* 主视频
* PDF（上载后专门将 PDF 标记为发布时，以避免发送现有 eCatalog/PDF 工作流的所有 PDF）
* PrX 视频
* SVG
* XML
* ZIP

动态媒体经典不提供生成静态内容预览URL的选项。

### 文件名要求 {#filename-requirements}

由于在文件上载过程中将去除文件名中的扩展名，因此系统不允许文件使用相同的根名称。在Dynamic Media经典系统中，资产文件名减去文件名扩展名将成为资产的资产ID。因此，两个资源不能同名。

确保贵公司的所有用户都了解以下文件命名规则：

* 系统中不允许存在名称完全相同的资源 ID。
* 资源 ID 的名称区分大小写。
* 最佳做法是确保资源 ID 不包含空格（例如 black jacket.tif 和 blue jacket.jpg）。当资产名称使用资产名称构造URL字符串时，动态媒体经典ASCII可以对资产名称中的空白区域进行编码。这些 ASCII 编码不易理解，从而使 URL 更难理解。
* 文件名中允许特定语言字符。但是，文件名中不能出现以下字符：

   \ ; / ? : @ &amp; = + $ , * " &lt; &gt; | ' { } %

   如果文件名包含一个或多个上述字符，将会在上载时删除这些字符。

在多数情况下，资源文件名可以与其商品号、产品 SKU 或以下其他名称相同：

| 商品 | 文件名 | 资源 ID |
|--- |--- |--- |
| 896649 | 896649.jpg | 896649 |
| 48A3_2X | 48A3_2X.tif | 48A3_2X |

### 文件夹组织和结构 {#folder-organization-and-structure}

在将内容上载至 Scene7 Publishing System 之前，对系统中的内容进行组织，并建立其文件夹及子文件夹结构。采用这种方式提前进行规划主要有两个好处：

* 在通过 FTP 将内容上载至 SPS 时，可以通知系统在上载期间复制文件夹结构。这样，在 SPS 中，您的内容所在的文件夹和子文件夹就与其在您的计算机或网络上时所在的文件夹和子文件夹相同。（要在 SPS 中复制您的文件夹结构，在通过 FTP 上载资源时，选择“包括子文件夹”选项。）
* 与在开始就使用经过仔细计划的文件夹结构相比，在文件上载之后重新对系统内的文件夹进行组织要困难得多。

您选择用来在 Scene7 Publishing System 上存储内容的文件夹命名方法和结构取决于贵组织的需求。以下是一些文件夹结构示例：

**基于SKU的** 文件夹根据SKU或项目编号进行命名。例如，为所有以 0、20、30 开头的编号序列分别创建单独的文件夹。

**基于品牌** 的面向具有多个品牌的制造商和营销其他公司的其他品牌的零售商，将文件分为为不同品牌命名的产品文件夹。

**基于项目** 的文件夹是根据转出/拖放日期或项目名称组织的。主要生成 eCatalog 的客户喜欢使用这种方法。

**网站文件夹层次结构** 的镜像此文件夹结构镜像网站的文件夹结构，其中包括用于产品类别的文件夹。

## 关于上传文件 {#uploading-your-files}

可以从桌面上载单个文件或通过 FTP 上载文件夹。If you want to upload more than 100 MB of files or upload entire folders and subfolders, select the **VIA FTP** tab.

如果安装了Scene Publishing System桌面应用程序，则可以将文件和文件夹直接从桌面拖动到目标上传文件夹。

Scene7 Publishing System 在您的上载作业开始和结束时向您发送一封电子邮件以进行确认，并向您通知任何问题。

执行大批量上载作业执行期间（或随后），有些新商品可能显示“尚未优化图像”消息。此时将显示此消息，因为文件尚未完全处理并添加到SPS。您可以稍后优化这些文件。（请参阅[优化文件](application-setup.md#optimize_files)。）

### 使用FROM Desktop选项卡上传文件 {#upload-files-using-sps-desktop-application}

Scene7 Publishing System 桌面应用程序允许通过拖动上载文件和文件夹。

1. 在 Scene7 Publishing System 桌面应用程序中，单击全局导航栏上的“**上载**”。
1. On the Upload page, click the **FROM DESKTOP** tab.
1. 在上传页面左侧 **的“为上传** 区域选择文件”中，单击 **“浏览** ”选择要上传的一个或多个文件夹，然后单击 **“打开**”。
1. 在上传页面的右侧，在 **“选择文件夹目标** ”区域中，导航到要在其中添加上传的文件或文件夹的目标文件夹。
1. (可选)在上传页面底部附近，在 **“作业名称** ”字段中指定上传作业的新名称。或者，您只需使用SPS提供的默认系统生成的名称。将在“作业”页中记录此作业和其他上载和发布作业，可以在此页中检查作业的状态。请参阅[检查作业文件](checking-job-files.md#checking_job_files)。
1. (可选)如果您希望自动发布上传的资产，请在上传页面底部附近选择 **** 发布后发布。
在发布文件时，文件将发送到实时服务器。然后，可以在外部网站和应用程序中使用这些文件的 URL。请注意，“作业选项”对话框中也提供此相同选项。
1. (可选)在上传页面的底部附近，在任何文件夹中选择 **覆盖，无论您希望上传的文件以** 相同名称替换现有文件，请在任何文件夹中选择覆盖。请注意，“作业选项”对话框中也提供此相同选项。
The name of this option could be different, depending on the settings in **Application Setup &gt; General Settings &gt; Upload to Application &gt; Overwrite Images**.
1. Near the lower-right corner of the Upload page, click **Job Options**, then specify the options you want.

   请参阅[上载选项](uploading-files.md#upload_options)。

1. 在“上载作业选项”对话框中，单击“**保存**”。
1. 在上传页面的右下角，单击 **“提交上传**”。
要查看上载进度，请单击全局导航栏上的“**作业**”。您可以继续在 Scene7 Publishing System 中工作，并随时返回到“作业”页以检查进行中的作业。要取消正在进行的上载作业，请选择“持续时间”旁边的“**取消**”。

### 使用“通过FTP”选项卡上传文件 {#upload-files-using-via-ftp}

1. 登录特定于特定区域的动态媒体经典FTP站点。使用您从管理员那里收到的 FTP 用户名和密码。
1. 在Dynamic Media经典的全局导航栏上，单击 **上传**。
1. On the Upload page, click the **VIA FTP** tab.
1. 在上传页面左侧 **的“选择FTP文件夹for上传** ”区域中，选择要从中上传文件的FTP文件夹。
1. 在上传页面右侧的 **“选择SPS文件夹目标** 区域”中，在Scene Publishing System中选择目标文件夹。
1. (可选)在上传页面底部附近，在 **“作业名称** ”字段中指定上传作业的新名称。或者，您只需使用SPS提供的默认系统生成的名称。将在“作业”页中记录此作业和其他上载和发布作业，可以在此页中检查作业的状态。请参阅[检查作业文件](checking-job-files.md#checking_job_files)。
1. (可选)如果您希望自动发布上传的资产，请在上传页面底部附近选择 **** 发布后发布。
在发布文件时，文件将发送到实时服务器。然后，可以在外部网站和应用程序中使用这些文件的 URL。请注意，“作业选项”对话框中也提供此相同选项。
1. (可选)在上传页面的底部附近，在任何文件夹中选择 **覆盖，无论您希望上传的文件以** 相同名称替换现有文件，请在任何文件夹中选择覆盖。请注意，“作业选项”对话框中也提供此相同选项。
The name of this option could be different, depending on the settings in **Application Setup &gt; General Settings &gt; Upload to Application &gt; Overwrite Images**.
1. (可选；仅当您单击 **“通过FTP** ”选项卡时，在上传页面底部附近，如果 **您希望自动从上传的ZIP或TAR文件中提取所有文件，请选择“上传** 时解压缩Zip文件或Tar文件”。请注意，“作业选项”对话框中也提供此相同选项。
1. Near the lower-right corner of the Upload page, click **Job Options**, then specify the options you want.

   请参阅[上载选项](uploading-files.md#upload_options)。

1. 在“上载作业选项”对话框中，单击“**保存**”。
1. 在上传页面的右下角，单击 **“提交上传**”。

   要查看上载进度，请单击全局导航栏上的“**作业**”。“作业”页将显示上载进度。您可以继续在 Scene7 Publishing System 中工作，并随时返回到“作业”页以检查进行中的作业。

要取消正在进行的上载作业，请单击“持续时间”旁边的“**取消**”。

## “上载作业选项”对话框 {#upload-options}

上传文件时，您可以在“上传作业选项”对话框中的以下选项中进行选择：

* **工作-单击**“作业”**以选择影响整个上传作业的选项。**

   请注意，您还可以使用 *常规* 设置中的“ **默认上传选项”** 对话框选择上传作业的默认选项。单击 **“设置”&gt;“应用程序设置”&gt;“常规设置”&gt;“默认上传选项**”，然后设置所需的默认选项。

   * **** &mdash; **“何时”** 选项仅在您选择 **了“通过FTP** ”选项卡时才可用。
      * **** 一次性-指定一次运行的上传作业。选项包括：
         * **** 现在—在“上传作业选项”对话框中单击 **“保存”** 后立即运行上传作业，然后单击 **上传页面上的“提交上传** ”。
         * **计划以后** -选择您希望上传作业运行的年、月、日和时间(以15分钟为单位递增)。
      * **重复** —指定每日、每周或每月运行的上传作业。或者，根据自己的规范自定义上传作业。
         * **每天** —设置您希望作业每天运行的时间。如果希望作业仅在星期一至星期五运行，请选择“仅 **工作日”**。
         * **每周** —选择一周中的特定日期，并选择要运行的作业。
         * **Monthly** -选择一周中的某一天或一周中的某天(包括您希望作业运行的开始时间)。
         * **自定义** -根据自己的规范自定义上传或发布作业时间间隔。请参阅[创建自定义上载或发布作业时间间隔](checking-job-files.md#creating-a-custom-upload-or-publish-job-time-interval)。
   * **上传后发布** —如果您选择了“FROM Desktop”( **从桌面)** 选项卡或“FROM FTP”( **通过FTP)** 选项卡，则可用。选择此选项以自动发布上载的资源。在发布文件时，文件将发送到实时服务器。然后，可以在外部网站和应用程序中使用这些文件的 URL。“上载”页中也提供了该选项。

   * **在任何文件夹中覆盖，无论扩展名为什么，均可使用相同的基本资产名称** -如果您选择了“FROM Desktop”( **从桌面)** 选项卡或“FROM FTP”( **通过FTP)** 选项卡，则可用。如果要使上载的文件替换现有同名文件，请选中此选项。“上载”页中也提供了该选项。The name of this option could be different, depending on the settings in **Application Setup &gt; General Settings &gt; Upload to Application &gt; Overwrite Images**.

   * **上传** 时解压缩Zip或Tar文件-如果您选择了“FROM Desktop”( **从桌面)** 选项卡或“FROM FTP”( **通过FTP)** 选项卡，则可用。
如果要自动从上传的ZIP或TAR文件中提取所有文件，请选择此选项。请注意，“作业选项”对话框中也提供此相同选项。

   * **包括子文件夹** -仅当您选择 **了“通过FTP** ”选项卡时才可用。
如果要上载文件夹的子文件夹，请选中此选项。在 SPS 中会自动输入您上载的文件夹及其子文件夹的名称。

   * **处理元数据文件** —仅当您选择 **了“通过FTP** ”选项卡时才可用。如果要上载制表符分隔的文件或 XML 文件以将元数据添加到多个资源中，可以选择该选项。请参阅[导入元数据（通过 FTP）](viewing-adding-exporting-metadata.md#import-metadata)。


* **裁剪选项** —要从图像自动裁切空白像素，请打开“裁剪”菜单，选择“手动”，然后在“顶部”、“右侧”、“底部”和“左侧”字段中输入像素测量，以便从侧边裁剪。您也可以从“裁切”菜单中选择“修剪”并选择以下选项：

   * **修剪掉基于** -选择是否基于颜色或透明度裁剪：

      * **颜色** —选择“颜色”选项。然后选择“角”菜单，并选择所具有的颜色能最好地表示您想要裁切的空白颜色的图像角。

         基于颜色修剪：指定 0 则仅当像素与您在图像的角中选择的颜色完全匹配时才会裁切像素。数字越接近 1，允许的色差越大。

      * **透明度** —选择透明度选项。

         基于透明度修剪：指定 0 则仅当像素完全透明时裁切像素；数字值越接近 1，允许的透明度就越多。

      * **容差** -拖动滑块以指定到1之间的容差。

* **颜色配置文件选项** —在创建用于动态媒体经典动态交付的优化文件时选择颜色转换：

   * **默认颜色保留** -在图像包含色彩空间信息时保留源图像颜色；没有颜色转换。几乎目前的所有图像都嵌入了相应的颜色配置文件。不过，如果 CMYK 源图像不包含嵌入的颜色配置文件，则会将颜色转换为 sRGB（标准红绿蓝）色彩空间。在网页上显示图像时，推荐使用 sRGB 颜色空间。

   * **保留原始色彩空间** -在摄取到Scene Publishing System时，保留原始颜色而无需任何颜色转换。对于没有嵌入的颜色配置文件的图像，将使用发布设置中配置的默认颜色配置文件完成处理图像请求所需的任何颜色转换。这些颜色配置文件可能与使用此选项创建的文件中的颜色不匹配。因此，建议您使用“默认护色”选项。

   * **自定义自&gt;到** -打开菜单，以便您可以选择“从中转换”和“转换为色彩空间”。此高级选项覆盖在源文件中嵌入的任何颜色信息。仅当提交的所有图像包含错误或缺失的颜色配置文件数据时，才应选择此选项。

* **图像编辑选项** —您可以保留图像中的剪切&lt;&gt;蒙版，并选择颜色配置文件。
请参阅[上载时的图像编辑选项](image-editing-options-upload.md#image-editing-options-at-upload)。

* **POSTSCRIPT选项** —您可以栅格化PostScript®文件、裁剪文件、维护透明背景、选择分辨率并选择色彩空间。
请参阅[使用 PostScript 和 Illustrator 文件](postscript-illustrator-files.md#working_with_postscript_and_illustrator_files)。

* **PHOTOSHOP选项** —您可以从Adobe® Photoshop®文件创建模板、维护图层、指定如何命名图层、提取文本以及指定如何定位到模板中。
请参阅[PSD 上载选项](psd-files.md#psd_upload_options)。

* **PDF选项** —您可以栅格化文件、提取搜索词和链接、自动生成电子目录、设置分辨率并选择色彩空间。
请参阅[PDF 上载选项](pdfs.md#pdf_upload_options)。

* **Illustrator选项** —您可以栅格化Adobe Illustrator®文件、保持透明背景、选择分辨率并选择色彩空间。
请参阅[使用 PostScript 和 Illustrator 文件](postscript-illustrator-files.md#working_with_postscript_and_illustrator_files)。

* **EVIDEO选项** —您可以通过选择视频预设来转码视频文件。
请参阅[使用视频编码预设](uploading-encoding-videos.md#working_with_video_encoding_presets)。

* **附加元数据** —输入描述要上传的文件的关键字。用逗号分隔关键字。关键字简化了资源搜索。请参阅[实施高级搜索](searching-assets.md#conducting_an_advanced_search)。

* **批量设置预设** -如果要从上传的文件创建图像集、多轴旋转集或样本集，请单击要使用的预设的“活动”列。可以选择多个预设。您可以在“应用程序设置/批量集预设”页中创建预设。请参阅[批量级预设](application-setup.md#batch_set_presets)。

* **高级** —请参阅 [与其他作业](uploading-files.md#follow-an-upload-with-another-job)一起上传。

## 上载后执行其他作业 {#follow-an-upload-with-another-job}

使用 FTP 上载项目时，可以安排一个后续作业在上载完成后立即开始执行。（如果有其他作业计划在此时开始，您在此处计划的作业将在队列中排在其他作业的后面。）

新作业将向您指定的地址发送一条通知，以触发该位置的代码。该后续发布作业所使用的名称与上载作业相同，但在开头加有文本 *Pub_*。

**上载后执行其他作业**

1. Click **Upload**, then click the **VIA FTP** tab.
1. In the lower-right corner of the Upload page, click **Job Options**.
1. 在“上传作业选项”对话框中，展开 **“高级”** 部分。
1. 从“后续上传 **”下** 拉列表中选择以下任一选项：

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
   >定期计划的作业不会导致发布任何文件。

>[!MORELIKETHIS]
>
>* [使用资源文件夹](asset-folders.md#working_with_asset_folders)
>* [Handling recurring upload and publish jobs](checking-job-files.md#handling_recurring_upload_and_publish_jobs)
>* [使用上载或发布作业作为触发器](checking-job-files.md#using_an_upload_or_publish_job_as_a_trigger)

