---
title: 应用程序设置
description: 了解如何设置和配置Adobe Dynamic Media Classic的“应用程序”区域。 利用“应用程序”区域，可输入常规设置、创建图像、查看器和视频编码预设、定义默认查看器和元数据、发布设置和视频SEO设置。 您还可以使用区域设置批集预设，以自动生成2D旋转集。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/setup
feature: Dynamic Media Classic
role: Admin
exl-id: 3f96606e-ef5c-4c01-aa0f-3148f14e28be
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '11299'
ht-degree: 40%

---

# 应用程序设置{#application-setup}

您可以使用“应用程序设置”页面输入常规设置、创建图像预设、视频编码预设、查看器预设，或定义默认查看器和元数据。 您可以设置批集预设，以便还自动生成2D旋转集（例如）、发布设置和视频SEO设置。

>[!NOTE]
>
>只有Adobe Dynamic Media Classic管理员才能更改“应用程序设置”页面上的设置。

## 常规设置 {#general-settings}

要打开“应用程序常规设置”页面，请在全局导航栏中，转到 **[!UICONTROL 设置]** > **[!UICONTROL 应用程序设置]** > **[!UICONTROL 常规设置]**.

### 服务器

在创建帐户时，Adobe Dynamic Media Classic会自动为您的公司提供分配的服务器。 这些服务器用于构建网站和应用程序的 URL 字符串。这些 URL 调用是您的帐户所特有的。

