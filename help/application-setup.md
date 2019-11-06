---
title: 应用程序设置
seo-title: 应用程序设置
description: 了解如何设置Dynamic Media Classic的应用程序区域。
seo-description: 了解如何设置Dynamic Media Classic的应用程序区域。
uuid: 3e2f1d30-8f33-4a9d-bbe4-e8c3dbc968f8
contentOwner: admin
content-type: 引用
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEEVENTONDEMAND_PK/categories/setup
discoiquuid: ae2d1895-a437-4463-bfac-3960c8027551
translation-type: tm+mt
source-git-commit: 917ba4469b5ef22e62c572f80008e470dccdebe4

---


# 应用程序设置{#application-setup}

您可以使用“应用程序设置”页输入常规设置、创建图像预设、视频编码预设、查看器预设，或定义默认查看器和元数据。 您还可以设置批量集预设来自动生成 2D 旋转集（例如）、发布设置和视频 SEO 设置。

>[!NOTE]
>
>只有 Scene7 Publishing System 管理员可以在“应用程序设置”页面上更改这些设置。

## 常规设置 {#general-settings}

To open the Application General Settings page, on the Global Navigation bar, click **[!UICONTROL Setup &gt; Application Setup &gt; General Settings]**.

### 服务器

在创建帐户时，Dynamic Media Classic会自动为您的公司提供分配的服务器。 这些服务器用于构建网站和应用程序的 URL 字符串。这些 URL 调用是您的帐户所特有的。

