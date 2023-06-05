---
title: 上传视频并进行编码
description: 了解如何在Adobe Dynamic Media Classic中上传视频并进行编码。
uuid: 9a7d6513-b10c-40b0-aebb-18a795c2b8d1
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: a0941823-850c-4373-9e37-f32032de3805
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: 93ad91d7-f3dd-484b-b62c-633fcb864bbf
source-git-commit: 65e3b69bdcbd651a5f9ab100592217e61a8c05ef
workflow-type: tm+mt
source-wordcount: '3967'
ht-degree: 56%

---

# 上传视频并进行编码{#uploading-and-encoding-videos}

要创建单个视频或自适应视频集以交付到Web或移动设备，您首先要将主视频文件上传到Adobe Dynamic Media Classic。 Adobe Dynamic Media Classic将视频编码为MP4格式，并以以下文件格式发布视频：

* **MP4** - Adobe Dynamic Media Classic建议将MP4作为首选的视频文件格式。 将 MP4 文件用于以下内容：

   * 桌面的 HTTP 动态流。
   * HTTP 实时流（Apple 的流协议）。
   * 渐进式视频交付到Android™、BlackBerry®和Windows®移动设备

   Adobe Dynamic Media Classic提供两种上传视频文件的工作流：

* **预编码视频**  — 直接将MP4文件上传到Adobe Dynamic Media Classic。 对于该工作流程，在上载文件时，不会对文件进行编码。文件在准备传送到桌面和移动设备时进行预编码。