另请参阅 [测试安全测试服务](testing-assets-making-them-public.md#testing_the_secure_testing_service).

* **[!UICONTROL 已发布的服务器名称]**  — 此服务器是实时CDN（内容交付网络）服务器，用于特定于您帐户的所有系统生成URL调用。 除非Adobe Dynamic Media Classic支持技术人员指示您更改此服务器名称，否则请勿更改此服务器名称。

* **[!UICONTROL 源服务器名称]**  — 此服务器仅用于质量保证测试。 除非Adobe Dynamic Media Classic支持技术人员指示您更改此服务器名称，否则请勿更改此服务器名称。

<!-- **AGM Server Name** This server is used for Web-to-Print templates. This server is set on a company-wide basis. Do not change this server name unless instructed to do so by an Adobe DynamicMedia Classic support technician. -->

* **[!UICONTROL Test&amp;Target服务器名称]**  — 您的Test&amp;Target URL，最多包含.com。 有关获取此URL的说明，请参阅集成 [!DNL Adobe Dynamic Media Classic] with [!DNL Adobe Target Standard/Premium].

<!-- **Test Publish Context Server Name** -->

* **[!UICONTROL iOS流服务器名称]**  — 指向您的 [!DNL Adobe Dynamic Media Classic] iOS流服务器。 该服务器使用 HTTP 协议将流视频发送至 iOS 设备。

* **[!UICONTROL 渐进式视频服务器名称]**  — 指向您的 [!DNL Adobe Dynamic Media Classic] 渐进式视频服务器。 该服务器使用 HTTP 协议发送渐进式视频。

* **[!UICONTROL 显示未发布资产的URL]**  — 如果需要，请选择此选项 [!DNL Adobe Dynamic Media Classic] 来显示URL，无论是否发布了任何资产。 如果资源未发布，此 URL 将无效。但是，您可以使用 URL 进行计划或组织。

<!-- **Allow AIR install** Select this option to allow users to download Adobe Dynamic Media Classic desktop version to their local hard drives. Users install the application from the Desktop Version area of the Personal Setup screen. -->

<!-- AIR users must manually uninstall their existing app and reinstall from the web version of Adobe Dynamic Media Classic (in Personal Settings). After this one-time reinstallation, you are prompted to upgrade whenever the server has a newer version of Adobe Dynamic Media Classic AIR. Adobe Dynamic Media Classic is integrated with the Application Update Framework which streamlines the upgrade process. -->

* **[!UICONTROL CDN失效模板]**  — 指定用于使CDN（内容交付网络）缓存失效的模板。

   例如，假定您输入了引用 `<ID>`，而不是像以下示例中那样使用特定的图像ID:

   `https://sample.scene7.com/is/image/Company/<ID>?$s7product$`

   如果模板仅包含 `<ID>`，则Adobe Dynamic Media Classic填充 `https://<server>/is/image`，其中 `<server>` 是在“常规设置”中定义的“发布服务器名称”。

   设置CDN无效模板，选择名为Backpack_B的图像，然后转到 **[!UICONTROL 文件]** > **[!UICONTROL 无效CDN]** 会在CDN无效界面中生成以下生成的URL:

   `https://sample.scene7.com/is/image/Company/Backpack_B?$s7product$`

   在URL列表框中，选择 **[!UICONTROL 继续]** 以清除该特定图像URL调用的缓存。 您也可以通过键入或粘贴URL列表框来添加URL;您无需预先设置模板。

   选择CDN失效模板并发出无效CDN请求后，用户界面中会弹出一个指示器。 它可让您估计清除缓存需要多长时间。

   同样，如果您在转到 **[!UICONTROL 文件]** > **[!UICONTROL 无效CDN]**，则会在保存的模板URL中引用每个图像。 因此，您可以定义CDN无效模板，以引用网站上引用的每个URL（如产品详细信息和搜索结果）。 然后，当您从缓存中选择一个或多个要失效的图像时，URL 会自动填充该界面。

   请参阅[内容缓存](dmc-platform-overview.md#content_caching)。

   请参阅[重新发布的资源和 CDN 延迟](publishing-files.md#republished_assets_and_cdn_delays)。

### 浏览

* **[!UICONTROL 显示项目]**  — 确定项目是否可用作组织Adobe Dynamic Media Classic资产的方法。 请参阅 [组织您的项目工作](/help/organizing-projects.md).

* **[!UICONTROL 显示示例eVideo内容]**  — 打开或关闭eVideo示例内容的显示。

* **[!UICONTROL 显示生成的内容]**  — 在文件夹中，显示从资产生成的内容。 例如，当PDF文件在上传时被栅格化时，Adobe Dynamic Media Classic会为原始PDF中的每个页面创建一个图像。 如果选择“显示生成的内容”，则在上载原始 PDF 时生成的每个图像都会与该 PDF 一起显示在将 PDF 上载到的文件夹中。

* **[!UICONTROL 显示编码视频]**  — 默认情况下，取消选中（关闭）。

   要在Adobe Dynamic Media Classic中快速搜索和浏览视频，而无需浏览同一视频的大量编码派生项，请取消选中此选项（默认）。 只显示主视频缩略图（您上传并用于创建派生项的源视频）和“父”自适应视频集缩略图（包含编码视频集的“子”派生项）。

   但是，您仍可以从主视频或自适应视频集中访问各个已编码视频。 要执行以上操作，请双击视频缩略图图像，打开详细信息视图。然后选择 **[!UICONTROL 编码视频]** ，以便您能够访问所有“子”视频。

   您还可以转到 **[!UICONTROL 文件]** > **[!UICONTROL 重新处理]** 直接从自适应视频集创建更多编码的“子”视频。 Adobe Dynamic Media Classic会自动找到自适应视频集的“父”主视频，并将其用作转码的源视频。 但是，如果保存新的单个编码视频，您在搜索或浏览时将看不到这些视频。但是，您仍可以从详细信息视图的“编码的视频”选项卡进行访问。

   请参阅 [上传和转码视频](uploading-encoding-videos.md#uploading_and_encoding_videos).

   要继续保留在搜索和浏览时可以访问所有编码视频派生的功能，请选择“**[!UICONTROL 显示已编码视频]**”。

   “构建”菜单上的某些操作只能对单个视频或选择性地对单个视频生效。此功能要求必须显示所有可以选择的编码视频派生（无论如何设置“**[!UICONTROL 显示已编码视频]**”）。过渡的生成操作 **[!UICONTROL 显示编码视频]** 设置包含 **[!UICONTROL 自适应视频集]**&#x200B;和 **[!UICONTROL 电子目录]**.

   >[!NOTE]
   >
   >如果您没有使用Adobe Dynamic Media Classic来上传视频资产并对其进行编码，则Adobe Dynamic Media Classic会显示您所有单独编码的视频，即使已取消选择此选项也是如此。

* **[!UICONTROL “显示刷新子文件夹”按钮]**  — 打开或关闭子文件夹“刷新”按钮的显示。

### Adobe Dynamic Media Classic FTP帐户

* **[!UICONTROL 服务器]**  — 列出您的FTP帐户服务器。

* **[!UICONTROL 用户名]**  — 列出您的FTP帐户用户名。

### 上载到应用程序

另请参阅 [默认上传作业选项](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/569_Default%20Job%20Options_converted%20renamed_Getting%20Started-AVS) 培训视频。

* **[!UICONTROL 覆盖图像]** - Adobe Dynamic Media Classic不允许两个文件具有相同的名称。 每个项目的Adobe Dynamic Media Classic ID（图像名称减去文件扩展名）必须唯一。 由于此规则，“上载”对话框中有一个“覆盖”选项。该选项的准确效果取决于指定的“覆盖图像”选项。这些选项指定了如何上载替换图像：替换原始图像，还是成为重复图像。重复图像会用“-1”重命名（例如，chair.tif 会重命名为 chair-1.tif）。这些选项会影响上载到的文件夹与原始图像不同的图像，或文件扩展名（如 JPG、TIF 或 PNG）与原始图像不同的图像。请参阅 [使用覆盖图像选项](#using-the-overwrite-images-option).

   * **[!UICONTROL 在当前文件夹中覆盖，基本图像名称/扩展名相同]**  — 此选项是最严格的替换规则。 它要求您将替换图像上载到原始图像所在的文件夹中，并且该替换图像与原始图像具有相同的文件扩展名。如果不满足这些要求，则会创建重复的图像。

   * **[!UICONTROL 在当前文件夹中覆盖相同的基本资产名称，而不考虑扩展名]**  — 要求您将替换图像上传到与原始图像相同的文件夹，但文件扩展名可能与原始图像不同。 例如，chair.tif 会替换 chair.jpg。

   * **[!UICONTROL 在任何文件夹中覆盖相同的基本资产名称/扩展名]**  — 要求替换图像的文件扩展名与原始图像相同（例如，chair.jpg必须替换chair.jpg，而不是chair.tif）。 但是，可以将替换图像上载到与原始图像不同的文件夹中。更新的图像位于新文件夹；而不再位于其原始位置

   * **[!UICONTROL 在任意文件夹中覆盖相同的基本资产名称，而不考虑扩展名]**  — 此选项是包含性最强的替换规则。 可以将替换图像上载到与原始文件所在文件夹不同的文件夹，使用不同的文件扩展名上载文件，并替换原始文件。如果原始文件在不同的文件夹中，替换图像则位于其所上载至的新文件夹。

* **[!UICONTROL 保留发布]**  — 指定上传到Adobe Dynamic Media Classic的替换图像是保留正在替换的图像的“准备发布”设置，还是在上传时指定该设置。

* **[!UICONTROL 默认颜色配置文件]**  — 指定在添加CMYK图像时作为“默认颜色配置文件选项”一部分应用的颜色配置文件。

* **[!UICONTROL 默认上传选项]**  — 打开“上传作业选项”对话框，您可以在其中指定默认的上传选项。 有关这些选项的信息，请参阅[上载选项](/help/uploading-files.md#upload_options)。

### 应用程序的图像映射编辑器

* **[!UICONTROL 默认图像映射HREF]**  — 定义用于图像映射中HREF列的默认URL。 此URL是您在创建图像映射时看到的默认URL。

* **[!UICONTROL 默认图像映射模板]**  — 为图像映射中的HREF模板定义默认JavaScript。 您可以在此处设置自定义代码，以便在您选择图像映射时运行。

### 应用程序的其他设置

* **[!UICONTROL 垃圾桶可以清理警告]**  — 垃圾桶中的资产会在七天内自动删除。 如果您需要在“垃圾桶”中的资源距永久删除还有四天时间时向公司管理员发送通知，请选择“自动删除垃圾桶项目之前会发送电子邮件”。请参阅 [管理垃圾桶文件夹](/help/trash-folder.md).

## 使用覆盖图像选项 {#using-the-overwrite-images-option}

Adobe Dynamic Media Classic不允许两个文件具有相同的名称。 每个项目的Adobe Dynamic Media Classic ID（图像名称减去文件扩展名）必须唯一。 由于该规则，所以“上载”对话框会包括“覆盖图像”选项。此选项的确切效果取决于每个公司的Adobe Dynamic Media Classic内部设置的设置。

如果您之前上传了图像，然后更改了原始文件（或替换了它们），则所选的覆盖选项会指定Adobe Dynamic Media Classic替换图像的方式。 没有关于图像更改的信息，但是新图像会替换旧图像。如果文件夹还包含Adobe Dynamic Media Classic中尚未包含的图像，则会添加这些图像。

如果您上传的图像在某种程度上发生了更改（图像已经更改），但对图像的引用保持不变，请使用此选项。 在上载和翻录 Adobe® PDF 时“覆盖”也很有用。微调Adobe Dynamic Media Classic *rip* 在图像中，调整“上传”对话框中的ICC颜色配置文件选项，然后使用“覆盖”功能重新上传。

用于从生产服务器访问图像的Adobe Dynamic Media Classic ID是从图像文件名派生的。 在替换现有文件和用于访问图像的Adobe Dynamic Media Classic ID时，文件名中必须使用大写和小写字符。 在上传到Adobe Dynamic Media Classic之前，请确保在文件名中使用大写和小写字符是正确的，以避免Adobe Dynamic Media Classic ID仅对于同一图像大小写不同。

如果您取消选择此选项，将与现有图像具有相同文件名的所有图像都视为重复图像，并且不予添加。

## 图像预设 {#image-presets}

“图像预设”屏幕用于创建和编辑图像预设。图像预设使Adobe Dynamic Media Classic能够以不同大小动态传送来自同一主图像的图像。 每个图像预设都表示用于显示图像的一组预定义大小和格式命令。在创建图像预设时，您可以选择图像交付的大小。 您还可以选择格式设置命令，以便在传送图像以供查看时优化图像的外观。

管理员可以创建导出资源的预设。用户在导出图像时可以选择预设，这也会按照管理员指定的规范对图像进行重新格式化。

要打开“图像预设”屏幕，请在全局导航栏上，转到 **[!UICONTROL 设置]** > **[!UICONTROL 图像预设]**.

请参阅 [智能成像](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/imaging-faq.html#dynamic).

### 创建并编辑图像预设 {#creating-and-editing-image-presets}

1. 转到 **[!UICONTROL 设置]** > **[!UICONTROL 图像预设]**.
1. 创建预设或从现有预设开始：

   * **创建图像预设**  — 选择 **[!UICONTROL 添加]**.
   * **从现有预设创建图像预设**  — 选择与您要创建的图像预设最相似的图像预设，然后选择 **[!UICONTROL 编辑]**.

1. 在添加（或编辑）预设页面上，输入预设的名称。
1. 设置所需的预设选项。

   请参阅[图像预设选项](application-setup.md#image_preset_options)。

1. 选择 **[!UICONTROL 保存]**，或者如果您从现有预设开始，请选择 **[!UICONTROL 另存为]**.
1. 要使用您自己的图像预览预设，请选择 **[!UICONTROL 浏览]** 然后选择图像。 要使用默认图像进行预览，请选择 **[!UICONTROL 重置]**.

您可以编辑图像预设，方法是在“图像预设”屏幕中选择图像预设的名称，然后选择 **[!UICONTROL 编辑]**. 要删除图像预设，请选择它，然后选择 **[!UICONTROL 删除]**.

### 图像预设选项 {#image-preset-options}

“添加预设”和“编辑预设”屏幕提供了用于创建和编辑图像预设的选项：

* **[!UICONTROL 预设名称]**  — 输入描述性名称，不留任何空格。 为帮助用户识别此图像预设，请在名称中包含图像大小规范。

* **[!UICONTROL 宽度和高度]**  — 以像素为单位输入传送图像的大小。

* **[!UICONTROL 格式]**  — 从菜单中选择格式。 选择GIF、JPEG、PDF或TIFF格式可显示更多选项：

   * GIF 颜色量化选项

      * **[!UICONTROL 类型]**  — 选择“自适应”（默认）、“Web”或“Macintosh”。 如果您选择 **[!UICONTROL GIFAlpha]**，则“ Macintosh”选项不可用。

      * **[!UICONTROL Dither]**  — 选择扩散或关闭。

      * **[!UICONTROL 颜色数量]**  — 拖动滑块以进入2-255。

      * **[!UICONTROL 颜色列表]**  — 输入以逗号分隔的列表。 例如，对于白色、灰色和黑色，输入 `000000,888888,ffffff`.
   * JPEG 选项

      * **[!UICONTROL 质量]**  — 控制JPEG压缩级别。 此设置既影响文件大小，又影响图像质量。JPEG质量比例尺为1-100。

      * **[!UICONTROL 启用JPG色度缩减采样]**  — 由于眼睛对高频颜色信息的敏感程度低于高频亮度，JPEG图像将图像信息分为亮度和颜色分量。 压缩 JPEG 图像时，通过将各组像素放到一起平均，亮度分量为全分辨率，颜色分量为缩减像素取样。缩减像素采样会将数据量减少二分之一或三分之一，而对于用户所能感知到的质量而言却几乎没有任何影响。缩减像素采样不适用于灰度图像。这种方法会减少对于高对比度图像有用的压缩的数量（例如，包含覆盖文本的图像）。
   * PDF 和 TIFF 选项

      * **[!UICONTROL 压缩]**  — 选择压缩算法。



* **[!UICONTROL Colorspace]**  — 选择色彩空间。

* **[!UICONTROL 锐化]**  — 选择启用简单锐化选项，以便在进行所有缩放后对图像应用基本锐化滤镜。 锐化可以帮助补偿在以不同尺寸显示图像时可能导致的模糊。

   有关锐化、重新采样模式和USM锐化的更多信息，请参阅 [锐化图像](sharpening-image.md#sharpening_an_image). 另请参阅 [锐化](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/547_sharpening1_converted%20renamed_Done-AVS) 培训视频。

* **[!UICONTROL 重新示例模式]**  — 选择一个重新取样模式选项。 当图像缩减像素取样时，以下选项锐化该图像：

* **[!UICONTROL B线性]**  — 最快的重新取样方法；会出现一些锯齿伪像。

* **[!UICONTROL 两次立方]**  — 提高图像服务器上的CPU使用率，但生成较锐利的图像，出现的锯齿伪像较少。

* **[!UICONTROL 锐化2]**  — 生成的结果比两次立方选项更锐利，但图像服务器的CPU成本更高。

* **[!UICONTROL 三线性]**  — 使用较高和较低分辨率（如果可用）；仅当出现锯齿问题时，才建议使用。 由于减少了高频数据，此方法会减小 JPEG 的大小。

* **[!UICONTROL 钝化蒙版]**  — 选择以下选项以微调锐化：

* **[!UICONTROL 金额]**  — 控制对边缘像素应用的对比度量。 默认值为 1.0。对于高分辨率图像，可将该值增加到 5.0。数量用于衡量滤镜强度。

* **[!UICONTROL 半径]**  — 确定边缘像素周围影响锐化的像素数。 对于高分辨率图像，请输入 1 到 2 之间的值。较低的数值仅锐化边缘像素，较高的数值则锐化范围更宽的像素。值正确与否取决于图像的大小。

* **[!UICONTROL 阈值]**  — 确定在应用USM锐化滤镜时要忽略的对比度范围。 换言之，此选项确定锐化的像素必须与周围区域相差多少，才被滤镜看作边缘像素并被锐化。为避免引进干扰，请用 0.02 到 0.2 之间的值做试验。默认值 6 锐化图像中的所有像素。

* **[!UICONTROL 色彩空间]**  — 确定图像是使用创建图像的空间，通常是RGB（原始）还是亮度空间（强度）。

* **[!UICONTROL 颜色]** 选择以下选项：

* **[!UICONTROL 输出颜色配置文件]**  — 选择 **[!UICONTROL 使用默认值]** 或Adobe Dynamic Media Classic上可用的ICC颜色配置文件之一。

   另请参阅[ ICC 配置文件](icc-profiles.md#icc_profiles)。

* **[!UICONTROL 渲染意图]**  — 如果要覆盖颜色配置文件的缺省渲染意图，请选择一个选项。 如果默认的ICC配置文件之一是颜色转换的目标颜色空间，则使用此选项。 或者，输出设备（打印机或显示器）具有此配置文件的特征，并且指定的渲染意图对此配置文件有效。

* **[!UICONTROL 嵌入配置文件]**  — 选择此选项，以便您在Adobe® Photoshop®中打开此图像时，该图像会使用此配置文件。

* **[!UICONTROL 打印分辨率]**  — 选择打印此图像的分辨率；默认为72像素。

* **[!UICONTROL URL修饰符]**  — 如果您要指定用于定义图像预设（而非设置）的URL修饰符，请在此处输入修饰符。

* **[!UICONTROL 示例图像URL]**  — 列出Dynamic Media图像服务器用于传送带有您添加或编辑的图像预设的图像的“原始”URL字符串。 此URL字符串会对您在“添加预设”或“编辑预设”屏幕中选择的所有格式设置进行编码。

### 编辑、删除或停用图像预设 {#editing-removing-or-deactivating-an-image-preset}

1. 转到 **[!UICONTROL 设置]** > **[!UICONTROL 图像预设]**.
1. 在“图像预设”屏幕中，选择表中的某个预设，然后执行以下任一操作：

   * 选择 **[!UICONTROL 编辑]** ，然后在“编辑预设”对话框中指定新选项。
   * 选择 **[!UICONTROL 删除]** 从列表中删除预设。
   * 取消选择 **[!UICONTROL 活动]** 如果要从整个Adobe Dynamic Media Classic用户界面中为MediaPortal用户删除预设名称，请选中预设名称旁边的复选框。

## 激活或停用自适应视频预设 {#activating-or-deactivating-adaptive-video-presets}

Adobe Dynamic Media Classic提供了自适应视频编码预设。 它是一个主要的预设列表，这些预设将16:9自适应视频预设和4:3自适应视频预设都合并到一个组中。 这些预定义的预设反映了最常用的编码设置，并且经过优化以便在目标移动设备、平板电脑和台式机上播放。

默认情况下，仅激活（启用或“打开”）“自适应视频”编码预设。您可以根据需要将其停用。在“上载作业选项”对话框的 eVideo 部分中，非活动自适应视频预设不会显示为可选择的选项。

请参阅 [上传和编码视频](uploading-encoding-videos.md#uploading_and_encoding_videos).

另请参阅 [视频预设](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/549_video-presets_converted%20renamed_Done-AVS) 培训视频。

**激活或停用自适应视频预设:**

1. 在Adobe Dynamic Media Classic的右上角附近，转到 **[!UICONTROL 设置]** > **[!UICONTROL 应用程序设置]** > **[!UICONTROL 视频预设]** > **[!UICONTROL 自适应视频预设]**.
1. 在“自适应视频预设”页中，取消选中某个预设名称旁边的复选框，以将该预设从“上载作业选项”对话框的“eVideo 选项”列表中删除。
1. 选择 **[!UICONTROL 关闭]**.

## 用于编码视频文件的视频预设 {#video-presets-for-encoding-video-files}

要选择编码预设，请在“上传”页面的右下角选择 **[!UICONTROL 作业选项]**. 在上传作业选项对话框中，展开eVideo选项，然后选择所需的视频编码预设。

>[!NOTE]
>
>除了默认启用的“自适应视频”之外，您在“上传作业选项”对话框中看不到所有其他自适应视频或单个视频编码预设。 Adobe Dynamic Media Classic管理员可确定在“上传作业选项”对话框中显示哪些视频编码预设。

* 从以下自适应视频编码预设或单个编码预设中进行选择：

   * **[!UICONTROL 16:9自适应视频]**  — 创建16:9宽高比视频，以将其交付到台式机、移动设备(iPhone、iPad、Android™)和平板电脑(iPad、Android™)，并使用与查看器的连接速度最匹配的分辨率和比特率进行优化。

   * **[!UICONTROL 4:3自适应视频]**  — 创建4:3宽高比视频，以交付到台式机、移动设备(iPhone、iPad、Android™)和平板电脑(iPad、Android™)，并使用与查看器连接速度最匹配的分辨率和比特率进行优化。

   * **[!UICONTROL 自适应视频]**  — 单个编码预设，可与任意宽高比配合使用，以创建视频以传送到移动设备、平板电脑和桌面。 使用该预设编码的上载的源视频将设置为固定高度。但是，自动调整宽度以保持视频的高宽比。

      默认情况下，在创建您自己的自定义视频编码预设时，也可以灵活地进行这种“自动缩放”。

      请参阅 [添加或编辑视频编码预设](uploading-encoding-videos.md#adding_or_editing_a_video_encoding_preset).

   * **[!UICONTROL 自适应视频编码（16:9或4:3）]**  — 创建16:9和4:3宽高比视频，以便交付到台式机、移动设备(iPhone、iPad、Android™)和平板电脑(iPad、Android™)。 所有这些都通过与查看器的连接速度最匹配的分辨率和比特率进行优化。

      请参阅[自适应视频编码（16:9 或 4:3）视频预设](application-setup.md#adaptive_video_encoding_16_9_or_4_3_video_presets)。

   * **[!UICONTROL 单个编码预设]**

      >[!NOTE]
      >
      >要将视频交付到iPad，您可以选择移动编码预设或平板电脑编码预设。 平板电脑预设专为 iPad 而设计，通常具有更高的分辨率和质量，以充分利用更大的屏幕尺寸和带宽连接。传送使用平板电脑预设编码的视频文件要求您在移动站点或应用程序上加入设备检测代码。此代码会根据播放设备在 iPhone 或 iPad 视频体验之间切换。更简单的工作流程是选择移动设备预设将视频文件传送到 iPad。原因在于您可以将同一视频文件用于 iPhone 和 iPad。但是，将质量标准化为分辨率更低的 iPhone 体验。

      * 在“编码预设”组下的“编码预设排序”下拉列表中，选择名称或大小来按名称或分辨率大小对预设进行排序。
      * 根据您计划播放视频的分辨率大小和带宽选择编码预设。
      * 您可以选择自适应视频编码，以及每个视频的一个或多个编码预设。 例如，您可以在一个上载作业中针对桌面和移动设备编码文件。

在选择 **[!UICONTROL 开始上传]**，则会上传原始主视频文件，并从主文件生成编码文件。

### 关于编码预设选项 {#about-encoding-preset-options}

编码预设选项的参数如下：

* **[!UICONTROL 目标连接速度]**  — 目标最终用户的Internet连接速度。

* **[!UICONTROL 编码文件后缀]**  — 附加到编码视频文件以用于标识的后缀。

* **[!UICONTROL 视频比特率（数据率）]**  — 编码为构成视频播放一秒的数据量（千比特/秒）。

* **[!UICONTROL 像素宽度/高度]**  — 屏幕图像的宽度尺寸（以像素为单位）；屏幕图像的高度尺寸（以像素为单位）。

* **[!UICONTROL 每秒帧数(fps)]**  — 每秒视频的帧数或静止图像数。 在美国和日本，大部分视频以 29.97 fps 拍摄；在欧洲和亚洲（不包括日本），大部分视频以 25 fps 拍摄。电影以 24 fps 拍摄。

* **[!UICONTROL 音频比特率]**  — 经过编码以构成一秒音频播放的数据量，以千比特/秒为单位。

下表显示了选择视频预设的建议最佳做法和用于指定编码文件的命名约定。

### 自适应视频（默认） {#adaptive-video-default}

这是一个适用于任何高宽比的编码预设，可用于创建传送到移动设备、平板电脑和台式机的视频。使用该新预设（默认和最佳做法）编码的上载的源视频将设置为固定高度，同时自动调整宽度以保持视频的高宽比。

**自适应视频（默认）**

|  | 编码预设名称/工具提示文本 | 编码文件后缀 | 视频数据速率 (Kbps) | 宽度/高度（像素） | Fps | 音频比特率 (kbps) | 推荐 |
|--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | Auto x360, 800 Kbps | _Mobile_Autox360p_800K | 800 | Autox360 | 与源相同 | 64 | 对于移动设备(iPhone、iPad、Android™) |
| 2 | Auto x 480, 1400 Kbps | _Tablet_Autox480p_1400K | 1400 | Autox480 | 与源相同 | 96 | 对于平板电脑(iPad、Android™) |
| 3 | Auto x 720, 2600 Kbps | _Desktop_Autox720p_2600K | 2600 | Autox720 | 与源相同 | 128 | 桌面版 |

### 自适应视频编码（16:9 或 4:3）视频预设 {#adaptive-video-encoding-or-video-presets}

这些自适应视频编码预设合并了一系列单独的编码预设，将根据上载的视频的高宽比自动为您选择这些预设。例如，如果您上传4:3视频，则会使用(位于 **自适应视频编码（16:9或4:3）** 选项。

有关编码选项参数的信息，请参阅[关于编码预设选项](application-setup.md#about_encoding_preset_options)。

**自适应视频编码（16:9 或 4:3）预设**

|  | 编码预设名称/工具提示文本 | 目标连接速度 (Kbps) | 编码文件后缀 | 视频数据速率 (Kbps) | 宽度/高度（像素） | Fps | 音频比特率 (kbps) | 推荐 |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | `16:9, 512x288, Mobile (iPhone, iPad, Android™), (400 Kbps)` | 500 | _Mobile_512x288_400K | 400 | 512x288 | 与源相同 | 64 | 低分辨率、3G |
| 2 | `4:3, 384x288px, Mobile (iPhone, iPad, Android™), (400 Kbps)` | 500 | _Mobile_384x288_400K | 400 | 384x288 | 与源相同 | 64 | 低分辨率、3G |
| 3 | `16:9, 512x288, Mobile (iPhone, iPad, Android™), (600 Kbps)` | 700 | _Mobile_512x288_600K | 600 | 512x288 | 与源相同 | 64 | 中分辨率、3G |
| 4 | `4:3, 384x288, Mobile (iPhone, iPad, Android™), (600 Kbps)` | 700 | _Mobile_384x288_600 | 600 | 384x288 | 与源相同 | 64 | 中分辨率、3G |
| 5 | `16:9, 640x360, Tablet (iPad, Android™), (800 Kbps)` | 900 | _iPad_640x360_800K | 800 | 640x360 | 与源相同 | 80 | 中分辨率、WiFi |
| 6 | `4:3, 640x480, Tablet (iPad, Android™), (800 Kbps)` | 900 | _iPad_640x480_800K | 800 | 640x480 | 与源相同 | 80 | 中分辨率、WiFi |
| 7 | `16:9, 768x432, Tablet (iPad, Android™), (1200 Kbps)` | 1.5 Mbps | _iPad_768x432_1200K | 1200 | 768 x 432 | 与源相同 | 96 | 高分辨率、WiFi |
| 8 | `4:3, 768x576, Tablet (iPad, Android™), (1200 Kbps)` | 1.5 Mbps | _iPad_768x576_1200K | 1200 | 768x576 | 与源相同 | 96 | 高分辨率、WiFi |
| 9 | `16:9, 1280x720, Desktop, (2000 Kbps)` | 3.0 Mbps | _1280x720_2000K | 2000 | 1280x720 | 与源相同 | 128 | 高清、宽屏 |
| 10 | `4:3, 1280x960, Desktop, (2000 Kbps)` | 3.0 Mbps | _1280x960_2000K | 2000 Kbps | 1280x960 | 与源相同 | 128 | 高清 |

### 台式机视频编码预设 {#desktop-video-encoding-presets}

台式机上的 MP4 和 OGV 视频编码预设。

有关编码选项参数的信息，请参阅[关于编码预设选项](application-setup.md#about_encoding_preset_options)。

**H264 Main 3.2 - 音频 AAC、MP4 文件扩展名**

|  | 编码预设名称/工具提示文本 | 目标连接速度 (Kbps) | 编码文件后缀 | 视频数据速率 (Kbps) | 宽度/高度（像素） | Fps | 音频比特率 (Kbps) | 推荐 |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | 16:9、480x270 (400 Kbps) | 500 | _480x270_400K | 400 | 480x270 | 与源相同 | 64 | 低宽屏分辨率 |
| 2 | 16:9、640x360 (800 Kbps) | 900 | _640x360_800K | 800 | 640x360 | 与源相同 | 80 | 中等宽屏分辨率 |
| 3 | 16:9、800x450 (1200 Kbps) | 1.5 Mbps | _800x450_1200K | 1200 | 800x450 | 与源相同 | 96 | 中高分辨率 |
| 4 | 16:9、1280x720 (2000 Kbps) | 3.0 Mbps | _1280x720_2000K | 2000年 | 1280x720 | 与源相同 | 128 | 高清、宽屏 |
| 5 | 4:3、320x240 (400 Kbps) | 500 | _320X240_400K | 400 | 320x240 | 与源相同 | 64 | 低分辨率 |
| 6 | 4:3、480x360 (800 Kbps) | 900 | _480x360_800K | 800 | 480x360 | 与源相同 | 80 | 中分辨率 |
| 7 | 4:3、640x480 (1200 Kbps) | 1.5 Mbps | _640x480_1200K | 1200 | 640x480 | 与源相同 | 96 | 中高分辨率 |
| 8 | 4:3、1280x960 (2000 Kbps) | 3.0 Mbps | _1280x960_2000K | 2000年 | 1280x960 | 与源相同 | 128 | 高清 |

**OGG Theora Vorbis - OGV 文件扩展名**

|  | 编码预设名称/工具提示文本 | 目标连接速度 (Kbps) | 编码文件后缀 | 视频数据速率 (Kbps) | 宽度/高度（像素） | Fps | 音频比特率 (Kbps) | 推荐 |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | 16:9、480x270 (400 Kbps)、OGG | 500 | _OGG_480x270_400K | 400 | 480x270 | 与源相同 | 64 | 低宽屏分辨率 |
| 2 | 16:9、640x360 (800 Kbps)、OGG | 900 | _OGG_640x360_800K | 800 | 640x360 | 与源相同 | 80 | 中等宽屏分辨率 |
| 3 | 16:9、800x450 (1200 Kbps)、OGG | 1.5 Mbps | _OGG_800x450_1200K | 1200 | 800x450 | 与源相同 | 96 | 中高分辨率 |
| 4 | 16:9、1280x720 (2000 Kbps)、OGG | 3.0 Mbps | _OGG_1280x720_2000K | 2000年 | 1280x720 | 与源相同 | 128 | 高清、宽屏 |
| 5 | 4:3、320x240 (400 Kbps)、OGG | 500 | _OGG_320X240_400K | 400 | 320x240 | 与源相同 | 64 | 低分辨率 |
| 6 | 4:3、480x360 (800 Kbps)、OGG | 900 | _OGG_480x360_800K | 800 | 480x360 | 与源相同 | 80 | 中分辨率 |
| 7 | 4:3、640x480 (1200 Kbps)、OGG | 1.5 Mbps | _OGG_640x480_1200K | 1200 | 640x480 | 与源相同 | 96 | 中高分辨率 |
| 8 | 4:3、1280x960 (2000 Kbps)、OGG | 3.0 Mbps | _OGG_1280x960_2000K | 2000年 | 1280x960 | 与源相同 | 128 | 高清 |

### 移动设备视频编码预设 {#mobile-video-encoding-presets}

与源 fps 相同。iPhone、iPad和Android™移动设备的视频编码预设。

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
>**Flash查看器生命周期终止通知**  — 自2017年1月31日起，Adobe Dynamic Media Classic正式停止对Flash查看器平台的支持。

*查看器预设*&#x200B;是一组设置，决定了用户如何在其计算机屏幕和移动设备上查看富媒体资源。作为管理员，您可以创建查看器预设。提供适用于一系列查看器配置选项的设置。例如，您可以更改查看器显示尺寸、缩放行为、颜色方案、边框和字体。

最佳做法是使用Adobe Dynamic Media Classic HTML5视频查看器。 HTML5 视频查看器中使用的预设是功能强大的视频播放器。

通过将以下内容组合到单个播放器中：

* 使用HTML5和CSS设计播放组件的功能。
* 已嵌入播放。
* 根据浏览器的功能使用自适应流和渐进式流。

您可以将富媒体内容的访问范围扩展到桌面、平板电脑和移动设备用户，并确保简化视频体验。

请参阅 [关于HTML5查看器](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/library/viewers-for-aem-assets-only/c-html5-aem-asset-viewers.html?lang=en#viewers-for-aem-assets-only) (在《Adobe查看器参考指南》中)。

请参阅 [Adobe Dynamic Media Classic查看器预设兼容性矩阵](application-setup.md#scene7_viewer_preset_compatibility_matrix).

请参阅[最佳做法：使用 HTML5 视频查看器](best-practice-using-html5-video.md#best_practice_using_the_html5_video_viewer)。

您可以根据查看器添加社区功能。社区功能包括“嵌入”按钮、“电子邮件”按钮、“链接”按钮和“访问站点”按钮。通过这些按钮，使用查看器的用户可以与他人共享查看器或打开Adobe Dynamic Media Classic网站。

另请参阅 [Adobe查看器参考库示例](https://landing.adobe.com/zh-Hans/na/dynamic-media/ctir-2755/live-demos.html).

### 查看器支持响应式设计的网页 {#viewer-support-for-responsive-designed-web-pages}

不同的网页具有不同的需求。有时，您希望网页提供一个链接，以在单独的浏览器窗口中打开HTML5查看器。 在其他情况下，需要直接将HTML5查看器嵌入到托管页面。 在后一种情况下，网页可能具有静态布局。 或者，它是“响应式”的，并在不同设备上或针对不同浏览器窗口大小显示不同。 为了满足这些需求，Adobe Dynamic Media Classic附带的HTML5查看器支持静态网页和响应式设计的网页。

有关如何将响应式查看器嵌入网页的更多信息，请参阅 [关于响应式图像库](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/responsive-static-image-library/c-about-responsive-static-image-library.html#image-serving-api), [使用响应式图像库](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/responsive-static-image-library/t-using-responsive-static-image-library.html#image-serving-api)和 [命令引用 — 命令属性](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/responsive-static-image-library/t-using-responsive-static-image-library.html#responsive-static-image-library).

### 查看器预设类型 {#viewer-preset-types}

管理员可以创建和自定义以下类型的查看器预设：

* **[!UICONTROL eCatalog查看器]**  — 模拟阅读打印目录的体验。 您可以在页面之间移动、放大和缩小页面上的项目、使用图像映射查看有关页面上项目的更多信息或搜索目录。 还可以包括“信息面板”，在映射区域具有有效的 rollover_key 属性时显示详细信息和图像映射的物品。要包括“信息面板”，请在“eCatalog 查看器预设”窗口的“信息面板设置”面板中指定“信息服务器 URL”。

* **[!UICONTROL 样本集查看器]**  — 以不同的颜色、材料、纹理、外观或结构显示图像。 用户选择缩略图可查看图像中的变体。

* **[!UICONTROL 混合媒体集查看器]**  — 在一个查看器中显示不同类型的媒体。 您可以包括样本集、旋转集、图像和视频。您可以设置各个选项卡，以包含不同类型的内容，例如，一个选项卡用于图像集、一个选项卡用于视频。从混合媒体集播放的视频使用具有时间线和视频控件（如停止、暂停、回放和播放）的标准视频查看器。您设置混合媒体集查看器预设时，指定要将哪些查看器用于“混合媒体集”中的不同类型的资源。您还可以使用“网格查看器”或“轮盘式查看器”来查看混合媒体集。

* **[!UICONTROL 旋转集查看器]**  — 提供图像的多个视图，以便用户可以旋转对象以检查不同的侧边和角度。

* **视频查看器**  — 使用源文件的分辨率尺寸或自定义大小显示视频。 Adobe Dynamic Media Classic附带了许多用于播放视频的预定义查看器预设，如果您是管理员，则可以创建自定义视频查看器预设。 有12个以上不同的设置用于配置视频查看器。 您可以配置其大小、前景和背景颜色、视频和音频控件、进度条、用户界面外观、社交功能和“帮助”。

* **[!UICONTROL 缩放查看器]**  — 提供三种类型的缩放查看器选项：

* **[!UICONTROL 缩放查看器]**  — 允许用户通过选择区域来放大区域。 他们可以选择用于放大、缩小图像并将图像重置为默认大小的控件。

* **[!UICONTROL 缩放查看器：飞出]**  — 在原始图像旁边显示缩放区域的第二个图像。 没有控件可以使用，用户只需将选取范围移动到他们要查看的区域上即可。

在确定此查看器的完整带宽使用量时，请考虑在查看器中有主图像和弹出图像。主图像大小（舞台宽度和高度）和缩放系数决定了弹出图像大小。为防止弹出文件大小变得太大，需对这两个值进行平衡：如果您的主图像大小很大，请降低缩放系数值。（弹出宽度和弹出高度决定了弹出窗口的大小，但不决定提供给查看器的弹出图像的大小。）

例如，如果您的主图像大小是 350 X 350 像素，缩放系数为 3，则生成的弹出图像是 1050 X 1050 像素。如果您的主图像大小是 300 X 300 像素，缩放系数为 4，则弹出图像是 1200 X 1200 像素。根据 JPEG 品质设置（推荐的设置介于 80-90），您可以显著地减少文件大小。建议的缩放系数为 2.5 至 4，取决于您的主图像的大小。

### Adobe Dynamic Media Classic查看器预设兼容性矩阵 {#scene-viewer-preset-compatibility-matrix}

**Flash查看器生命周期终止通知**:自2017年1月31日起，Adobe Dynamic Media Classic正式停止对Flash查看器平台的支持。

下表标识了当前可用的Adobe Dynamic Media Classic查看器预设。 该表还指定了查看器与桌面和移动设备的兼容性，以及对每个指定查看器使用的技术。

另请参阅 [Adobe查看器参考库示例](https://landing.adobe.com/en/na/dynamic-media/ctir-2755/live-demos.html).

有关查看器支持的 Web 浏览器和操作系统版本的信息，您可以查阅查看器发行说明。

请参阅 [Adobe查看器参考发行说明](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources.html).

|  | 查看器技术 | 桌面 | Apple iPhone | Apple iPad | Android™智能手机 | Android™平板电脑 |
|--- |--- |--- |--- |--- |--- |--- |
| 缩放查看器 |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML5 | X | X | X | X | X |
| Universal_HTML5_Zoom_inline | HTML5 | X | X | X | X | X |
| Universal_HTML5_Zoom_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_Zoom_light | HTML5 | X | X | X | X | X |


|  | 查看器技术 | 桌面 | AppleiPhone | AppleiPad | Android™智能手机 | Android™平板电脑 |
|--- |--- |--- |--- |--- |--- |--- |
| 图像集查看器 |  |  |  |  |  |  |
| Universal_HTML5_弹出 | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_light | HTML5 | X | X | X | X | X |

|  | 查看器技术 | 桌面 | AppleiPhone | AppleiPad | Android™智能手机 | Android™平板电脑 |
|--- |--- |--- |--- |--- |--- |--- |
| 样本集查看器 |  |  |  |  |  |  |
| Universal_HTML5_弹出 | HTML5 | X | X | X | X | X |
| Universal_HTML5_SwatchSet_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_SwatchSet_light | HTML5 | X | X | X | X | X |

|  | 查看器技术 | 桌面 | AppleiPhone | AppleiPad | Android™智能手机 | Android™平板电脑 |
|--- |--- |--- |--- |--- |--- |--- |
| eCatalog 查看器 |  |  |  |  |  |  |
| Universal_HTML5_eCatalog_Adv（包括对社交媒体和目录搜索的支持。） | HTML5 | X | X | X | X | X |
| Universal_HTML5_eCatalog（包括对社交媒体和目录搜索的支持。） | HTML5 | X | X | X | X | X |

|  | 查看器技术 | 桌面 | AppleiPhone | AppleiPad | Android™智能手机 | Android™平板电脑 |
|--- |--- |--- |--- |--- |--- |--- |
| 旋转查看器 |  |  |  |  |  |  |
| Universal_HTML5_SpinSet_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_SpinSet_light | HTML5 | X | X | X | X | X |

**eVideo 查看器**

Adobe Dynamic Media Classic支持为MP4 H.264视频播放移动设备视频。

* 您可以在以下位置找到支持此视频格式的BlackBerry®设备： [BlackBerry®上支持的视频格式](https://developers.blackberry.com/us/en)
* 您还可以在以下位置找到支持此视频格式的Windows®设备： [Windows® Phone上支持的视频格式](https://docs.microsoft.com/en-us/windows/uwp/audio-video-camera/supported-codecs)

|  | 查看器技术 | 桌面 | AppleiPhone | AppleiPad | Android™智能手机 | Android™平板电脑 | BlackBerry® Smartphone | Windows® Phone |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| Universal_HTML5_Video（包括对隐藏式字幕的支持。） 请参阅 [最佳实践：使用通用HTML5视频查看器。](best-practice-using-html5-video.md#best_practice_using_the_html5_video_viewer) | HTML5 | X | X | X | X | X | X | X |
| Universal_HTML5_Video_social（包括对隐藏式字幕和社交媒体的支持。） | HTML5 | X | X | X | X | X | X | X |

|  | 查看器技术 | 桌面 | AppleiPhone | AppleiPad | Android™智能手机 | Android™平板电脑 |
|--- |--- |--- |--- |--- |--- |--- |
| 混合媒体集查看器 |  |  |  |  |  |  |
| Universal_HTML5_MixedMedia_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_MixedMedia_light | HTML5 | X | X | X | X | X |

### 支持的移动查看器手势表格 {#supported-mobile-viewers-gestures-matrix}

下表标识了iOS、Android™ 2.x和Android™ 3.x设备上支持的移动查看器手势。

|  | 查看器技术 | 桌面 | AppleiPhone | AppleiPad | Android™智能手机 | Android™平板电脑 |
|--- |--- |--- |--- |--- |--- |--- |
| 图像集查看器 |  |  |  |  |  |  |
| Universal_HTML5_弹出 | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_light | HTML5 | X | X | X | X | X |

### 关于“查看者预设”屏幕 {#about-the-viewer-preset-screen}

在“查看器预设”屏幕上创建和管理“查看器预设”。要打开此屏幕，请转到 **[!UICONTROL 设置]** > **[!UICONTROL 查看器预设]**.

“查看器预设”屏幕提供了用于执行以下任务的工具：

* **添加预设**  — 选择 **[!UICONTROL 添加]** 和，在“添加查看器预设”对话框中进行选择。

       请参阅[添加和编辑查看器预设](application-setup.md#adding_and_editing_viewer_presets)。
   
* **编辑预设**  — 选择预设，然后选择 **[!UICONTROL 编辑]**.

       请参阅[添加和编辑查看器预设](application-setup.md#adding_and_editing_viewer_presets)。
   
* **删除预设**  — 选择预设，然后选择 **[!UICONTROL 删除]**.

* **导出预设**  — 选择HTML5查看器预设，然后选择 **[!UICONTROL 导出]** 以下载查看器外观，以便您可以将其用作创建和添加其他查看器预设的基础。

       请参阅[导出HTML5查看器预设](application-setup.md#exporting_an_html5_viewer_preset)。
   
* **过滤查看器预设列表**  — 使用这些工具过滤列表：

       *打开**活动/不活动**下拉列表，然后选择一个选项以显示活动预设、不活动预设或所有预设。
       *打开**查看器**下拉列表，然后选择一个选项以仅查看特定类型的查看器。 选择**[!UICONTROL 所有查看器]**查看所有查看器。
   
* **排序预设**  — 选择列标题(**[!UICONTROL 活动]**, **[!UICONTROL 类型]**, **[!UICONTROL 预设]**&#x200B;或 **[!UICONTROL 平台]**)来对列的列表进行排序。 再次选择列标题，以按降序（或升序）对列表进行排序。

* **激活和停用预设**  — 选择一个预设，然后选择其“活动”选项以激活或取消激活该预设。

       请参阅[激活或停用查看器预设](application-setup.md#activating_or_deactivating_viewer_presets)。
   
>[!NOTE]
>
>选择 **[!UICONTROL 预览]** 在“查看器预设”页面的右侧，您可以查看您选择的查看器预设中资产的外观。 要查看其他资产，请选择 **[!UICONTROL 浏览]** 在“查看器预设”页面中，并在“选择资产预览”对话框中选择其他资产。

### 添加和编辑查看器预设 {#adding-and-editing-viewer-presets}

除了使用 **[!UICONTROL 添加]** 在用户界面中，您还可以使用 **[!UICONTROL 导出]** 添加查看器预设。 您只需导出现有的HTML5查看器预设，然后将其用作新预设的基础。

请参阅 [导出HTML5查看器预设](application-setup.md#exporting_an_html5_viewer_preset).

另请参阅 [查看器预设](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/550_viewer-presets_converted%20renamed_Done-AVS) 培训视频。

**添加和编辑查看器预设:**

1. 在Adobe Dynamic Media Classic的右上角附近，转到 **[!UICONTROL 设置]** > **[!UICONTROL 查看器预设]**.

   您可以过滤预设列表。例如，要仅查看视频查看器的预设，请从表正上方的工具栏上的“查看器”下拉列表中选择“视频查看器”。

1. 在“查看器预设”页面中，在“查看器预设”屏幕上添加或编辑查看器预设。

   * **添加**  — 在工具栏中，选择 **[!UICONTROL 添加]**. 在添加查看器预设对话框中，选择一个平台，然后选择富媒体资产类型。

          选择**[!UICONTROL 另存为]**查看器预设创建完成后。
      
   * **从现有查看器预设开始添加**  — 在表中，选择视频查看器预设，然后选择 **[!UICONTROL 编辑]** 中。

          重新配置视频查看器后，选择**[!UICONTROL 另存为]**以在“预设名称”文本字段中使用其他名称保存预设。
      
   * **编辑**  — 选择现有的查看器预设，然后选择 **[!UICONTROL 编辑]**.

1. 在配置查看器屏幕的预设名称字段中，输入或编辑预设名称。
1. 设置其余所需的选项。

   >[!NOTE]
   >
   >选择 **[!UICONTROL 与源相同]** 以自动将视频查看器的大小调整为编码视频本身的分辨率大小。 如果选择此选项，则无法输入阶段宽度和阶段高度。 相反，这些选项来自视频自身。如果您选择 **[!UICONTROL 与源相同]**，设置边距大小选项以反映视频播放区域外的外观尺寸。 该边距大小是视频控件的像素高度和宽度。您可以使用下图来帮助确定要使用的边距大小。*

   ![视频查看器的边距配置](assets/vs_video_viewer_configure_margin.png)

1. 执行以下任一操作：

   * 选择 **[!UICONTROL 另存为]** 是否从现有预设开始添加查看器预设。
   * 选择 **[!UICONTROL 保存]** 如果添加或编辑了查看器预设，请执行以下操作：

### 导出HTML5查看器预设 {#exporting-an-html-viewer-preset}

您可以导出现有的HTML5查看器预设，以用作创建HTML5查看器预设的基础。 该导出选项很有用，因为您不必从头开始创建查看器。相反，您会导出外观和行为与所需预设接近的预设，然后以此为基础开始进行设计调整。

Adobe Dynamic Media Classic中所有默认的现成查看器预设CSS文件都使用指向上资产的相对图像提供路径 `Scene7SharedAssets`. 例如，以下是查看器预设CSS文件中图像资产的相对路径，位于

`Scene7SharedAsset`: `.s7videoviewer .s7fullscreenbutton[state][selected] { background-image: url(/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha); }`

但是，如果您在自己的网站上托管查看器CSS文件，则必须通过在自己的环境中使用指向图像服务器的显式路径来解析这些相对图像路径。 例如，如果要将上面的相对路径更新为显式路径，则可能如下所示，其中 `https://s7d1.scene7.com` 是图像服务器的直接路径： `https://s7d1.scene7.com/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha`

**要导出HTML5查看器预设，请执行以下操作：**

```as3
.s7videoviewer .s7fullscreenbutton[state][selected] 
{ background-image: url(/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha); }
```

```as3
https://s7d1.scene7.com/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha
```

1. 转到 **[!UICONTROL 设置]** > **[!UICONTROL 查看器预设]**.
1. 在“查看器预设”工具栏的左侧第二个下拉列表中，选择 **[!UICONTROL HTML5]**.
1. 在左边的第三个下拉列表中，选择“**[!UICONTROL 所有查看器]**”。
1. 选择要用作新查看器预设基础的查看器HTML5查看器预设。
1. 在工具栏中，选择 **[!UICONTROL 导出]**.
1. 在导出选定的资产对话框中，选择 **[!UICONTROL 提交导出]**.

   导出后，您将获取CSS文件。 下载并解压缩此文件。

1. 在 CSS 编辑器中打开 CSS 文件，进行更改，然后保存该文件。
1. 将CSS文件上传到Adobe Dynamic Media Classic。

   请参阅 [上传文件](uploading-files.md#uploading_files).

1. 将CSS文件发布到Dynamic Media图像服务器。

   请参阅 [发布文件](publishing-files.md#publishing_files).

1. 照常添加新的查看器预设。选择您上传的查看器CSS文件。

   请参阅 [添加和编辑查看器预设](application-setup.md#adding_and_editing_viewer_presets).

### 激活或停用查看器预设 {#activating-or-deactivating-viewer-presets}

要创建用于显示资产的URL，用户需在“预览”对话框中打开“预设”下拉列表，选择查看器预设，然后选择 **[!UICONTROL 复制URL]** (请参阅 [复制查看器预设的URL](application-setup.md#copying_the_url_of_a_viewer_preset))。 此“预设”列表提供了管理员在“查看器预设”屏幕上添加和管理的“查看器预设”。例如，在用户预览 eCatalog 时，所有活动的 eCatalog 查看器预设都显示在“预览”对话框的“预设”下拉列表上。

除非您在“查看器预设”屏幕上停用查看器预设，否则“预览”对话框的“预设”下拉列表可能变得内容越来越多。

**激活或停用查看器预设:**

1. 转到 **[!UICONTROL 设置]** > **[!UICONTROL 查看器预设]**.
1. 在“查看器预设”页面上，选择或取消选择 **[!UICONTROL 活动]** 用于激活或取消激活查看器预设的选项。

### 复制查看器预设的URL {#copying-the-url-of-a-viewer-preset}

发布资源后，您可以复制以查看器预设的设置显示资源的 URL。

URL 即复制到剪贴板中。您可以根据需要在网页的 HTML 代码、移动设备或应用程序中使用它。

**复制查看器预设的 URL:**

1. 在“浏览”面板中选择资源。
1. 在“资源浏览”面板上方的工具栏右侧，执行以下任一操作：

   * 选择 **[!UICONTROL 网格视图]**. 在“资源浏览”面板中，双击单个资源以便在详细信息视图中将其打开。在右侧的URL和嵌入代码面板中，选择 **[!UICONTROL 复制URL]** 查看者的右侧。
   * 选择 **[!UICONTROL 网格视图]**. 在资产浏览面板中，选择一个资产，然后在缩略图图像下方，转到 **[!UICONTROL 预览]** > **[!UICONTROL 查看器列表]**.

   在“查看器列表”页面的表的“操作”列下，选择 **[!UICONTROL 复制URL]**.

   * 选择 **[!UICONTROL 列表视图]**. 在资产浏览面板中，选择一个资产，然后在缩略图图像的右侧，转到 **[!UICONTROL 预览]** > **[!UICONTROL 查看器列表]**.
   在“查看器列表”页面的表的“操作”列下，选择 **[!UICONTROL 复制URL]**.

   * 选择 **[!UICONTROL 网格视图]**, **[!UICONTROL 列表视图]**&#x200B;或 **[!UICONTROL 详细信息视图]**. 在同一工具栏上，转到 **[!UICONTROL 预览]** > **[!UICONTROL 查看器列表]**.
   在“查看器列表”页面的表的“操作”列下，选择 **[!UICONTROL 复制URL]**.

### 复制查看器预设的嵌入代码 {#copying-the-embed-code-of-a-viewer-preset}

使用嵌入代码功能，您可以查看用于所选查看器预设的查看器代码。您也可以将代码复制到剪贴板中，以便可以将其粘贴到网页中以部署查看器。

不允许在“嵌入代码”对 话框中编辑代码 。

**复制查看器预设的嵌入代码:**

1. 在“资源浏览”面板中选择资源。
1. 在“资源浏览”面板上方的工具栏右侧，执行以下任一操作：

   * 选择 **[!UICONTROL 网格视图]**. 在“资源浏览”面板中，双击单个资源以便在详细信息视图中将其打开。在右侧的URL面板中，选择 **[!UICONTROL 嵌入代码]**.
   * 选择 **[!UICONTROL 网格视图]**. 在资产浏览面板中，选择一个资产，然后在缩略图图像下方，转到 **[!UICONTROL 预览]** > **[!UICONTROL 查看器列表]**.

   在“查看器列表”页面的表的“操作”列下，选择 **[!UICONTROL 嵌入代码]**.

   * 选择 **[!UICONTROL 列表视图]**. 在资产浏览面板中，选择一个资产，然后在缩略图图像的右侧，转到 **[!UICONTROL 预览]** > **[!UICONTROL 查看器列表]**.
   在“查看器列表”页面的表的“操作”列下，选择 **[!UICONTROL 嵌入代码]**.

   * 选择 **[!UICONTROL 网格视图]**, **[!UICONTROL 列表视图]**&#x200B;或 **[!UICONTROL 详细信息视图]**. 在同一工具栏上，转到 **[!UICONTROL 预览]** > **[!UICONTROL 查看器列表]**.
   在“查看器列表”页面的表的“操作”列下，选择 **[!UICONTROL 嵌入代码]**.

1. 在“嵌入代码”对话框中，选择 **[!UICONTROL 复制到剪贴板]**.
1. 选择 **[!UICONTROL 关闭]**.

## 配置默认查看器 {#configuring-default-viewers}

在Adobe Dynamic Media Classic中使用预览时，您可以使用默认查看器配置与资产关联的默认查看器。 您可以为下列资源类型设置默认预览体验：

* 图像
* 视频
* 旋转集
* 目录
* 图像集
* 样本集
* 媒体集

**配置默认查看器:**

1. 在设置下拉列表中，选择 **[!UICONTROL 应用程序设置]**.
1. 在“设置”窗口的左窗格中，转到 **[!UICONTROL 应用程序设置]** > **[!UICONTROL 查看器]**
1. 选择 **[!UICONTROL 默认查看器]**.
1. 在“默认查看器”窗口中，在每种资源类型的下拉列表中，选择要与该资源的预览关联的查看器。
1. 在“默认查看器”窗口的右下角，选择 **[!UICONTROL 保存设置]**.
1. 在“设置”窗口的右下角，选择 **[!UICONTROL 关闭]** 返回“资产”窗口。

## 元数据视图 {#metadata-views}

*元数据*&#x200B;是关于资源的标准化信息。您可以使用元数据来简化工作流程、组织资源和改进搜索。Adobe Dynamic Media Classic支持IPTC（国际新闻电信理事会）标准和XMP（可扩展元数据平台）标准。 在用户在详细信息视图中查看或输入有关资产的元数据之前，他们可以打开元数据视图菜单。 从中，他们可以选择要查看或用于描述资产的元数据字段集。

Adobe Dynamic Media Classic提供了预定义的元数据视图，管理员可以创建自己的元数据视图，供用户在输入元数据时进行选择。

### 创建元数据视图 {#creating-a-metadata-view}

1. 转到 **[!UICONTROL 设置]** > **[!UICONTROL 应用程序设置]** > **[!UICONTROL 元数据]** > **[!UICONTROL 元数据视图]**.
1. 选择 **[!UICONTROL 添加]**.
1. 在预设名称文本字段中，输入视图的名称。
1. （可选）检查 **[!UICONTROL 设为默认值]** 使此视图成为用户在详细信息视图中打开元数据面板时看到的视图。
1. （可选）选择 **[!UICONTROL 包括UDF]** ，以在视图中包含用户定义的字段。 用户定义的字段显示在详细信息视图的“元数据”面板的顶部。
1. 选择您希望查看的字段(选择 **[!UICONTROL 全选]** 选择所有字段)。
1. 选择 **[!UICONTROL 保存]**.

   视图的选定类别和字段显示在“预览”面板中。

### 管理元数据视图 {#managing-metadata-views}

1. 转到 **[!UICONTROL 设置]** > **[!UICONTROL 应用程序设置]** > **[!UICONTROL 元数据]** > **[!UICONTROL 元数据视图]**.
1. 执行以下任一操作：

   * 要预览视图，请将其选中。视图中的字段将显示在“预览”面板中。
   * 要编辑视图，请选择它，然后选择 **[!UICONTROL 编辑]**. 然后，在“预览”面板上选择或取消选择字段名称，然后选择或取消选择 **[!UICONTROL 包括UDF]** 选项。
   * 要删除视图，请选择它，然后选择 **[!UICONTROL 删除]**.
   * 要使视图成为默认视图，请选择它，然后选择 **[!UICONTROL 设为默认值]**. 默认视图是用户在详细信息视图中打开资产并转到元数据面板时看到的视图。

## 元数据预设 {#metadata-presets}

元数据预设为管理员提供了控制和调整分配给资源的元数据的一种方式。在详细信息视图中，用户可以在为此目的而提供的字段中输入有关资产的元数据。 例如，用户可以输入所有者名称、版权说明和地址。为确保用户准确、完整地输入此信息，您可以创建元数据预设。 在详细信息视图中选择元数据预设会使用预定义的值填充元数据字段。 例如，会自动输入所有者名称、版权说明和地址。

为您希望用户能够在详细信息视图中自动输入以描述资产的每组元数据值创建元数据预设。

### 创建或编辑元数据预设 {#creating-or-editing-a-metadata-preset}

1. 转到 **[!UICONTROL 设置]** > **[!UICONTROL 应用程序设置]** > **[!UICONTROL 元数据]** > **[!UICONTROL 元数据预设]**.
1. 在“元数据预设”屏幕中，执行以下任一操作：

   * 要创建预设，请选择 **[!UICONTROL 添加]**. 在元数据模板名称文本字段中，键入预设的名称。 选择 **[!UICONTROL 元数据视图]**，然后从下拉列表中选择一个视图(请参阅 [元数据视图](application-setup.md#metadata_views))。
   * 要编辑现有预设，请从元数据预设列表中选择该预设，然后选择 **[!UICONTROL 编辑]**.

1. 展开要包含在预设中的标题，然后在要包含在预设中的不同字段中输入值。
1. 选择 **[!UICONTROL 保存]**.

   预设的所选类别和字段将显示在“预览”面板中。

### 管理元数据预设 {#managing-metadata-presets}

1. 转到 **[!UICONTROL 设置]** > **[!UICONTROL 应用程序设置]** > **[!UICONTROL 元数据]** > **[!UICONTROL 元数据预设]**.
1. 执行以下任一操作：

   * 要预览预设，请选择您要预览的预设。预设信息（类别和字段）将显示在“预览”屏幕中。
   * 要删除预设，请选择预设，然后选择 **[!UICONTROL 删除]**.

## 用户定义的字段 {#user-defined-fields}

Media Portal 管理员或公司管理员可以创建自定义的、用户定义的元数据字段。自定义字段可帮助您组织Adobe Dynamic Media Classic中的资产。 您可以根据需要将字段标记为活动。 激活后，这些自定义元数据字段的名称会显示在详细信息视图的“元数据”面板中。 用户可以在用户定义的元数据字段中输入信息以描述资源。用户也可以使用户定义的元数据字段成为搜索条件。

高效使用用户定义的元数据字段的一种方式是为特定启动或销售延迟资源的激活时间。您可以根据类型定义“激活”字段 *日期*. 然后，使用 **[!UICONTROL 元数据]** 面板，或者 **[!UICONTROL 文件]** > **[!UICONTROL 编辑信息]**，您可以指定资产的激活时间。 Adobe Dynamic Media Classic会检查资产的发布状态和发布历史记录。 如果未在激活时间内，则发布状态将显示为“未发布”。

>[!NOTE]
>
>要使用户定义的字段显示在详细信息视图的元数据面板中，请在元数据视图中包含用户定义的字段。 在“元数据视图”屏幕上，选择“包括 UDF”（用户定义的字段）选项。有关更多信息，请参阅[元数据视图](application-setup.md#metadata_views)。

>[!NOTE]
>
>要使用用户定义的自定义字段搜索资产，请转到 **[!UICONTROL 设置]** > **[!UICONTROL 个人设置]**，然后选择 **[!UICONTROL 在搜索中包含UDF]**. 请参阅[个人设置](personal-setup.md#personal_setup)。

### 创建用户定义的元数据字段 {#creating-a-user-defined-metadata-field}

1. 转到 **[!UICONTROL 设置]** > **[!UICONTROL 应用程序设置]** > **[!UICONTROL 元数据]** > **[!UICONTROL 用户定义的字段]**.
1. 选择 **[!UICONTROL 添加]**
1. 在“自定义字段”对话框中，设置所需的选项。

   * **[!UICONTROL 名称]**  — 输入元数据字段的名称。

   * **[!UICONTROL 类型]**  — 选择一个选项，用于定义用户可在元数据字段中输入的信息类型：

   * **[!UICONTROL 字符串]**  — 文本字符串。

   * **[!UICONTROL 整数]**  — 整数。

   * **[!UICONTROL 浮动]**  — 浮点数。

   * **[!UICONTROL 是/否]**  — 是/否布尔值。

   * **[!UICONTROL 日期]**  — 日期。 接受 MM/DD/YYYY 格式。

   * **[!UICONTROL 文件名]**  — 文件的名称。

   * **[!UICONTROL 颜色]**  — 颜色的名称。

   * **[!UICONTROL Dimension]**  — 资产的宽度和高度。

   * **[!UICONTROL 未键入]**  — 用于向后兼容性。 请勿选择此选项。

   * **[!UICONTROL 默认值]**  — （可选）在字段中输入用户最可能输入的值。 您输入的值会成为您所创建的字段的默认值。

   * **[!UICONTROL 适用于]**  — （可选）如果您希望元数据字段仅应用于特定类型的资产，请选择资产类型。

      >[!NOTE]
      >
      >选择 **[!UICONTROL 适用于]** 选项，因为您无法更改 **[!UICONTROL 适用于]** 选项。 Adobe Dynamic Media Classic允许您编辑用户定义的字段的名称、类型和默认值，但不能编辑 **[!UICONTROL 适用于]** 设置。*

1. 选择 **[!UICONTROL 保存]** 完成元数据字段的创建时。

### 管理用户定义的字段 {#manage-user-defined-fields}

“用户定义的字段”屏幕提供了用于管理自定义、用户定义的元数据字段的命令。

只有 Media Portal 管理员或公司管理员可以管理用户定义的字段。

要打开此屏幕，请转到 **[!UICONTROL 设置]** > **[!UICONTROL 应用程序设置]** > **[!UICONTROL 元数据]** > **[!UICONTROL 用户定义的字段]**.

* **编辑字段**  — 选择字段，然后选择 **[!UICONTROL 编辑]**.

* **删除字段**  — 选择字段，然后选择 **[!UICONTROL 删除]**.

* **激活字段**  — 选择或取消选择 **[!UICONTROL 活动]** 选项。 如果您具有公司管理角色，则不会显示此选项。 由于此选项与MediaPortal相关，因此您必须选择（打开）在个人设置中显示MediaPortal功能，才能查看激活字段。

## 优化文件 {#optimize-files}

将文件上传到Adobe Dynamic Media Classic时，系统会优化这些文件以进行存储和发布。 然而，如果上载过程中断，则无法优化某些图像。在这种情况下，您会看到“尚未优化图像”消息。然而，如果您是管理员，则可以优化这些文件。

Adobe Dynamic Media Classic会搜索您的文件，并仅优化之前未完全优化的图像。

1. 转到 **[!UICONTROL 设置]** > **[!UICONTROL 应用程序设置]**，然后选择 **[!UICONTROL 优化文件]**.
1. 输入优化作业的信息并选择 **[!UICONTROL 提交]**.

   如果您在与多家公司协作，请分别优化属于不同公司的文件。

## 批量集预设 {#batch-set-presets}

运行作业时，使用批集预设自动创建图像集或旋转集，以将资产上传到Adobe Dynamic Media Classic。

公司管理员首先为要在规则集中分组的资产定义命名约定。 然后，您可以创建批集预设以引用这些图像。 每个预设都是单独命名的、自成体系的指令集，指令集可定义如何使用与预设方法中定义的命名约定匹配的图像构建集。

“上载作业选项”对话框会列出公司的所有活动批量集预设，以便您指定要在每个上载会话期间应用的预设。公司管理员将看到所有活动和非活动的批量集预设。上传文件时，Adobe Dynamic Media Classic会自动创建一个文件集，其中包含与活动预设中定义的命名约定相匹配的所有文件。

### 默认命名 {#default-naming}

公司管理员创建在任何批量集预设方法中使用的默认命名约定。在批量集预设定义中选择的默认命名约定可能是贵公司为所有网站批量生成集所需的全部命名约定。 要使用您定义的默认命名约定，需创建批量集预设。如果公司定义的默认命名有例外情况，您可以为一组特定内容根据需要使用备用的自定义命名规则创建任意数量的批量集预设。

使用批量集预设功能时，不需要设置默认的命名约定。 但是，Adobe最佳实践建议您使用默认的命名约定来定义要分组到一组中的命名约定的任意多个元素。 这样做有助于简化批集创建过程。

1. 转到 **[!UICONTROL 设置]** > **[!UICONTROL 应用程序设置]** > **[!UICONTROL 批集预设]** > **[!UICONTROL 默认命名]**.
1. 选择&#x200B;**[!UICONTROL 查看表单]**&#x200B;或&#x200B;**[!UICONTROL 查看代码]**，以指定要查看的方式并输入有关每个元素的信息。

   您可以选择 **[!UICONTROL 查看代码]** 复选框，以查看生成的正则表达式值与表单选项的旁边。 如果表单视图因某种原因对您构成限制，您可以输入或更改上述值，以帮助定义命名约定的元素。如果无法在表单视图中分析您的值，则表单字段将变为不活动。

   >[!NOTE]
   >
   >停用的表单字段并不表示正则表达式无效。没有针对正则表达式正确性的验证措施。您会在“结果”行的后面看到您为每个元素构建的正则表达式的结果。完整的正则表达式显示在页面底部。

1. 根据需要展开每个元素，并输入您要使用的命名约定。
1. 根据需要，选择 **[!UICONTROL 添加]** 为元素添加其他命名约定。 或者，选择 **[!UICONTROL 删除]** 删除元素的命名约定。
1. 选择 **[!UICONTROL 另存为]** 并键入预设的名称。 或者，选择 **[!UICONTROL 保存]** 编辑现有预设时，才会显示该预设。

另外，您还可以使用没有表单字段的“查看代码”。在此视图中，您可以完全使用正则表达式创建命名约定定义。

有两个元素可用于定义，即“匹配”和“基本名称”。在这些字段中，您可以定义命名约定的所有元素，并指定用于命名它们所在的集的约定部分。公司的单个命名约定可以对其中每个元素使用一行或多行定义。 可以在您的特有定义中使用所需数量的行，并将它们分组到不同的元素中，例如，用于主图像、颜色元素、备选视图元素和样本元素。

### 创建批量集预设 {#creating-a-batch-set-preset}

Adobe Dynamic Media Classic使用批量集预设将共享某些常见信息或内容的资产组织到一组图像中，以便在查看器中显示。 批集预设方法会随您在Adobe Dynamic Media Classic中计划的资产导入作业一起自动运行。

可以使用“批量集预设”创建、编辑和管理批量集预设。您可以创建所需数量的预设，以涵盖您需要的所有资产引入作业。 有两种形式的批集预设定义：一个用于您设置的默认命名约定，另一个用于您动态创建的自定义命名约定。

您可以使用表单字段方法定义批集预设，也可以使用代码方法来使用正则表达式。 与 **[!UICONTROL 默认命名]**，您可以选择 **[!UICONTROL 代码视图]** 同时，您在表单视图中定义，并使用正则表达式来构建定义。 或者，您可以取消选中任一视图，只使用其一个视图。

另请参阅 [创建批集预设以自动生成2D旋转集](application-setup.md#creating_a_batch_set_preset_for_the_auto_generation_of_a_2d_spin_set).

另请参阅 [2D旋转集](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/537_2d-spin_converted%20renamed_Done-AVS) 培训视频。

**创建批量集预设:**

1. 转到 **[!UICONTROL 设置]** > **[!UICONTROL 应用程序设置]** > **[!UICONTROL 批集预设]** > **[!UICONTROL 批集预设]**. 默认视图为“**[!UICONTROL 查看表单]**”（在“详细信息”页面的右上角设置）。
1. 在“预设列表”面板中，选择 **[!UICONTROL 添加]** 激活页面右侧“详细信息”面板中的定义字段。
1. 在“详细信息”面板的“预设名称”字段中，键入预设的名称。
1. 在“批量集类型”下拉菜单中，选择预设类型。

   要自动生成 2D 旋转集，请在“批量集类型”下拉列表中选择“**[!UICONTROL 多轴旋转集]**”。

1. 执行以下任一操作：

   * 如果您使用的是之前在 **[!UICONTROL 应用程序设置]** > **[!UICONTROL 批集预设]** > **[!UICONTROL 默认命名]**，展开 **[!UICONTROL 资产命名约定]**，然后在文件命名下拉列表中，选择 **[!UICONTROL 默认]**.
   * 要在设置预设时定义命名约定，请展开 **[!UICONTROL 资产命名约定]**，然后在文件命名下拉列表中，选择 **[!UICONTROL 自定义]**.

1. 对于序列顺序，在将图像集分组到Adobe Dynamic Media Classic后定义图像的顺序。 默认情况下，将按字母数字顺序对您的资源排序。不过，可以使用逗号分隔的正则表达式列表来定义顺序。
1. 对于设置命名和创建约定，为您在“资源命名约定”中定义的基本名称指定后缀或前缀。此外，还定义在Adobe Dynamic Media Classic文件夹结构中创建图像集的位置。

   如果您定义大量图像集，请将这些集与包含资产本身的文件夹分开。 许多客户会创建一个“图像集”文件夹，并让应用程序将批量集生成的集合放在此处。

1. 选择 **[!UICONTROL 保存]** 中。

### 创建批集预设以自动生成2D旋转集 {#creating-a-batch-set-preset-for-the-auto-generation-of-a-d-spin-set}

您可以使用批量集类型“**多轴旋转集**”来创建用于自动生成 2D 旋转集的“方法”。对图像进行分组时采用“行”和“列”正则表达式，以便图像资源在多维数组的对应位置中正确对齐。

另请参阅 [创建批集预设](application-setup.md#creating_a_batch_set_preset).

在多轴旋转集中，没有必须具有的最小或最大行数或列数。

例如，假定要创建一个名为 *旋转2dspin*. 有一组旋转集图像包含 3 行，每行 12 个图像。这些图像命名如下：

```as3
spin-01-01
spin-01-02
… 
spin-01-12
spin-02-01
… 
spin-03-12
```

根据此信息，可以按如下方式创建批集类型方法：

![批次集方法图像](assets/se_batch_set_recipe.png)

旋转集的共享资产名称部分的分组将添加到“匹配”字段（高亮显示）。 资产名称中包含行和列的变量部分将分别添加到 行 和 列字段 。

上传和发布旋转集后，您可以激活上传作业选项对话框中&#x200B;**[!UICONTROL 批集预设]**&#x200B;下方 2D 旋转集方法的名称。

**创建用于自动生成 2D 旋转集的批量集预设:**

1. 转到 **[!UICONTROL 设置]** > **[!UICONTROL 应用程序设置]** > **[!UICONTROL 批集预设]** > **[!UICONTROL 批集预设]**. 默认视图为“**[!UICONTROL 查看表单]**”（在“详细信息”页面的右上角设置）。
1. 在“预设列表”面板中，选择 **[!UICONTROL 添加]** 激活页面右侧“详细信息”面板中的定义字段。
1. 在“详细信息”面板的“预设名称”字段中，键入预设的名称。
1. 在“批集类型”下拉菜单中，选择&#x200B;**[!UICONTROL 资产集]**。
1. 在“子类型”下拉列表中，选择“**[!UICONTROL 多轴旋转集]**”。
1. 展开 **[!UICONTROL 资产命名约定]**，然后在文件命名下拉列表中，选择 **[!UICONTROL 自定义]**.
1. 使用&#x200B;**[!UICONTROL 匹配]**&#x200B;和（可选）**[!UICONTROL 基本名称]**&#x200B;属性定义组成分组的图像资产命名的正则表达式。

   例如，您的文字“匹配”正则表达式可能如下所示：

   `(\w+)-\w+-\w+`

1. 展开“**[!UICONTROL 行列位置]**”，然后为 2D 旋转集数组中图像资源的位置定义名称格式。

   使用圆括号将文件名中的行或列位置括起来。

   例如，对于行正则表达式，它可能如下所示：

   `\w+-R([0-9]+)-\w+`

   或者

   `\w+-(\d+)-\w+`

   对于列正则表达式，可能如下所示：

   `\w+-\w+-C([0-9]+)`

   或者

   `\w+-\w+-C(\d+)`

   请记住，这些表达式只是示例。 您可以创建任何满足自己需要的正则表达式。

   >[!NOTE]
   >
   >如果行和列中的正则表达式组合无法确定资产在多维旋转集数组中的位置，则不会将该资产添加到旋转集，并且会记录错误。

1. 对于设置命名和创建约定，为您在“资源命名约定”中定义的基本名称指定后缀或前缀。此外，还定义在Adobe Dynamic Media Classic文件夹结构中创建图像集的位置。

   如果您定义大量图像集，请将这些集与包含资产本身的文件夹分开。 许多客户会创建一个“图像集”文件夹，并让应用程序将批量集生成的集合放在此处。

1. 选择 **[!UICONTROL 保存]** 中。
1. 照常上载和发布您的旋转集，同时确保您在“作业加载选项”对话框中的“批量集预设”下激活 2D 旋转集的名称。

>[!MORELIKETHIS]
>
>* [预览资产](previewing-asset.md#previewing_an_asset)
>* [设置图像预设](setting-image-presets.md#setting_up_image_presets)
>* [查看、添加和导出元数据](viewing-adding-exporting-metadata.md#viewing_adding_and_exporting_metadata)
>* [检查作业文件](checking-job-files.md#checking_job_files)

