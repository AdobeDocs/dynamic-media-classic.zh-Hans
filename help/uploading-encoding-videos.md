---
title: 上傳並編碼視訊
description: 瞭解如何在Adobe Dynamic Media Classic中上傳視訊並進行編碼。
uuid: 9a7d6513-b10c-40b0-aebb-18a795c2b8d1
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: a0941823-850c-4373-9e37-f32032de3805
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: 93ad91d7-f3dd-484b-b62c-633fcb864bbf
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '3967'
ht-degree: 56%

---

# 上傳並編碼視訊{#uploading-and-encoding-videos}

若要建立單一視訊或自我調整視訊集以傳送至網頁或行動裝置，您必須先將主要視訊檔案上傳至Adobe Dynamic Media Classic。 Adobe Dynamic Media Classic會將視訊編碼為MP4格式，併發佈下列檔案格式的視訊：

* **MP4** - Adobe Dynamic Media Classic建議將MP4作為慣用的視訊檔案格式。 将 MP4 文件用于以下内容：

   * 桌面的 HTTP 动态流。
   * HTTP 实时流（Apple 的流协议）。
   * 漸進式視訊傳送至Android™、BlackBerry®和Windows®行動裝置

   Adobe Dynamic Media Classic提供上傳視訊檔案的兩個工作流程：

* **預先編碼的視訊**  — 您直接將MP4檔案上傳至Adobe Dynamic Media Classic。 对于该工作流程，在上载文件时，不会对文件进行编码。文件在准备传送到桌面和移动设备时进行预编码。

