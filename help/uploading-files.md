---
title: 上载文件
seo-title: 上载文件
description: 'null'
seo-description: 了解如何上传文件。
uuid: b3025f84-4f28-4276-bc9c-f0c0c2a26e12
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: b2bc3bf9-e313-481a-8670-c3bedde21b1a
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '3855'
ht-degree: 44%

---


# 上载文件{#uploading-files}

在将资产文件上传到Dynamic Media经典之前，请确保资产文件的命名正确，并且文件夹结构已按照您的需要设置和组织。 您可以从Dynamic Media经典提供的FTP站点上传文件，也可以直接从计算机或网络上传文件。 Dynamic Media经典优惠选项，用于在上传文件时优化文件。 如果您安装了AdobeDynamic Media经典桌面应用程序，则可以直接从桌面拖动文件和文件夹来上传它们。 （请参阅[应用程序常规设置](application-setup.md#general_settings)。）

## 准备将上载的资源和文件夹 {#preparing-your-assets-and-folders-for-uploading}

在将资产上传到Dynamic Media经典之前，请确保其格式和大小均正确。 您还必须遵守Dynamic Media经典资产命名规则。 通过设置文件的文件夹组织和结构，可确保可以轻松定位及处理文件。

### 支持的资源文件格式  {#supported-asset-file-formats}

此表列表了Dynamic Media经典支持的资产文件格式。 有关支持的Camera Raw文件的信息，请参阅[www.adobe.com/go/learn_s7_cameraraw_en](https://www.adobe.com/go/learn_s7_cameraraw_en)。

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
| Dynamic Media经典图像创作 | VNC、VNT、VNW |
| SVG | SVG、SVGX |
| TAR | TAR |
| 视频 | 3GP、AVI、M2P、M2T、M2TS、M2V、M4V、MOV、MP4、MPEG、MPG、MTS、OGV、TS、VOB、WMV/ASF |
| XML | XML |
| ZIP | ZIP |

TAR 和 ZIP 上载支持包括一个复选框，用于选择是否要解压缩文件。

### Dynamic Media{#unsupported-image-formats-dynamic-media}中不支持的图像格式

以下列表描述了Dynamic Media支持的&#x200B;*not*&#x200B;的栅格图像文件格式的子类型。

另请参阅[检测不支持的Dynamic Media文件格式](https://helpx.adobe.com/experience-manager/kb/detect-unsupported-assets-for-dynamic-media.html)。

* IDAT区块大小大于100 MB的PNG文件。
* PSB文件。
* 不支持色彩空间不是CMYK、RGB、灰度或位图的PSD文件。 不支持DuoTone、Lab和索引色彩空间。
* 位深度大于16的PSD文件。
* 具有浮点数据的TIFF文件。
* 具有Lab色彩空间的TIFF文件。

### 资源类型 {#asset-types}

要通过Dynamic Media经典平台获得最佳效果，请务必使用推荐的文件格式和大小。 下表列出了资源类型，其中一些资源类型列有常用资源的推荐格式和文件大小。

| 资源类型 | 说明/推荐 |
|--- |--- |
| 音频 | 输入音频资源格式，其中包括 AAC、HE-AAC、AC3、WAV、WMA、AIFF、MP3。可以将音频转码为以下格式：MP3、AAC 和 HE-AAC。 |
| 图像（用于调整图像大小、缩放、图像集、旋转集） | 图像的最大尺寸必须至少为 2000 像素；典型图像大小最大尺寸范围在 1500 到 2500 像素之间。推荐使用无损图像格式，包括 TIFF 和 PNG 文件。如果使用 JPEG 图像，请使用最高质量设置。动画GIF文件的处理方式与其他静态内容相同。 |
| eCatalog | 使用在 Adobe® Acrobat® 或 Creative Suite 应用程序中创建并保存为“印刷就绪”的高分辨率 PDF 文件。PDF 包括所有需要的字体、图像、蒙版以及引用的图形元素，采用单页、两页跨页或多页格式。通过按字母数字顺序为文件命名来排列页面顺序。将 eCatalog 类型的所有 PDF 文件放于一个文件夹中，以便于上载。您可以在上载时选择裁切选项，以便从 PDF 中删除修剪区域，包括裁切标记、对齐目标或颜色条。多数印刷就绪的 PDF 文件采用 CMYK 颜色空间，因此务必要获得用于 PDF 文件的 CMYK ICC 颜色配置文件。 |
| 模板 | 分层图像或布局设计，可以包括文本、图像和图层。可以将图层、文本字符串和属性（如颜色和大小）参数化，从而可以自定义变量数据。在模板中使用时的图像要求与其他图像相同。在 Photoshop 或其他图像编辑程序中准备图形。采用 TIFF 或 PNG 格式将每个图形保存为平面化透明文件。确保图像分辨率适合所要求的用途。准备打印的图像应为 300 PPI。 |
| 视频 | Dynamic Media经典支持以OGV和MP4格式保存的视频文件。 您可以在上传时将文件转码为MP4格式。请参阅[支持的资产文件格式](#supported-static-file-formats)。 |
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
>将图像文件和PDF上传到Dynamic Media经典时，系统会将这些源文件转换为P-TIFF(Pyramid TIFF)文件。 这些P-TIFF是稍后发布到Dynamic Media图像服务器的文件。 Dynamic Media经典使用金字塔Tiff文件格式，因为它包含各种缩放比率，当使用Dynamic Media经典缩放查看器查看时，这些比率允许快速缩放。

### 支持静态文件格式 {#supported-static-file-formats}

Dynamic Media经典支持多种静态文件格式。 静态内容是按“原样”发布的任何资产，如CSS、PDF、SVG、XML等。

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

Dynamic Media经典不提供生成静态内容的预览URL的选项。

### 文件名要求 {#filename-requirements}

由于在文件上载过程中将去除文件名中的扩展名，因此系统不允许文件使用相同的根名称。在Dynamic Media经典系统中，资产文件名减去文件扩展名即成为资产ID。 因此，两个资源不能同名。

确保贵公司的所有用户都了解以下文件命名规则：

* 系统中不允许存在名称完全相同的资源 ID。
* 资源 ID 的名称区分大小写。
* 最佳做法是确保资源 ID 不包含空格（例如 black jacket.tif 和 blue jacket.jpg）。Dynamic Media经典ASCII在使用资产名称构建URL字符串时对资产名称中的空格进行编码。 这些 ASCII 编码不易理解，从而使 URL 更难理解。
* 文件名中允许特定语言字符。但是，文件名中不能出现以下字符：

   \ ;/ ? :@ &amp; = + $, * &quot; &lt; > | &#39; { } %

   如果文件名包含一个或多个上述字符，将会在上载时删除这些字符。

在多数情况下，资源文件名可以与其商品号、产品 SKU 或以下其他名称相同：

| 商品 | 文件名 | 资源 ID |
|--- |--- |--- |
| 896649 | 896649.jpg | 896649 |
| 48A3_2X | 48A3_2X.tif | 48A3_2X |

### 文件夹组织和结构  {#folder-organization-and-structure}

在将内容上传到系统之前，在Dynamic Media经典中为您的内容组织和构建文件夹及子文件夹。 采用这种方式提前进行规划主要有两个好处：

* 当您通过FTP将内容上传到Dynamic Media经典时，您可以告诉系统在上传过程中复制文件夹结构。 这样，您的内容就会组织到与您的计算机或网络相同的Dynamic Media经典文件夹和子文件夹中。 (要在Dynamic Media经典中复制文件夹结构，请在通过FTP上传资产时选择“包含子文件夹”选项。)
* 与在开始就使用经过仔细计划的文件夹结构相比，在文件上载之后重新对系统内的文件夹进行组织要困难得多。

您选择在Dynamic Media经典上存储内容的文件夹命名方法和结构取决于您组织的需求。 以下是一些文件夹结构示例：

**基于SKU** 的文件夹根据SKU或物料编号命名。例如，为所有以 0、20、30 开头的编号序列分别创建单独的文件夹。

**基于品** 牌对于拥有多个品牌线的制造商和销售其他公司品牌的零售商，请将文件分离到为不同品牌命名的产品文件夹中。

**根据转** 出／删除日期或项目名称组织基于项目的文件夹。主要生成 eCatalog 的客户喜欢使用这种方法。

**网站文件夹层次结构** 的镜像此文件夹结构反映网站的文件夹结构，例如，为产品类别命名的文件夹。

## 关于上传文件{#uploading-your-files}

可以从桌面上载单个文件或通过 FTP 上载文件夹。如果要上传超过100 MB的文件或上传整个文件夹和子文件夹，请选择&#x200B;**VIA FTP**&#x200B;选项卡。

Dynamic Media经典会向您发送一封电子邮件，确认您的上传作业何时开始和结束，并通知您有任何问题。

执行大批量上载作业执行期间（或随后），有些新商品可能显示“尚未优化图像”消息。出现此消息是因为文件尚未完全处理并添加到Dynamic Media经典。 您可以稍后优化这些文件。（请参阅[优化文件](application-setup.md#optimize_files)。）

### 使用“从桌面”选项卡{#upload-files-using-sps-desktop-application}上传文件

Dynamic Media经典桌面应用程序允许您通过拖动上传文件和文件夹。

1. 在“Dynamic Media经典桌面”应用程序的全局导航栏上，单击&#x200B;**上传**。
1. 在“Upload”（上载）页面上，单击&#x200B;**FROM DESKTOP**&#x200B;选项卡。
1. 在“上传”页面的左侧，在&#x200B;**选择要上传的文件**&#x200B;区域，单击&#x200B;**浏览**&#x200B;以选择要上传的文件或文件夹，然后单击&#x200B;**打开**。
1. 在“上传”页面的右侧，在&#x200B;**选择文件夹目标**&#x200B;区域，导览至要添加已上载文件或文件夹的目标文件夹。
1. （可选）在“上传”页面底部附近的&#x200B;**作业名称**&#x200B;字段中，指定上传作业的新名称。 或者，您只需使用Dynamic Media经典提供的默认系统生成的名称。 将在“作业”页中记录此作业和其他上载和发布作业，可以在此页中检查作业的状态。请参阅[检查作业文件](checking-job-files.md#checking_job_files)。
1. （可选）如果要自动发布上传的资产，请在上传页面底部附近选择&#x200B;**上传后发布**。
在发布文件时，文件将发送到实时服务器。然后，可以在外部网站和应用程序中使用这些文件的 URL。请注意，“作业选项”对话框中也提供了相同的选项。
1. （可选）如果希望上传的文件用相同的名称替换现有文件，请在“上传”页面底部附近选择&#x200B;**覆盖任意文件夹中相同的基本资产名称，而不管扩展名**。 请注意，“作业选项”对话框中也提供了相同的选项。
此选项的名称可能不同，具体取决于**“应用程序设置”>“常规设置”>“上传到应用程序”>“覆盖图像”**&#x200B;中的设置。
1. 在上传页面的右下角附近，单击&#x200B;**作业选项**，然后指定所需的选项。

   请参阅[上载选项](uploading-files.md#upload_options)。

1. 在“上载作业选项”对话框中，单击“**保存**”。
1. 在上传页面的右下角，单击&#x200B;**提交上传**。
要查看上载进度，请单击全局导航栏上的“**作业**”。您可以继续在Dynamic Media经典中工作，并随时返回“作业”页面来查看正在进行的作业。 要取消正在进行的上载作业，请选择“持续时间”旁边的“**取消**”。

### 使用VIA FTP选项卡{#upload-files-using-via-ftp}上传文件

1. 登录特定于您特定区域的Dynamic Media经典FTP站点。 使用您从管理员那里收到的 FTP 用户名和密码。
1. 在Dynamic Media经典中，在全局导航栏上，单击&#x200B;**上传**。
1. 在“上传”页面上，单击&#x200B;**VIA FTP**&#x200B;选项卡。
1. 在“上传”页面的左侧，在&#x200B;**选择“FTP文件夹进行上传”**&#x200B;区域，选择要从中上传文件的FTP文件夹。
1. 在“上传”页面的右侧，在&#x200B;**选择AdobeDynamic Media文件夹目标**&#x200B;区域，在Dynamic Media经典中选择目标文件夹。
1. （可选）在“上传”页面底部附近的&#x200B;**作业名称**&#x200B;字段中，指定上传作业的新名称。 或者，您只需使用Dynamic Media经典提供的默认系统生成的名称。 将在“作业”页中记录此作业和其他上载和发布作业，可以在此页中检查作业的状态。请参阅[检查作业文件](checking-job-files.md#checking_job_files)。
1. （可选）如果要自动发布上传的资产，请在上传页面底部附近选择&#x200B;**上传后发布**。
在发布文件时，文件将发送到实时服务器。然后，可以在外部网站和应用程序中使用这些文件的 URL。请注意，“作业选项”对话框中也提供了相同的选项。
1. （可选）如果希望上传的文件用相同的名称替换现有文件，请在“上传”页面底部附近选择&#x200B;**覆盖任意文件夹中相同的基本资产名称，而不管扩展名**。 请注意，“作业选项”对话框中也提供了相同的选项。
此选项的名称可能不同，具体取决于**“应用程序设置”>“常规设置”>“上传到应用程序”>“覆盖图像”**&#x200B;中的设置。
1. (可选；仅当您单击了&#x200B;**VIA FTP**&#x200B;选项卡)“上传”页面底部附近，如果要从上传的ZIP或TAR文件自动解压所有文件，请选择&#x200B;**“上传时解压缩Zip或Tar文件”。**&#x200B;请注意，“作业选项”对话框中也提供了相同的选项。
1. 在上传页面的右下角附近，单击&#x200B;**作业选项**，然后指定所需的选项。

   请参阅[上载选项](uploading-files.md#upload_options)。

1. 在“上载作业选项”对话框中，单击“**保存**”。
1. 在上传页面的右下角，单击&#x200B;**提交上传**。

   要查看上载进度，请单击全局导航栏上的“**作业**”。“作业”页将显示上载进度。您可以继续在Dynamic Media经典中工作，并随时返回“作业”页面来查看正在进行的作业。

要取消正在进行的上载作业，请单击“持续时间”旁边的“**取消**”。

## “上载作业选项”对话框{#upload-options}

上传文件时，您可以在“上传作业选项”对话框中选择以下选项：

* **作业** —单击 **** 作业以选择影响整个上传作业的选项。

   请注意，您还可以使用“常规设置”中的“默认上传选项”**“默认上传选项”**&#x200B;对话框，为上传作业选择&#x200B;*默认*&#x200B;选项。 单击&#x200B;**“设置”>“应用程序设置”>“常规设置”>“默认上传选项”**，然后设置所需的默认选项。

   * **When**  — When选 **** 项仅在选择了VIA FTP选项 **卡时** 可用。
      * **一次性** —指定运行一次的上载作业。选项包括：
         * **现在** —在单击“上传作业选项”对话框 **** 的“保存”后立即运行上传作业，然后单 **击“** 上传”页面上的“提交上传”。
         * **计划稍后** -选择您希望上传作业运行的年、月、日和时间（以15分钟为增量）。
      * **重复** —指定每日、每周或每月运行的上载作业。或者，根据您自己的规范自定义上传作业。
         * **每天** —设置您希望工作每天运行的时间。如果希望作业仅在星期一至星期五运行，请选择&#x200B;**仅工作日**。
         * **每周** —选择您希望该作业运行的一周中的特定日期和时间。
         * **每月** -选择要运行作业的月或周的某一天，包括开始时间。
         * **自定义** —根据您自己的规范自定义上载或发布作业时间间隔。请参阅[创建自定义上载或发布作业时间间隔](checking-job-files.md#creating-a-custom-upload-or-publish-job-time-interval)。
   * **上传后发布** —如果您选择了“从桌面”选 **项** 卡或“通 **过FTP”** 选项卡。选择此选项以自动发布上载的资源。在发布文件时，文件将发送到实时服务器。然后，可以在外部网站和应用程序中使用这些文件的 URL。“上载”页中也提供了该选项。

   * **在任意文件夹中覆盖相同的基本资产名称，而不考虑扩展名** —如果您选择了“从桌面”选项 **卡** 或“通过FTP **”选** 项卡，则可用。如果要使上载的文件替换现有同名文件，请选中此选项。“上载”页中也提供了该选项。此选项的名称可能不同，具体取决于&#x200B;**“应用程序设置”>“常规设置”>“上传到应用程序”>“覆盖图像”**&#x200B;中的设置。

   * **上传时解压缩Zip或Tar文件** —如果您选择了“从桌面”选 **项** 卡或“通 **过FTP** ”选项卡。如果要自动从上传的ZIP或TAR文件解压所有文件，请选择此选项。 请注意，“作业选项”对话框中也提供了相同的选项。

   * **包含子文件夹** —仅在您选择了“通过FTP”选 **项卡** 时可用。如果要上载文件夹的子文件夹，请选中此选项。您上传的文件夹及其子文件夹的名称会自动输入到Dynamic Media经典中。

   * **处理元数据文** 件——仅当您选择了“通过FTP”选 **项卡** 时可用。如果要上载制表符分隔的文件或 XML 文件以将元数据添加到多个资源中，可以选择该选项。请参阅[导入元数据（通过 FTP）](viewing-adding-exporting-metadata.md#import-metadata)。


* **裁剪OPTIONS** -要自动裁剪图像中的空白像素，请打开“裁剪”菜单，选择“手动”，然后在“顶部”、“右”、“底部”和“左”字段中输入像素度量值以从两侧进行裁剪。您也可以从“裁切”菜单中选择“修剪”并选择以下选项：

   * **基于进行裁切** -选择是基于颜色还是透明度进行裁剪：

      * **颜色** (Color)-选择“颜色”选项。然后选择“角”菜单，并选择所具有的颜色能最好地表示您想要裁切的空白颜色的图像角。

         基于颜色修剪：指定 0 则仅当像素与您在图像的角中选择的颜色完全匹配时才会裁切像素。数字越接近 1，允许的色差越大。

      * **透明度** (Transparency)-选择“透明度”(Transparency)选项。

         基于透明度修剪：指定 0 则仅当像素完全透明时裁切像素；数字值越接近 1，允许的透明度就越多。

      * **容差** (Tolerance)-拖动滑块以指定从0到1的容差。

* **颜色用户档案OPTIONS** -在创建用于Dynamic Media经典动态投放的优化文件时选择颜色转换：

   * **默认颜色保留** -当图像包含色彩空间信息时，保留源图像颜色；没有颜色转换。几乎目前的所有图像都嵌入了相应的颜色配置文件。不过，如果 CMYK 源图像不包含嵌入的颜色配置文件，则会将颜色转换为 sRGB（标准红绿蓝）色彩空间。在网页上显示图像时，推荐使用 sRGB 颜色空间。

   * **保留原始色彩空间** -在引入Dynamic Media经典时，无需进行任何颜色转换即可保留原始颜色。对于没有嵌入的颜色配置文件的图像，将使用发布设置中配置的默认颜色配置文件完成处理图像请求所需的任何颜色转换。这些颜色配置文件可能与使用此选项创建的文件中的颜色不匹配。因此，建议您使用“默认护色”选项。

   * **“自定义自”>“至** ”-打开菜单，以便您选择“转换自”和“转换至色彩空间”。此高级选项覆盖在源文件中嵌入的任何颜色信息。仅当要提交的所有图像都包含不正确或缺少颜色用户档案数据时，才应选择此选项。

* **图像编辑OPTIONS** -您可以保留图像 &lt;> 中的剪切蒙版，并选择颜色用户档案。请参阅[上载时的图像编辑选项](image-editing-options-upload.md#image-editing-options-at-upload)。

* **POSTSCRIPTOPTIONS** -您可以栅格化PostScript®文件、裁剪文件、维护透明背景、选择分辨率和选择色彩空间。请参阅[使用 PostScript 和 Illustrator 文件](postscript-illustrator-files.md#working_with_postscript_and_illustrator_files)。

* **PHOTOSHOPOPTIONS** -您可以从Adobe®Photoshop®文件创建模板、维护图层、指定如何命名图层、提取文本以及指定如何将图像定位到模板中。请参阅[PSD 上载选项](psd-files.md#psd_upload_options)。

* **PDFOPTIONS** —您可以栅格化文件、提取搜索词和链接、自动生成电子目录、设置分辨率和选择色彩空间。请参阅[PDF 上载选项](pdfs.md#pdf_upload_options)。

* **ILLUSTRATOROPTIONS** -您可以栅格化Adobe Illustrator®文件、维护透明背景、选择分辨率和选择色彩空间。请参阅[使用 PostScript 和 Illustrator 文件](postscript-illustrator-files.md#working_with_postscript_and_illustrator_files)。

* **EVIDEOOPTIONS** -您可以通过选择视频预设对视频文件进行转码。请参阅[使用视频编码预设](uploading-encoding-videos.md#working_with_video_encoding_presets)。

* **其他元数据** —输入描述要上传的文件的关键字。用逗号分隔关键字。关键字简化了资源搜索。请参阅[实施高级搜索](searching-assets.md#conducting_an_advanced_search)。

* **批集预设** -如果要从已上传的文件创建图像集、多轴旋转集或样本集，请单击要使用的预设的活动列。可以选择多个预设。您可以在“应用程序设置/批量集预设”页中创建预设。请参阅[批量级预设](application-setup.md#batch_set_presets)。

* **高级** —请参 [阅使用其他作业进行上传](uploading-files.md#follow-an-upload-with-another-job)。

## 上载后执行其他作业 {#follow-an-upload-with-another-job}

使用 FTP 上载项目时，可以安排一个后续作业在上载完成后立即开始执行。（如果有其他作业计划在此时开始，您在此处计划的作业将在队列中排在其他作业的后面。）

新作业将向您指定的地址发送一条通知，以触发该位置的代码。该后续发布作业所使用的名称与上载作业相同，但在开头加有文本 *Pub_*。

**上载后执行其他作业**

1. 单击&#x200B;**上传**，然后单击&#x200B;**VIA FTP**&#x200B;选项卡。
1. 在上传页面的右下角，单击&#x200B;**作业选项**。
1. 在“上载作业选项”对话框中，展开&#x200B;**ADVANCED**&#x200B;部分。
1. 从&#x200B;**使用另一个作业执行上传操作**&#x200B;下拉列表中选择以下选项之一：

   * 无
   * HTTP 请求
   * 图像服务发布
   * 图像渲染发布
   * 视频发布

1. 指定 HTTP 地址。
1. 指定是否仅在上传文件时运行。
1. 指出是要在每次完成该作业时运行该请求，还是仅在发布文件时运行该请求。

   >[!NOTE]
   >
   >定期计划的作业不会导致发布任何文件。

>[!MORELIKETHIS]
>
>* [使用资源文件夹](asset-folders.md#working_with_asset_folders)
>* [Handling recurring upload and publish jobs](checking-job-files.md#handling_recurring_upload_and_publish_jobs)
>* [使用上载或发布作业作为触发器](checking-job-files.md#using_an_upload_or_publish_job_as_a_trigger)