* **主要源视频**  — 上传主源视频文件，并在上传时将这些文件编码为MP4文件。 在浏览面板中，编码的视频标记为“视频”。Adobe Dynamic Media Classic支持对多种格式的视频文件进行编码。

   * 确保要编码的主要源视频文件受支持。

      请参阅[支持编码的视频文件类型](uploading-encoding-videos.md#supported-video-file-types-for-encoding)。

   * 选择一个视频编码预设。

      请参阅[用于编码视频文件的视频预设](application-setup.md#video-presets-for-encoding-video-files)。

      请参阅[视频编码最佳做法](uploading-encoding-videos.md#best-practices-for-video-encoding)。

Adobe Dynamic Media Classic还会生成视频缩略图。 您可以了解有关视频缩略图的详细信息，如何获取其 URL 以及修改海报帧。

参见 [使用视频缩略图](deploying-video-websites-mobile-sites.md#working-with-video-thumbnails).

**上载和编码视频:**

执行以下任一操作：.

*如果您的视频已经编码*

1. 在全局导航栏上，选择 **[!UICONTROL 上传]**.
1. 在“上传”页面中，选择 **[!UICONTROL 从桌面]** 选项卡。
1. 在上传页面上，在 **[!UICONTROL 选择要上载的文件]** 面板，选择 **[!UICONTROL 浏览]**，导航到MP4视频文件，然后选择 **[!UICONTROL 打开]**.
1. 在 **[!UICONTROL 选择文件夹目标]** 面板中，为上传的文件选择一个文件夹。
1. 在上传页面上，确保 **[!UICONTROL 上传后发布]** 已选中。
1. 选择 **[!UICONTROL 提交上传]**.

*如果要使用Adobe Dynamic Media Classic对视频进行编码*

1. 在全局导航栏上，选择 **[!UICONTROL 上传]**.
1. 在“上传”页面中，选择 **[!UICONTROL 从桌面]** 选项卡。
1. 在 **[!UICONTROL 选择要上载的文件]** 面板，选择 **[!UICONTROL 浏览]**，导航到主源视频文件，然后选择 **[!UICONTROL 打开]**.
1. 在 **[!UICONTROL 选择文件夹目标]** 面板中，为上传的文件选择一个文件夹。
1. 在页面的右下角，选择 **[!UICONTROL 作业选项]**，
1. 在上载作业选项对话框中，展开 **[!UICONTROL EVideo选项]**，然后执行以下操作之一：

   * 最佳实践是选择 **[!UICONTROL 自适应视频编码]**. 请参阅[自适应视频（默认）](application-setup.md#adaptive-video-default)。
   * 可选. 如果要使用单独的编码设置，请展开 **[!UICONTROL 单个编码预设]**，然后选择所需的台式机、移动设备和平板电脑编码选项。
请参阅[台式机视频编码预设](application-setup.md#desktop-video-encoding-presets)、[移动设备视频编码预设](application-setup.md#mobile-video-encoding-presets)和[平板电脑视频编码预设](application-setup.md#tablet-video-encoding-presets)。
1. 在“上载作业选项”对话框中，选择 **[!UICONTROL 保存]**.
1. 在上传页面上，确保 **[!UICONTROL 上传后发布]** 已选中。
1. 在上传页面的右下角，选择 **[!UICONTROL 提交上传]**.

*如果要重新编码以前上载的视频文件*

1. 在Adobe Dynamic Media Classic的“浏览”面板中，导航到视频并将其选定。
1. 转到 **[!UICONTROL 文件]** > **[!UICONTROL 重新处理]**.
1. 在重新处理资源对话框中，展开 **[!UICONTROL EVideo选项]**，然后执行以下操作之一：
   * 最佳做法是使用以下方法。选择“**自适应视频**”。请参阅[自适应视频（默认）](application-setup.md#adaptive-video-default)。
   * 可选. 如果要使用单独的编码设置，请展开 **[!UICONTROL 单个编码预设]**，然后选择所需的台式机、移动设备和平板电脑编码选项。
请参阅[台式机视频编码预设](application-setup.md#desktop-video-encoding-presets)、[移动设备视频编码预设](application-setup.md#mobile-video-encoding-presets)和[平板电脑视频编码预设](application-setup.md#tablet-video-encoding-presets)。
1. 在重新处理资源对话框中，选择 **[!UICONTROL 提交]**.

在使用自适应视频编码预设或多个单编码预设时，结果是以多个视频编码自动创建的自适应视频集。也可以选择各个视频以手动创建自适应视频集。

只有在自动或手动生成自适应视频集时，才会创建 MP4 和 M4V 文件类型。

## 支持编码的视频文件类型 {#supported-video-file-types-for-encoding}

下表列出了在上载文件时可以编码为 MP4 或 OGV 格式的视频文件类型（包含允许的视频编解码器）。此表列出了文件格式和编码解码器：

* **视频文件格式**  — 与ZIP文件类似，视频文件格式可确定视频文件中包含文件的方式。 视频文件通常包含多个轨道 — 一个视频轨道（没有音频）和一个或多个音频轨道（没有视频） — 这些轨道相互联系并且同步。视频文件格式决定了这些不同的数据轨道和元数据的组织方式。

* **视频编解码器**  — 视频编解码器描述用于对视频进行编码的算法。 视频播放器根据其编码解码器对视频进行解码，然后在屏幕显示一系列图像或帧。编解码器将视频文件存储为播放视频所需的信息量降至最低。只会存储一个帧和下一个帧之间差异的相关信息，而不存储每个单独帧的相关信息。由于大多数视频在帧间变化不大，因此编解码器允许较高的压缩率，从而缩小文件大小。

   | 视频文件格式 | 视频编解码器 |
   | --- | --- |
   | 3GP | H.263、H.264 |
   | AVI | DivX、DV |
   | M2P | MPEG-2 PS |
   | M2T | MPEG-2 TS |
   | M2TS | MPEG-2 TS |
   | M2V | MPEG-2 ES |
   | M4V | H.264 |
   | MOV | DV、DVCPro 50、H.261、H.263、H.264、Sorenson Video 1 |
   | MP4 | H.264/MPEG-4 AVC |
   | MPEG | MPEG-2 SS |
   | MPG | MPEG-2 SS |
   | MTS | MPEG-2 |
   | ProRes | APCN、APCS、APCO、APCH、AP4H |
   | TS | DVCPro 50 |
   | VOB | MPEG-2 |
   | WMV/ASF | VC-1、Windows® Media Video 7、Windows® Media Video 8 |

   >[!NOTE]
   >
   >如果上载并尝试编码视频文件，但由于文件包含不兼容的编码解码器或文件容器而被拒绝，“作业”屏幕将发出警告。有关更多信息，请参阅 [检查作业文件](checking-job-files.md).

## 视频编码最佳做法 {#best-practices-for-video-encoding}

以下是在Adobe Dynamic Media Classic中对源视频文件进行编码的最佳实践提示。

<!-- THE FOLLOWINGS LINKS APPEAR TO BE DEAD AND THE CONTENT COMPLETELY LOST. THE GO URL DOESN'T EVEN WORK ANYMORE.
For advice about video encoding, see the following:

* Article: [Streaming 101: The Basics — Codecs, Bandwidth, Data Rate, and Resolution][www.adobe.com/go/learn_s7_streaming101_en](https://www.adobe.com/go/learn_s7_streaming101_en). THIS MATERIAL WAS FOUND ON A THIRD PARTY WEBSITE HERE: https://streaminglearningcenter.com/articles/streaming-101-the-basics-codecs-bandwidth-data-rate-and-resolution.html MATERIAL IS GOOD BUT DO NOT LINK TO IT
* Video: [Video Encoding Basics][www.adobe.com/go/learn_s7_encoding_en](https://www.adobe.com/go/learn_s7_encoding_en). -->

### 源视频文件 {#source-video-files}

您编码视频文件时，使用可实现的最高品质的源视频文件。避免使用以前编码的视频文件，因为这些文件已经过压缩，进一步编码会创建质量达不到标准的视频。

下表描述了编码源视频文件时，建议的大小、长宽比和最小比特率：

| 大小 | 高宽比 | 最小比特率 |
| --- | --- | --- |
| 1024 X 768 | 4:3 | 大多数视频为 4500 kbps。 |
| 1280 X 720 | 16:9 | 3000 - 6000 kbps，具体取决于视频中动作的数量。 |
| 1920 X 1080 | 16:9 | 6000 - 8000 kbps，具体取决于视频中动作的数量。 |

### 获取文件的元数据 {#obtaining-a-file-s-metadata}

您可以通过以下方式获取文件的元数据：在Adobe Dynamic Media Classic中查看其元数据、使用视频编辑工具或使用专为获取元数据而设计的应用程序。 以下是使用第三方应用程序 MediaInfo 获取视频文件元数据的说明：

1. 转到此网页： [https://mediaarea.net/en/MediaInfo](https://mediaarea.net/en/MediaInfo).
1. 选择和下载图形界面版本的安装程序，并按安装说明操作。
1. 安装后，右键单击视频文件(仅限Windows®)并选择MediaInfo，或打开MediaInfo并将视频文件拖到应用程序中。 您会看到与视频文件相关的所有元数据，其中包括其宽度、高度和 fps。

### 高宽比 {#aspect-ratio}

当为主视频文件选择或创建视频编码预设时，请确保预设具有与主视频文件相同的纵横比。 *高宽比*&#x200B;是视频宽度和视频高度的比例。

要确定视频文件的纵横比，请获取该文件的元数据，并注意该文件的宽度和高度(请参阅 [获取文件的元数据](uploading-encoding-videos.md#obtaining_a_file_s_metadata))。 然后，使用以下公式来确定高宽比：

宽度/高度 = 高宽比

下表描述了如何将公式结果转换为常用高宽比选项：

| 公式结果 | 高宽比 |
| --- | --- |
| 1.33 | 4:3 |
| 0.75 | 3:4 |
| 1.78 | 16:9 |
| 0.56 | 9:16 |

例如，1440宽度x 1080高度的视频的长宽比为1440/1080，即1.33。在这种情况下，您可以选择具有4:3纵横比的视频编码预设来编码视频文件。

### 数据速率 {#data-rate}

*数据速率*（也称为&#x200B;*比特率*）是用于编码以组成一秒钟视频播放的数据量。数据速率以千比特/秒 (Kbps) 为度量单位。

>[!NOTE]
>
>因为所有编码解码器使用有损压缩，所以数据速率是决定视频质量的最重要因素。使用有损压缩时，将视频文件压缩的越多，质量下降的越多。因此，所有其他特性（分辨率、帧速率和编码解码器）不变时，数据速率越低，压缩文件的质量越低。

选择视频编码预设时，请记住考虑目标最终用户的连接速度。 选择数据速率为该速度 80% 的预设。例如，如果目标最终用户的连接速度为 1000 Kbps，最佳预设是视频数据速率为 800 Kbps 的预设。

下表描述了标准连接速度的数据速率。

| 速度 (Kbps) | 连接类型 |
| --- | --- |
| 256 | 拨号连接。 |
| 800 | 标准移动连接。对于此连接，将数据速率设定在 400 至最大值为 800 的范围内，以实现 3G 体验。 |
| 2000 | 标准带宽桌面连接。对于这种连接，数据速率目标在800-2000 Kbps范围内，大多数目标平均为1200-1500 Kbps。 |
| 5000 | 标准高带宽连接。不推荐在此上限范围内编码，因为大部分消费者无法使用此速度的视频传送。 |

### 分辨率 {#resolution}

*分辨率*&#x200B;说明了视频文件的高度和宽度（以像素为单位）。大多数源视频都以高分辨率（例如，1920 x 1080）存储。为了实现流，将源视频压缩为更小的分辨率（640 x 480 或更小）。

分辨率和数据速率是决定视频质量的两个不可分割的因素。为获得相同的视频质量，视频文件的像素数（分辨率越高）越高，数据速率必须越高。例如，以分辨率为 320 x 240 和分辨率为 640 x 480 的视频文件中的每帧像素数为例：

| 分辨率 | 每帧像素数 |
| --- | --- |
| 320 x 240 | 76,800 |
| 640 x 480 | 307,200 |

640 x 480 文件的每帧像素数是另一个文件的四倍。要针对这两个示例分辨率实现相同的数据速率，须对 640 x 480 文件进行四倍的压缩，这会降低视频的质量。因此，250 Kbps 的视频数据速率在 320 x 240 分辨率下会产生高质量的视觉效果，但在 640 x 480 分辨率下却达不到这种效果。

>[!NOTE]
>
>通常，使用的数据速率越高，视频的显示效果越好，使用的分辨率越高，必须保持查看质量的数据速率越高（与分辨率较低相比）。

因为分辨率和数据速率是关联的，在编码视频时您有两个选择：

* 选择数据速率，然后以最高分辨率进行编码，该分辨率以您选择的数据速率显示得最好。
* 选择一个分辨率，然后用在您选择的分辨率下实现高质量视频所需的数据速率编码。

为主视频文件选择（或创建）视频编码预设时，请使用此表定位正确的分辨率：

| 分辨率 | 高度（像素） | 屏幕大小 |
| --- | --- | --- |
| 240p | 240 | 极小屏幕 |
| 300p | 300 | 通常用于移动设备的小屏幕 |
| 360p | 360 | 小屏幕 |
| 480p | 480 | 中等屏幕 |
| 720p | 720 | 大屏幕 |
| 1080p | 1080 | 高清大屏幕 |

### Fps（每秒帧数） {#fps-frames-per-second}

在美国和日本，大部分视频以 29.97 帧/秒 (fps) 拍摄；在欧洲，大部分视频以 25 fps 拍摄。电影以 24 fps 拍摄。

选择与主视频文件的fps速率匹配的视频编码预设。 例如，如果主视频为25 fps，请选择具有25 fps的编码预设。 默认情况下，所有自定义编码都使用主视频文件的fps。 因此，在创建视频编码预设时，您不需要明确指定 fps 设置。

### 视频编码尺寸 {#video-encoding-dimensions}

为获得最佳结果，请选择编码尺寸，以便源视频是您的所有编码视频的整数倍。

要计算此比例，您可以用源视频宽度除以编码视频的宽度，得到宽度比例。然后，用源视频高度除以编码视频的高度，得到高度比例。

如果得到的比例为整数，表示视频已得到最佳缩放。如果得到的比例不是整数，则剩余的像素伪影会保留在显示屏上，从而影响视频质量。当视频中包含文本时，此影响尤为明显。

例如，假设您的源视频是 1920 x 1080。下表中的三种编码视频提供了可供使用的最佳编码设置。

| 视频类型 | 宽度 X 高度 | 宽度比例 | 高度比例 |
| --- | --- | --- | --- |
| 源视频 | 1920 x 1080 | 1 | 1 |
| 编码视频 | 960 x 540 | 2 | 2 |
| 编码视频 | 640 x 360 | 3 | 3 |
| 编码视频 | 480 x 270 | 4 | 4 |

### 编码视频文件格式 {#encoded-video-file-format}

Adobe Dynamic Media Classic建议使用MP4 H.264视频编码预设。 由于 MP4 文件使用 H.264 视频编解码器，因此可以提供压缩文件大小的高品质视频。

## 使用视频编码预设 {#working-with-video-encoding-presets}

使用视频制作设备和视频编辑软件创建的主视频文件通常太大，并且格式不正确，无法传送到在线目标。 要将数字视频转换为适用于在不同屏幕上播放的适当格式和规格，您可以将视频文件&#x200B;*转码*（此过程也称为&#x200B;*编码*）。在编码过程中，视频将压缩为最适合传送到网站和移动设备的较小且有效的文件大小。

参见 [上传视频并进行编码](uploading-encoding-videos.md#uploading-and-encoding-videos).

Adobe Dynamic Media Classic为您提供了一个预定义的视频编码预设库，这些预设反映了当前最常用的编码设置。 这些编码预设针对在目标屏幕上播放进行了优化。此外，管理员还可以创建自己的视频编码预设，以便为最终用户自定义视频大小和播放质量。所有视频编码预设(无论是来自Adobe Dynamic Media Classic的现成预设，还是自定义预设)都以MP4文件格式输出视频。

在“视频预设”屏幕上，管理员可以设置和管理视频编码。他们可以执行以下操作：

* 激活和停用视频编码预设。
* 创建视频编码预设。
* 编辑视频编码预设。
* 删除视频预设。

您上传到Adobe Dynamic Media Classic或您在Adobe Dynamic Media Classic中编码的任何视频都将被视为“视频”。 即此资源类别表示您可以传送此视频以便在桌面、移动设备或同时在两者上播放。例如，您可以在Adobe Dynamic Media Classic中预览这些类型的视频。 也可以生成 URL（使用复制 URL）和可嵌入的代码（使用嵌入代码）以用于视频播放器、网站，等等。

参见 [在视频查看器中预览视频](previewing-videos-video-viewer.md#previewing-videos-in-a-video-viewer).

参见 [将视频URL链接到移动网站或网站](deploying-video-websites-mobile-sites.md#linking-a-video-url-to-a-mobile-site-or-a-website).

参见 [在网页上嵌入视频查看器](deploying-video-websites-mobile-sites.md#embedding-the-video-viewer-on-a-web-page).

对于您在Adobe Dynamic Media Classic中上传并编码的视频资产，视频将以下列文件格式交付：

**MP4 H.264** 将MP4文件用于以下内容：

* 桌面的 HTTP 动态流。
* HLS(HTTP实时流、Apple的流协议)。
* 渐进式视频交付到Android™、BlackBerry®和Windows®移动设备。

任何其他视频格式和编解码器都将被视为“主视频”。 此资源类别表示此类视频为源视频文件，无法进行传送以便在桌面或移动设备上播放。例如，您无法在Adobe Dynamic Media Classic中预览这些类型的视频。 您也无法生成复制 URL 和嵌入代码，以便在视频播放器、网站等平台上使用。

### 筛选视频编码预设列表 {#filtering-the-list-of-video-encoding-presets}

“视频预设”页面和“自适应视频预设”页面包含一个表，其中列出了每个视频预设的活动状态、预设名称、预期播放设备、视频大小和数据速率。

您可以选择按“两者全部”、“活动”或“非活动”进行过滤以优化列表，以便查看所有视频预设或将列表范围缩小为活动或非活动预设。

也可以根据播放设备选项进行过滤，将列表范围缩小为用于在所有设备、台式机、移动设备或平板电脑上播放视频的视频预设。

**过滤视频编码预设列表:**

1. 在Adobe Dynamic Media Classic的全局导航栏上，转到 **[!UICONTROL 设置]** > **[!UICONTROL 应用程序设置]** > **[!UICONTROL 视频预设]** > **[!UICONTROL 自适应视频预设]** 或 **[!UICONTROL 单个编码预设]**.

   自适应视频预设和单一编码预设的页面包括一个表，其中列出了每个视频预设的活动状态、预设名称、预期播放设备、视频维度和数据速率。

1. 在“视频预设”工具栏上的“单个编码预设”页中，使用两个下拉列表根据活动状态和播放设备优化表格中的预设列表。

   * 在第一个较小的下拉列表中，选择“**[!UICONTROL 两者全部]**”以查看所有视频预设，或者选择“**[!UICONTROL 活动]**”或“**[!UICONTROL 非活动]**”以将列表范围缩小为活动或非活动预设。
   * 在第二个较大的下拉列表中，选择一个播放设备选项以将列表范围缩小为用于在台式机、移动设备或平板设备上播放视频的视频预设。

### 激活或停用视频编码预设 {#activating-or-deactivating-video-encoding-presets}

激活的视频预设将显示在“上载作业选项”对话框中。当用户在上传过程中上传视频文件时，会显示该对话框。 他们可以从所有激活的编码预设列表中进行选择。

1. 在Adobe Dynamic Media Classic的全局导航栏上，转到 **[!UICONTROL 设置]** > **[!UICONTROL 应用程序设置]** > **[!UICONTROL 视频预设]**.
1. 执行以下任一操作：

   * 选择 **[!UICONTROL 自适应视频预设]**.
   * 选择 **[!UICONTROL 单个编码预设]**.

1. 执行以下任一操作：

   * 要激活某个视频预设，请在“预设”页中的“活动”列下面，选中预设名称旁边的复选框。
   * 要停用视频预设，请取消选中要停用的视频预设旁边的框。

      >[!NOTE]
      >
      >非活动视频预设不会显示在“上载作业选项”对话框中。

1. 在页面的右下角，选择 **[!UICONTROL 关闭]**.

### 添加或编辑视频编码预设 {#adding-or-editing-a-video-encoding-preset}

您可以创建自己的自定义单一编码视频预设，并将其添加到视频预设表中。 如果您使用新名称保存编辑的预设，您还可以更改Adobe Dynamic Media Classic随附的任何预定义的单一编码视频预设。

Adobe Dynamic Media Classic为目标数据速率、分辨率高度和分辨率宽度设置了最大限制，以确保有正确的播放体验。 如果超过以下限制，则会显示警告消息：

* 对于计算机播放，限制为： （宽度/16） &#42; (Height/16) &lt; 8192。
* 对于移动设备播放，限制为： （宽度/16） &#42; （高度/16） &lt; 660；目标数据速率&lt; 4000。
* 对于平板电脑播放，限制为：（宽度/16） &#42; (Height/16) &lt; 3600。

**添加或编辑视频编码预设:**

1. 在Adobe Dynamic Media Classic的全局导航栏上，转到 **[!UICONTROL 设置]** > **[!UICONTROL 应用程序设置]** > **[!UICONTROL 视频预设]**.
1. 选择 **[!UICONTROL 单个编码预设]**.
1. 在“视频预设”页中，执行以下操作之一：

   * 在“视频预设”工具栏上，选择 **[!UICONTROL 添加]** 以便添加视频预设。
   * 选择一个视频预设。在工具栏中，选择 **[!UICONTROL 编辑]**.

      您无法编辑Adobe Dynamic Media Classic预定义预设；您只能通过选择从现有预设创建预设 **[!UICONTROL 另存为]**.

1. 在“添加视频预设”或“编辑视频预设”页中，设置所需的视频预设选项。

   有关建议的设置，请参阅[视频编码最佳做法](uploading-encoding-videos.md#best-practices-for-video-encoding)。

   | 视频预设选项 | 说明 |
   | --- | --- |
   | 预设名称 | 输入视频预设的描述性名称。您输入的名称显示在“上载作业选项”对话框中，用户在此对话框中选择转码选项。 |
   | 说明 | 描述视频预设。在“上载作业选项”对话框中，将指针移动到预设名称上方时，输入的内容会显示为工具提示，用户可在其中选择转码选项。 |
   | 播放设备 | 选择要在其上播放视频的设备。这些选项为“计算机”（台式机）、“移动设备”(iPhone、iPad、Android™)或“平板电脑”(仅限iPad)。 此设置会自动确定在编码期间使用的适当视频和音频编解码器。 |
   | 目标数据速率 | 输入目标最终用户的 Internet 平均连接速度（千比特/秒）。您可以输入速率，或拖动滑块进行输入。用户连接速度范围列出了宽带、DSL、移动设备和拨号连接的标准速度。此设置会自动确定组合的视频和音频数据速率。也就是构成一秒钟视频播放所编码的数据量。数据速率越高，所得到视频的品质就越高。但是，如果数据速率太高，则导致文件非常大，并导致低带宽连接的用户的观看体验欠佳。最好是在高数据速率和低数据速率之间找到一个平衡点。旨在创建优质播放体验，带宽较低的用户也能享受该体验。 |
   | 高宽比 | 高宽比是视频宽度和视频高度的比例。下面列出的前两个高宽比通常用于水平显示视频：<ul><li> 4:3 - 适用于几乎所有的标清电视广播内容。</li><li>16:9 — 用于高清电视(HDTV)上的几乎所有宽屏内容和电影。</li><li>自动缩放 -（默认）这是适用于任何高宽比的单个编码预设，可用于创建传送到移动设备、平板电脑和台式机的视频。使用该预设编码的上载的源视频将设置为固定高度。但是，自动调整宽度以保持视频的高宽比。</li><li>自定义 - 要定义非标准视频大小时使用。</li><li>您选择的纵横比决定了“分辨率大小”的宽度和高度设置；宽度和高度值会自动缩放到适当的纵横比。</li></ul> |
   | 分辨率大小 | 分辨率大小（用宽度的像素数乘以高度的像素数表示）决定大小。 以像素为单位输入宽度和高度值，或拖动滑块来输入这些值。分辨率范围列出了标准分辨率大小。宽度和高度值会自动遵循您选择的长宽比。 例如，如果您选择 4:3 作为高宽比，并且为宽度输入 400，则会自动为高度输入 300。如果为高宽比设置选择了“自动缩放”，则自动将分辨率大小的宽度值设置为“自动”。选择 **[!UICONTROL 预览]** 因此您可以打开浏览器窗口，并在其中查看解决方案选择。 |
   | 编码文件后缀 | 输入后缀。该后缀会附加到生成的编码视频文件的后面。您可以在名称中输入连字符和下划线；不允许使用空格和特殊字符。 |
   | 其他设置 | Adobe Dynamic Media Classic会根据最佳实践编码准则自动确定所有其他编码设置。 |

1. 执行以下任一操作：

   * 选择 **[!UICONTROL 保存]** 是否添加或编辑了视频预设。
   * 选择 **[!UICONTROL 另存为]** 如果您通过从现有预设开始添加视频预设。

### 删除视频编码预设 {#deleting-a-video-encoding-preset}

管理员可以删除自定义视频预设。不能删除Adobe Dynamic Media Classic附带的视频预设。

1. 在Adobe Dynamic Media Classic的全局导航栏上，转到 **[!UICONTROL 设置]** > **[!UICONTROL 应用程序设置]** > **[!UICONTROL 视频预设]**.
1. 选择 **[!UICONTROL 单个编码预设]**.
1. 在“视频预设”页中，在表格中选择不再需要的视频预设。
1. 在“视频预设”工具栏上，选择 **[!UICONTROL 删除]**.
1. 在删除预设对话框中，选择 **[!UICONTROL 删除]**.

>[!MORELIKETHIS]
>
>* [快速入门： Adobe Dynamic Media Classic中的视频](quick-start-video.md#quick-start-video)
>* [上传视频并进行编码](uploading-encoding-videos.md#uploading-and-encoding-videos)
>* [使用视频查看器预设](previewing-videos-video-viewer.md#working-with-video-viewer-presets)
>* [视频预设](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/549_video-presets_converted%20renamed_Done-AVS) 训练视频