另请参阅[测试安全测试服务](testing-assets-making-them-public.md#testing_the_secure_testing_service)。

**发布的服务器名** ：此服务器是在特定于您的帐户的所有系统生成的URL调用中使用的实时CDN服务器。 除非Dynamic Media Classic支持技术人员指示您更改此服务器名称。

**源服务器名称** 此服务器仅用于质量保证测试。 除非Dynamic Media Classic支持技术人员指示更改此服务器名称，否则请勿更改此名称。

**AGM服务器名称** 此服务器用于Web到打印模板。 在公司范围内设置此服务器。除非Dynamic Media Classic支持技术人员指示更改此服务器名称，否则请勿更改此名称。

**Test&amp;Target服务器名称** Test&amp;Target URL，最多包括。com。 有关获取此URL的说明，请参阅将Dynamic Media Classic与Target Classic集成。

**iOS Streaming server名称** Dynamic Media Classic iOS流服务器的URL。 该服务器使用 HTTP 协议将流视频发送至 iOS 设备。

**渐进式视频服务器名** ，指向Dynamic Media Classic渐进式视频服务器的URL。 该服务器使用 HTTP 协议发送渐进式视频。

**显示未发布资产的URL** 如果您希望Dynamic Media Classic在预览任何资产时显示URL（无论是否已发布），请选择此选项。 如果资源未发布，此 URL 将无效。但是，您可以使用 URL 进行计划或组织。

**允许AIR安装** 选择此选项可允许用户将Scene7 Publishing system桌面版本下载到其本地硬盘。 用户从“个人设置”屏幕的“桌面版本”区域中安装该应用程序。

AIR 用户必须手动卸载其现有应用程序，并通过 Scene7 Publishing System 的 Web 版本（在“个人设置”中）重新安装。在本次一次性重新安装后，只要服务器有 Scene7 Publishing System AIR 的新版本就会提示您升级。Scene7 Publishing System 与应用程序更新框架集成在一起，从而简化了升级过程。

**CDN失效模板** 指定用于使CDN（内容交付网络）缓存失效的模板。

For example, suppose you enter an image URL (including image presets or modifiers) referencing `<ID>`, instead of a specific image ID as in the following example:

`https://sample.scene7.com/is/image/Company/<ID>?$s7product$`

If the Template just contains `<ID>`, then SPS fills in the `https://<server>/is/image`, where `<server>` is the Publish Server Name that is defined in General Settings.

如果设置 CDN 失效模板，选择名为 Backpack_B 的图像，然后单击“**文件**”&gt;“**使 CDN 失效**”，则会在“使 CDN 失效”界面中生成以下 URL：

`https://sample.scene7.com/is/image/Company/Backpack_B?$s7product$`

在 URL 列表框中，单击“**继续**”以清除该特定图像 URL 调用的缓存。请注意，也可以键入 URL 或将其粘贴到 URL 列表框中以添加 URL；无需预先设置模板。

在选择 CDN 失效模板并发出使 CDN 失效请求后，将在用户界面中弹出指示符以估算清除缓存需要多长时间。

同样，如果在单击“**文件**”&gt;“**使 CDN 失效**”时在 SPS 中选择了多个图像，将在保存的模板 URL 中引用每个图像。因此，您可以定义一个引用您网站上所引用的各 URL（如产品详细信息、搜索结果等）的 CDN 失效模板。随后，当您从缓存中选择一个或多个图像以便设为失效时，这些 URL 将自动填充界面。

请参阅[内容缓存](scene7-platform-overview.md#content_caching)。

请参阅[重新发布的资源和 CDN 延迟](publishing-files.md#republished_assets_and_cdn_delays)。

**浏览**

**显示项目** 确定项目是否可作为组织Dynamic Media Classic资产的一种方式。 请参阅用项目组织工作。

**显示示例eVideo内容** 打开或关闭eVideo示例内容的显示。

**显示生成的内容** “在文件夹中”，显示从资产生成的内容。 例如，当PDF文件在上传时栅格化时，Dynamic Media Classic会为原始PDF中的每页创建一个图像。 如果选择“显示生成的内容”，则在上载原始 PDF 时生成的每个图像都会与该 PDF 一起显示在将 PDF 上载到的文件夹中。

**默认情况下** ，显示已编码视频已取消选择。

若要在 Scene7 发布系统中快速搜索和浏览视频，而无需在同一视频的大量编码派生项中导航，请取消选择此选项（默认设置）。用户界面上显示的只有“主视频”缩略图（您上传并用于创建所有派生项的源视频）和“父”自适应视频集缩略图（包含编码视频集的所有“子”派生项）。

但是，您仍可以访问主视频或自适应视频集的各个编码视频。要执行以上操作，请双击视频缩略图图像，打开详细信息视图。然后单击右边侧面板的“**编码的视频**”，访问所有“子”视频。

您也可以使用“**文件”&gt;“重新处理**”以直接从自适应视频集创建更多编码的“子”视频。Scene7 Publishing System 可自动查找自适应视频集的“父”主视频并将其用作转码的源视频。但是，如果保存新的单个编码视频，您在搜索或浏览时将看不到这些视频。但是，您仍可以从详细信息视图的“编码的视频”选项卡进行访问。

请参阅[上载和转码视频](uploading-encoding-videos.md#uploading_and_encoding_videos)。

要继续保留在搜索和浏览时可以访问所有编码视频派生的功能，请选择“**显示已编码视频**”。

“构建”菜单上的某些操作只能对单个视频或选择性地对单个视频生效。此功能要求必须显示所有可以选择的编码视频派生（无论如何设置“**显示已编码视频**”）。The Build actions that over-ride the **Show Encoded Videos** setting include **Adaptive Video Sets**, and **eCatalogs**.

>[注意]
>
>如果您未使用Scene7 Publishing system上传视频资产并对其进行编码，Dynamic Media Classic会显示您的所有单独编码视频，即使取消选择此选项也是如此。

**显示“刷新子文件夹** ”按钮打开或关闭子文件夹“刷新”按钮的显示。

**Dynamic Media Classic FTP帐户**

**服务器** 列出您的FTP帐户服务器。

**用户名** ，列出您的FTP帐户用户名。

**上载到应用程序**

**覆盖图像** Dynamic Media Classic不允许两个文件具有相同的名称。 每个项目的 Scene7 Publishing System ID（图像名称去掉文件扩展名）必须唯一。由于此规则，“上载”对话框中有一个“覆盖”选项。该选项的准确效果取决于指定的“覆盖图像”选项。这些选项指定了如何上载替换图像：替换原始图像，还是成为重复图像。重复图像会用“-1”重命名（例如，chair.tif 会重命名为 chair-1.tif）。这些选项会影响上载到的文件夹与原始图像不同的图像，或文件扩展名（如 JPG、TIF 或 PNG）与原始图像不同的图像。（请参阅使用覆盖图像选项。）

**在当前文件夹内，使用相同的基本图像名称和扩展名进行覆盖**

该选项是替换的最严格规则。它要求您将替换图像上载到原始图像所在的文件夹中，并且该替换图像与原始图像具有相同的文件扩展名。如果不满足这些要求，则会创建重复的图像。

**在当前文件夹内，使用相同的基本资源名称（不论扩展名是什么）进行覆盖**

要求您将替换图像上载到原始图像所在的文件夹中，文件扩展名可以不同于原始图像。例如，chair.tif 会替换 chair.jpg。

**在任意文件夹内，使用相同的基本资源名称和扩展名进行覆盖**

要求替换图像必须具有与原始图像一样的文件扩展名（例如，chair.jpg 必须替换 chair.jpg，而不是替换 chair.tif）。但是，可以将替换图像上载到与原始图像不同的文件夹中。更新的图像位于新文件夹；而不再位于其原始位置

**在任意文件夹内，使用相同的基本资源名称（不论扩展名是什么）进行覆盖**

此选项是最具包容性的替换规则。可以将替换图像上载到与原始文件所在文件夹不同的文件夹，使用不同的文件扩展名上载文件，并替换原始文件。如果原始文件在不同的文件夹中，替换图像则位于其所上载至的新文件夹。

**保留发布** ：指定上传到Dynamic Media Classic的替换图像是保留其要替换的图像的“准备发布”设置，还是在上传时指定该设置。

**默认颜色配置文件** -指定在添加CMYK图像时作为默认颜色配置文件选项的一部分应用的颜色配置文件。

**默认上传选项** 打开“上传作业选项”对话框，您可以在其中指定默认的上传选项。 有关这些选项的信息，请参阅上载选项。

**应用程序的图像映射编辑器**

**默认图像映射HREF** 定义用于图像映射href列的默认URL。 此 URL 是您在创建新图像映射时看到的默认 URL。

**默认图像映射模板** -为图像映射href模板定义默认Javascript。 每当单击图像映射时，都可以在此处设置要执行的自定义代码。

**应用程序的其他设置**

**垃圾桶可以清理垃圾桶中的警告** ，资源会在七天内自动删除。 如果您需要在“垃圾桶”中的资源距永久删除还有四天时间时向公司管理员发送通知，请选择“自动删除垃圾桶项目之前会发送电子邮件”。请参阅管理垃圾桶文件夹。

## 使用“覆盖图像”选项 {#using-the-overwrite-images-option}

动态媒体经典不允许两个文件具有相同的名称。 每个项目的 Scene7 Publishing System ID（图像名称去掉文件扩展名）必须唯一。由于该规则，所以“上载”对话框会包括“覆盖图像”选项。该选项的具体影响取决于每个公司 Scene7 Publishing System 内部设置的设置。

如果您之前上传了图像，然后更改了原始文件（或替换了它们），则选择的“覆盖”选项将指定Dynamic Media Classic如何替换图像。 没有关于图像更改的信息，但是新图像会替换旧图像。如果文件夹还包含Dynamic Media Classic中尚未包含的图像，则会添加这些图像。

如果您已上载的图像在某些方面有所更改（图像已改变），但是对图像的引用保持不变，请使用此选项。在上载和翻录 Adobe® PDF 时“覆盖”也很有用。To fine-tune how Dynamic Media Classic *rips* the image, adjust the ICC color profile options in the Upload dialog box and re-upload using the Overwrite feature.

用于从生产服务器访问图像的Dynamic Media Classic ID源自图像文件名。 在替换现有文件和用于访问图像的Dynamic Media Classic ID时，文件名中使用大小写字符很重要。 在上传到Dynamic Media Classic之前，请确保文件名中的大小写字符的使用正确，以避免仅对同一图像大小写不同的Dynamic Media Classic ID。

如果您取消选择此选项，将与现有图像具有相同文件名的所有图像都视为重复图像，并且不予添加。

## 图像预设 {#image-presets}

“图像预设”屏幕用于创建和编辑图像预设。图像预设使Dynamic Media Classic能够以不同大小动态传送来自同一主图像的图像。 每个图像预设都表示用于显示图像的一组预定义大小和格式命令。在您创建图像预设时，可以选择图像的传送大小。您还可以选择格式命令，以便在传送图像供查看时优化图像的外观。

管理员可以创建导出资源的预设。用户可以在导出图像时选择预设，这同时将按照管理员指定的规范重新设置图像的格式。

To open the Image Preset screen, on the Global Navigation bar, click **Setup** &gt; **Image Presets**.

请参阅 [智能成像](https://helpx.adobe.com/experience-manager/6-3/assets/using/imaging-faq.html)。

### 创建和编辑图像预设 {#creating-and-editing-image-presets}

1. 单击“**设置**”&gt;“**图像预设**”。
1. 创建新预设或从现有预设开始：
   * **创建图像预设** -单击“添 **加”**。
   * **从现有预设创建图像预设** -选择与要创建的图像预设最相似的图像预设，然后单击编辑。

1. 在“添加（或编辑）预设”屏幕上，输入预设的名称。
1. 设置所需的预设选项。

   请参阅[图像预设选项](application-setup.md#image_preset_options)。

1. Click **Save**, or if you started from an existing preset, click **Save As**.
1. To preview the preset with your own image, click **Browse** and then select an image. To preview with the default image, click **Reset**.

在“图像预设”屏幕上选择图像预设的名称，然后单击“编辑”可以编辑图像预设。要删除某个图像预设，请将其选中，然后单击“删除”。

### 图像预设选项 {#image-preset-options}

“添加预设”和“编辑预设”屏幕提供了用于创建和编辑图像预设的选项：

**预设名称** 输入一个描述性名称，不带任何空格。 将图像大小规格包括在名称中，以帮助用户识别该图像预设。

**宽度和高度** 输入传送图像时所用的像素大小。

**格式** 从菜单中选择格式。 选择 GIF、JPEG、PDF 或 TIFF 格式会显示其他选项：

* GIF 颜色量化选项

   **类型**

   选取“自适应”（默认设置）、“Web”或“Macintosh”。如果选取“带 Alpha 通道的 GIF”，则“Macintosh®”选项不可用。

   **仿色**

   选择“扩散”或“关闭”。

   **颜色数目**

   拖动滑块以进入2-255。

   **颜色列表**

   输入以逗号分隔的列表。例如，对于白色、灰色和黑色，输入 000000、888888、ffffff。

* JPEG 选项

   **品质**

   控制 JPEG 压缩等级。此设置既影响文件大小，又影响图像质量。JPEG质量比例为1-100。

   **启用 JPG 色度缩减像素采样**

   由于眼睛对高频亮度的敏感程度要超过高频颜色信息，JPEG 图像将图像信息划分成亮度和颜色分量。压缩 JPEG 图像时，通过将各组像素放到一起平均，亮度分量为全分辨率，颜色分量为缩减像素取样。缩减像素采样会将数据量减少二分之一或三分之一，而对于用户所能感知到的质量而言却几乎没有任何影响。缩减像素采样不适用于灰度图像。这种方法会减少对于高对比度图像有用的压缩的数量（例如，包含覆盖文本的图像）。

* PDF 和 TIFF 选项

   **压缩**

   选择一个压缩算法。

**色彩空间** ：选择色彩空间。

**锐化** 选择启用简单锐化选项，以在进行所有缩放后对图像应用基本锐化滤镜。 锐化可以帮助补偿在以不同尺寸显示图像时可能导致的模糊。

有关锐化、重新采样模式和 USM 锐化的详细信息，请参阅[锐化图像](sharpening-image.md#sharpening_an_image)。

**重新取样模式** 选择重新取样模式选项。 当图像缩减像素取样时，以下选项锐化该图像：

**B-Linear** The fastly respaming method;会出现一些锯齿伪像。

**两次立方** (Bi-Cubic)提高了图像服务器上的CPU使用率，但生成的图像更锐利，锯齿伪像较少。

**锐化2** 可以比“两次立方”选项产生略微锐利的结果，但图像服务器的CPU成本更高。

**三线性** （如果可用）同时使用较高和较低分辨率；仅当出现锯齿问题时建议。 由于减少了高频数据，此方法会减小 JPEG 的大小。

**USM锐化** ：选择以下选项可微调锐化：

**数量** ：控制应用于边缘像素的对比度数量。 默认值为 1.0。对于高分辨率图像，可将该值增加到 5.0。数量用于衡量滤镜强度。

**半径** 确定边缘像素周围影响锐化的像素数。 对于高分辨率图像，请输入 1 到 2 之间的值。较低的数值仅锐化边缘像素，较高的数值则锐化范围更宽的像素。值正确与否取决于图像的大小。

**阈值** 确定应用USM锐化滤镜时要忽略的对比度范围。 换言之，此选项确定锐化的像素必须与周围区域相差多少，才被滤镜看作边缘像素并被锐化。为避免引进干扰，请用 0.02 到 0.2 之间的值做试验。默认值 6 锐化图像中的所有像素。

**色彩空间** ：确定图像是使用创建图像的空间，通常为RGB（原始）还是明亮度空间（强度）。

**颜色** ：选择以下选项：

**输出颜色配置文件** 选择“使用默认值”或Scene7 Publishing system上提供的ICC颜色配置文件之一。

另请参阅[ ICC 配置文件](icc-profiles.md#icc_profiles)。

**渲染方法** 如果要覆盖颜色配置文件的默认渲染方法，请选择一个选项。 其中一个默认 ICC 配置文件是颜色转换的目标颜色空间、输出设备（打印机或显示器）具有此配置文件、指定的渲染方法对此配置文件有效时，请使用此选项。

**嵌入配置文件** -选择此选项后，如果您在Adobe® Photoshop®中打开此图像，它将使用此配置文件。

**打印分辨率** ：选择打印此图像的分辨率；默认为72像素。

**URL修饰符** 如果您希望指定用于定义图像预设的URL修饰符，而不是设置，请在此处输入修饰符。

**示例图像URL** 列出Dynamic Media图像服务器用来传送包含您添加或编辑的图像预设的图像的“原始”URL字符串。 该 URL 字符串编码您在“添加预设”或“编辑预设”屏幕中选择的所有格式设置。

### 编辑、删除或停用图像预设 {#editing-removing-or-deactivating-an-image-preset}

1. 单击“**设置**”&gt;“**图像预设**”。
1. 在“图像预设”屏幕中，选择表中的某个预设，然后执行以下任一操作：

   * Click **Edit** and then specify new options in the Edit Preset dialog box.
   * Click **Delete** to remove the preset from the list.
   * 取消选中预设名称旁的“活动”复选框将预设从 MediaPortal 用户的整个 Scene7 Publishing System 用户界面中删除。

## 激活或停用自适应视频预设 {#activating-or-deactivating-adaptive-video-presets}

Dynamic Media Classic提供自适应视频编码预设。 它是一个将 16:9 自适应视频预设和 4:3 自适应视频预设合并为一组的总预设列表。这些预定义的预设反映了最常用的编码设置，并且经过优化以便在目标移动设备、平板电脑和台式机上播放。

默认情况下，仅激活（启用或“打开”）“自适应视频”编码预设。您可以根据需要将其停用。在“上载作业选项”对话框的 eVideo 部分中，非活动自适应视频预设不会显示为可选择的选项。

请参阅[上载和编码视频](uploading-encoding-videos.md#uploading_and_encoding_videos)。

**激活或停用自适应视频预设**

1. 在 Scene7 Publishing System 的右上角附近，单击“**设置**”&gt;“**应用程序设置**”&gt;“**视频预设**”&gt;“**自适应视频预设**”。
1. 在“自适应视频预设”页中，取消选中某个预设名称旁边的复选框，以将该预设从“上载作业选项”对话框的“eVideo 选项”列表中删除。
1. 单击“**关闭**”。

## 用于编码视频文件的视频预设 {#video-presets-for-encoding-video-files}

要选择编码预设，请单击“上载”页面右下角的“作业选项”。在“上载作业选项”对话框中，展开“eVideo 选项”，然后选择所需的视频编码预设。

>[!NOTE]
>
>除了“自适应视频”（默认启用）以外，在“上载作业选项”对话框中看不到所有其他自适应视频或单个视频编码预设。Dynamic Media Classic管理员可确定在“上传作业选项”对话框中显示哪些视频编码预设。

* 从下列自适应视频编码或单个编码预设中进行选择：

   **16:9 自适应视频**

   创建16:9长宽比视频，以交付到台式机、手机(iPhone、iPad、Android)和平板电脑(iPad、Android)，并使用最匹配查看器连接速度的分辨率和比特率进行优化。

   **4:3 自适应视频**

   创建4:3长宽比视频，以交付到台式机、手机(iPhone、iPad、Android)和平板电脑(iPad、Android)，并使用最匹配查看器连接速度的分辨率和比特率进行优化。

   **自适应视频**

   这是适用于任何高宽比的单个编码预设，可用于创建传送到移动设备、平板电脑和台式机的视频。使用该预设编码的上载的源视频将设置为固定高度。但是，自动调整宽度以保持视频的高宽比。

   默认情况下，在创建您自己的自定义视频编码预设时，也可以灵活地进行这种“自动缩放”。

   请参阅[添加或编辑视频编码预设](uploading-encoding-videos.md#adding_or_editing_a_video_encoding_preset)。

   **自适应视频编码（16:9 或 4:3）**

   创建16:9和4:3长宽比视频，以便交付到台式机、手机(iPhone、iPad、Android)和平板电脑(iPad、Android)，并使用最匹配查看器连接速度的分辨率和比特率进行优化。

   请参阅[自适应视频编码（16:9 或 4:3）视频预设](application-setup.md#adaptive_video_encoding_16_9_or_4_3_video_presets)。

   **单个编码预设**

   >[注��]
   >
   >要将视频传送到 iPad，您可以选择“移动设备”编码预设，或“平板电脑”编码预设。平板电脑预设专为 iPad 而设计，通常具有更高的分辨率和质量，以充分利用更大的屏幕尺寸和带宽连接。传送使用平板电脑预设编码的视频文件要求您在移动站点或应用程序上加入设备检测代码。此代码会根据播放设备在 iPhone 或 iPad 视频体验之间切换。更简单的工作流程是选择移动设备预设将视频文件传送到 iPad。原因在于您可以将同一视频文件用于 iPhone 和 iPad。但是，将质量标准化为分辨率更低的 iPhone 体验。

   * 在“编码预设”组下的“编码预设排序”下拉列表中，选择名称或大小来按名称或分辨率大小对预设进行排序。
   * 根据您计划播放视频的分辨率大小和带宽，选择编码预设。
   * 您可以选择自适应视频编码，以及为每个视频选择一个或多个编码预设。例如，您可以在一个上载作业中针对桌面和移动设备编码文件。

在单击“**开始上载**”后，将上载原始主视频文件，并通过主文件生成编码的文件。

### 关于编码预设选项 {#about-encoding-preset-options}

编码预设选项的参数如下：

**目标连接速度** 目标最终用户的Internet连接速度。

**编码文件后缀** ：附加到编码视频文件以用于标识目的的后缀。

**视频比特率（数据速率）** ，编码以组成一秒钟视频回放的数据量（千位／秒）。

**像素宽度** /高度屏幕图像的宽度尺寸，以像素为单位；屏幕图像的高度尺寸（以像素为单位）。

**每秒帧数(fps)** ：每秒视频的帧数，或静态图像。 在美国和日本，大部分视频以 29.97 fps 拍摄；在欧洲和亚洲（不包括日本），大部分视频以 25 fps 拍摄。电影以 24 fps 拍摄。

**音频比特率** ：编码以组成一秒钟音频回放的数据量，以千位／秒为单位。

下表显示了选择视频预设的建议最佳做法和用于指定编码文件的命名约定。

### 自适应视频（默认） {#adaptive-video-default}

这是一个适用于任何高宽比的编码预设，可用于创建传送到移动设备、平板电脑和台式机的视频。使用该新预设（默认和最佳做法）编码的上载的源视频将设置为固定高度，同时自动调整宽度以保持视频的高宽比。

**自适应视频（默认）**

|  | 编码预设名称/工具提示文本 | 编码文件后缀 | 视频数据速率 (Kbps) | 宽度/高度（像素） | Fps | 音频比特率 (kbps) | 推荐 |
|--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | Auto x360, 800 Kbps | _Mobile_Autox360p_800K | 800 | Autox360 | 与源相同 | 64 | 用于移动设备（iPhone、iPad、Android） |
| 2 | Auto x 480, 1400 Kbps | _Tablet_Autox480p_1400K | 1400 | Autox480 | 与源相同 | 96 | 用于平板电脑（iPad、Android） |
| 3 | Auto x 720, 2600 Kbps | _Desktop_Autox720p_2600K | 2600 | Autox720 | 与源相同 | 128 | 桌面版 |

### 自适应视频编码（16:9 或 4:3）视频预设 {#adaptive-video-encoding-or-video-presets}

这些自适应视频编码预设合并了一系列单独的编码预设，将根据上载的视频的高宽比自动为您选择这些预设。例如，如果上载一个 4:3 视频，系统会自动使用“**自适应视频编码（16:9 或 4:3）**”选项中主预设列表内的所有五个 4:3 预设来对该视频进行编码。

有关编码选项参数的信息，请参阅[关于编码预设选项](application-setup.md#about_encoding_preset_options)。

**自适应视频编码（16:9 或 4:3）预设**

|  | 编码预设名称/工具提示文本 | 目标连接速度 (Kbps) | 编码文件后缀 | 视频数据速率 (Kbps) | 宽度/高度（像素） | Fps | 音频比特率 (kbps) | 推荐 |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | 16:9，512x288，移动设备（iPhone、iPad、Android），(400 Kbps) | 500 | _Mobile_512x288_400K | 400 | 512x288 | 与源相同 | 64 | 低分辨率、3G |
| 2 | 4:3，384x288px，移动设备（iPhone、iPad、Android），(400 Kbps) | 500 | _Mobile_384x288_400K | 400 | 384x288 | 与源相同 | 64 | 低分辨率、3G |
| 3 | 16:9，512x288，移动设备（iPhone、iPad、Android），(600 Kbps) | 700 | _Mobile_512x288_600K | 600 | 512x288 | 与源相同 | 64 | 中分辨率、3G |
| 4 | 4:3，384x288，移动设备（iPhone、iPad、Android），(600 Kbps) | 700 | _Mobile_384x288_600 | 600 | 384x288 | 与源相同 | 64 | 中分辨率、3G |
| 5 | 16:9，640x360，平板电脑（iPad、Android），(800 Kbps) | 900 | _iPad_640x360_800K | 800 | 640x360 | 与源相同 | 80 | 中分辨率、WiFi |
| 6 | 4:3，640x480，平板电脑（iPad、Android），(800 Kbps) | 900 | _iPad_640x480_800K | 800 | 640x480 | 与源相同 | 80 | 中分辨率、WiFi |
| 7 | 16:9，768x432，平板电脑（iPad、Android），(1200 Kbps) | 1.5 Mbps | _iPad_768x432_1200K | 1200 | 768 x 432 | 与源相同 | 96 | 高分辨率、WiFi |
| 8 | 4:3，768x576，平板电脑（iPad、Android），(1200 Kbps) | 1.5 Mbps | _iPad_768x576_1200K | 1200 | 768x576 | 与源相同 | 96 | 高分辨率、WiFi |
| 9 | 16:9、1280x720、台式机、(2000 Kbps) | 3.0 Mbps | _1280x720_2000K | 2000 | 1280x720 | 与源相同 | 128 | 高清、宽屏 |
| 10 | 4:3、1280x960、台式机、(2000 Kbps) | 3.0 Mbps | _1280x960_2000K | 2000 Kbps | 1280x960 | 与源相同 | 128 | 高清 |

### 台式机视频编码预设 {#desktop-video-encoding-presets}

台式机上的 MP4 和 OGV 视频编码预设。

有关编码选项参数的信息，请参阅[关于编码预设选项](application-setup.md#about_encoding_preset_options)。

**H264 Main 3.2 - 音频 AAC、MP4 文件扩展名**

|  | 编码预设名称/工具提示文本 | 目标连接速度 (Kbps) | 编码文件后缀 | 视频数据速率 (Kbps) | 宽度/高度（像素） | Fps | 音频比特率 (Kbps) | 推荐 |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | 16:9、480x270 (400 Kbps) | 500 | _480x270_400K | 400 | 480x270 | 与源相同 | 64 | 低宽屏分辨率 |
| 2 | 16:9、640x360 (800 Kbps) | 900 | _640x360_800K | 800 | 640x360 | 与源相同 | 80 | 中等宽屏分辨率 |
| 3 | 16:9、800x450 (1200 Kbps) | 1.5 Mbps | _800x450_1200K | 1200 | 800x450 | 与源相同 | 96 | 中高分辨率 |
| 4 | 16:9、1280x720 (2000 Kbps) | 3.0 Mbps | _1280x720_2000K | 2000 | 1280x720 | 与源相同 | 128 | 高清、宽屏 |
| 5 | 4:3、320x240 (400 Kbps) | 500 | _320X240_400K | 400 | 320x240 | 与源相同 | 64 | 低分辨率 |
| 6 | 4:3、480x360 (800 Kbps) | 900 | _480x360_800K | 800 | 480x360 | 与源相同 | 80 | 中分辨率 |
| 7 | 4:3、640x480 (1200 Kbps) | 1.5 Mbps | _640x480_1200K | 1200 | 640x480 | 与源相同 | 96 | 中高分辨率 |
| 8 | 4:3、1280x960 (2000 Kbps) | 3.0 Mbps | _1280x960_2000K | 2000 | 1280x960 | 与源相同 | 128 | 高清 |

**OGG Theora Vorbis - OGV 文件扩展名**

|  | 编码预设名称/工具提示文本 | 目标连接速度 (Kbps) | 编码文件后缀 | 视频数据速率 (Kbps) | 宽度/高度（像素） | Fps | 音频比特率 (Kbps) | 推荐 |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | 16:9、480x270 (400 Kbps)、OGG | 500 | _OGG_480x270_400K | 400 | 480x270 | 与源相同 | 64 | 低宽屏分辨率 |
| 2 | 16:9、640x360 (800 Kbps)、OGG | 900 | _OGG_640x360_800K | 800 | 640x360 | 与源相同 | 80 | 中等宽屏分辨率 |
| 3 | 16:9、800x450 (1200 Kbps)、OGG | 1.5 Mbps | _OGG_800x450_1200K | 1200 | 800x450 | 与源相同 | 96 | 中高分辨率 |
| 4 | 16:9、1280x720 (2000 Kbps)、OGG | 3.0 Mbps | _OGG_1280x720_2000K | 2000 | 1280x720 | 与源相同 | 128 | 高清、宽屏 |
| 5 | 4:3、320x240 (400 Kbps)、OGG | 500 | _OGG_320X240_400K | 400 | 320x240 | 与源相同 | 64 | 低分辨率 |
| 6 | 4:3、480x360 (800 Kbps)、OGG | 900 | _OGG_480x360_800K | 800 | 480x360 | 与源相同 | 80 | 中分辨率 |
| 7 | 4:3、640x480 (1200 Kbps)、OGG | 1.5 Mbps | _OGG_640x480_1200K | 1200 | 640x480 | 与源相同 | 96 | 中高分辨率 |
| 8 | 4:3、1280x960 (2000 Kbps)、OGG | 3.0 Mbps | _OGG_1280x960_2000K | 2000 | 1280x960 | 与源相同 | 128 | 高清 |

### 移动设备视频编码预设 {#mobile-video-encoding-presets}

与源 fps 相同。iPhone、iPad 和 Android 移动设备的视频编码预设。

有关编码选项参数的信息，请参阅[关于编码预设选项](application-setup.md#about_encoding_preset_options)。

**H264 Baseline 2.1 - 音频 AAC、MP4 文件扩展名**

|  | 编码预设名称/工具提示文本 | 目标连接速度 (Kbps) | 编码文件后缀 | 视频比特率 (Kbps) | 像素宽度/高度 | Fps | 音频比特率 (Kbps) | 推荐 |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | 16:9、512x288、移动设备 (400 Kbps) | 500 | _Mobile_512x288_400K | 400 | 512x288 | 与源相同 | 64 | 低分辨率、3G |
| 2 | 16:9、512x288、移动设备 (600 Kbps) | 700 | _Mobile_512x288_600K | 600 | 512x288 | 与源相同 | 64 | 中分辨率、3G |
| 3 | 16:9、512x288、移动设备 (800 Kbps) | 900 | _Mobile_512x288_800K | 800 | 512x288 | 与源相同 | 80 | 中等分辨率、Wi-Fi |
| 4 | 16:9、512x288、移动设备 (1000 Kbps) | 1.2 Mbps | _Mobile_512x288_1000K | 1000 | 512x288 | 与源相同 | 80 | 高分辨率、Wi-Fi |
| 5 | 16:9、512x288、移动设备 (1200 Kbps) | 1.5 Mbps | _Mobile_512x288_1200K | 1200 | 512x288 | 与源相同 | 96 | 高分辨率、Wi-Fi |
| 6 | 4:3、384x288、移动设备 (400 Kbps) | 500 | _Mobile_384x288_400K | 400 | 384x288 | 与源相同 | 64 | 低分辨率、3G |
| 7 | 4:3、384x288、移动设备 (600 Kbps) | 700 | _Mobile_384x288_600K | 600 | 384x288 | 与源相同 | 64 | 中分辨率、3G |
| 8 | 4:3、448x336、移动设备 (800 Kbps) | 900 | _Mobile_448x336_800K | 800 | 448x336 | 与源相同 | 80 | 中等分辨率、Wi-Fi |
| 9 | 4:3、448x336、移动设备 (1000 Kbps) | 1.2 Mbps | _Mobile_448x336_1000K | 1000 | 448x336 | 与源相同 | 80 | 高分辨率、Wi-Fi |
| 10 | 4:3、448x336、移动设备 (1200 Kbps) | 1.5 Mbps | _Mobile_448x336_1200K | 1200 | 448x336 | 与源相同 | 96 | 高分辨率、Wi-Fi |

## 查看器预设 {#viewer-presets}

>[!NOTE]
>
>**Flash查看器生命周期结束通知** -自2017年1月31日起，Adobe Scene7 Publishing system正式终止对Flash查看器平台的支持。 有关此重要更改的更多信息，请参阅以下常见问题解答网站： [https://docs.adobe.com/content/docs/en/aem/6-1/administer/integration/marketing-cloud/scene7/flash-eol.html](https://docs.adobe.com/content/docs/en/aem/6-1/administer/integration/marketing-cloud/scene7/flash-eol.html)。

*查看器预设*&#x200B;是一组设置，决定了用户如何在其计算机屏幕和移动设备上查看富媒体资源。作为管理员，您可以创建查看器预设。提供适用于一系列查看器配置选项的设置。例如，您可以更改查看器显示尺寸、缩放行为、颜色方案、边框和字体。

作为最佳实践，请使用Dynamic Media Classic HTML5视频查看器。 HTML5 视频查看器中使用的预设是功能强大的视频播放器。将使用 HTML5 和 CSS 设计播放组件的功能合并到一个单独播放器中实现了嵌入播放，并可根据浏览器功能选择使用自适应流和渐进式流，从而将富媒体内容的范围扩展到台式机、平板电脑和移动用户并确保视频体验一体化。

请参 [阅《Adobe查看器参考指南](https://marketing.adobe.com/resources/help/en_US/s7/viewers_ref/c_html5_viewers_about.html) 》中的“关于HTML5查看器”。

请参 [阅Dynamic Media Classic查看器预设兼容性矩阵](application-setup.md#scene7_viewer_preset_compatibility_matrix)。

请参阅[最佳做法：使用 HTML5 视频查看器](best-practice-using-html5-video.md#best_practice_using_the_html5_video_viewer)。

您可以根据查看器添加社区功能。社区功能包括“嵌入”按钮、“电子邮件”按钮、“链接”按钮和“访问站点”按钮。通过这些按钮，使用查看器的用户可以与他人共享查看器或打开Dynamic Media Classic网站。

另请参阅此处和此处的Adobe查看器参 [考库](/help/assets/vlist/vlist.html)[示例](https://landing.adobe.com/en/na/dynamic-media/ctir-2755/live-demos.html)。

### 用于响应式设计网页的查看器支持 {#viewer-support-for-responsive-designed-web-pages}

不同的网页具有不同的需求。有时，您希望在网页中提供一个链接，以便在单独的浏览器窗口中打开 HTML5 查看器。在其他情况下，可能需要直接在承载页面中嵌入 HTML5 查看器。对于后一种情况，网页可能具有静态的布局。或者，网页也可能是“响应式的”，将针对不同的设备或浏览器窗口大小显示不同的内容。为满足这些需求，Dynamic Media Classic附带的HTML5查看器支持静态网页和响应式设计的网页。

See [Responsive Static Image library](https://marketing.adobe.com.com/resources/help/en_US/s7/is_ir_api/is_api/c_about_responsive_static_image_library.html)in the *Adobe Image Serving API Help* for more information on how to embed responsive viewers onto your web pages.

### 查看器预设类型 {#viewer-preset-types}

管理员可以创建和自定义以下类型的查看器预设：

**eCatalog Viewer** 模拟阅读打印目录的体验。 您可以在页面之间移动、放大和缩小页面上的项目、使用图像映射查看有关页面上的项目的更多信息或搜索目录。 还可以包括“信息面板”，在映射区域具有有效的 rollover_key 属性时显示详细信息和图像映射的物品。要包括“信息面板”，请在“eCatalog 查看器预设”窗口的“信息面板设置”面板中指定“信息服务器 URL”。

**样本集查看器** -以不同的颜色、材料、纹理、外表或结构显示图像。 用户单击一个缩略图即可查看图像的变动。

**混合媒体集查看器** -在一个查看器中显示不同类型的媒体。 您可以包括样本集、旋转集、图像和视频。您可以设置各个选项卡，以包含不同类型的内容，例如，一个选项卡用于图像集、一个选项卡用于视频。从混合媒体集播放的视频使用具有时间线和视频控件（如停止、暂停、回放和播放）的标准视频查看器。您设置混合媒体集查看器预设时，指定要将哪些查看器用于“混合媒体集”中的不同类型的资源。您还可以使用“网格查看器”或“轮盘式查看器”来查看混合媒体集。

**旋转集查看器** -提供图像的多个视图，以便用户可以旋转对象以检查不同的侧面和角度。

**视频查看器** -使用源文件的分辨率尺寸或自定义大小显示视频。 Dynamic Media Classic附带许多用于播放视频的预定义查看器预设，如果您是管理员，则可以创建自定义视频查看器预设。 有十几种不同的设置可用于配置“视频查看器”。您可以配置其大小、前景和背景颜色、视频和音频控件、进度条、用户界面外观、社交功能和“帮助”。

**缩放查看器** ：提供三种缩放查看器类型的选项：

**缩放查看器** -允许用户通过单击来放大区域。 用户可以单击控件来放大、缩小图像、并将图像重置为其默认大小。

**缩放查看器：飞出** “在原始图像旁边显示缩放区域的第二幅图像”。 没有控件可以使用，用户只需将选取范围移动到他们要查看的区域上即可。

在确定此查看器的完整带宽使用量时，请考虑在查看器中有主图像和弹出图像。主图像大小（舞台宽度和高度）和缩放系数决定了弹出图像大小。为防止弹出文件大小变得太大，需对这两个值进行平衡：如果您的主图像大小很大，请降低缩放系数值。（弹出宽度和弹出高度决定了弹出窗口的大小，但不决定提供给查看器的弹出图像的大小。）

例如，如果您的主图像大小是 350 X 350 像素，缩放系数为 3，则生成的弹出图像是 1050 X 1050 像素。如果您的主图像大小是 300 X 300 像素，缩放系数为 4，则弹出图像是 1200 X 1200 像素。根据 JPEG 品质设置（推荐的设置介于 80-90），您可以显著地减少文件大小。建议的缩放系数为 2.5 至 4，取决于您的主图像的大小。

### Dynamic Media Classic查看器预设兼容性表 {#scene-viewer-preset-compatibility-matrix}

**Flash查看器生命周期结束通知**:自2017年1月31日起，Adobe Scene7 Publishing system正式终止对Flash查看器平台的支持。

有关此重要更改的更多信息，请参阅以下常见问题解答网站： [https://docs.adobe.com/content/docs/en/aem/6-1/administer/integration/marketing-cloud/scene7/flash-eol.html](https://docs.adobe.com/content/docs/en/aem/6-1/administer/integration/marketing-cloud/scene7/flash-eol.html)。

下表标识了当前可用的Dynamic Media Classic Viewer Presets。 该表还指定了查看器与桌面和移动设备的兼容性，以及对每个指定查看器使用的技术。

另请参阅此处和此处的Adobe查看器参 [考库](/help/assets/vlist/vlist.html)[示例](https://landing.adobe.com/en/na/dynamic-media/ctir-2755/live-demos.html)。

有关查看器支持的 Web 浏览器和操作系统版本的信息，您可以查阅查看器发行说明。

请参 [阅Adobe查看器参考发行说明](https://marketing.adobe.com/resources/help/en_US/s7/viewers_ref/)。

|  | 查看器技术 | 桌面 | Apple iPhone | Apple iPad | Android 智能手机 | Android 平板电脑 |
|--- |--- |--- |--- |--- |--- |--- |
| 缩放查看器 |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML5 | X | X | X | X | X |
| Universal_HTML5_Zoom_inline | HTML5 | X | X | X | X | X |
| Universal_HTML5_Zoom_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_Zoom_light | HTML5 | X | X | X | X | X |


|  | 查看器技术 | 桌面 | Apple iPhone | Apple iPad | Android 智能手机 | Android 平板电脑 |
|--- |--- |--- |--- |--- |--- |--- |
| 图像集查看器 |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_light | HTML5 | X | X | X | X | X |

|  | 查看器技术 | 桌面 | Apple iPhone | Apple iPad | Android 智能手机 | Android 平板电脑 |
|--- |--- |--- |--- |--- |--- |--- |
| 样本集查看器 |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML5 | X | X | X | X | X |
| Universal_HTML5_SwatchSet_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_SwatchSet_light | HTML5 | X | X | X | X | X |

|  | 查看器技术 | 桌面 | Apple iPhone | Apple iPad | Android 智能手机 | Android 平板电脑 |
|--- |--- |--- |--- |--- |--- |--- |
| eCatalog 查看器 |  |  |  |  |  |  |
| Universal_HTML5_eCatalog_Adv（包括对社交媒体和目录搜索的支持。） | HTML5 | X | X | X | X | X |
| Universal_HTML5_eCatalog（包括对社交媒体和目录搜索的支持。） | HTML5 | X | X | X | X | X |

|  | 查看器技术 | 桌面 | Apple iPhone | Apple iPad | Android 智能手机 | Android 平板电脑 |
|--- |--- |--- |--- |--- |--- |--- |
| 旋转查看器 |  |  |  |  |  |  |
| Universal_HTML5_SpinSet_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_SpinSet_light | HTML5 | X | X | X | X | X |

**eVideo 查看器**

Dynamic Media Classic支持MP4 H.264视频的移动视频播放。

* 您可以在以下位置找到支持此视频格式的Blackberry设备：Blackberry [上支持的视频格式](https://developer.blackberry.com/devzone/develop/supported_media/bb10_media_support.html)
* 您还可以在以下位置找到支持此视频格式的Windows设备：Windows Phone[上支持的视频格式](https://docs.microsoft.com/en-us/previous-versions/windows/apps/ff462087(v=vs.105)?redirectedfrom=MSDN)

|  | 查看器技术 | 桌面 | Apple iPhone | Apple iPad | Android 智能手机 | Android 平板电脑 | Blackberry 智能手机 | Windows Phone |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| Universal_HTML5_Video（包括对隐藏式字幕的支持。）See [Best practice: Using the Universal HTML5 Video viewer.](best-practice-using-html5-video.md#best_practice_using_the_html5_video_viewer) | HTML5 | X | X | X | X | X | X | X |
| Universal_HTML5_Video_social（包括对隐藏式字幕和社交媒体的支持。） | HTML5 | X | X | X | X | X | X | X |

|  | 查看器技术 | 桌面 | Apple iPhone | Apple iPad | Android 智能手机 | Android 平板电脑 |
|--- |--- |--- |--- |--- |--- |--- |
| 混合媒体集查看器 |  |  |  |  |  |  |
| Universal_HTML5_MixedMedia_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_MixedMedia_light | HTML5 | X | X | X | X | X |

### 支持的移动查看器手势表格 {#supported-mobile-viewers-gestures-matrix}

下表标识 iOS、Android 2.x 和 Android 3.x 设备上支持的移动查看器手势。

|  | 查看器技术 | 桌面 | Apple iPhone | Apple iPad | Android 智能手机 | Android 平板电脑 |
|--- |--- |--- |--- |--- |--- |--- |
| 图像集查看器 |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_light | HTML5 | X | X | X | X | X |

### 关于“查看者预设”屏幕 {#about-the-viewer-preset-screen}

在“查看器预设”屏幕上创建和管理“查看器预设”。要打开此屏幕，请单击“**设置**”&gt;“**查看器预设**”。

“查看器预设”屏幕提供了用于执行以下任务的工具：

**添加预设** ，单击添加，然后在添加查看器预设对话框中进行选择。

请参阅[添加和编辑查看器预设](application-setup.md#adding_and_editing_viewer_presets)。

**编辑预设** 选择预设，然后单击编 **辑**。

请参阅[添加和编辑查看器预设](application-setup.md#adding_and_editing_viewer_presets)。

**删除预设** 选择预设，然后单击删 **除**。

**导出预设** 选择HTML5查看器预设，然后单击导出以下载查看器外观，以便您能够将其用作创建和添加新查看器预设的基础。

请参 [阅导出HTML5查看器预设](application-setup.md#exporting_an_html5_viewer_preset)。

**筛选查看器预设列表** 使用这些工具筛选列表：

* 打开“**活动/非活动**”下拉列表并选择一个选项，以显示活动预设、非活动预设或所有预设。
* 打开“**查看器**”下拉列表并选择一个选项，以仅查看特定类型的查看器。选择“**所有查看器**”以查看所有查看器。

**排序预设** 单击列标题（活动、类型、预设或平台）可对列上的列表进行排序。 再一次单击列标题可按降序（或升序）排序列表。

**激活和取消激活预设** 选择预设，然后单击其“活动”选项以激活或取消激活预设。

请参阅[激活或停用查看器预设](application-setup.md#activating_or_deactivating_viewer_presets)。

>[!NOTE]
>
>单击“查看器预设”屏幕右侧的“预览”，以查看资源在您所选择的“查看器预设”中的显示效果。要查看不同的资源，您可以单击“查看器预设”屏幕中的“浏览”，并在“选择资源预览”对话框中选择不同的资源。

### 添加和编辑查看器预设 {#adding-and-editing-viewer-presets}

除使用用户界面中的“添加”来添加查看器预设以外，还可以使用“导出”来添加查看器预设。您只需导出现有的HTML5查看器预设，然后将其用作新预设的基础。

请参 [阅导出HTML5查看器预设](application-setup.md#exporting_an_html5_viewer_preset)。

**添加和编辑查看器预设**

1. 在 Scene7 Publishing System 的右上角附近，单击“**设置**”&gt;“**查看器预设**”。

   您可以过滤预设列表。例如，要仅查看视频查看器的预设，请从表正上方的工具栏上的“查看器”下拉列表中选择“视频查看器”。

1. 在“查看器预设”屏幕中，添加或编辑查看器预设。

   **添加** 、单击工具栏上的添加。 在“添加查看器预设”对话框中，选择一个平台，然后选择一种富媒体资源类型。

   在您创建完“查看器预设”时，单击“**另存为**”。

   **通过从现有查看器预设开始添加** 。在表中，选择视频查看器预设，然后单击工具栏中的编辑。

   在重新配置“视频查看器”后，在“预设名称”文本字段中单击“**另存为**”以使用不同的名称保存预设。

   **编辑** ：选择现有的查看器预设，然后单击编 **辑**。

1. 在“配置查看器”屏幕的“预设名称”字段中，输入或编辑预设名称。
1. 设置其余所需的选项。

   >[注��]
   >
   >选择“与源相同”，可将“视频查看器”自动调整为编码视频自身的分辨率大小。如果选择该选项，则不能输入“舞台宽度”和“舞台高度”。相反，这些选项来自视频自身。如果您选择“与源相同”，请设置“边距大小”选项，以反映视频播放区域外部的外观尺寸。该边距大小是视频控件的像素高度和宽度。您可以借助以下图示来帮助您确定要使用的边距大小。*

   ![](assets/vs_video_viewer_configure_margin.png)

1. 执行以下任一操作：

   * 如果通过现有的预设添加查看器预设，请单击“**另存为**”。
   * 如果添加或编辑了查看器预设，请单击“**保存**”。

### 导出HTML5查看器预设 {#exporting-an-html-viewer-preset}

您可以导出现有的HTML5查看器预设，作为创建新HTML5查看器预设的基础。 该导出选项很有用，因为您不必从头开始创建查看器。相反，您会导出外观和行为与所需预设接近的预设，然后以此为基础开始进行设计调整。

请注意，SPS中所有默认的现成查看器预设CSS文件都使用指向位于上的资源的相对图像服务路径 `Scene7SharedAssets`。 例如，以下是位于以下位置的查看器预设CSS文件中图像资产的相对路径 `Scene7SharedAsset`:但是， `.s7videoviewer .s7fullscreenbutton[state][selected] { background-image: url(/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha); }`如果您在自己的站点上承载查看器CSS文件，则必须通过在自己的环境中使用指向图像服务器的显式路径来解析这些相对图像路径。 为便于说明，如果要将上面的相对路径更新为显式路径，则其可能如下所示，其中 `https://s7d1.scene7.com` 是图像服务器的直接路径： `https://s7d1.scene7.com/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha`

**导出HTML5查看器预设**

```as3
.s7videoviewer .s7fullscreenbutton[state][selected] 
{ background-image: url(/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha); }
```

```as3
https://s7d1.scene7.com/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha
```

1. 单击“**设置**”&gt;“**查看器预设**”。
1. On the Viewer Presets toolbar, in the second drop-down list from the left, select **HTML5**.
1. 在左边的第三个下拉列表中，选择“**所有查看器**”。
1. 选择要用作新HTML5查看器预设基础的查看器预设。
1. 在工具栏中，单击“**导出**”。
1. 在“导出所选资源”对话框中，单击“**提交导出**”。

   导出后，您将获得CSS文件。 下载并解压缩此文件。

1. 在 CSS 编辑器中打开 CSS 文件，进行更改，然后保存该文件。
1. 将CSS文件上传到Scene7 Publishing System。

   请参阅[上载文件](uploading-files.md#uploading_files)。

1. 将CSS文件发布到Dynamic Media Image Server。

   请参阅[发布文件](publishing-files.md#publishing_files)。

1. 照常添加新的查看器预设。选择您上传的查看器CSS文件。

   请参阅[添加和编辑查看器预设](application-setup.md#adding_and_editing_viewer_presets)。

### 激活或停用查看器预设 {#activating-or-deactivating-viewer-presets}

要创建用于显示资源的 URL，用户需要在“预览”对话框中打开“预设”下拉列表，选择“查看器预设”，然后单击“复制 URL”（请参阅[复制查看器预设的 URL](application-setup.md#copying_the_url_of_a_viewer_preset)）。此“预设”列表提供了管理员在“查看器预设”屏幕上添加和管理的“查看器预设”。例如，在用户预览 eCatalog 时，所有活动的 eCatalog 查看器预设都显示在“预览”对话框的“预设”下拉列表上。

除非您在“查看器预设”屏幕上停用查看器预设，否则“预览”对话框的“预设”下拉列表可能变得内容越来越多。

**激活或停用查看器预设**

1. Choose **Setup** &gt; **Viewer Presets** to open the Viewer Presets screen.
1. 选择或取消选择“活动”选项以激活或停用“查看器预设”。

### 复制查看器预设的 URL {#copying-the-url-of-a-viewer-preset}

发布资源后，您可以复制以查看器预设的设置显示资源的 URL。

URL 即复制到剪贴板中。您可以根据需要在网页的 HTML 代码、移动设备或应用程序中使用它。

**复制查看器预设的 URL**

1. 在“浏览”面板中选择资源。
1. 在“资源浏览”面板上方的工具栏右侧，执行以下任一操作：

   * 单击“**网格视图**”。在“资源浏览”面板中，双击单个资源以便在详细信息视图中将其打开。在右侧的“URL 和嵌入代码”面板中，单击所需查看器右侧的“**复制 URL**”。
   * 单击“**网格视图**”。在“资源浏览”面板中，选择单个资源，然后在缩略图图像下方单击“**预览**”&gt;“**查看器列表**”。
   在“查看器列表”页面中表的“操作”列下，单击“**复制 URL**”。

   * 单击“**列表视图**”。在“资源浏览”面板中，选择单个资源，然后在缩略图图像右侧单击“**预览**”&gt;“**查看器列表**”。
   在“查看器列表”页面中表的“操作”列下，单击“**复制 URL**”。

   * 单击“**网格视图**”、“**列表视图**”或“**详细信息视图**”。在同一工具栏上，单击“**预览**”&gt;“**查看器列表**”。
   在“查看器列表”页面中表的“操作”列下，单击“**复制 URL**”。

### 复制查看器预设的嵌入代码 {#copying-the-embed-code-of-a-viewer-preset}

使用嵌入代码功能，您可以查看用于所选查看器预设的查看器代码。您也可以将代码复制到剪贴板中，以便可以将其粘贴到网页中以部署查看器。

在“嵌入代码”对话框中不允许编辑代码。

**复制查看器预设的嵌入代码**

1. 在“资源浏览”面板中选择资源。
1. 在“资源浏览”面板上方的工具栏右侧，执行以下任一操作：

   * 单击“**网格视图**”。在“资源浏览”面板中，双击单个资源以便在详细信息视图中将其打开。在右侧的“URL”面板中，单击“**嵌入代码**”。
   * 单击“**网格视图**”。在“资源浏览”面板中，选择单个资源，然后在缩略图图像下方单击“**预览**”&gt;“**查看器列表**”。
   在“查看器列表”页面中表的“操作”列下，单击“**嵌入代码**”。

   * 单击“**列表视图**”。在“资源浏览”面板中，选择单个资源，然后在缩略图图像右侧单击“**预览**”&gt;“**查看器列表**”。
   在“查看器列表”页面中表的“操作”列下，单击“**嵌入代码**”。

   * 单击“**网格视图**”、“**列表视图**”或“**详细信息视图**”。在同一工具栏上，单击“**预览**”&gt;“**查看器列表**”。
   在“查看器列表”页面中表的“操作”列下，单击“**嵌入代码**”。

1. 在“嵌入代码”对话框中，单击“**复制到剪贴板**”。
1. 单击“**关闭**”。

## 配置默认查看器 {#configuring-default-viewers}

您可以使用默认查看器来配置默认查看器，当您在 Scene7 Publishing System 中使用预览时，该默认查看器与资源关联。您可以为下列资源类型设置默认预览体验：

* 图像
* 视频
* 旋转集
* 目录
* 图像集
* 样本集
* 媒体集

**配置默认查看器**

1. In the Setup drop-down list, click **Application Setup**.
1. In the Setup window, in the left pane, expand **Application Setup** &gt; **Viewers**
1. Click **Default Viewers**.
1. 在“默认查看器”窗口中，在每种资源类型的下拉列表中，选择要与该资源的预览关联的查看器。
1. In the lower-right corner of the Default Viewers window, click **Save Settings**.
1. In the lower-right corner of the Setup window, click **Close** to return to the Asset window.

## 元数据视图 {#metadata-views}

*元数据*&#x200B;是关于资源的标准化信息。您可以使用元数据来简化工作流程、组织资源和改进搜索。Dynamic Media Classic支持IPTC（国际出版电信委员会）标准和XMP（可扩展元数据平台）标准。 在用户在详细信息视图中查看或输入有关资源的元数据之前，可以打开“元数据视图”菜单，并选择要查看或用于描述资源的一组元数据字段。

Dynamic Media Classic附带预定义的元数据视图，管理员可以创建自己的元数据视图供用户在输入元数据时进行选择。

### 创建元数据视图 {#creating-a-metadata-view}

1. Click **Setup** &gt; **Application Setup** &gt; **Metadata** &gt; **Metadata Views**.
1. 单击“**添加**”。
1. 在“预设名称”文本字段中，输入视图的名称。
1. (Optional) Check **Make Default** to make this view the one that users see when they open the Metadata panel in Detail View.
1. (Optional) Select **Include UDF** to include user-defined fields in the view. 用户定义的字段显示在详细信息视图的“元数据”面板的顶部。
1. Select the fields you want for the view (click **Select All** to select all the fields).
1. 单击“**保存**”。

   视图的选定类别和字段显示在“预览”面板中。

### 管理元数据视图 {#managing-metadata-views}

1. Click **Setup** &gt; **Application Setup** &gt; **Metadata** &gt; **Metadata Views**.
1. 执行以下任一操作：

   * 要预览视图，请将其选中。视图中的字段将显示在“预览”面板中。
   * To edit a view, select it and then click **Edit**. Then select or deselect field names on the Preview panel, and select or deselect the **Include UDF** option.
   * To delete a view, select it and then click **Delete**.
   * To make a view the default, select it and then click **Make Default**. 默认视图是用户在详细信息视图中打开资源并转到“元数据”面板时看到的一个视图。

## 元数据预设 {#metadata-presets}

元数据预设为管理员提供了控制和调整分配给资源的元数据的一种方式。在详细信息视图中，用户可以在相应的字段中输入有关资源的元数据。例如，用户可以输入所有者名称、版权说明和地址。要确保用户准确详尽地输入该信息，您可以创建“元数据预设”。在详细信息视图中选择元数据预设会使用预定义的值填充元数据字段。例如，会自动输入所有者名称、版权说明和地址。

为您希望用户可以在详细信息视图中自动输入来描述资源的每组元数据值创建“元数据预设”。

### 创建或编辑元数据预设 {#creating-or-editing-a-metadata-preset}

1. Click **Setup** &gt; **Application Setup** &gt; **Metadata** &gt; **Metadata Presets** .
1. 在“元数据预设”屏幕中，执行以下任一操作：

   * To create a preset, click **Add**. 在“元数据模板名称”文本字段中，键入预设的名称，然后单击“元数据视图” **，并从下拉列表中选择一个视图(请参** 阅元数据视图 [](application-setup.md#metadata_views))。
   * To edit an existing preset, select the preset from the Metadata Presets list and then click **Edit**.

1. 展开您要在预设中包括的标题，并在您要在预设中包括的不同字段中输入值。
1. 单击“**保存**”。

   预设的所选类别和字段将显示在“预览”面板中。

### 管理元数据预设 {#managing-metadata-presets}

1. Click **Setup** &gt; **Application Setup** &gt; **Metadata** &gt; **Metadata Presets**.
1. 执行以下任一操作：

   * 要预览预设，请选择您要预览的预设。预设信息（类别和字段）将显示在“预览”屏幕中。
   * To delete a preset, select the preset, and then click **Delete**.

## 用户定义的字段 {#user-defined-fields}

Media Portal 管理员或公司管理员可以创建自定义的、用户定义的元数据字段。自定义字段可以帮助您在Scene7 Publishing system中组织资产。 您可以根据需要将字段标记为“活动”。 激活后，这些自定义元数据字段的名称会显示在详细信息视图中的“元数据”面板中。用户可以在用户定义的元数据字段中输入信息以描述资源。用户也可以使用户定义的元数据字段成为搜索条件。

高效使用用户定义的元数据字段的一种方式是为特定启动或销售延迟资源的激活时间。您可以根据“日期”类型定义“激活” *字段*。 Then, using the **Metadata** panel in **Detail** view or **File** &gt; **Edit Info**, you can specify when the asset is activated. Scene7 Publishing System 会检查资源的发布状态和发布历史记录。如果它不在激活时间内，则发布状态显示为“未发布”。

>[!NOTE]
>
>要使用户定义的字段显示在详细信息视图中的“元数据”面板中，请将用户定义的字段加入元数据视图中。在“元数据视图”屏幕上，选择“包括 UDF”（用户定义的字段）选项。有关更多信息，请参阅[元数据视图](application-setup.md#metadata_views)。

>[!NOTE]
>
>要使用自定义的、用户定义的字段搜索资源，请单击“**设置**”&gt;“**个人设置**”，然后选择“**在搜索中包括 UDF**”。请参阅[个人设置](personal-setup.md#personal_setup)。

### 创建用户定义的元数据字段 {#creating-a-user-defined-metadata-field}

1. 单击“**设置**”&gt;“**应用程序设置**”&gt;“**元数据**”&gt;“**用户定义的字段**”。
1. 单击“**添加**”。
1. 在“自定义字段”对话框中，设置所需的选项。

   **名称** 输入元数据字段的名称。

   **类型** 选择一个选项，它定义用户可在元数据字段中输入的信息类型：

   **字符串** ：文本字符串。

   **整数** 。

   **浮点** ：浮点数。

   **是／否** ：是／否布尔值。

   **日期** A日期。 接受 MM/DD/YYYY 格式。

   **文件名** ：文件的名称。

   **颜色** ：颜色的名称。

   **尺寸** 资产的宽度和高度。

   **无类型** ，以实现向后兼容性。 请勿选择此选项。

   **默认值** （可选）输入用户最可能在字段中输入的值。 您输入的值会成为您所创建的字段的默认值。

   **应用至** （可选）如果希望元数据字段仅应用于特定类型的资产，请选择资产类型。

   ***Note**: Choose an **Applies To** option carefully because you cannot change the **Applies To** option after you create a user-defined field. Dynamic Media Classic lets you edit the name, type, and default value of a user-defined field, but not the **Applies To** setting. *

1. 创建元数据字段完成后，单击“**保存**”。

### 管理用户定义的字段 {#manage-user-defined-fields}

“用户定义的字段”屏幕提供了用于管理自定义、用户定义的元数据字段的命令。

只有 Media Portal 管理员或公司管理员可以管理用户定义的字段。

要打开该屏幕，请单击“**设置**”&gt;“**应用程序设置**”&gt;“**元数据**”&gt;“**用户定义的字段**”。

**编辑字段** 选择字段，然后单击“编 **辑”**。

**删除字段** 选择字段，然后单击“删 **除”**。

**激活字段** 单击以选择或取消选择字段名称旁边的活动选项。 如果您具有公司管理角色，则可能不会显示此选项。由于此选项与MediaPortal相关，因此必须在“个人设置”中选择（打开）“显示MediaPortal功能”以查看激活字段。

## 优化文件 {#optimize-files}

在将文件上载到 Scene7 Publishing System 时，系统会针对存储和发布优化对文件进行优化。然而，如果上载过程中断，则无法优化某些图像。在这种情况下，您会看到“尚未优化图像”消息。然而，如果您是管理员，则可以优化这些文件。

Scene7 Publishing System 会在您的文件中搜索，并且只优化那些之前未完全优化的图像。

1. 选择“ **设置** ”&gt;“应 **用程序设置**”，然后选择“**优化文件”**。
1. Enter information for the optimization job and click **Submit**.

   如果您在与多家公司协作，请分别优化属于不同公司的文件。

## 批量集预设 {#batch-set-presets}

使用批量集预设在作业运行时自动创建图像集或旋转集，以将资源上载到 Scene7 Publishing System。

公司管理员首先要分为一组的资源定义命名约定。然后，您可以创建批量集预设来引用这些图像。每个预设都是单独命名的、自成体系的指令集，指令集可定义如何使用与预设方法中定义的命名约定匹配的图像构建集。

“上载作业选项”对话框会列出公司的所有活动批量集预设，以便您指定要在每个上载会话期间应用的预设。公司管理员将看到所有活动和非活动的批量集预设。上传文件时，Dynamic Media Classic会自动创建一个集，其中包含与活动预设中定义的命名约定相匹配的所有文件。

### 默认命名 {#default-naming}

公司管理员创建在任何批量集预设方法中使用的默认命名约定。您的公司只需要在批量集预设定义中选择默认命名约定，以针对所有网站批量生成集。要使用您定义的默认命名约定，需创建批量集预设。如果公司定义的默认命名有例外情况，您可以为一组特定内容根据需要使用备用的自定义命名规则创建任意数量的批量集预设。

虽然使用批量集预设功能不需要设置默认命名约定，但建议您最好使用默认命名约定来尽可能多地定义您要分组在一个集合中的命名约定元素，以简化批量集创建。

1. 单击“**设置**”&gt;“**应用程序设置**”&gt;“**批量集预设**”&gt;“**默认命名**”。
1. 选择“**查看表单**”或“**查看代码**”，以指定您希望如何查看和输入有关每个元素的信息。

   您可以选中“查看代码”复选框，以查看和您的表单选项一起构建的正则表达式值。如果表单视图因某种原因对您构成限制，您可以输入或更改上述值，以帮助定义命名约定的元素。如果在表单视图中无法解析您的值，则表单字段会变为非活动状态。

   >[!NOTE]
   停用的表单字段并不表示正则表达式无效。没有针对正则表达式正确性的验证措施。您会在“结果”行的后面看到您为每个元素构建的正则表达式的结果。完整的正则表达式显示在页面底部。

1. 根据需要展开每个元素，并输入您要使用的命名约定。
1. 根据需要，单击“**添加**”，以便为元素添加其他命名约定。或者，单击“**删除**”以删除元素的命名约定。
1. 单击“**另存为**”并键入预设的名称。或者，如果要编辑现有的预设，请单击“**保存**”。

另外，您还可以使用没有表单字段的“查看代码”。在此视图中，完全使用正则表达式创建您的命名约定定义。

有两个元素可用于定义，即“匹配”和“基本名称”。在这些字段中，您可以定义命名约定的所有元素，并指定用于命名它们所在的集的约定部分。公司的单个命名约定可以使用上述每个元素的一行或多行定义。可以在您的特有定义中使用所需数量的行，并将它们分组到不同的元素中，例如，用于主图像、颜色元素、备选视图元素和样本元素。

### 创建批量集预设 {#creating-a-batch-set-preset}

Dynamic Media Classic使用批量集预设将共享一些公共信息或内容的资产组织到一组图像中，以便在查看器中显示。 批集预设方法会自动与您在Dynamic Media Classic中计划的资产导入作业一起运行。

可以使用“批量集预设”创建、编辑和管理批量集预设。您可以创建所需数量的批量集预设以满足所需的所有资源采纳作业的要求。共有两种形式的批量集预设定义：一种用于您可能已设置的默认命名约定，另一种用于您临时创建的自定义命名约定。

您可以使用表单字段方法来定义批量集预设或代码方法，后者允许您使用正则表达式。如同在默认命名中一样，在“表单视图”中进行定义时可以选择“代码视图”并使用正则表达式来构建您的定义。或者，您可以取消选中任一视图，只使用其一个视图。

另请参阅[创建用于自动生成 2D 旋转集的批量集预设](application-setup.md#creating_a_batch_set_preset_for_the_auto_generation_of_a_2d_spin_set)。

**创建批量集预设**

1. 单击“**设置**”&gt;“**应用程序设置**”&gt;“**批量集预设**”&gt;“**批量集预设**”。默认视图为“**查看表单**”（在“详细信息”页面的右上角设置）。
1. 在“预设列表”面板中，单击“**添加**”以激活屏幕右侧“详细信息”面板中的定义字段。
1. 在“详细信息”面板的“预设名称”字段中，键入预设的名称。
1. 在“批量集类型”下拉菜单中，选择预设类型。

   要自动生成 2D 旋转集，请在“批量集类型”下拉列表中选择“**多轴旋转集**”。

1. 执行以下任一操作：

   * 如果您使用的是之前在“应用程序设置”&gt;“批量集预设”&gt;“默认命名”下设置的默认命名约定，请展开“**资源命名约定**”，然后在“文件命名”下拉列表中，单击“**默认**”。
   * 要在设置预设时定义命名约定，请展开“**资源命名约定**”，然后在“文件命名”下拉列表中，单击“**自定义**”。

1. 对于“序列”顺序，定义在Dynamic Media Classic中将图像集分组在一起后图像的顺序。 默认情况下，将按字母数字顺序对您的资源排序。不过，可以使用逗号分隔的正则表达式列表来定义顺序。
1. 对于设置命名和创建约定，为您在“资源命名约定”中定义的基本名称指定后缀或前缀。还可以定义在Dynamic Media Classic文件夹结构中创建图像集的位置。

   如果定义大量图像集，您可能要将这些图像集与资源本身所在的文件夹分开。许多客户会创建一个“图像集”文件夹，并让应用程序将批量集生成的集合放在此处。

1. 单击“详细信息”面板中的“**保存**”。

### 创建用于自动生成 2D 旋转集的批量集预设 {#creating-a-batch-set-preset-for-the-auto-generation-of-a-d-spin-set}

您可以使用批量集类型“**多轴旋转集**”来创建用于自动生成 2D 旋转集的“方法”。对图像进行分组时采用“行”和“列”正则表达式，以便图像资源在多维数组的对应位置中正确对齐。

另请参阅[创建批量集预设](application-setup.md#creating_a_batch_set_preset)。

多轴旋转集中没有最小或最大的行数或列数限制。

例如，假设您要创建名为 *spin-2dspin* 的多轴旋转集。有一组旋转集图像包含 3 行，每行 12 个图像。这些图像命名如下：

```as3
spin-01-01
spin-01-02
… 
spin-01-12
spin-02-01
… 
spin-03-12
```

根据此信息，您的批量集类型方法可以按如下方式创建：

![](assets/se_batch_set_recipe.png)

将旋转集的共享资源名称部分的分组添加到“**匹配**”字段（高亮显示）。将包含行和列的资源名称的变量部分分别添加到“**行**”和“**列**”字段。

在上载和发布旋转集时，将激活在“**上载作业选项**”对话框的“**批量集预设**”下面列出的 2D 旋转集方法名称。

**创建用于自动生成 2D 旋转集的批量集预设**

1. 选择“**设置**”&gt;“**应用程序设置**”&gt;“**批量集预设**”&gt;“**批量集预设**”。默认视图为“**查看表单**”（在“详细信息”页面的右上角设置）。
1. 在“预设列表”面板中，单击“**添加**”以激活屏幕右侧“详细信息”面板中的定义字段。
1. 在“详细信息”面板的“预设名称”字段中，键入预设的名称。
1. 在“批量集类型”下拉菜单中，选择“**资源集**”。
1. 在“子类型”下拉列表中，选择“**多轴旋转集**”。
1. 展开“**资源命名约定**”，然后在“文件命名”下拉列表中，单击“**自定义**”。
1. 使用“**匹配**”和（可选）“**基本名称**”属性定义用于对构成分组的图像资源进行命名的正则表达式。

   例如，文本匹配正则表达式可能如下所示：

   `(\w+)-\w+-\w+`

1. 展开“**行列位置**”，然后为 2D 旋转集数组中图像资源的位置定义名称格式。

   使用圆括号将文件名中的行或列位置括起来。

   例如，行正则表达式可能如下所示：

   `\w+-R([0-9]+)-\w+`

   或者

   `\w+-(\d+)-\w+`

   列正则表达式可能如下所示：

   `\w+-\w+-C([0-9]+)`

   或者

   `\w+-\w+-C(\d+)`

   请记住，这些只是示例。您可以创建任何满足自己需要的正则表达式。

   >[!NOTE]
   如果行和列正则表达式的组合无法确定资源在多维旋转集数组中的位置，则不会将该资源添加到集中，而会记录错误。

1. 对于设置命名和创建约定，为您在“资源命名约定”中定义的基本名称指定后缀或前缀。还可以定义在Dynamic Media Classic文件夹结构中创建图像集的位置。

   如果定义大量图像集，您可能要将这些图像集与资源本身所在的文件夹分开。许多客户会创建一个“图像集”文件夹，并让应用程序将批量集生成的集合放在此处。

1. 单击“详细信息”面板中的“**保存**”。
1. 照常上载和发布您的旋转集，同时确保您在“作业加载选项”对话框中的“批量集预设”下激活 2D 旋转集的名称。

>[!MORELIKETHIS]
* [预览资源](previewing-asset.md#previewing_an_asset)
* [设置图像预设](setting-image-presets.md#setting_up_image_presets)
* [查看、添加和导出元数据](viewing-adding-exporting-metadata.md#viewing_adding_and_exporting_metadata)
* [Checking job files](checking-job-files.md#checking_job_files)

