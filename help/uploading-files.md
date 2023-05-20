---
title: 上载文件
description: 瞭解如何在Adobe Dynamic Media Classic中上傳檔案。
uuid: b3025f84-4f28-4276-bc9c-f0c0c2a26e12
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: b2bc3bf9-e313-481a-8670-c3bedde21b1a
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 8dfcfb3f-6472-4efd-bc87-d5111eee45ce
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '3929'
ht-degree: 31%

---

# 上载文件{#uploading-files}

在將資產檔案上傳至Adobe Dynamic Media Classic之前，請確定資產檔案已正確命名，且您的資料夾結構已依您想要的方式設定和組織。 您可以從Adobe Dynamic Media Classic提供的FTP站台上傳檔案，也可以直接從您的電腦或網路上傳檔案。 Adobe Dynamic Media Classic提供上傳檔案時最佳化檔案的選項。 如果您已安裝Adobe Dynamic Media Classic案頭應用程式，則可直接從案頭拖曳檔案和資料夾，即可將其上傳。 请参阅[应用程序常规设置](application-setup.md#general_settings)。

## 準備資產和資料夾以進行上傳 {#preparing-your-assets-and-folders-for-uploading}

將資產上傳至Adobe Dynamic Media Classic之前，請確定它們的格式和大小正確。 您也必須遵守資產命名的Adobe Dynamic Media Classic規則。 通过设置文件的文件夹组织和结构，可确保可以轻松定位及处理文件。

### 支持的资源文件格式 {#supported-asset-file-formats}

下表列出Adobe Dynamic Media Classic支援的資產檔案格式。 如需有關支援的Camera Raw檔案的資訊，請參閱 [https://helpx.adobe.com/camera-raw/using/supported-cameras.html](https://helpx.adobe.com/camera-raw/using/supported-cameras.html).

| 资源文件格式 | 说明 |
| --- | --- |
| 音频 | AAC、HE-AAC、AC3、WAV、WMA、AIFF、MP3 |
| 级联样式表 | CSS |
| 颜色配置文件 | ICC、ICM |
| 字体 | AFM、OTF、PFB、PFM、PhotoFont、TTC、TTF |
| FXG | FXG |
| Illustrator | AI、FXG |
| 图像 | BMP、FPX、GIF、JPEG、JPG、PNG、PICT (僅限Windows®)、TIF、TIFF |
| InDesign | INDD、INDT |
| MS® Office | DOC、PPT、RTF、XLS |
| PDF | PDF |
| Photoshop | PSD、FXG 和 Camera Raw |
| PostScript | EPS、PS |
| Adobe Dynamic Media Classic影像製作 | VNC、VNT、VNW |
| SVG | SVG、SVGX |
| TAR | TAR |
| 视频 | 3GP、AVI、M2P、M2T、M2TS、M2V、M4V、MOV、MP4、MPEG、MPG、MTS、OGV、TS、VOB、WMV/ASF |
| XML | XML |
| ZIP | ZIP |

TAR 和 ZIP 上载支持包括一个复选框，用于选择是否要解压缩文件。

### Dynamic Media不支援的影像格式 {#unsupported-image-formats-dynamic-media}

下列清單說明點陣影像檔案格式的子型別 *not* 在Dynamic Media中支援。

另請參閱 [偵測Dynamic Media不支援的檔案格式](https://helpx.adobe.com/experience-manager/kb/detect-unsupported-assets-for-dynamic-media.html).

* IDAT區塊大小大於100 MB的PNG檔案。
* PSB檔案。
* 不支援色彩空間不是CMYK、RGB、灰階或點陣圖的PSD檔案。 不支援DuoTone、Lab和索引色域。
* 位元深度大於16的PSD檔案。
* TIFF含有浮點資料的檔案。
* TIFF具有Lab色域的檔案。

### 资源类型 {#asset-types}

若要使用Adobe Dynamic Media Classic程式取得最佳結果，請務必使用建議的檔案格式和大小。 下表列出了资源类型，其中一些资源类型列有常用资源的推荐格式和文件大小。

| 资源类型 | 说明/推荐 |
| --- | --- |
| 音频 | 输入音频资源格式，其中包括 AAC、HE-AAC、AC3、WAV、WMA、AIFF、MP3。可以将音频转码为以下格式：MP3、AAC 和 HE-AAC。 |
| 图像（用于调整图像大小、缩放、图像集、旋转集） | 最大大小的影像必須至少為2000畫素；最大大小的典型影像大小範圍是1500到2500畫素。 推荐使用无损图像格式，包括 TIFF 和 PNG 文件。如果使用 JPEG 图像，请使用最高质量设置。處理動畫GIF檔案的方式與其他靜態內容相同。 |
| eCatalog | 使用在Adobe Acrobat中建立的高解析度PDF檔案，或是儲存為「備妥」的AdobeCreative Suite應用程式。 PDF 包括所有需要的字体、图像、蒙版以及引用的图形元素，采用单页、两页跨页或多页格式。通过按字母数字顺序为文件命名来排列页面顺序。将 eCatalog 类型的所有 PDF 文件放于一个文件夹中，以便于上载。您可以在上载时选择裁切选项，以便从 PDF 中删除修剪区域，包括裁切标记、对齐目标或颜色条。多数印刷就绪的 PDF 文件采用 CMYK 颜色空间，因此务必要获得用于 PDF 文件的 CMYK ICC 颜色配置文件。 |
| 模板 | 分层图像或布局设计，可以包括文本、图像和图层。可以将图层、文本字符串和属性（如颜色和大小）参数化，从而可以自定义变量数据。在模板中使用时的图像要求与其他图像相同。在 Photoshop 或其他图像编辑程序中准备图形。采用 TIFF 或 PNG 格式将每个图形保存为平面化透明文件。确保图像分辨率适合所要求的用途。列印影像為300 ppi。 |
| 视频 | Adobe Dynamic Media Classic支援以OGV和MP4格式儲存的視訊檔案。 您可以在上载时将文件转码为 MP4 格式。请参阅[支持的资源文件格式](#supported-static-file-formats)。 |
| 字体 | 已上傳TrueType、Type1 (僅限Windows®)、OpenType®字型和PhotoFonts。 |
| 图像 | 图像和分层图像文件。 |
| 图像集和样本集 | 可以显示在查看器中的一组相关图像。 |
| ICC 配置文件 | 一種色彩設定檔，可用來將上傳的影像從來源色域轉換為不同的色域。 |
| 晕影 | 使用影像製作程式製作的影像和相關檔案。 |
| 内容文件 | Adobe InDesign、Illustrator 或 Photoshop 内容文件。 |
| FXG 文件 | 与分辨率无关的图形格式文件；可用于创建可自定义的模板，以输出到打印、网络、电子邮件、桌面和设备。 |
| SVG 文件 | 图像服务服务器可以渲染的可缩放矢量图形文件。 |
| XML 文件 | 定义用于修改请求的路径和查询部分的预处理规则的文件。 |
| 级联样式表文件。 | 上载用于自定义 HTML5 查看器的 CSS 外观。 |
| JavaScript 文件 | JavaScript檔案用於viewer instrumentation以儲存帳戶資訊。 Adobe安全性建議僅針對使用不同網域進行傳送的使用者端帳戶使用此資產型別（以避免跨網站指令碼）。 |

>[!NOTE]
>
>當您將影像檔案和PDF上傳到Adobe Dynamic Media Classic時，系統將這些來源檔案轉換為PTIFF(金字塔TIFF)檔案。 這些PTIFF是稍後發佈至Dynamic Media影像伺服器的檔案。 Adobe Dynamic Media Classic使用「金字塔Tiff」檔案格式，因為它包含各種縮放比例，以便在使用Adobe Dynamic Media Classic縮放檢視器檢視時可快速縮放。

### 支持静态文件格式 {#supported-static-file-formats}

Adobe Dynamic Media Classic支援多種靜態檔案格式。 靜態內容是以「原樣」發佈的任何資產，例如CSS、PDF、SVG和XML。

可以发布以下文件类型：

* GIF 动画
* 音频文件
* CSS
* JavaScript（为公司配置自己的域时）
* 主要影片
* PDF(當PDF在上傳後標籤為發佈時，以避免交付現有eCatalog/PDF工作流程的所有PDF)
* PrX 视频
* SVG
* XML
* ZIP

Adobe Dynamic Media Classic不提供產生靜態內容預覽URL的選項。

### 文件名要求 {#filename-requirements}

由于在文件上载过程中将去除文件名中的扩展名，因此系统不允许文件使用相同的根名称。在Adobe Dynamic Media Classic系統中，資產檔案名稱減去副檔名後，即為資產的資產ID。 因此，两个资源不能同名。

請確定貴公司的所有使用者都瞭解這些檔案命名規則：

* 系统中不允许存在名称完全相同的资源 ID。
* 資產ID名稱會區分大小寫。
* 最佳做法是确保资源 ID 不包含空格（例如 black jacket.tif 和 blue jacket.jpg）。Adobe Dynamic Media Classic使用資產名稱來建構URL字串時，會對資產名稱中的空白進行ASCII編碼。 这些 ASCII 编码不易理解，从而使 URL 更难理解。
* 文件名中允许特定语言字符。但是，文件名中不能出现以下字符：

   \ ; / ? : @ &amp; = + $ , &#42; &quot; &lt; > | &#39; { } %

   如果文件名包含一个或多个上述字符，将会在上载时删除这些字符。

通常，資產檔案名稱可以與其料號、產品SKU或其他名稱相同，如下所示：

| 商品 | 文件名 | 资源 ID |
| --- | --- | --- |
| 896649 | 896649.jpg | 896649 |
| 48A3_2X | 48A3_2X.tif | 48A3_2X |

### 文件夹组织和结构 {#folder-organization-and-structure}

上傳內容至系統之前，先在Adobe Dynamic Media Classic中組織和建構內容的資料夾和子資料夾。 采用这种方式提前进行规划主要有两个好处：

* 透過FTP將內容上傳至Adobe Dynamic Media Classic時，您可以指示系統在上傳期間復寫您的資料夾結構。 如此一來，您的內容就會在Adobe Dynamic Media Classic中與在您電腦或網路上的資料夾和子資料夾中加以整理。 (若要在Adobe Dynamic Media Classic中復寫資料夾結構，請在透過FTP上傳資產時選取「包含子資料夾」選項。)
* 与在开始就使用经过仔细计划的文件夹结构相比，在文件上载之后重新对系统内的文件夹进行组织要困难得多。

您選擇在Adobe Dynamic Media Classic上儲存內容的資料夾命名方法和結構取決於貴組織的需求。 以下是一些文件夹结构示例：

**以SKU為基礎**  — 資料夾會根據SKU或專案編號命名。 例如，为所有以 0、20、30 开头的编号序列分别创建单独的文件夹。

**品牌型**  — 針對擁有多個品牌線的製造商和銷售其他公司品牌的銷售商，將檔案分割成不同品牌的產品資料夾。

**以專案為基礎**  — 根據轉出/放置日期或專案名稱來組織資料夾。 主要生成 eCatalog 的客户喜欢使用这种方法。

**網站資料夾階層的映象**  — 此資料夾結構會映象網站的資料夾結構，例如產品類別的資料夾名稱為時。

## 關於上傳檔案 {#uploading-your-files}

可以从桌面上载单个文件或通过 FTP 上载文件夹。如果您想要上傳超過100 MB的檔案或上傳整個資料夾和子資料夾，請選取 **透過FTP** 標籤。

Adobe Dynamic Media Classic會傳送電子郵件給您，以確認上傳工作開始和結束的時間，並通知您發生任何問題。

在大型上載工作期間（或緊接在其後），某些新專案可能會顯示「影像尚未最佳化」訊息。 出現此訊息是因為檔案尚未完全處理並新增至Adobe Dynamic Media Classic。 您可以稍后优化这些文件。另請參閱 [最佳化檔案](application-setup.md#optimize_files).

### 使用「從案頭」標籤上傳檔案 {#upload-files-using-sps-desktop-application}

Adobe Dynamic Media Classic案頭應用程式可讓您透過拖曳方式來上傳檔案和資料夾。

1. 在Adobe Dynamic Media Classic案頭應用程式中，於全域導覽列上選取 **[!UICONTROL 上傳]**.
1. 在上傳頁面上，選取 **[!UICONTROL 從案頭]** 標籤。
1. 在「上傳」頁面的左側，在 **[!UICONTROL 選取要上傳的檔案]** 區域，選取 **[!UICONTROL 瀏覽]** 以選取您要上傳的檔案或資料夾，然後選取 **[!UICONTROL 開啟]**.
1. 在上傳頁面的右側，在 **選擇資料夾目的地** 區域，導覽至您想要新增已上傳檔案或資料夾的目標資料夾。
1. （選擇性）在「上傳」頁面底部附近的「工作名稱」文字欄位中，輸入上傳工作的新名稱。 或者，您只需使用Adobe Dynamic Media Classic提供的預設系統產生名稱。 将在“作业”页中记录此作业和其他上载和发布作业，可以在此页中检查作业的状态。请参阅[检查作业文件](checking-job-files.md#checking_job_files)。
1. （選用）在上傳頁面底部附近，選取 **[!UICONTROL 上傳後發佈]** 如果您想要自動發佈您上傳的資產。
在发布文件时，文件将发送到实时服务器。然后，可以在外部网站和应用程序中使用这些文件的 URL。「工作選項」對話方塊中也提供相同選項。
1. （選用）在上傳頁面底部附近，選取 **[!UICONTROL 任何檔案夾內若有基本資產名稱相同者（無論副檔名為何），將予以覆寫]** 如果您希望上傳的檔案以相同名稱取代現有檔案。 「工作選項」對話方塊中也提供相同選項。
此選項的名稱可能會有所不同，視中的設定而定 **[!UICONTROL 應用程式設定]** > **[!UICONTROL 一般設定]** > **[!UICONTROL 上傳至應用程式]** > **[!UICONTROL 覆寫影像]**.
1. 在「上傳」頁面的右下角附近，選取 **[!UICONTROL 工作選項]**，然後指定您想要的選項。

   请参阅[上载选项](uploading-files.md#upload_options)。

1. 在「上載工作選項」對話方塊中，選取 **[!UICONTROL 儲存]**.
1. 在「上傳」頁面的右下角，選取 **[!UICONTROL 提交上傳]**.
若要檢視上傳進度，請選取 **[!UICONTROL 工作]** 全域導覽列上。 您可以繼續在Adobe Dynamic Media Classic中工作，並隨時返回「工作」頁面來檢閱進行中的工作。 要取消正在进行的上载作业，请选择“持续时间”旁边的“**[!UICONTROL 取消]**”。

### 使用「透過FTP」索引標籤上傳檔案 {#upload-files-using-via-ftp}

1. 登入特定地區的Adobe Dynamic Media Classic FTP網站。 使用您从管理员那里收到的 FTP 用户名和密码。
1. 在Adobe Dynamic Media Classic中的全域導覽列上，選取「 」 **[!UICONTROL 上傳]**.
1. 在上傳頁面上，選取 **[!UICONTROL 透過FTP]** 標籤。
1. 在「上傳」頁面的左側，在 **[!UICONTROL 選擇要上傳的FTP資料夾]** 區域，選擇要從中上傳檔案的FTP資料夾。
1. 在上傳頁面的右側，在 **[!UICONTROL 選擇AdobeDynamic Media資料夾目的地]** 區域，選擇Adobe Dynamic Media Classic中的目的地資料夾。
1. （選擇性）在「上傳」頁面底部附近的「工作名稱」文字欄位中，輸入上傳工作的新名稱。 或者，您只需使用Adobe Dynamic Media Classic提供的預設系統產生名稱。 将在“作业”页中记录此作业和其他上载和发布作业，可以在此页中检查作业的状态。请参阅[检查作业文件](checking-job-files.md#checking_job_files)。
1. （選用）在上傳頁面底部附近，選取 **[!UICONTROL 上傳後發佈]** 如果您想要自動發佈您上傳的資產。
在发布文件时，文件将发送到实时服务器。然后，可以在外部网站和应用程序中使用这些文件的 URL。「工作選項」對話方塊中也提供相同選項。
1. （選用）在上傳頁面底部附近，選取 **[!UICONTROL 任何檔案夾內若有基本資產名稱相同者（無論副檔名為何），將予以覆寫]** 如果您希望上傳的檔案以相同名稱取代現有檔案。 「工作選項」對話方塊中也提供相同選項。
此選項的名稱可能會有所不同，視中的設定而定 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 一般設定]** > **[!UICONTROL 上傳至應用程式]** > **[!UICONTROL 覆寫影像]**.
1. 選擇性；只有當您按一下 **[!UICONTROL 透過FTP]** 標籤。 在上傳頁面底部附近，選取 **[!UICONTROL 上傳時解壓縮Zip或Tar檔案]** 如果您想從上傳的ZIP或TAR檔案中自動解壓縮所有檔案。 「工作選項」對話方塊中也提供相同選項。
1. 在「上傳」頁面的右下角附近，選取 **[!UICONTROL 工作選項]**，然後指定您想要的選項。

   请参阅[上载选项](uploading-files.md#upload_options)。

1. 在「上載工作選項」對話方塊中，選取 **[!UICONTROL 儲存]**.
1. 在「上傳」頁面的右下角，選取 **[!UICONTROL 提交上傳]**.

   若要檢視上傳進度，請在全域導覽列上選取 **[!UICONTROL 工作]**. “作业”页将显示上载进度。您可以繼續在Adobe Dynamic Media Classic中工作，並隨時返回「工作」頁面來檢閱進行中的工作。

要取消正在进行的上载作业，请选择“持续时间”旁边的“**[!UICONTROL 取消]**”。

## 上載工作選項對話方塊 {#upload-options}

上傳檔案時，您可以在「上傳工作選項」對話方塊中選擇以下選項：

* **工作**  — 選取 **[!UICONTROL 工作]** 以選擇影響整個上載工作的選項。

   您也可以選擇 *預設* 使用上傳作業的選項 **[!UICONTROL 預設上傳選項]** 對話方塊。 前往 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 一般設定]** > **[!UICONTROL 預設上傳選項]**，然後設定您想要的預設選項。

   * **[!UICONTROL 時間]**  — 只有當您選取 **[!UICONTROL 透過FTP]** 標籤。
      * **[!UICONTROL 一次性]**  — 指定執行一次的上傳工作。 選項包括：
         * **[!UICONTROL 現在]**  — 選取後立即執行上載工作 **[!UICONTROL 儲存]** 在「上載工作選項」對話方塊中，然後選取 **[!UICONTROL 提交上傳]** （在上傳頁面上）。
         * **[!UICONTROL 排程供日後使用]**  — 選取您要執行上載工作的年、月、日和時間（以15分鐘為增量）。
      * **[!UICONTROL 週期性]**  — 指定每日、每週或每月執行的上傳工作。 或者，根據您自己的規格自訂上載工作。
         * **[!UICONTROL 每日]**  — 設定每天要執行工作的時間。 如果您希望工作只在星期一到星期五執行，請選取 **[!UICONTROL 僅限工作日]**.
         * **[!UICONTROL 每週]**  — 選擇您想要執行工作的一週中的特定日和時間。
         * **[!UICONTROL 每月]**  — 選擇您想要執行工作的特定日期（當月或當週某日），包括開始時間。
         * **[!UICONTROL 自訂]**  — 根據您自己的規格自訂上載或發佈工作時間間隔。 另請參閱 [建立自訂上載或發佈工作時間間隔](checking-job-files.md#creating-a-custom-upload-or-publish-job-time-interval).
   * **[!UICONTROL 上傳後發佈]**  — 若您選取 **[!UICONTROL 從案頭]** 標籤或 **[!UICONTROL 透過FTP]** 標籤。 选择此选项以自动发布上载的资源。在发布文件时，文件将发送到实时服务器。然后，可以在外部网站和应用程序中使用这些文件的 URL。“上载”页中也提供了该选项。

   * **[!UICONTROL 任何檔案夾內若有基本資產名稱相同者（無論副檔名為何），將予以覆寫]**  — 若您選取 **[!UICONTROL 從案頭]** 標籤或 **[!UICONTROL 透過FTP]** 標籤。 如果要使上载的文件替换现有同名文件，请选中此选项。“上载”页中也提供了该选项。此選項的名稱可能會有所不同，視中的設定而定 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 一般設定]** > **[!UICONTROL 上傳至應用程式]** > **[!UICONTROL 覆寫影像]**.

   * **[!UICONTROL 上傳時解壓縮Zip或Tar檔案]**  — 若您選取 **[!UICONTROL 從案頭]** 標籤或 **[!UICONTROL 透過FTP]** 標籤。
如果您想要自動從上傳的ZIP或TAR檔案解壓縮所有檔案，請選取此選項。 「工作選項」對話方塊中也提供相同選項。

   * **[!UICONTROL 包含子資料夾]**  — 僅當您選取 **[!UICONTROL 透過FTP]** 標籤。
如果要上载文件夹的子文件夹，请选中此选项。您上傳的資料夾及其子資料夾的名稱會自動在Adobe Dynamic Media Classic中輸入。

   * **[!UICONTROL 處理中繼資料檔案]**  — 僅當您選取 **[!UICONTROL 透過FTP]** 標籤。 如果要上载制表符分隔的文件或 XML 文件以将元数据添加到多个资源中，可以选择该选项。请参阅[导入元数据（通过 FTP）](viewing-adding-exporting-metadata.md#import-metadata)。


* **裁切選項**  — 若要自動裁切影像中的空白畫素，請開啟 **[!UICONTROL 裁切]** 功能表，選取 **[!UICONTROL 手動]**，並在「上」、「右」、「下」和「左」文字欄位中輸入畫素度量，從側面裁切。 您也可以選取 **[!UICONTROL Trim]** 在「裁切」選單上，選擇下列選項：

   * **[!UICONTROL 修剪依據]**  — 選擇根據顏色或透明度裁切：
      * **[!UICONTROL 顏色]**  — 選擇「顏色」選項。 然后选择“角”菜单，并选择所具有的颜色能最好地表示您想要裁切的空白颜色的图像角。基于颜色修剪：指定 0 则仅当像素与您在图像的角中选择的颜色完全匹配时才会裁切像素。数字越接近 1，允许的色差越大。
      * **[!UICONTROL 透明度]**  — 選擇 **[!UICONTROL 透明度]** 選項。
根據透明度裁剪：指定0可裁切透明畫素；數字越接近1則透明度越高。
      * **[!UICONTROL 容許度]**  — 拖曳滑桿以指定從0到1的公差。

* **色彩設定檔選項**  — 當您建立用於Adobe Dynamic Media Classic動態傳送的最佳化檔案時，請選擇色彩轉換：

   * **[!UICONTROL 預設色彩儲存]**  — 當影像包含色域資訊時，維持來源影像色彩；沒有色彩轉換。 几乎目前的所有图像都嵌入了相应的颜色配置文件。不过，如果 CMYK 源图像不包含嵌入的颜色配置文件，则会将颜色转换为 sRGB（标准红绿蓝）色彩空间。在网页上显示图像时，推荐使用 sRGB 颜色空间。
   * **[!UICONTROL 保留原始色域]**  — 保留原始顏色，在擷取至Adobe Dynamic Media Classic時不會進行任何顏色轉換。 對於沒有內嵌色彩設定檔的影像，處理影像要求所需的任何色彩轉換都是使用在「發佈」設定中設定的預設色彩設定檔來完成。 這些色彩設定檔並不總是與使用此選項建立的檔案中的色彩一致。 因此，建议您使用“默认护色”选项。
   * **[!UICONTROL 自訂來源]** > **[!UICONTROL 至]**  — 開啟功能表，讓您選擇 **[!UICONTROL 轉換自]** 和 **[!UICONTROL 轉換為]** 色域。 此高级选项覆盖在源文件中嵌入的任何颜色信息。只有在您要提交的所有影像包含不正確或遺失色彩設定檔資料時，才選取此選項。

* **影像編輯選項**  — 您可以保留影像中的剪裁&lt;>遮色片，並選擇色彩設定檔。
另請參閱 [上傳時影像微調選項](image-editing-options-upload.md#image-editing-options-at-upload).

* **PostScript®選項**  — 您可以點陣化PostScript®檔案、裁切檔案、保留透明背景、選擇解析度，以及選擇色域。
另請參閱 [使用PostScript和Illustrator檔案](postscript-illustrator-files.md#working_with_postscript_and_illustrator_files).

* **Photoshop選項**  — 您可以從Adobe® Photoshop®檔案建立範本、維護圖層、指定圖層的命名方式、擷取文字，以及指定影像錨定到範本的方式。
请参阅[PSD 上载选项](psd-files.md#psd_upload_options)。

* **PDF選項**  — 您可以點陣化檔案、擷取搜尋字詞和連結、自動產生eCatalog、設定解析度，以及選擇色域。
请参阅[PDF 上载选项](pdfs.md#pdf_upload_options)。

* **Illustrator選項**  — 您可以點陣化Adobe Illustrator®檔案、保留透明背景、選擇解析度以及選擇色域。
另請參閱 [使用PostScript和Illustrator檔案](postscript-illustrator-files.md#working_with_postscript_and_illustrator_files).

* **EVIDEO選項**  — 您可以選擇視訊預設集，將視訊檔案轉碼。
另請參閱 [使用視訊編碼預設集](uploading-encoding-videos.md#working_with_video_encoding_presets).

* **其他中繼資料**  — 輸入說明您要上傳之檔案的關鍵字。 用逗号分隔关键字。关键字简化了资源搜索。另請參閱 [執行進階搜尋](searching-assets.md#conducting_an_advanced_search). 另請參閱 [上傳關鍵字](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/548_upload-keywords_converted%20renamed_Done-AVS) 訓練影片。

* **批次集預設集**  — 如果要從上傳的檔案建立影像集、迴轉集或色票集，請選取 **[!UICONTROL 作用中]** 欄中選取您要使用的預設集。 可以选择多个预设。您可以在“应用程序设置/批量集预设”页中创建预设。请参阅[批量级预设](application-setup.md#batch_set_presets)。

* **進階**  — 請參閱 [上載後執行其他工作](uploading-files.md#follow-an-upload-with-another-job).

## 上载后执行其他作业 {#follow-an-upload-with-another-job}

使用FTP上傳專案時，您可以排程後續工作，以便在上傳完成時開始。 如果排程開始其他工作，您在此排程的工作會在它們之後排入佇列。

新工作會將通知傳送至您指定的地址，以便觸發該位置的代碼。 该后续发布作业所使用的名称与上载作业相同，但在开头加有文本 *Pub_*。

**上载后执行其他作业:**

1. 選取 **[!UICONTROL 上傳]**，然後選取 **[!UICONTROL 透過FTP]** 標籤。
1. 在「上傳」頁面的右下角，選取 **[!UICONTROL 工作選項]**.
1. 在「上載工作選項」對話方塊中，展開 **[!UICONTROL 進階]** 區段。
1. 從下列選項中選擇一項 **[!UICONTROL 上載後執行其他工作]** 下拉式清單：

   * 无
   * HTTP 请求
   * 图像服务发布
   * 图像渲染发布
   * 视频发布

1. 指定 HTTP 地址。
1. 指定您是否只想在上傳檔案時執行。
1. 指出是要在每次完成该作业时运行该请求，还是仅在发布文件时运行该请求。

   >[!NOTE]
   >
   >定期排程的工作有時會導致未發佈任何檔案。

>[!MORELIKETHIS]
>
>* [使用資產資料夾](asset-folders.md#working_with_asset_folders)
>* [處理週期性上傳和發佈工作](checking-job-files.md#handling_recurring_upload_and_publish_jobs)
>* [使用上載或發佈工作作為觸發器](checking-job-files.md#using_an_upload_or_publish_job_as_a_trigger)

