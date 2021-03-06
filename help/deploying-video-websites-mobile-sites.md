---
title: 将视频部署到网站和移动站点
description: 了解如何从AdobeDynamic Media Classic将视频部署到您的网站和移动设备网站。
uuid: 22bb4402-c0ab-4df0-89b9-99707d111927
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
discoiquuid: 0d006314-c4cc-4f6c-a51c-6075bb445e39
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: 3df22d48-edb5-4927-aefb-104b53f81f1a
source-git-commit: 44045daa35052f01a26c67e0b2a0fb1405c53292
workflow-type: tm+mt
source-wordcount: '1703'
ht-degree: 34%

---

# 将视频部署到网站和移动站点{#deploying-video-to-your-websites-and-mobile-sites}

网站、移动设备网站和桌面应用程序可使用URL字符串或嵌入代码访问AdobeDynamic Media Classic服务器内容（包括视频）。 AdobeDynamic Media Classic在发布过程中激活这些URL字符串。 要将视频的URL字符串或嵌入代码放入网页、移动页面和桌面应用程序中，请从AdobeDynamic Media Classic中复制该代码。

>[!NOTE]
>
>在发布资源之前，URL 或嵌入代码处于非活动状态。

## 发布视频 {#publishing-video}

通过发布视频，AdobeDynamic Media Classic服务器可以将视频交付到您的网站、移动设备网站或应用程序。

可以使用两种不同的方法发布视频：

* **在上载时自动立即发布视频**  — 在视频上传过程中，AdobeDynamic Media Classic可以在上传和编码视频时自动发布视频。 立即发布功能意味着，无需事后单独发布视频。

* **在上载后手动发布视频**  — 如果您不想立即发布视频，可以随时手动发布视频。

发布视频后，AdobeDynamic Media Classic会为您的HTML页面或应用程序代码激活URL字符串。

**发布视频:**

1. 执行以下任一操作：

   * 要在上传时自动且立即发布视频，请在“上传”页面中，选择&#x200B;**[!UICONTROL 上传后发布]**。 您已完成相应的操作，不需要执行其他步骤。
   * 要在上传后手动发布视频，请在浏览面板中，选择视频，然后在全局导航栏中，选择&#x200B;**发布**。

## 将视频URL关联到移动设备网站或网站 {#linking-a-video-url-to-a-mobile-site-or-a-website}

在发布视频后，您可以获取该视频的 URL 以在网站、移动站点或台式机应用程序中使用。如果要在网页顶部的弹出或模式窗口中显示视频，请使用视频 URL。

当客户选择链接时，会自动检测其设备、带宽和屏幕大小。 在桌面的预定义查看器中会显示适当的视频进行播放，智能手机和平板电脑在移动设备的本地视频播放器中播放。