* **主要來源影片**  — 上傳主要來源視訊檔案，並在上傳時將這些檔案編碼為MP4檔案。 在浏览面板中，编码的视频标记为“视频”。Adobe Dynamic Media Classic支援多種格式的視訊檔案編碼。

   * 請確定您想要編碼的主要來源視訊檔案受到支援。

      请参阅[支持编码的视频文件类型](uploading-encoding-videos.md#supported-video-file-types-for-encoding)。

   * 选择一个视频编码预设。

      请参阅[用于编码视频文件的视频预设](application-setup.md#video-presets-for-encoding-video-files)。

      请参阅[视频编码最佳做法](uploading-encoding-videos.md#best-practices-for-video-encoding)。

Adobe Dynamic Media Classic也會產生視訊縮圖。 您可以了解有关视频缩略图的详细信息，如何获取其 URL 以及修改海报帧。

另請參閱 [使用視訊縮圖](deploying-video-websites-mobile-sites.md#working-with-video-thumbnails).

**上载和编码视频:**

执行以下任一操作：.

*如果您的视频已经编码*

1. 在全域導覽列上，選取 **[!UICONTROL 上傳]**.
1. 在上傳頁面中，選取 **[!UICONTROL 從案頭]** 標籤。
1. 在上傳頁面上，在 **[!UICONTROL 選取要上傳的檔案]** 面板，選取 **[!UICONTROL 瀏覽]**，導覽至MP4視訊檔案，然後選取「 」 **[!UICONTROL 開啟]**.
1. 在 **[!UICONTROL 選擇資料夾目的地]** 面板中，選取已上傳檔案的資料夾。
1. 在上傳頁面上，確認 **[!UICONTROL 上傳後發佈]** 已勾選。
1. 選取 **[!UICONTROL 提交上傳]**.

*如果您想要使用Adobe Dynamic Media Classic對視訊進行編碼*

1. 在全域導覽列上，選取 **[!UICONTROL 上傳]**.
1. 在上傳頁面中，選取 **[!UICONTROL 從案頭]** 標籤。
1. 在 **[!UICONTROL 選取要上傳的檔案]** 面板，選取 **[!UICONTROL 瀏覽]**，導覽至主要來源視訊檔案，然後選取 **[!UICONTROL 開啟]**.
1. 在 **[!UICONTROL 選擇資料夾目的地]** 面板中，選取已上傳檔案的資料夾。
1. 在頁面的右下角，選取 **[!UICONTROL 工作選項]**，
1. 在上傳工作選項對話方塊中，展開 **[!UICONTROL EVideo選項]**，然後執行下列任一項作業：

   * 最佳實務是選取 **[!UICONTROL 自我調整視訊編碼]**. 请参阅[自适应视频（默认）](application-setup.md#adaptive-video-default)。
   * 可选. 如果您想使用個別編碼設定，請展開 **[!UICONTROL 單一編碼預設集]**，然後選取您要用於「案頭」、「行動裝置」和「平板電腦」的編碼選項。
请参阅[台式机视频编码预设](application-setup.md#desktop-video-encoding-presets)、[移动设备视频编码预设](application-setup.md#mobile-video-encoding-presets)和[平板电脑视频编码预设](application-setup.md#tablet-video-encoding-presets)。
1. 在「上載工作選項」對話方塊中，選取 **[!UICONTROL 儲存]**.
1. 在上傳頁面上，確認 **[!UICONTROL 上傳後發佈]** 已勾選。
1. 在「上傳」頁面的右下角，選取 **[!UICONTROL 提交上傳]**.

*如果要重新编码以前上载的视频文件*

1. 在Adobe Dynamic Media Classic的「瀏覽」面板中，導覽至視訊並加以選取。
1. 前往 **[!UICONTROL 檔案]** > **[!UICONTROL 重新處理]**.
1. 在「重新處理資產」對話方塊中，展開 **[!UICONTROL EVideo選項]**，然後執行下列任一項作業：
   * 最佳做法是使用以下方法。选择“**自适应视频**”。请参阅[自适应视频（默认）](application-setup.md#adaptive-video-default)。
   * 可选. 如果您想使用個別編碼設定，請展開 **[!UICONTROL 單一編碼預設集]**，然後選取您要用於「案頭」、「行動裝置」和「平板電腦」的編碼選項。
请参阅[台式机视频编码预设](application-setup.md#desktop-video-encoding-presets)、[移动设备视频编码预设](application-setup.md#mobile-video-encoding-presets)和[平板电脑视频编码预设](application-setup.md#tablet-video-encoding-presets)。
1. 在「重新處理資產」對話方塊中，選取 **[!UICONTROL 提交]**.

在使用自适应视频编码预设或多个单编码预设时，结果是以多个视频编码自动创建的自适应视频集。也可以选择各个视频以手动创建自适应视频集。

只有在自动或手动生成自适应视频集时，才会创建 MP4 和 M4V 文件类型。

## 支持编码的视频文件类型 {#supported-video-file-types-for-encoding}

下表列出了在上载文件时可以编码为 MP4 或 OGV 格式的视频文件类型（包含允许的视频编解码器）。此表列出了文件格式和编码解码器：

* **視訊檔案格式**  — 與ZIP檔案類似，視訊檔案格式會決定檔案包含在視訊檔案中的方式。 视频文件通常包含多个轨道 — 一个视频轨道（没有音频）和一个或多个音频轨道（没有视频） — 这些轨道相互联系并且同步。视频文件格式决定了这些不同的数据轨道和元数据的组织方式。

* **視訊轉碼器**  — 視訊轉碼器說明視訊的編碼演演算法。 视频播放器根据其编码解码器对视频进行解码，然后在屏幕显示一系列图像或帧。编解码器将视频文件存储为播放视频所需的信息量降至最低。只会存储一个帧和下一个帧之间差异的相关信息，而不存储每个单独帧的相关信息。由於大部分的視訊在不同影格之間幾乎不會變化，轉碼器可提供高壓縮率，進而縮小檔案大小。

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
   >如果上载并尝试编码视频文件，但由于文件包含不兼容的编码解码器或文件容器而被拒绝，“作业”屏幕将发出警告。如需詳細資訊，請參閱 [檢查工作檔案](checking-job-files.md).

## 视频编码最佳做法 {#best-practices-for-video-encoding}

以下是在Adobe Dynamic Media Classic中編碼來源視訊檔案的最佳實務提示。

<!-- THE FOLLOWINGS LINKS APPEAR TO BE DEAD AND THE CONTENT COMPLETELY LOST. THE GO URL DOESN'T EVEN WORK ANYMORE.
For advice about video encoding, see the following:

* Article: [Streaming 101: The Basics — Codecs, Bandwidth, Data Rate, and Resolution][www.adobe.com/go/learn_s7_streaming101_en](https://www.adobe.com/go/learn_s7_streaming101_en). THIS MATERIAL WAS FOUND ON A THIRD PARTY WEBSITE HERE: https://streaminglearningcenter.com/articles/streaming-101-the-basics-codecs-bandwidth-data-rate-and-resolution.html MATERIAL IS GOOD BUT DO NOT LINK TO IT
* Video: [Video Encoding Basics][www.adobe.com/go/learn_s7_encoding_en](https://www.adobe.com/go/learn_s7_encoding_en). -->

### 源视频文件 {#source-video-files}

您编码视频文件时，使用可实现的最高品质的源视频文件。避免使用以前编码的视频文件，因为这些文件已经过压缩，进一步编码会创建质量达不到标准的视频。

下表說明編碼來源視訊檔案時，其建議大小、外觀比例和最低位元速率等：

| 大小 | 高宽比 | 最小比特率 |
| --- | --- | --- |
| 1024 X 768 | 4:3 | 大多数视频为 4500 kbps。 |
| 1280 X 720 | 16:9 | 3000 - 6000 kbps，具体取决于视频中动作的数量。 |
| 1920 X 1080 | 16:9 | 6000 - 8000 kbps，具体取决于视频中动作的数量。 |

### 取得檔案的中繼資料 {#obtaining-a-file-s-metadata}

您可以在Adobe Dynamic Media Classic中檢視檔案的中繼資料、使用視訊編輯工具，或使用專為取得中繼資料而設計的應用程式，以取得檔案的中繼資料。 以下是使用第三方应用程序 MediaInfo 获取视频文件元数据的说明：

1. 前往此網頁： [https://mediaarea.net/en/MediaInfo](https://mediaarea.net/en/MediaInfo).
1. 选择和下载图形界面版本的安装程序，并按安装说明操作。
1. 安裝後，請以滑鼠右鍵按一下視訊檔案(僅限Windows®)並選取MediaInfo，或開啟MediaInfo並將視訊檔案拖曳到應用程式中。 您会看到与视频文件相关的所有元数据，其中包括其宽度、高度和 fps。

### 高宽比 {#aspect-ratio}

當您選擇或建立主要視訊檔案的視訊編碼預設集時，請確定預設集具有與主要視訊檔案相同的外觀比例。 *高宽比*&#x200B;是视频宽度和视频高度的比例。

若要判斷視訊檔案的外觀比例，請取得檔案的中繼資料，並注意檔案的寬度和高度(請參閱 [取得檔案的中繼資料](uploading-encoding-videos.md#obtaining_a_file_s_metadata))。 然后，使用以下公式来确定高宽比：

宽度/高度 = 高宽比

下表描述了如何将公式结果转换为常用高宽比选项：

| 公式结果 | 高宽比 |
| --- | --- |
| 1.33 | 4:3 |
| 0.75 | 3:4 |
| 1.78 | 16:9 |
| 0.56 | 9:16 |

例如，1440寬度x 1080高度的視訊外觀比例為1440/1080，即1.33。在這種情況下，您可以選擇長寬比為4:3的視訊編碼預設集，來編碼視訊檔案。

### 数据速率 {#data-rate}

*数据速率*（也称为&#x200B;*比特率*）是用于编码以组成一秒钟视频播放的数据量。数据速率以千比特/秒 (Kbps) 为度量单位。

>[!NOTE]
>
>因为所有编码解码器使用有损压缩，所以数据速率是决定视频质量的最重要因素。使用有损压缩时，将视频文件压缩的越多，质量下降的越多。因此，所有其他特性（分辨率、帧速率和编码解码器）不变时，数据速率越低，压缩文件的质量越低。

當您選擇視訊編碼預設集時，請記得考慮目標使用者的連線速度。 选择数据速率为该速度 80% 的预设。例如，如果目标最终用户的连接速度为 1000 Kbps，最佳预设是视频数据速率为 800 Kbps 的预设。

下表描述了标准连接速度的数据速率。

| 速度 (Kbps) | 连接类型 |
| --- | --- |
| 256 | 拨号连接。 |
| 800 | 标准移动连接。对于此连接，将数据速率设定在 400 至最大值为 800 的范围内，以实现 3G 体验。 |
| 2000 | 标准带宽桌面连接。針對此連線，將資料速率目標設定在800到2000 Kbps範圍內，大部分目標平均為1200到1500 Kbps。 |
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
>一般而言，您使用的資料速率越高，視訊的顯示效果就越好，而且您使用的解析度越高，您必須維持檢視品質的資料速率就越高（與解析度較低相比）。

因为分辨率和数据速率是关联的，在编码视频时您有两个选择：

* 選擇資料速率，然後以您選擇之資料速率的最佳顯示解析度編碼。
* 选择一个分辨率，然后用在您选择的分辨率下实现高质量视频所需的数据速率编码。

當您選擇（或建立）主要視訊檔案的視訊編碼預設集時，請使用此表格來鎖定正確解析度：

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

選擇符合主要視訊檔案的fps速率的視訊編碼預設集。 例如，如果您的主要視訊是25 fps，請選擇具有25 fps的編碼預設集。 依預設，所有自訂編碼都會使用主要視訊檔案的fps。 因此，在创建视频编码预设时，您不需要明确指定 fps 设置。

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

Adobe Dynamic Media Classic建議使用MP4 H.264視訊編碼預設集。 由于 MP4 文件使用 H.264 视频编解码器，因此可以提供压缩文件大小的高品质视频。

## 使用視訊編碼預設集 {#working-with-video-encoding-presets}

使用視訊製作裝置和視訊編輯軟體建立的主要視訊檔案通常太大，而且格式不正確，無法傳送到線上目的地。 要将数字视频转换为适用于在不同屏幕上播放的适当格式和规格，您可以将视频文件&#x200B;*转码*（此过程也称为&#x200B;*编码*）。在编码过程中，视频将压缩为最适合传送到网站和移动设备的较小且有效的文件大小。

另請參閱 [上傳並編碼視訊](uploading-encoding-videos.md#uploading-and-encoding-videos).

Adobe Dynamic Media Classic提供您預先定義的視訊編碼預設集資料庫，可反映目前最常用的編碼設定。 这些编码预设针对在目标屏幕上播放进行了优化。此外，管理员还可以创建自己的视频编码预设，以便为最终用户自定义视频大小和播放质量。所有視訊編碼預設集，無論是來自Adobe Dynamic Media Classic的現成可用或自訂的，都會以MP4檔案格式輸出視訊。

在“视频预设”屏幕上，管理员可以设置和管理视频编码。他们可以执行以下操作：

* 激活和停用视频编码预设。
* 创建视频编码预设。
* 编辑视频编码预设。
* 删除视频预设。

上傳至Adobe Dynamic Media Classic或在Adobe Dynamic Media Classic中編碼的任何視訊都會視為「視訊」。 即此资源类别表示您可以传送此视频以便在桌面、移动设备或同时在两者上播放。例如，您可以在Adobe Dynamic Media Classic中預覽這些型別的影片。 也可以生成 URL（使用复制 URL）和可嵌入的代码（使用嵌入代码）以用于视频播放器、网站，等等。

另請參閱 [在視訊檢視器中預覽視訊](previewing-videos-video-viewer.md#previewing-videos-in-a-video-viewer).

另請參閱 [將視訊URL連結至行動網站或網站](deploying-video-websites-mobile-sites.md#linking-a-video-url-to-a-mobile-site-or-a-website).

另請參閱 [將視訊檢視器內嵌在網頁上](deploying-video-websites-mobile-sites.md#embedding-the-video-viewer-on-a-web-page).

對於您在Adobe Dynamic Media Classic中上傳和編碼的視訊資產，會以下列檔案格式傳送視訊：

**MP4 H.264** 將MP4檔案用於下列專案：

* 桌面的 HTTP 动态流。
* HLS (HTTP即時資料流、Apple的資料流通訊協定)。
* 漸進式視訊傳送至Android™、BlackBerry®和Windows®行動裝置。

任何其他視訊格式及轉碼器會視為「主要視訊」。 此资源类别表示此类视频为源视频文件，无法进行传送以便在桌面或移动设备上播放。例如，您無法在Adobe Dynamic Media Classic中預覽這些型別的影片。 您也无法生成复制 URL 和嵌入代码，以便在视频播放器、网站等平台上使用。

### 篩選視訊編碼預設集清單 {#filtering-the-list-of-video-encoding-presets}

「視訊預設集」頁面和「自我調整視訊預設集」頁面包含一個表格，其中列出作用中狀態、預設集名稱、預期的播放裝置、視訊大小和每個視訊預設集的資料速率。

您可以选择按“两者全部”、“活动”或“非活动”进行过滤以优化列表，以便查看所有视频预设或将列表范围缩小为活动或非活动预设。

也可以根据播放设备选项进行过滤，将列表范围缩小为用于在所有设备、台式机、移动设备或平板电脑上播放视频的视频预设。

**过滤视频编码预设列表:**

1. 在Adobe Dynamic Media Classic中的全域導覽列上，前往 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 視訊預設集]** > **[!UICONTROL 最適化視訊預設集]** 或 **[!UICONTROL 單一編碼預設集]**.

   「自我調整視訊預設集」和「單一編碼預設集」頁面包含一個表格，其中列出「作用中」狀態、預設集名稱、預期的播放裝置、視訊維度和每個視訊預設集的資料速率。

1. 在“视频预设”工具栏上的“单个编码预设”页中，使用两个下拉列表根据活动状态和播放设备优化表格中的预设列表。

   * 在第一个较小的下拉列表中，选择“**[!UICONTROL 两者全部]**”以查看所有视频预设，或者选择“**[!UICONTROL 活动]**”或“**[!UICONTROL 非活动]**”以将列表范围缩小为活动或非活动预设。
   * 在第二个较大的下拉列表中，选择一个播放设备选项以将列表范围缩小为用于在台式机、移动设备或平板设备上播放视频的视频预设。

### 啟用或停用視訊編碼預設集 {#activating-or-deactivating-video-encoding-presets}

激活的视频预设将显示在“上载作业选项”对话框中。當使用者在上傳過程中上傳視訊檔案時，會出現此對話方塊。 他们可以从所有激活的编码预设列表中进行选择。

1. 在Adobe Dynamic Media Classic中的全域導覽列上，前往 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 視訊預設集]**.
1. 执行以下任一操作：

   * 選取 **[!UICONTROL 最適化視訊預設集]**.
   * 選取 **[!UICONTROL 單一編碼預設集]**.

1. 执行以下任一操作：

   * 要激活某个视频预设，请在“预设”页中的“活动”列下面，选中预设名称旁边的复选框。
   * 要停用视频预设，请取消选中要停用的视频预设旁边的框。

      >[!NOTE]
      >
      >非活动视频预设不会显示在“上载作业选项”对话框中。

1. 在頁面的右下角，選取 **[!UICONTROL 關閉]**.

### 新增或編輯視訊編碼預設集 {#adding-or-editing-a-video-encoding-preset}

您可以建立自己的自訂單一編碼視訊預設集，並將其新增至「視訊預設集」表格。 您也可以變更Adobe Dynamic Media Classic隨附的任何預先定義單一編碼視訊預設集，前提是您以新名稱儲存編輯的預設集。

Adobe Dynamic Media Classic已設定目標資料速率、解析度高度和解析度寬度的最大限制，以確保適當的播放體驗。 如果超过以下限制，则会显示警告消息：

* 電腦播放的限製為： （寬度/16） &#42; (Height/16) &lt; 8192。
* 行動播放的限製為： （寬度/16） &#42; （高度/16） &lt; 660；目標資料速率&lt; 4000。
* 平板電腦播放的限製為：（寬度/16） &#42; (Height/16) &lt; 3600。

**添加或编辑视频编码预设:**

1. 在Adobe Dynamic Media Classic中的全域導覽列上，前往 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 視訊預設集]**.
1. 選取 **[!UICONTROL 單一編碼預設集]**.
1. 在“视频预设”页中，执行以下操作之一：

   * 在「視訊預設集」工具列上，選取 **[!UICONTROL 新增]** 以便新增視訊預設集。
   * 选择一个视频预设。在工具列中，選取 **[!UICONTROL 編輯]**.

      您無法編輯Adobe Dynamic Media Classic預先定義的預設集；您只能通過選擇從現有預設集建立預設集 **[!UICONTROL 另存為]**.

1. 在“添加视频预设”或“编辑视频预设”页中，设置所需的视频预设选项。

   有关建议的设置，请参阅[视频编码最佳做法](uploading-encoding-videos.md#best-practices-for-video-encoding)。

   | 视频预设选项 | 说明 |
   | --- | --- |
   | 预设名称 | 输入视频预设的描述性名称。您输入的名称显示在“上载作业选项”对话框中，用户在此对话框中选择转码选项。 |
   | 说明 | 描述视频预设。當您將指標移到「上載工作選項」對話方塊中的預設集名稱上時，您輸入的內容會顯示為工具提示，使用者可在其中選擇轉碼選項。 |
   | 播放设备 | 选择要在其上播放视频的设备。選項包括「電腦」（桌上型電腦）、「行動」(iPhone、iPad、Android™)或「平板電腦」(僅限iPad)。 此设置会自动确定在编码期间使用的适当视频和音频编解码器。 |
   | 目标数据速率 | 输入目标最终用户的 Internet 平均连接速度（千比特/秒）。您可以输入速率，或拖动滑块进行输入。用户连接速度范围列出了宽带、DSL、移动设备和拨号连接的标准速度。此设置会自动确定组合的视频和音频数据速率。也就是构成一秒钟视频播放所编码的数据量。数据速率越高，所得到视频的品质就越高。但是，如果数据速率太高，则导致文件非常大，并导致低带宽连接的用户的观看体验欠佳。最好是在高数据速率和低数据速率之间找到一个平衡点。旨在创建优质播放体验，带宽较低的用户也能享受该体验。 |
   | 高宽比 | 高宽比是视频宽度和视频高度的比例。下面列出的前两个高宽比通常用于水平显示视频：<ul><li> 4:3 - 适用于几乎所有的标清电视广播内容。</li><li>16:9 — 用於高解析度電視(HDTV)上的幾乎所有寬熒幕內容和電影。</li><li>自动缩放 -（默认）这是适用于任何高宽比的单个编码预设，可用于创建传送到移动设备、平板电脑和台式机的视频。使用该预设编码的上载的源视频将设置为固定高度。但是，自动调整宽度以保持视频的高宽比。</li><li>自定义 - 要定义非标准视频大小时使用。</li><li>您選擇的外觀比例會決定「解析度大小」的寬度和高度設定；寬度和高度值會自動縮放到適當的外觀比例。</li></ul> |
   | 分辨率大小 | 解析度大小（以寬畫素數乘以高畫素數表示）決定大小。 以像素为单位输入宽度和高度值，或拖动滑块来输入这些值。分辨率范围列出了标准分辨率大小。寬度和高度值會自動符合您選取的外觀比例。 例如，如果您选择 4:3 作为高宽比，并且为宽度输入 400，则会自动为高度输入 300。如果为高宽比设置选择了“自动缩放”，则自动将分辨率大小的宽度值设置为“自动”。選取 **[!UICONTROL 預覽]** 因此您可以開啟瀏覽器視窗，並在其中檢視您的解決方案選擇。 |
   | 编码文件后缀 | 输入后缀。该后缀会附加到生成的编码视频文件的后面。您可以在名称中输入连字符和下划线；不允许使用空格和特殊字符。 |
   | 其他设置 | Adobe Dynamic Media Classic會根據最佳實務編碼准則，自動決定所有其他編碼設定。 |

1. 执行以下任一操作：

   * 選取 **[!UICONTROL 儲存]** 如果您已新增或編輯視訊預設集。
   * 選取 **[!UICONTROL 另存為]** 如果您是從現有的預設集開始新增「視訊預設集」。

### 刪除視訊編碼預設集 {#deleting-a-video-encoding-preset}

管理员可以删除自定义视频预设。Adobe Dynamic Media Classic隨附的視訊預設集無法刪除。

1. 在Adobe Dynamic Media Classic中的全域導覽列上，前往 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 視訊預設集]**.
1. 選取 **[!UICONTROL 單一編碼預設集]**.
1. 在“视频预设”页中，在表格中选择不再需要的视频预设。
1. 在「視訊預設集」工具列上，選取 **[!UICONTROL 刪除]**.
1. 在「刪除預設集」對話方塊中，選取 **[!UICONTROL 刪除]**.

>[!MORELIKETHIS]
>
>* [快速入門： Adobe Dynamic Media Classic中的影片](quick-start-video.md#quick-start-video)
>* [上傳並編碼視訊](uploading-encoding-videos.md#uploading-and-encoding-videos)
>* [使用視訊檢視器預設集](previewing-videos-video-viewer.md#working-with-video-viewer-presets)
>* [視訊預設集](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/549_video-presets_converted%20renamed_Done-AVS) 訓練影片