另请参阅[将视频查看器嵌入网页](deploying-video-websites-mobile-sites.md#embedding_the_video_viewer_on_a_web_page)。

**将视频 URL 链接到移动站点或网站:**

1. 在“资产浏览”面板的&#x200B;**[!UICONTROL 显示]**&#x200B;下拉列表中，选择&#x200B;**[!UICONTROL 视频]**&#x200B;或&#x200B;**[!UICONTROL 自适应视频集]**。
1. 在左侧的“资源库”面板中，导航到包含要链接到的视频或自适应视频集的资源文件夹。
1. 在“资源浏览”面板上方的工具栏右侧，执行以下任一操作：

   * 选择&#x200B;**[!UICONTROL 网格视图]**&#x200B;或&#x200B;**[!UICONTROL 列表视图]**。 在“资源浏览”面板中，双击单个资源的视频缩略图，以便在详细信息视图中将其打开。在右侧的“URL和嵌入代码”面板的HTTP流下，选择所需查看器右侧的&#x200B;**[!UICONTROL 复制URL]** 。 最佳做法是复制与`Universal_HTML5_Video`查看器关联的URL。
   * 选择&#x200B;**[!UICONTROL 网格视图]**。 在“资产浏览”面板中，选择一个资产，然后在缩略图图像下方，转到&#x200B;**[!UICONTROL 预览]** > **[!UICONTROL 查看器列表]**。

      在“查看器列表”页面的表的“操作”列下，选择&#x200B;**[!UICONTROL 复制URL]**。 最佳做法是复制与`Universal_HTML5_Video`查看器关联的URL。

   * 选择&#x200B;**[!UICONTROL 列表视图]**。 在“资产浏览”面板中，选择一个资产，然后转到缩略图图像右侧的&#x200B;**[!UICONTROL 预览]** > **[!UICONTROL 查看器列表]**。

      在“查看器列表”页面的表的“操作”列下，选择&#x200B;**[!UICONTROL 复制URL]**。 最佳做法是复制与`Universal_HTML5_Video`查看器关联的URL。

   * 选择&#x200B;**[!UICONTROL 网格视图]**、**[!UICONTROL 列表视图]**&#x200B;或&#x200B;**[!UICONTROL 详细信息视图]**。 在同一工具栏中，转到&#x200B;**[!UICONTROL 预览]** > **[!UICONTROL 查看器列表]**。

      在“查看器列表”页面的表的“操作”列下，选择&#x200B;**[!UICONTROL 复制URL]**。 最佳做法是复制与`Universal_HTML5_Video`查看器关联的URL。

1. 将 HTML5 视频 URL 链接粘贴到您的网站和移动站点中。

## 在网页上嵌入视频查看器 {#embedding-the-video-viewer-on-a-web-page}

如果要播放网页中嵌入的视频，请使用嵌入代码功能。将嵌入代码复制到剪贴板，以便将其粘贴到网页中。 不允许在“嵌入代码”对 话框中编辑代码 。

另请参阅[将视频URL链接到移动网站或网站](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website)。

**在网页中嵌入视频查看器:**

1. 在“资产浏览”面板的“显示”下拉列表中，选择&#x200B;**[!UICONTROL 视频]**&#x200B;或&#x200B;**[!UICONTROL 自适应视频集]**。
1. 在左侧的“资源库”面板中，导航到包含要复制其嵌入代码的视频或自适应视频集的资源文件夹。
1. 在“资源浏览”面板上方的工具栏右侧，执行以下任一操作：

   * 选择&#x200B;**[!UICONTROL 网格视图]**&#x200B;或&#x200B;**[!UICONTROL 列表视图]**。 在“资源浏览”面板中，双击单个资源的视频缩略图，以便在详细信息视图中将其打开。在右侧的“URL和嵌入代码”面板的HTTP流下，选择所需查看器右侧的&#x200B;**[!UICONTROL 嵌入代码]** 。 最好选择与`Universal_HTML5_Video`查看器关联的&#x200B;**[!UICONTROL 嵌入代码]**。
   * 选择&#x200B;**[!UICONTROL 网格视图]**。 在“资产浏览”面板中，选择一个资产，然后在视频缩略图图像的下方，选择&#x200B;**[!UICONTROL 预览]** > **[!UICONTROL 查看器列表]**。

      在“查看器列表”页面的表的“操作”列下，选择&#x200B;**[!UICONTROL 嵌入代码]**。 最好选择与`Universal_HTML5_Video`查看器关联的&#x200B;**[!UICONTROL 嵌入代码]**。

   * 选择&#x200B;**[!UICONTROL 列表视图]**。 在“资产浏览”面板中，选择一个资产，然后转到缩略图图像右侧的&#x200B;**[!UICONTROL 预览]** > **[!UICONTROL 查看器列表]**。

      在“查看器列表”页面的表的“操作”列下，选择&#x200B;**[!UICONTROL 嵌入代码]**。 最好选择与`Universal_HTML5_Video`查看器关联的&#x200B;**[!UICONTROL 嵌入代码]**。

   * 选择&#x200B;**[!UICONTROL 网格视图]**、**[!UICONTROL 列表视图]**&#x200B;或&#x200B;**[!UICONTROL 详细信息视图]**。 在同一工具栏中，转到&#x200B;**[!UICONTROL 预览]** > **[!UICONTROL 查看器列表]**。

      在“查看器列表”页面的表的“操作”列下，选择&#x200B;**[!UICONTROL 嵌入代码]**。 最好选择与`Universal_HTML5_Video`查看器关联的&#x200B;**[!UICONTROL 嵌入代码]**。

1. 在“嵌入代码”对话框中，选择&#x200B;**[!UICONTROL 复制到剪贴板]**。

   在“嵌入代码”对话框中不允许编辑代码。

1. 选择&#x200B;**[!UICONTROL 关闭]**。
1. 在网页中粘贴嵌入代码。

### 实施用于在MP4视频资产中使用HTML5视频的嵌入代码 {#implementing-embed-code-for-using-html-video-with-mp-video-assets}

如果您没有使用AdobeDynamic Media Classic HTML5视频播放器，而是希望将本机HTML5 `<video>`标记与MP4视频资产结合使用，则可以使用以下嵌入代码示例：

```as3
<video poster="S7 video thumbnail URL" controls> 
        <source src="S7 OGG video asset URL (no player)" type='video/ogg; codecs="theora, vorbis"'/> 
        <source src="S7 MP4 mobile progressive video asset URL (no player)" type='video/mp4; codecs="avc1.4D401E, mp4a.40.2"'/> 
        <p>This is fallback content</p> 
</video>
```

* 将`"S7 video thumbnail URL"`替换为视频的缩略图URL，即用户在播放视频之前看到的视频缩略图图像。

   请参阅[获取视频缩略图URL](deploying-video-websites-mobile-sites.md#obtaining_video_thumbnail_urls)。

* 将`"S7 OGG video asset URL (no player)"`替换为OGG视频的视频渐进式URL。

   请参阅[将视频URL链接到移动网站或网站](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website)。

* 将`"S7 MP4 mobile progressive video asset URL (no player)"`替换为视频的移动渐进式URL。

   请参阅[将视频URL链接到移动网站或网站](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website)。

## 使用第三方视频播放器部署视频 {#deploying-video-using-a-third-party-video-player}

如果您使用第三方视频播放器或自定义构建的视频播放器而不是Dynamic Media Classic视频查看器，则可以获取适用于HLS多比特率视频流播放或渐进式下载的直接视频URL。

**使用第三方视频播放器部署视频:**

1. 在AdobeDynamic Media Classic的全局导航栏上，转到&#x200B;**[!UICONTROL 设置]** > **[!UICONTROL 应用程序设置]** > **[!UICONTROL 常规设置]**。
1. 根据要使用的 URL 类型，请执行以下任务之一：

* 生成直接HLS流视频URL（多比特率）

   在&#x200B;**[!UICONTROL 应用程序常规设置]**&#x200B;页面的&#x200B;**[!UICONTROL Servers]**&#x200B;组的&#x200B;**[!UICONTROL Published Server Name]**&#x200B;文本字段中，构建直接URL。 使用以下语法：`server/is/content/company/folder/filename.m3u8`

   例如，假设已发布的服务器名称为`https://s7d9.scene7.com/.`使用步骤2中的语法，则直接URL可能如下所示：
   `https://s7d9.scene7.com/is/content/GeoRetail/AdobeRIA-AVS.m3u8`

* 生成直接HLS流视频URL（单比特率）

   在&#x200B;**[!UICONTROL 应用程序常规设置]**&#x200B;页面的&#x200B;**[!UICONTROL Servers]**&#x200B;组的&#x200B;**[!UICONTROL HLS流服务器名称]**&#x200B;文本字段中，使用以下语法构建直接URL:

   `server/company/folder/filename.ext.m3u8`

   例如，假定HLS流服务器名称为`https://s7mbrstream.scene7.com/hls-vod/`。 使用步骤2中的语法，直接URL可能如下所示：
   `https://s7mbrstream.scene7.com/hls-vod/GeoRetail/MBR/ToyStory3\_Teaser1\_High\_iPad\_768x432\_1296K.mp4.m3u8`

* 生成直接渐进式视频 URL

   在“**[!UICONTROL 应用程序常规设置]**”页面的“**[!UICONTROL 服务器]**”组的“**[!UICONTROL 渐进式视频服务器名称]**”文本框中，使用以下语法构建直接 eVideo URL：

   `server/company/folder/filename`

   例如，假定渐进式视频服务器名称为`https://s7d9.scene7.com/is/content/`。 使用步骤2中的语法，直接URL可能如下所示：
   `https://s7d9.scene7.com/e2/GeoRetail/SourceVideo/outdoors.mp4`

## 使用视频缩略图 {#working-with-video-thumbnails}

AdobeDynamic Media Classic为编码视频和预编码视频生成缩略图。 您可以像使用任何图像资源一样使用视频缩略图。此外，您还可以获取AdobeDynamic Media Classic生成的视频缩略图的URL，并在AdobeDynamic Media Classic之外部署这些URL。 例如，您可以在搜索结果、相关视频列表和网站上的视频播放列表中部署缩略图。

基于视频的第一个异构帧（不是全黑帧或全白帧等）生成缩略图。

### 获取视频缩略图URL {#obtaining-video-thumbnail-urls}

AdobeDynamic Media Classic在上传过程中会自动生成视频缩略图。 缩略图显示在列表视图和网格视图的“浏览”面板中。

要生成视频缩略图的 URL，请执行发布操作。

请参阅[发布视频](deploying-video-websites-mobile-sites.md#publishing_video)。

发布后，您可以在“URL 和嵌入代码”面板的“详细信息视图”中获取视频缩略图 URL。选择视频缩略图右侧的&#x200B;**[!UICONTROL 复制URL]** ，以便复制其URL。

### 在视频查看器中修改海报帧 {#modifying-poster-frames-in-video-viewers}

*海报帧*&#x200B;是在开始播放视频之前在视频查看器中显示的初始帧。AdobeDynamic Media Classic使用视频缩略图作为海报框架。

您可以将图像修饰符应用于海报帧。例如，您可以裁切海报帧或使其变得透明。要修改海报帧，请打开视频查看器配置屏幕，并在“海报图像修饰符”部分中输入修饰符。

请参阅[添加或编辑视频查看器预设](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset)。

请参阅[Image Serving指南](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/c-is-home.html?lang=en#image-serving-api)。

还可以通过将修饰符附加到视频缩略图 URL 的后面来修改视频缩略图。

>[!MORELIKETHIS]
>
>* [发布文件](publishing-files.md#publishing_files)