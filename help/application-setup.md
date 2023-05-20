---
title: 应用程序设置
description: 瞭解如何設定和設定Adobe Dynamic Media Classic的應用程式區域。 「應用程式」區域可讓您輸入一般設定、建立影像、檢視器和視訊編碼預設集、定義預設檢視器和中繼資料、發佈設定以及視訊SEO設定。 您也可以使用區域來設定批次集預設集，以自動產生2D迴轉集。
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

您可以使用「應用程式設定」頁面來輸入一般設定、建立影像預設集、視訊編碼預設集、檢視器預設集，或定義預設檢視器和中繼資料。 您可以設定批次集預設集，以自動產生2D迴轉集（例如）、發佈設定和視訊SEO設定。

>[!NOTE]
>
>只有Adobe Dynamic Media Classic管理員才能變更「應用程式設定」頁面上的設定。

## 常规设置 {#general-settings}

若要開啟「應用程式一般設定」頁面，請前往「全域導覽」列上的 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 一般設定]**.

### 服务器

建立帳戶時，Adobe Dynamic Media Classic會自動提供指派給貴公司的伺服器。 这些服务器用于构建网站和应用程序的 URL 字符串。这些 URL 调用是您的帐户所特有的。

另請參閱 [測試Secure Testing service](testing-assets-making-them-public.md#testing_the_secure_testing_service).

* **[!UICONTROL 已發佈的伺服器名稱]**  — 此伺服器是您的帳戶專屬之所有系統產生URL呼叫所使用的即時CDN （內容傳遞網路）伺服器。 除非得到Adobe Dynamic Media Classic支援技術人員的指示，否則請勿變更此伺服器名稱。

* **[!UICONTROL 原始伺服器名稱]**  — 此伺服器僅用於品質保證測試。 除非得到Adobe Dynamic Media Classic支援技術人員的指示，否則請勿變更此伺服器名稱。

<!-- **AGM Server Name** This server is used for Web-to-Print templates. This server is set on a company-wide basis. Do not change this server name unless instructed to do so by an Adobe DynamicMedia Classic support technician. -->

* **[!UICONTROL Test&amp;Target伺服器名稱]**  — 您的Test&amp;Target URL，最多（包括.com）。 如需取得此URL的說明，請參閱整合 [!DNL Adobe Dynamic Media Classic] 替換為 [!DNL Adobe Target Standard/Premium].

<!-- **Test Publish Context Server Name** -->

* **[!UICONTROL iOS串流伺服器名稱]**  — 您的URL [!DNL Adobe Dynamic Media Classic] iOS串流伺服器。 该服务器使用 HTTP 协议将流视频发送至 iOS 设备。

* **[!UICONTROL 漸進式視訊伺服器名稱]**  — 您的URL [!DNL Adobe Dynamic Media Classic] progressive video server. 该服务器使用 HTTP 协议发送渐进式视频。

* **[!UICONTROL 顯示未發佈資產的URL]**  — 如果您需要，請選取此選項 [!DNL Adobe Dynamic Media Classic] 在預覽任何資產時顯示URL （無論資產是否已發佈）。 如果资源未发布，此 URL 将无效。但是，您可以使用 URL 进行计划或组织。

<!-- **Allow AIR install** Select this option to allow users to download Adobe Dynamic Media Classic desktop version to their local hard drives. Users install the application from the Desktop Version area of the Personal Setup screen. -->

<!-- AIR users must manually uninstall their existing app and reinstall from the web version of Adobe Dynamic Media Classic (in Personal Settings). After this one-time reinstallation, you are prompted to upgrade whenever the server has a newer version of Adobe Dynamic Media Classic AIR. Adobe Dynamic Media Classic is integrated with the Application Update Framework which streamlines the upgrade process. -->

* **[!UICONTROL CDN失效範本]**  — 指定用於讓CDN （內容傳遞網路）快取失效的範本。

   例如，假設您輸入參照的影像URL （包括影像預設集或修飾元） `<ID>`，而非如下列範例所示的特定影像ID：

   `https://sample.scene7.com/is/image/Company/<ID>?$s7product$`

   如果範本僅包含 `<ID>`，然後Adobe Dynamic Media Classic填入 `https://<server>/is/image`，其中 `<server>` 是在「一般設定」中定義的發佈伺服器名稱。

   設定CDN失效範本，選取名為Backpack_B的影像，然後前往 **[!UICONTROL 檔案]** > **[!UICONTROL 使CDN失效]** 在CDN無效介面中導致以下產生的URL：

   `https://sample.scene7.com/is/image/Company/Backpack_B?$s7product$`

   在URL清單方塊中，選取 **[!UICONTROL 繼續]** 以清除該特定影像URL呼叫的快取。 您也可以輸入URL或將其貼到URL清單方塊中來新增URL；您不需要事先設定範本。

   選取CDN失效範本並提出CDN失效請求後，使用者介面中會彈出一個指示器。 它可讓您估計清除快取所需的時間。

   同樣地，如果您前往「 」，在Adobe Dynamic Media Classic中選取了多個影像， **[!UICONTROL 檔案]** > **[!UICONTROL 使CDN失效]**，每個影像都會在儲存的範本URL中參照。 因此，您可以定義CDN失效範本，以參考網站上參考的每個URL （例如產品詳細資料和搜尋結果）。 随后，当您从缓存中选择一个或多个图像以便设为失效时，这些 URL 将自动填充界面。

   请参阅[内容缓存](dmc-platform-overview.md#content_caching)。

   请参阅[重新发布的资源和 CDN 延迟](publishing-files.md#republished_assets_and_cdn_delays)。

### 浏览

* **[!UICONTROL 顯示專案]**  — 決定專案是否可作為組織您的Adobe Dynamic Media Classic資產的方法。 另請參閱 [組織您的專案工作](/help/organizing-projects.md).

* **[!UICONTROL 顯示範例eVideo內容]**  — 開啟或關閉eVideo範例內容的顯示。

* **[!UICONTROL 顯示產生的內容]**  — 在資料夾中，顯示從資產產生的內容。 例如，當PDF檔案在上傳時點陣化時，Adobe Dynamic Media Classic會以原始PDF為每個頁面建立一個影像。 如果选择“显示生成的内容”，则在上载原始 PDF 时生成的每个图像都会与该 PDF 一起显示在将 PDF 上载到的文件夹中。

* **[!UICONTROL 顯示編碼的視訊]**  — 預設為取消選取（關閉）。

   若要在Adobe Dynamic Media Classic中快速搜尋和瀏覽影片，而無需導覽相同影片的大量已編碼衍生影片，請將此選項保留為取消選取（預設）。 只會顯示主要視訊縮圖（您上傳並用來建立衍生影片的來源視訊）和「父」最適化視訊集縮圖（包含已編碼視訊集的「子」衍生影片）。

   不過，您仍然可以從主要視訊或最適化視訊集中存取個別編碼視訊。 要执行以上操作，请双击视频缩略图图像，打开详细信息视图。然後選取 **[!UICONTROL 編碼的視訊]** ，以便存取所有「兒童」影片。

   您也可以前往 **[!UICONTROL 檔案]** > **[!UICONTROL 重新處理]** 以直接從最適化視訊集建立更多編碼的「子」視訊。 Adobe Dynamic Media Classic會自動找到最適化視訊集的「父」主視訊，並將其用作轉碼的原始視訊。 但是，如果保存新的单个编码视频，您在搜索或浏览时将看不到这些视频。但是，您仍可以从详细信息视图的“编码的视频”选项卡进行访问。

   另請參閱 [上傳和轉碼視訊](uploading-encoding-videos.md#uploading_and_encoding_videos).

   要继续保留在搜索和浏览时可以访问所有编码视频派生的功能，请选择“**[!UICONTROL 显示已编码视频]**”。

   “构建”菜单上的某些操作只能对单个视频或选择性地对单个视频生效。此功能要求必须显示所有可以选择的编码视频派生（无论如何设置“**[!UICONTROL 显示已编码视频]**”）。覆寫的「建置」動作 **[!UICONTROL 顯示編碼的視訊]** 設定包括 **[!UICONTROL 最適化視訊集]**、和 **[!UICONTROL eCatalogs]**.

   >[!NOTE]
   >
   >如果您未使用Adobe Dynamic Media Classic上傳及編碼視訊資產，Adobe Dynamic Media Classic會顯示所有個別編碼的視訊，即使此選項已取消選取亦然。

* **[!UICONTROL 顯示重新整理子資料夾按鈕]**  — 開啟或關閉子資料夾[重新整理]按鈕的顯示。

### Adobe Dynamic Media Classic FTP帳戶

* **[!UICONTROL 伺服器]**  — 列出您的FTP帳戶伺服器。

* **[!UICONTROL 使用者名稱]**  — 列出您的FTP帳戶使用者名稱。

### 上载到应用程序

另請參閱 [預設上載工作選項](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/569_Default%20Job%20Options_converted%20renamed_Getting%20Started-AVS) 訓練影片。

* **[!UICONTROL 覆寫影像]** - Adobe Dynamic Media Classic不允許兩個檔案具有相同名稱。 每個專案的Adobe Dynamic Media Classic ID （影像名稱減去副檔名）必須是唯一的。 由于此规则，“上载”对话框中有一个“覆盖”选项。该选项的准确效果取决于指定的“覆盖图像”选项。这些选项指定了如何上载替换图像：替换原始图像，还是成为重复图像。重复图像会用“-1”重命名（例如，chair.tif 会重命名为 chair-1.tif）。这些选项会影响上载到的文件夹与原始图像不同的图像，或文件扩展名（如 JPG、TIF 或 PNG）与原始图像不同的图像。另請參閱 [使用覆寫影像選項](#using-the-overwrite-images-option).

   * **[!UICONTROL 在目前檔案夾中以相同的基本影像名稱/副檔名覆寫]**  — 此選項是最嚴格的取代規則。 它要求您将替换图像上载到原始图像所在的文件夹中，并且该替换图像与原始图像具有相同的文件扩展名。如果不满足这些要求，则会创建重复的图像。

   * **[!UICONTROL 目前檔案夾內若有基本資產名稱相同者（無論副檔名為何），將予以覆寫]**  — 要求您將取代影像上傳至與原始影像相同的資料夾，但副檔名可能與原始影像不同。 例如，chair.tif 会替换 chair.jpg。

   * **[!UICONTROL 任何檔案夾內若有基本資產名稱/副檔名相同者，將予以覆寫]**  — 取代影像的副檔名必須與原始影像相同（例如，chair.jpg必須取代chair.jpg，而不是chair.tif）。 但是，可以将替换图像上载到与原始图像不同的文件夹中。更新的图像位于新文件夹；而不再位于其原始位置

   * **[!UICONTROL 任何檔案夾內若有基本資產名稱相同者（無論副檔名為何），將予以覆寫]**  — 此選項是最具包容性的取代規則。 可以将替换图像上载到与原始文件所在文件夹不同的文件夹，使用不同的文件扩展名上载文件，并替换原始文件。如果原始文件在不同的文件夹中，替换图像则位于其所上载至的新文件夹。

* **[!UICONTROL 保留發佈]**  — 指定上傳至Adobe Dynamic Media Classic的取代影像是否保留其取代影像的「準備發佈」設定，或在上傳時指定此設定。

* **[!UICONTROL 預設色彩設定檔]**  — 指定新增CMYK影像時，套用為預設色彩設定檔選項一部分的色彩設定檔。

* **[!UICONTROL 預設上傳選項]**  — 開啟「上載工作選項」對話方塊，您可以在其中指定預設上載選項。 有关这些选项的信息，请参阅[上载选项](/help/uploading-files.md#upload_options)。

### 应用程序的图像映射编辑器

* **[!UICONTROL 預設影像對應HREF]**  — 定義影像對應中HREF欄使用的預設URL。 此URL是您在建立影像地圖時看到的預設URL。

* **[!UICONTROL 預設影像對應範本]**  — 定義影像對應中HREF範本的預設JavaScript。 您可以在此處設定自訂程式碼，以便在您選取影像地圖時執行。

### 应用程序的其他设置

* **[!UICONTROL 垃圾桶清理警告]**  — 垃圾桶中的資產會在七天內自動移除。 如果您需要在“垃圾桶”中的资源距永久删除还有四天时间时向公司管理员发送通知，请选择“自动删除垃圾桶项目之前会发送电子邮件”。另請參閱 [管理垃圾桶資料夾](/help/trash-folder.md).

## 使用覆寫影像選項 {#using-the-overwrite-images-option}

Adobe Dynamic Media Classic不允許兩個檔案具有相同名稱。 每個專案的Adobe Dynamic Media Classic ID （影像名稱減去副檔名）必須是唯一的。 由于该规则，所以“上载”对话框会包括“覆盖图像”选项。此選項的確切效果取決於每個公司「Adobe Dynamic Media Classic內部設定」的設定。

如果您先前已上傳影像，然後變更原始檔案（或取代原始檔案），則所選的「覆寫」選項會指定Adobe Dynamic Media Classic取代影像的方式。 没有关于图像更改的信息，但是新图像会替换旧图像。如果資料夾也包含Adobe Dynamic Media Classic中尚未包含的影像，則會新增這些影像。

如果您上傳的影像以某種方式變更（影像已變更），但影像的參照保持不變，請使用此選項。 在上载和翻录 Adobe® PDF 时“覆盖”也很有用。微調Adobe Dynamic Media Classic的方式 *裂縫* 請調整影像的「上傳」對話方塊中的ICC色彩設定檔選項，並使用「覆寫」功能重新上傳。

用來從生產伺服器存取影像的Adobe Dynamic Media Classic ID衍生自影像檔案名稱。 在檔案名稱中使用大寫和小寫字元是很重要的，不論是在取代現有檔案還是用來存取影像的Adobe Dynamic Media Classic ID中。 上傳至Adobe Dynamic Media Classic之前，請確認檔案名稱中的大寫和小寫字元使用正確，以避免同一影像的Adobe Dynamic Media Classic ID有所差異。

如果您取消选择此选项，将与现有图像具有相同文件名的所有图像都视为重复图像，并且不予添加。

## 图像预设 {#image-presets}

“图像预设”屏幕用于创建和编辑图像预设。影像預設集可讓Adobe Dynamic Media Classic以動態方式傳遞來自相同主要影像的不同大小影像。 每个图像预设都表示用于显示图像的一组预定义大小和格式命令。建立影像預設集時，您可以選取影像傳送的大小。 您也可以選取格式化指令，以便在傳送影像供檢視時最佳化影像的外觀。

管理员可以创建导出资源的预设。使用者可以在匯出影像時選擇預設集，這樣也會將影像重新格式化為管理員指定的規格。

若要開啟「影像預設集」畫面，請前往「全域導覽」列上的 **[!UICONTROL 設定]** > **[!UICONTROL 影像預設集]**.

另請參閱 [智慧型影像](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/imaging-faq.html#dynamic).

### 创建并编辑图像预设 {#creating-and-editing-image-presets}

1. 前往 **[!UICONTROL 設定]** > **[!UICONTROL 影像預設集]**.
1. 建立預設集或從現有預設集開始：

   * **建立影像預設集**  — 選取 **[!UICONTROL 新增]**.
   * **從現有預設集建立影像預設集**  — 選取最符合您要建立的影像預設集，然後選取 **[!UICONTROL 編輯]**.

1. 在「新增（或編輯）預設集」頁面上，輸入預設集名稱。
1. 设置所需的预设选项。

   请参阅[图像预设选项](application-setup.md#image_preset_options)。

1. 選取 **[!UICONTROL 儲存]**，或者，如果您是從現有的預設集開始，請選取 **[!UICONTROL 另存為]**.
1. 若要使用您自己的影像預覽預設集，請選取 **[!UICONTROL 瀏覽]** 然後選取影像。 若要以預設影像預覽，請選取 **[!UICONTROL 重設]**.

您可以在「影像預設集」畫面上選取影像預設集名稱，然後選取「 」，以編輯影像預設集 **[!UICONTROL 編輯]**. 若要刪除影像預設集，請選取該預設集，然後選取 **[!UICONTROL 刪除]**.

### 图像预设选项 {#image-preset-options}

“添加预设”和“编辑预设”屏幕提供了用于创建和编辑图像预设的选项：

* **[!UICONTROL 預設集名稱]**  — 輸入描述性名稱，不含任何空格。 為協助使用者識別此影像預設集，請在名稱中包含影像大小規格。

* **[!UICONTROL 寬度和高度]**  — 輸入遞送影像的畫素大小。

* **[!UICONTROL 格式]**  — 從功能表選取格式。 選擇GIF、JPEG、PDF或TIFF格式會提供更多選項：

   * GIF 颜色量化选项

      * **[!UICONTROL 型別]**  — 選取「最適化」（預設）、Web或Macintosh。 如果您選取 **[!UICONTROL 含Alpha的GIF]**，無法使用Macintosh選項。

      * **[!UICONTROL 遞色]**  — 選取「擴散」或「關閉」。

      * **[!UICONTROL 色彩數量]**  — 拖曳滑桿以輸入2-255。

      * **[!UICONTROL 色彩清單]**  — 輸入逗號分隔的清單。 例如，對於白色、灰色和黑色，請輸入 `000000,888888,ffffff`.
   * JPEG 选项

      * **[!UICONTROL 品質]**  — 控制JPEG壓縮等級。 此设置既影响文件大小，又影响图像质量。JPEG品質比例為1-100。

      * **[!UICONTROL 啟用JPG色度縮減取樣]**  — 由於眼睛對高頻色彩資訊的敏感度低於高頻亮度，因此JPEG影像會將影像資訊劃分為亮度和色彩分量。 压缩 JPEG 图像时，通过将各组像素放到一起平均，亮度分量为全分辨率，颜色分量为缩减像素取样。缩减像素采样会将数据量减少二分之一或三分之一，而对于用户所能感知到的质量而言却几乎没有任何影响。缩减像素采样不适用于灰度图像。这种方法会减少对于高对比度图像有用的压缩的数量（例如，包含覆盖文本的图像）。
   * PDF 和 TIFF 选项

      * **[!UICONTROL 壓縮]**  — 選取壓縮演演算法。



* **[!UICONTROL 色域]**  — 選取色域。

* **[!UICONTROL 銳利化]**  — 選取「啟用簡單銳利化」選項，在所有縮放完成後將基本銳利化濾鏡套用至影像。 锐化可以帮助补偿在以不同尺寸显示图像时可能导致的模糊。

   如需銳利化、重新取樣模式以及不銳利化遮色片的詳細資訊，請參閱 [銳利化影像](sharpening-image.md#sharpening_an_image). 另請參閱 [銳利化](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/547_sharpening1_converted%20renamed_Done-AVS) 訓練影片。

* **[!UICONTROL 重新取樣模式]**  — 選取重新取樣模式選項。 当图像缩减像素取样时，以下选项锐化该图像：

* **[!UICONTROL 線性]**  — 最快速的重新取樣方法；會產生某些明顯的鋸齒狀不自然感。

* **[!UICONTROL 雙立方式]**  — 增加影像伺服器上的CPU使用量，但產生較銳利的影像，且鋸齒狀不自然感較不明顯。

* **[!UICONTROL 銳利化2]**  — 產生的結果可能會比「雙立方式」選項稍微銳利，但影像伺服器的CPU成本更高。

* **[!UICONTROL 三線性]**  — 同時使用較高和較低的解析度（如果有的話）；僅在出現鋸齒問題時才建議使用。 由于减少了高频数据，此方法会减小 JPEG 的大小。

* **[!UICONTROL 不銳利化遮色片]**  — 選擇下列選項以微調銳利化：

* **[!UICONTROL 數量]**  — 控制套用至邊緣畫素的對比量。 默认值为 1.0。对于高分辨率图像，可将该值增加到 5.0。数量用于衡量滤镜强度。

* **[!UICONTROL 半徑]**  — 決定邊緣畫素周圍影響銳利化的畫素數量。 对于高分辨率图像，请输入 1 到 2 之间的值。较低的数值仅锐化边缘像素，较高的数值则锐化范围更宽的像素。值正确与否取决于图像的大小。

* **[!UICONTROL 臨界值]**  — 決定套用遮色片銳利化調整濾鏡時要忽略的對比範圍。 换言之，此选项确定锐化的像素必须与周围区域相差多少，才被滤镜看作边缘像素并被锐化。为避免引进干扰，请用 0.02 到 0.2 之间的值做试验。默认值 6 锐化图像中的所有像素。

* **[!UICONTROL 色域]**  — 決定影像使用建立影像的空間，通常是RGB（原始）或亮度空間（強度）。

* **[!UICONTROL 顏色]** 選擇下列選項：

* **[!UICONTROL 輸出色彩設定檔]**  — 選取 **[!UICONTROL 使用預設值]** 或Adobe Dynamic Media Classic上可用的其中一個ICC色彩設定檔。

   另请参阅[ ICC 配置文件](icc-profiles.md#icc_profiles)。

* **[!UICONTROL 演算色彩比對方式]**  — 如果要覆寫色彩設定檔的預設色彩演算比對方式，請選取選項。 當其中一個預設ICC設定檔是色彩轉換的目標色域時，請使用此選項。 或者，輸出裝置（印表機或熒幕）的特點是此設定檔，而且指定的演算色彩比對方式對此設定檔有效。

* **[!UICONTROL 內嵌設定檔]**  — 選取此選項，以便當您在Adobe® Photoshop®中開啟此影像時，它會使用此設定檔。

* **[!UICONTROL 列印解析度]**  — 選取列印此影像的解析度；預設為72畫素。

* **[!UICONTROL URL修飾元]**  — 如果您偏好指定定義影像預設集的URL修飾元，而非設定，請在此輸入修飾元。

* **[!UICONTROL 影像URL範例]**  — 列出「原始」 URL字串，Dynamic Media Image Server會使用您新增或編輯的影像預設集來傳送影像。 此URL字串會編碼您在「新增預設集」或「編輯預設集」畫面中選取的所有格式設定。

### 編輯、移除或停用影像預設集 {#editing-removing-or-deactivating-an-image-preset}

1. 前往 **[!UICONTROL 設定]** > **[!UICONTROL 影像預設集]**.
1. 在“图像预设”屏幕中，选择表中的某个预设，然后执行以下任一操作：

   * 選取 **[!UICONTROL 編輯]** 然後在「編輯預設集」對話方塊中指定新選項。
   * 選取 **[!UICONTROL 刪除]** 以從清單中移除預設集。
   * 取消選取 **[!UICONTROL 作用中]** 如果想要從MediaPortal使用者的整個Adobe Dynamic Media Classic使用者介面中移除預設集名稱，請勾選預設集名稱旁的方塊。

## 啟用或停用自我調整視訊預設集 {#activating-or-deactivating-adaptive-video-presets}

Adobe Dynamic Media Classic提供最適化視訊編碼預設集。 這是將16:9最適化視訊預設集和4:3最適化視訊預設集合併為一個群組的預設集主要清單。 这些预定义的预设反映了最常用的编码设置，并且经过优化以便在目标移动设备、平板电脑和台式机上播放。

默认情况下，仅激活（启用或“打开”）“自适应视频”编码预设。您可以根据需要将其停用。在“上载作业选项”对话框的 eVideo 部分中，非活动自适应视频预设不会显示为可选择的选项。

另請參閱 [上傳並編碼視訊](uploading-encoding-videos.md#uploading_and_encoding_videos).

另請參閱 [視訊預設集](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/549_video-presets_converted%20renamed_Done-AVS) 訓練影片。

**激活或停用自适应视频预设:**

1. 在Adobe Dynamic Media Classic的右上角附近，前往 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 視訊預設集]** > **[!UICONTROL 最適化視訊預設集]**.
1. 在“自适应视频预设”页中，取消选中某个预设名称旁边的复选框，以将该预设从“上载作业选项”对话框的“eVideo 选项”列表中删除。
1. 選取 **[!UICONTROL 關閉]**.

## 用于编码视频文件的视频预设 {#video-presets-for-encoding-video-files}

若要選取編碼預設集，請在「上傳」頁面的右下角選取 **[!UICONTROL 工作選項]**. 在「上傳工作選項」對話方塊中，展開「eVideo選項」並選取您想要的視訊編碼預設集。

>[!NOTE]
>
>除了預設啟用的「最適化視訊」之外，您無法在上傳工作選項對話方塊中看到所有其他最適化視訊或單一視訊編碼預設集。 Adobe Dynamic Media Classic管理員會決定哪些視訊編碼預設集會顯示在「上傳工作選項」對話方塊中。

* 從下列最適化視訊編碼或單一編碼預設集中選取：

   * **[!UICONTROL 16:9最適化影片]**  — 建立16:9畫面寬高比的視訊，以傳送至桌上型電腦、行動裝置(iPhone、iPad、Android™)和平板電腦(iPad、Android™)，並透過最符合檢視器連線速度的解析度和位元速率進行最佳化。

   * **[!UICONTROL 4:3自我調整視訊]**  — 建立4:3畫面寬高比視訊，以傳送至桌上型電腦、行動裝置(iPhone、iPad、Android™)和平板電腦(iPad、Android™)，並透過最符合檢視器連線速度的解析度和位元速率進行最佳化。

   * **[!UICONTROL 自我調整視訊]**  — 單一編碼預設集，可與任何長寬比搭配使用，建立視訊以傳送至行動裝置、平板電腦和案頭。 使用该预设编码的上载的源视频将设置为固定高度。但是，自动调整宽度以保持视频的高宽比。

      默认情况下，在创建您自己的自定义视频编码预设时，也可以灵活地进行这种“自动缩放”。

      另請參閱 [新增或編輯視訊編碼預設集](uploading-encoding-videos.md#adding_or_editing_a_video_encoding_preset).

   * **[!UICONTROL 自我調整視訊編碼（16:9或4:3）]**  — 建立16:9和4:3畫面寬高比視訊，以傳送至桌上型電腦、行動裝置(iPhone、iPad、Android™)和平板電腦(iPad、Android™)。 以最符合檢視器連線速度的解析度和位元速率最佳化。

      请参阅[自适应视频编码（16:9 或 4:3）视频预设](application-setup.md#adaptive_video_encoding_16_9_or_4_3_video_presets)。

   * **[!UICONTROL 单个编码预设]**

      >[!NOTE]
      >
      >若要將視訊傳送至iPad，您可以選取行動編碼預設集或Tablet編碼預設集。 平板电脑预设专为 iPad 而设计，通常具有更高的分辨率和质量，以充分利用更大的屏幕尺寸和带宽连接。传送使用平板电脑预设编码的视频文件要求您在移动站点或应用程序上加入设备检测代码。此代码会根据播放设备在 iPhone 或 iPad 视频体验之间切换。更简单的工作流程是选择移动设备预设将视频文件传送到 iPad。原因在于您可以将同一视频文件用于 iPhone 和 iPad。但是，将质量标准化为分辨率更低的 iPhone 体验。

      * 在“编码预设”组下的“编码预设排序”下拉列表中，选择名称或大小来按名称或分辨率大小对预设进行排序。
      * 根據您計畫播放視訊的解析度大小和頻寬，選取編碼預設集。
      * 您可以選取「最適化視訊編碼」，以及每個視訊的一或多個編碼預設集。 例如，您可以在一个上载作业中针对桌面和移动设备编码文件。

在您選取之後 **[!UICONTROL 開始上傳]**，則會上傳原始主要視訊檔案，並從主要檔案產生編碼檔案。

### 关于编码预设选项 {#about-encoding-preset-options}

编码预设选项的参数如下：

* **[!UICONTROL 目標連線速度]**  — 目標使用者的網際網路連線速度。

* **[!UICONTROL 編碼檔案字尾]**  — 附加至已編碼視訊檔案的尾碼，用於識別身分。

* **[!UICONTROL 視訊位元速率（資料速率）]**  — 經過編碼，可構成一秒的視訊播放資料量（以每秒千位元為單位）。

* **[!UICONTROL 畫素寬度/高度]**  — 熒幕影像的寬度尺寸（以畫素為單位）；熒幕影像的高度尺寸（以畫素為單位）。

* **[!UICONTROL 每秒影格(fps)]**  — 視訊每秒的影格數（或靜態影像）。 在美国和日本，大部分视频以 29.97 fps 拍摄；在欧洲和亚洲（不包括日本），大部分视频以 25 fps 拍摄。电影以 24 fps 拍摄。

* **[!UICONTROL 音訊位元速率]**  — 經過編碼以構成音訊播放一秒的資料量（以每秒千位元為單位）。

下表显示了选择视频预设的建议最佳做法和用于指定编码文件的命名约定。

### 自适应视频（默认） {#adaptive-video-default}

这是一个适用于任何高宽比的编码预设，可用于创建传送到移动设备、平板电脑和台式机的视频。使用该新预设（默认和最佳做法）编码的上载的源视频将设置为固定高度，同时自动调整宽度以保持视频的高宽比。

**自适应视频（默认）**

|  | 编码预设名称/工具提示文本 | 编码文件后缀 | 视频数据速率 (Kbps) | 宽度/高度（像素） | Fps | 音频比特率 (kbps) | 推荐 |
|--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | Auto x360, 800 Kbps | _Mobile_Autox360p_800K | 800 | Autox360 | 与源相同 | 64 | 適用於行動裝置(iPhone、iPad、Android™) |
| 2 | Auto x 480, 1400 Kbps | _Tablet_Autox480p_1400K | 1400 | Autox480 | 与源相同 | 96 | 適用於平板電腦(iPad、Android™) |
| 3 | Auto x 720, 2600 Kbps | _案頭_Autox720p_2600K | 2600 | Autox720 | 与源相同 | 128 | 適用於案頭 |

### 自适应视频编码（16:9 或 4:3）视频预设 {#adaptive-video-encoding-or-video-presets}

这些自适应视频编码预设合并了一系列单独的编码预设，将根据上载的视频的高宽比自动为您选择这些预设。例如，如果您上傳4:3視訊，系統會使用在下列專案的主要預設集清單中找到的所有五個4:3預設集自動對其編碼： **自我調整視訊編碼（16:9或4:3）** 選項。

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

与源 fps 相同。iPhone、iPad和Android™行動裝置的視訊編碼預設集。

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
>**Flash檢視器生命週期結束通知**  — 自2017年1月31日起，Adobe Dynamic Media Classic正式停止支援Flash檢視器平台。

*查看器预设*&#x200B;是一组设置，决定了用户如何在其计算机屏幕和移动设备上查看富媒体资源。作为管理员，您可以创建查看器预设。提供适用于一系列查看器配置选项的设置。例如，您可以更改查看器显示尺寸、缩放行为、颜色方案、边框和字体。

如需參考最佳作法，請使用Adobe Dynamic Media Classic HTML5影片檢視器。 HTML5 视频查看器中使用的预设是功能强大的视频播放器。

將下列專案結合至單一播放器：

* 能夠使用HTML5和CSS設計播放元件。
* 具有內嵌式播放。
* 根據瀏覽器的功能使用最適化和漸進式串流。

您可以將多媒體內容延伸至桌上型電腦、平板電腦和行動使用者，並確保簡化的視訊體驗。

另請參閱 [關於HTML5檢視器](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/library/viewers-for-aem-assets-only/c-html5-aem-asset-viewers.html?lang=en#viewers-for-aem-assets-only) 在Adobe檢視器參考指南中。

另請參閱 [Adobe Dynamic Media Classic檢視器預設集相容性對照表](application-setup.md#scene7_viewer_preset_compatibility_matrix).

请参阅[最佳做法：使用 HTML5 视频查看器](best-practice-using-html5-video.md#best_practice_using_the_html5_video_viewer)。

您可以根据查看器添加社区功能。社区功能包括“嵌入”按钮、“电子邮件”按钮、“链接”按钮和“访问站点”按钮。這些按鈕可讓使用檢視器的人員與其他人共用檢視器或開啟Adobe Dynamic Media Classic網站。

另請參閱 [Adobe檢視器參考資料庫範例](https://landing.adobe.com/en/na/dynamic-media/ctir-2755/live-demos.html).

### 回應式設計網頁的檢視器支援 {#viewer-support-for-responsive-designed-web-pages}

不同的网页具有不同的需求。有時候，您會想要一個網頁，提供可在個別瀏覽器視窗中開啟HTML5檢視器的連結。 在其他情況下，必須將HTML5 Viewer直接內嵌在託管頁面上。 在後一種情況下，網頁可能具有靜態配置。 或者，它是「回應式」的，且在不同裝置或不同瀏覽器視窗大小中顯示的方式不同。 為了滿足這些需求，Adobe Dynamic Media Classic隨附的HTML5檢視器同時支援靜態網頁和回應式設計的網頁。

如需如何將回應式檢視器內嵌至網頁的詳細資訊，請參閱 [關於Responsive影像資料庫](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/responsive-static-image-library/c-about-responsive-static-image-library.html#image-serving-api)， [使用Responsive影像資料庫](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/responsive-static-image-library/t-using-responsive-static-image-library.html#image-serving-api)、和 [命令參考 — 命令屬性](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/responsive-static-image-library/t-using-responsive-static-image-library.html#responsive-static-image-library).

### 查看器预设类型 {#viewer-preset-types}

管理员可以创建和自定义以下类型的查看器预设：

* **[!UICONTROL eCatalog檢視器]**  — 模擬讀取列印目錄時的體驗。 您可以在不同頁面間移動、放大和縮小頁面上的專案、使用影像地圖來檢視頁面上專案的詳細資訊，或搜尋目錄。 还可以包括“信息面板”，在映射区域具有有效的 rollover_key 属性时显示详细信息和图像映射的物品。要包括“信息面板”，请在“eCatalog 查看器预设”窗口的“信息面板设置”面板中指定“信息服务器 URL”。

* **[!UICONTROL 色票集檢視器]**  — 以不同的色彩、材質、紋理、光澤或織物顯示影像。 使用者可選取縮圖以檢視影像中的變化。

* **[!UICONTROL 混合媒體集檢視器]**  — 在一個檢視器中顯示不同型別的媒體。 您可以包括样本集、旋转集、图像和视频。您可以设置各个选项卡，以包含不同类型的内容，例如，一个选项卡用于图像集、一个选项卡用于视频。从混合媒体集播放的视频使用具有时间线和视频控件（如停止、暂停、回放和播放）的标准视频查看器。您设置混合媒体集查看器预设时，指定要将哪些查看器用于“混合媒体集”中的不同类型的资源。您还可以使用“网格查看器”或“轮盘式查看器”来查看混合媒体集。

* **[!UICONTROL 迴轉集檢視器]**  — 提供影像的多個檢視，讓使用者可以轉動物件來檢查不同的側邊和角度。

* **視訊檢視器**  — 使用來源檔案的解析度尺寸或自訂大小來顯示視訊。 Adobe Dynamic Media Classic隨附許多預先定義的檢視器預設集，可供您播放視訊，如果您是管理員，可以建立自訂的視訊檢視器預設集。 設定「視訊檢視器」有超過12種不同的設定。 您可以配置其大小、前景和背景颜色、视频和音频控件、进度条、用户界面外观、社交功能和“帮助”。

* **[!UICONTROL 縮放檢視器]**  — 提供三種縮放檢視器型別的選擇：

* **[!UICONTROL 縮放檢視器]**  — 可讓使用者透過選取區域來放大該區域。 他們可以選取控制項來放大、縮小影像，以及將影像重設為預設大小。

* **[!UICONTROL 縮放檢視器：彈出]**  — 在原始影像旁顯示縮放區域的第二個影像。 没有控件可以使用，用户只需将选取范围移动到他们要查看的区域上即可。

在确定此查看器的完整带宽使用量时，请考虑在查看器中有主图像和弹出图像。主图像大小（舞台宽度和高度）和缩放系数决定了弹出图像大小。为防止弹出文件大小变得太大，需对这两个值进行平衡：如果您的主图像大小很大，请降低缩放系数值。（弹出宽度和弹出高度决定了弹出窗口的大小，但不决定提供给查看器的弹出图像的大小。）

例如，如果您的主图像大小是 350 X 350 像素，缩放系数为 3，则生成的弹出图像是 1050 X 1050 像素。如果您的主图像大小是 300 X 300 像素，缩放系数为 4，则弹出图像是 1200 X 1200 像素。根据 JPEG 品质设置（推荐的设置介于 80-90），您可以显著地减少文件大小。建议的缩放系数为 2.5 至 4，取决于您的主图像的大小。

### Adobe Dynamic Media Classic檢視器預設集相容性對照表 {#scene-viewer-preset-compatibility-matrix}

**Flash檢視器生命週期結束通知**：自2017年1月31日起，Adobe Dynamic Media Classic正式停止支援Flash檢視器平台。

下表列出目前可用的Adobe Dynamic Media Classic Viewer預設集。 该表还指定了查看器与桌面和移动设备的兼容性，以及对每个指定查看器使用的技术。

另請參閱 [Adobe檢視器參考資料庫範例](https://landing.adobe.com/en/na/dynamic-media/ctir-2755/live-demos.html).

有关查看器支持的 Web 浏览器和操作系统版本的信息，您可以查阅查看器发行说明。

另請參閱 [Adobe檢視器參考發行說明](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources.html).

|  | 查看器技术 | 桌面 | Apple iPhone | Apple iPad | Android™智慧型手機 | Android™平板電腦 |
|--- |--- |--- |--- |--- |--- |--- |
| 缩放查看器 |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML5 | X | X | X | X | X |
| Universal_HTML5_Zoom_inline | HTML5 | X | X | X | X | X |
| Universal_HTML5_Zoom_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_Zoom_light | HTML5 | X | X | X | X | X |


|  | 查看器技术 | 桌面 | Apple iPhone | Apple iPad | Android™智慧型手機 | Android™平板電腦 |
|--- |--- |--- |--- |--- |--- |--- |
| 图像集查看器 |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_light | HTML5 | X | X | X | X | X |

|  | 查看器技术 | 桌面 | Apple iPhone | Apple iPad | Android™智慧型手機 | Android™平板電腦 |
|--- |--- |--- |--- |--- |--- |--- |
| 样本集查看器 |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML5 | X | X | X | X | X |
| Universal_HTML5_SwatchSet_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_SwatchSet_light | HTML5 | X | X | X | X | X |

|  | 查看器技术 | 桌面 | Apple iPhone | Apple iPad | Android™智慧型手機 | Android™平板電腦 |
|--- |--- |--- |--- |--- |--- |--- |
| eCatalog 查看器 |  |  |  |  |  |  |
| Universal_Catalog5_eCatalog_Adv(包含對社交HTML和目錄搜尋的支援。) | HTML5 | X | X | X | X | X |
| Universal_HTML5_eCatalog（包含對社群媒體和目錄搜尋的支援。） | HTML5 | X | X | X | X | X |

|  | 查看器技术 | 桌面 | Apple iPhone | Apple iPad | Android™智慧型手機 | Android™平板電腦 |
|--- |--- |--- |--- |--- |--- |--- |
| 旋转查看器 |  |  |  |  |  |  |
| Universal_HTML5_SpinSet_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_SpinSet_light | HTML5 | X | X | X | X | X |

**eVideo 查看器**

Adobe Dynamic Media Classic支援MP4 H.264視訊的行動視訊播放。

* 您可以在下列位置找到支援此視訊格式的BlackBerry®裝置： [BlackBerry®支援的視訊格式](https://developers.blackberry.com/us/en)
* 您也可以在下列位置找到支援此視訊格式的Windows®裝置： [Windows® Phone支援的視訊格式](https://docs.microsoft.com/en-us/windows/uwp/audio-video-camera/supported-codecs)

|  | 查看器技术 | 桌面 | Apple iPhone | Apple iPad | Android™智慧型手機 | Android™平板電腦 | BlackBerry®智慧型手機 | Windows® Phone |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| Universal_HTML5_Video（包含隱藏式字幕支援。） 另請參閱 [最佳實務：使用通用HTML5視訊檢視器。](best-practice-using-html5-video.md#best_practice_using_the_html5_video_viewer) | HTML5 | X | X | X | X | X | X | X |
| Universal_HTML5_Video_social（包含對隱藏式字幕和社群媒體的支援。） | HTML5 | X | X | X | X | X | X | X |

|  | 查看器技术 | 桌面 | Apple iPhone | Apple iPad | Android™智慧型手機 | Android™平板電腦 |
|--- |--- |--- |--- |--- |--- |--- |
| 混合媒体集查看器 |  |  |  |  |  |  |
| Universal_HTML5_MixedMedia_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_MixedMedia_light | HTML5 | X | X | X | X | X |

### 支持的移动查看器手势表格 {#supported-mobile-viewers-gestures-matrix}

下表識別iOS、Android™ 2.x和Android™ 3.x裝置支援的行動檢視器手勢。

|  | 查看器技术 | 桌面 | Apple iPhone | Apple iPad | Android™智慧型手機 | Android™平板電腦 |
|--- |--- |--- |--- |--- |--- |--- |
| 图像集查看器 |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_light | HTML5 | X | X | X | X | X |

### 关于查看器预设屏幕 {#about-the-viewer-preset-screen}

在“查看器预设”屏幕上创建和管理“查看器预设”。若要開啟此畫面，請前往 **[!UICONTROL 設定]** > **[!UICONTROL 檢視器預設集]**.

“查看器预设”屏幕提供了用于执行以下任务的工具：

* **新增預設集**  — 選取 **[!UICONTROL 新增]** 並在「新增檢視器預設集」對話方塊中進行選擇。

       請參閱[新增和編輯檢視器預設集](application-setup.md#adding_and_editing_viewer_presets)。
   
* **編輯預設集**  — 選取預設集，然後選取 **[!UICONTROL 編輯]**.

       請參閱[新增和編輯檢視器預設集](application-setup.md#adding_and_editing_viewer_presets)。
   
* **刪除預設集**  — 選取預設集，然後選取 **[!UICONTROL 刪除]**.

* **匯出預設集**  — 選取HTML5檢視器預設集，然後選取 **[!UICONTROL 匯出]** 以下載檢視器外觀，以便將其作為建立和新增其他檢視器預設集的基礎。

       請參閱[匯出HTML5檢視器預設集](application-setup.md#exporting_an_html5_viewer_preset)。
   
* **篩選檢視器預設集清單**  — 使用這些工具來篩選清單：

       *開啟**作用中/非作用中**下拉式清單，並選取顯示作用中預設集、非作用中預設集或所有預設集的選項。
       *開啟**檢視器**下拉式清單，並選取選項以僅檢視特定型別的檢視器。 選取**[!UICONTROL 所有檢視器]如**檢視所有檢視器。
   
* **排序預設集**  — 選取欄標題(**[!UICONTROL 作用中]**， **[!UICONTROL 型別]**， **[!UICONTROL 預設集]**，或 **[!UICONTROL Platform]**)來排序欄上的清單。 再次選取欄標題，依遞減（或遞增）順序排序清單。

* **啟用和停用預設集**  — 選取預設集，然後選取其「作用中」選項以啟用或停用。

       請參閱[啟動或停用檢視器預設集](application-setup.md#activating_or_deactivating_viewer_presets)。
   
>[!NOTE]
>
>選取 **[!UICONTROL 預覽]** 「檢視器預設集」頁面的右側，這樣您就能檢視資產在您選取的檢視器預設集中是什麼樣子。 若要檢視其他資產，請選取「 」 **[!UICONTROL 瀏覽]** 在「檢視器預設集」頁面中，並在「選取資產預覽」對話方塊中選取其他資產。

### 新增和編輯檢視器預設集 {#adding-and-editing-viewer-presets}

除了使用新增檢視器預設集之外 **[!UICONTROL 新增]** 在使用者介面中，您也可以使用 **[!UICONTROL 匯出]** 以新增檢視器預設集。 您只需匯出現有的HTML5檢視器預設集，然後使用該預設集作為新預設集的基礎。

另請參閱 [匯出HTML5檢視器預設集](application-setup.md#exporting_an_html5_viewer_preset).

另請參閱 [檢視器預設集](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/550_viewer-presets_converted%20renamed_Done-AVS) 訓練影片。

**添加和编辑查看器预设:**

1. 在Adobe Dynamic Media Classic的右上角附近，前往 **[!UICONTROL 設定]** > **[!UICONTROL 檢視器預設集]**.

   您可以过滤预设列表。例如，要仅查看视频查看器的预设，请从表正上方的工具栏上的“查看器”下拉列表中选择“视频查看器”。

1. 在「檢視器預設集」頁面的「檢視器預設集」畫面上，新增或編輯「檢視器預設集」。

   * **新增**  — 在工具列上，選取 **[!UICONTROL 新增]**. 在新增檢視器預設集對話方塊中，選取平台，然後選取多媒體資產型別。

          選取**[!UICONTROL 另存為]完成建立檢視器預設集時顯**。
      
   * **從現有的檢視器預設集開始新增**  — 在表格中，選取「視訊檢視器預設集」，然後選取 **[!UICONTROL 編輯]** （在工具列上）。

          重新設定Video Viewer後，請選取「 **[!UICONTROL 另存為]如**使用「預設集名稱」文字欄位中的不同名稱儲存預設集。
      
   * **編輯**  — 選取現有的檢視器預設集，然後選取 **[!UICONTROL 編輯]**.

1. 在「設定檢視器」畫面的「預設集名稱」欄位中，輸入或編輯預設集名稱。
1. 设置其余所需的选项。

   >[!NOTE]
   >
   >選取 **[!UICONTROL 與來源相同]** 自動調整視訊檢視器的大小，以符合已編碼視訊本身的解析度大小。 如果選取此選項，則無法輸入「舞台寬度」和「舞台高度」。 相反，这些选项来自视频自身。如果您選取 **[!UICONTROL 與來源相同]**，設定「邊界大小」選項可反映視訊播放區域以外的外觀元素尺寸。 该边距大小是视频控件的像素高度和宽度。您可以使用下列影像來協助您決定要使用的邊界大小。*

   ![視訊檢視器的邊界設定](assets/vs_video_viewer_configure_margin.png)

1. 执行以下任一操作：

   * 選取 **[!UICONTROL 另存為]** 如果您是從現有的預設集開始新增「檢視器」預設集。
   * 選取 **[!UICONTROL 儲存]** 如果您已新增或編輯檢視器預設集。

### 匯出HTML5檢視器預設集 {#exporting-an-html-viewer-preset}

您可以匯出現有的HTML5檢視器預設集，以作為建立HTML5檢視器預設集的基礎。 该导出选项很有用，因为您不必从头开始创建查看器。相反，您会导出外观和行为与所需预设接近的预设，然后以此为基础开始进行设计调整。

Adobe Dynamic Media Classic中所有預設、立即可用的檢視器預設集CSS檔案都使用指向所開啟資產的相對影像伺服路徑 `Scene7SharedAssets`. 例如，以下為上檢視器預設集CSS檔案中影像資產的相對路徑

`Scene7SharedAsset`： `.s7videoviewer .s7fullscreenbutton[state][selected] { background-image: url(/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha); }`

不過，如果您將Viewer CSS檔案託管在您自己的網站上，則必須在您自己的環境中使用影像伺服器的明確路徑來解析這些相對影像路徑。 例如，如果您要更新上方的相對路徑為明確路徑，可能會如下所示，其中 `https://s7d1.scene7.com` 是影像伺服器的直接路徑： `https://s7d1.scene7.com/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha`

**若要匯出HTML5檢視器預設集：**

```as3
.s7videoviewer .s7fullscreenbutton[state][selected] 
{ background-image: url(/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha); }
```

```as3
https://s7d1.scene7.com/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha
```

1. 前往 **[!UICONTROL 設定]** > **[!UICONTROL 檢視器預設集]**.
1. 在「檢視器預設集」工具列左側的第二個下拉式清單中，選取 **[!UICONTROL HTML5]**.
1. 在左边的第三个下拉列表中，选择“**[!UICONTROL 所有查看器]**”。
1. 選取您要用來作為新HTML5檢視器預設集基礎的檢視器預設集。
1. 在工具列中，選取 **[!UICONTROL 匯出]**.
1. 在「匯出選取的資產」對話方塊中，選取 **[!UICONTROL 提交匯出]**.

   匯出後，您會取得一個CSS檔案。 下载并解压缩此文件。

1. 在 CSS 编辑器中打开 CSS 文件，进行更改，然后保存该文件。
1. 將CSS檔案上傳至Adobe Dynamic Media Classic。

   另請參閱 [上傳檔案](uploading-files.md#uploading_files).

1. 將CSS檔案發佈至Dynamic Media影像伺服器。

   另請參閱 [發佈檔案](publishing-files.md#publishing_files).

1. 照常添加新的查看器预设。選取您上傳的檢視器CSS檔案。

   另請參閱 [新增和編輯檢視器預設集](application-setup.md#adding_and_editing_viewer_presets).

### 啟用或停用檢視器預設集 {#activating-or-deactivating-viewer-presets}

若要建立用於顯示資產的URL，使用者請在「預覽」對話方塊中開啟「預設集」下拉式清單，選取「檢視器預設集」，然後選取 **[!UICONTROL 複製URL]** (請參閱 [複製檢視器預設集的URL](application-setup.md#copying_the_url_of_a_viewer_preset))。 此“预设”列表提供了管理员在“查看器预设”屏幕上添加和管理的“查看器预设”。例如，在用户预览 eCatalog 时，所有活动的 eCatalog 查看器预设都显示在“预览”对话框的“预设”下拉列表上。

除非您在“查看器预设”屏幕上停用查看器预设，否则“预览”对话框的“预设”下拉列表可能变得内容越来越多。

**激活或停用查看器预设:**

1. 前往 **[!UICONTROL 設定]** > **[!UICONTROL 檢視器預設集]**.
1. 在「檢視器預設集」頁面上，選取或取消選取 **[!UICONTROL 作用中]** 啟用或停用檢視器預設集的選項。

### 複製檢視器預設集的URL {#copying-the-url-of-a-viewer-preset}

发布资源后，您可以复制以查看器预设的设置显示资源的 URL。

URL 即复制到剪贴板中。您可以根据需要在网页的 HTML 代码、移动设备或应用程序中使用它。

**复制查看器预设的 URL:**

1. 在“浏览”面板中选择资源。
1. 在“资源浏览”面板上方的工具栏右侧，执行以下任一操作：

   * 選取 **[!UICONTROL 格點檢視]**. 在“资源浏览”面板中，双击单个资源以便在详细信息视图中将其打开。在右側的「URL和內嵌程式碼」面板中，選取 **[!UICONTROL 複製URL]** 位於您想要的檢視器右側。
   * 選取 **[!UICONTROL 格點檢視]**. 在「資產瀏覽」面板中，選取單一資產，然後前往縮圖影像下方 **[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**.

   在「檢視器清單」頁面中，選取表格的「動作」欄下 **[!UICONTROL 複製URL]**.

   * 選取 **[!UICONTROL 清單檢視]**. 在「資產瀏覽」面板中，選取單一資產，然後在縮圖影像右側，前往 **[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**.
   在「檢視器清單」頁面中，選取表格的「動作」欄下 **[!UICONTROL 複製URL]**.

   * 選取 **[!UICONTROL 格點檢視]**， **[!UICONTROL 清單檢視]**，或 **[!UICONTROL 詳細資料檢視]**. 在相同工具列上，前往 **[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**.
   在「檢視器清單」頁面中，選取表格的「動作」欄下 **[!UICONTROL 複製URL]**.

### 複製檢視器預設集的內嵌程式碼 {#copying-the-embed-code-of-a-viewer-preset}

使用嵌入代码功能，您可以查看用于所选查看器预设的查看器代码。您也可以将代码复制到剪贴板中，以便可以将其粘贴到网页中以部署查看器。

在“嵌入代码”对话框中不允许编辑代码。

**复制查看器预设的嵌入代码:**

1. 在“资源浏览”面板中选择资源。
1. 在“资源浏览”面板上方的工具栏右侧，执行以下任一操作：

   * 選取 **[!UICONTROL 格點檢視]**. 在“资源浏览”面板中，双击单个资源以便在详细信息视图中将其打开。在右側的URL面板中，選取 **[!UICONTROL 內嵌程式碼]**.
   * 選取 **[!UICONTROL 格點檢視]**. 在「資產瀏覽」面板中，選取單一資產，然後前往縮圖影像下方 **[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**.

   在「檢視器清單」頁面中，選取表格的「動作」欄下 **[!UICONTROL 內嵌程式碼]**.

   * 選取 **[!UICONTROL 清單檢視]**. 在「資產瀏覽」面板中，選取單一資產，然後在縮圖影像右側，前往 **[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**.
   在「檢視器清單」頁面中，選取表格的「動作」欄下 **[!UICONTROL 內嵌程式碼]**.

   * 選取 **[!UICONTROL 格點檢視]**， **[!UICONTROL 清單檢視]**，或 **[!UICONTROL 詳細資料檢視]**. 在相同工具列上，前往 **[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**.
   在「檢視器清單」頁面中，選取表格的「動作」欄下 **[!UICONTROL 內嵌程式碼]**.

1. 在內嵌程式碼對話方塊中，選取 **[!UICONTROL 複製到剪貼簿]**.
1. 選取 **[!UICONTROL 關閉]**.

## 設定預設檢視器 {#configuring-default-viewers}

在Adobe Dynamic Media Classic中使用「預覽」時，您可以使用「預設檢視器」來設定與資產相關聯的預設檢視器。 您可以为下列资源类型设置默认预览体验：

* 图像
* 视频
* 旋转集
* 目录
* 图像集
* 样本集
* 媒体集

**配置默认查看器:**

1. 在「設定」下拉式清單中，選取 **[!UICONTROL 應用程式設定]**.
1. 在「設定」視窗的左窗格中，移至 **[!UICONTROL 應用程式設定]** > **[!UICONTROL 檢視者]**
1. 選取 **[!UICONTROL 預設檢視器]**.
1. 在“默认查看器”窗口中，在每种资源类型的下拉列表中，选择要与该资源的预览关联的查看器。
1. 在「預設檢視器」視窗的右下角，選取 **[!UICONTROL 儲存設定]**.
1. 在「設定」視窗的右下角，選取 **[!UICONTROL 關閉]** 以返回「資產」視窗。

## 元数据视图 {#metadata-views}

*元数据*&#x200B;是关于资源的标准化信息。您可以使用元数据来简化工作流程、组织资源和改进搜索。Adobe Dynamic Media Classic支援IPTC （國際新聞通訊委員會）標準和XMP （可延伸中繼資料平台）標準。 使用者在詳細資料檢視中檢視或輸入有關資產的中繼資料之前，可以開啟中繼資料檢視功能表。 在那裡，他們可以選取要檢視或用來描述資產的中繼資料欄位集。

Adobe Dynamic Media Classic提供預先定義的中繼資料檢視，管理員可以建立自己的中繼資料檢視，供使用者在輸入中繼資料時選擇。

### 创建元数据视图 {#creating-a-metadata-view}

1. 前往 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 中繼資料]** > **[!UICONTROL 中繼資料檢視]**.
1. 選取 **[!UICONTROL 新增]**.
1. 在「預設集名稱」文字欄位中，輸入檢視的名稱。
1. （可選）檢查 **[!UICONTROL 設為預設]** 讓此檢視成為使用者在「詳細資料檢視」中開啟「中繼資料」面板時看到的檢視。
1. （選用）選取 **[!UICONTROL 包含UDF]** 在檢視中加入使用者定義的欄位。 用户定义的字段显示在详细信息视图的“元数据”面板的顶部。
1. 選取您要用於檢視的欄位(選取 **[!UICONTROL 全選]** 以選取所有欄位)。
1. 選取 **[!UICONTROL 儲存]**.

   视图的选定类别和字段显示在“预览”面板中。

### 管理元数据视图 {#managing-metadata-views}

1. 前往 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 中繼資料]** > **[!UICONTROL 中繼資料檢視]**.
1. 执行以下任一操作：

   * 要预览视图，请将其选中。视图中的字段将显示在“预览”面板中。
   * 若要編輯檢視，請選取該檢視，然後選取 **[!UICONTROL 編輯]**. 然後在「預覽」面板上選取或取消選取欄位名稱，然後選取或取消選取 **[!UICONTROL 包含UDF]** 選項。
   * 若要刪除檢視，請選取該檢視，然後選取 **[!UICONTROL 刪除]**.
   * 若要將檢視設為預設值，請選取該檢視，然後選取 **[!UICONTROL 設為預設]**. 預設檢視是使用者在「詳細資料檢視」中開啟資產並前往「中繼資料」面板時看到的檢視。

## 元数据预设 {#metadata-presets}

元数据预设为管理员提供了控制和调整分配给资源的元数据的一种方式。在「詳細資料檢視」中，使用者可在為此目的而提供的欄位中輸入有關資產的中繼資料。 例如，用户可以输入所有者名称、版权说明和地址。為確保使用者正確且完整地輸入此資訊，您可以建立中繼資料預設集。 在「詳細資料檢視」中選擇中繼資料預設集會將預先定義的值填入中繼資料欄位。 例如，会自动输入所有者名称、版权说明和地址。

為您希望使用者能在詳細資料檢視中自動輸入以說明資產的每組中繼資料值建立中繼資料預設集。

### 创建或编辑元数据预设 {#creating-or-editing-a-metadata-preset}

1. 前往 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 中繼資料]** > **[!UICONTROL 中繼資料預設集]**.
1. 在“元数据预设”屏幕中，执行以下任一操作：

   * 若要建立預設集，請選取 **[!UICONTROL 新增]**. 在「中繼資料範本名稱」文字欄位中，輸入預設集名稱。 選取 **[!UICONTROL 中繼資料檢視]**，然後從下拉式清單中選取檢視(請參閱 [中繼資料檢視](application-setup.md#metadata_views))。
   * 若要編輯現有預設集，請從「中繼資料預設集」清單中選取預設集，然後選取 **[!UICONTROL 編輯]**.

1. 展開您要包含在預設集中的標題，然後在您要包含在預設集中的不同欄位中輸入值。
1. 選取 **[!UICONTROL 儲存]**.

   预设的所选类别和字段将显示在“预览”面板中。

### 管理元数据预设 {#managing-metadata-presets}

1. 前往 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 中繼資料]** > **[!UICONTROL 中繼資料預設集]**.
1. 执行以下任一操作：

   * 要预览预设，请选择您要预览的预设。预设信息（类别和字段）将显示在“预览”屏幕中。
   * 若要刪除預設集，請選取預設集，然後選取 **[!UICONTROL 刪除]**.

## 用户定义的字段 {#user-defined-fields}

Media Portal 管理员或公司管理员可以创建自定义的、用户定义的元数据字段。自訂欄位可協助您在Adobe Dynamic Media Classic中組織資產。 您可以視需要將欄位標示為「作用中」。 啟動後，這些自訂中繼資料欄位的名稱會顯示在「詳細資料檢視」的「中繼資料」面板中。 用户可以在用户定义的元数据字段中输入信息以描述资源。用户也可以使用户定义的元数据字段成为搜索条件。

高效使用用户定义的元数据字段的一种方式是为特定启动或销售延迟资源的激活时间。您可以根據型別定義「啟用」欄位 *日期*. 然後，使用 **[!UICONTROL 中繼資料]** 「詳細資料檢視」中的面板或 **[!UICONTROL 檔案]** > **[!UICONTROL 編輯資訊]**，您可以指定資產啟動的時間。 Adobe Dynamic Media Classic會檢查資產的發佈狀態和發佈歷史記錄。 如果不在啟動時間內，發佈狀態會顯示為「未發佈」。

>[!NOTE]
>
>若要讓使用者定義的欄位顯示在「詳細資料檢視」的中繼資料面板中，請在中繼資料檢視中加入使用者定義的欄位。 在“元数据视图”屏幕上，选择“包括 UDF”（用户定义的字段）选项。有关更多信息，请参阅[元数据视图](application-setup.md#metadata_views)。

>[!NOTE]
>
>若要使用自訂、使用者定義的欄位來搜尋資產，請前往 **[!UICONTROL 設定]** > **[!UICONTROL 個人設定]**，然後選取 **[!UICONTROL 在搜尋中包含UDF]**. 请参阅[个人设置](personal-setup.md#personal_setup)。

### 建立使用者定義的中繼資料欄位 {#creating-a-user-defined-metadata-field}

1. 前往 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 中繼資料]** > **[!UICONTROL 使用者定義的欄位]**.
1. 選取 **[!UICONTROL 新增]**
1. 在“自定义字段”对话框中，设置所需的选项。

   * **[!UICONTROL 名稱]**  — 輸入中繼資料欄位的名稱。

   * **[!UICONTROL 型別]**  — 選取一個選項，以定義使用者可在中繼資料欄位中輸入的資訊型別：

   * **[!UICONTROL 字串]**  — 文字字串。

   * **[!UICONTROL Int]**  — 整數。

   * **[!UICONTROL 浮點數]**  — 浮點數。

   * **[!UICONTROL 是/否]**  — 是/否布林值。

   * **[!UICONTROL 日期]**  — 日期。 接受 MM/DD/YYYY 格式。

   * **[!UICONTROL 檔案名稱]**  — 檔案的名稱。

   * **[!UICONTROL 顏色]**  — 顏色的名稱。

   * **[!UICONTROL Dimension]**  — 資產的寬度和高度。

   * **[!UICONTROL 無型別]**  — 提供回溯相容性。 请勿选择此选项。

   * **[!UICONTROL 預設值]**  — 選擇性地輸入使用者最有可能在欄位中輸入的值。 您输入的值会成为您所创建的字段的默认值。

   * **[!UICONTROL 套用至]**  — 如果您希望中繼資料欄位僅套用至特定型別的資產，您可以選擇性地選取資產型別。

      >[!NOTE]
      >
      >選取 **[!UICONTROL 套用至]** 選項，因為您無法變更 **[!UICONTROL 套用至]** 選項。 Adobe Dynamic Media Classic可讓您編輯使用者定義欄位的名稱、型別和預設值，但無法編輯 **[!UICONTROL 套用至]** 設定。*

1. 選取 **[!UICONTROL 儲存]** 當您完成建立中繼資料欄位時。

### 管理用户定义的字段 {#manage-user-defined-fields}

“用户定义的字段”屏幕提供了用于管理自定义、用户定义的元数据字段的命令。

只有 Media Portal 管理员或公司管理员可以管理用户定义的字段。

若要開啟此畫面，請前往 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 中繼資料]** > **[!UICONTROL 使用者定義的欄位]**.

* **編輯欄位**  — 選取欄位，然後選取 **[!UICONTROL 編輯]**.

* **刪除欄位**  — 選取欄位，然後選取 **[!UICONTROL 刪除]**.

* **啟用欄位**  — 選取或取消選取 **[!UICONTROL 作用中]** 欄位名稱旁的選項。 如果您處於公司管理角色，則不會顯示此選項。 由於此選項與MediaPortal有關，因此您必須選取（開啟） 「在個人設定中顯示MediaPortal功能」才能檢視啟用欄位。

## 优化文件 {#optimize-files}

上傳檔案至Adobe Dynamic Media Classic時，系統會最佳化檔案的儲存和發佈作業。 然而，如果上载过程中断，则无法优化某些图像。在这种情况下，您会看到“尚未优化图像”消息。然而，如果您是管理员，则可以优化这些文件。

Adobe Dynamic Media Classic只會搜尋您的檔案，並最佳化那些之前未完全最佳化的影像。

1. 前往 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]**，然後選取 **[!UICONTROL 最佳化檔案]**.
1. 輸入最佳化工作的資訊，然後選取 **[!UICONTROL 提交]**.

   如果您在与多家公司协作，请分别优化属于不同公司的文件。

## 批量集预设 {#batch-set-presets}

當工作執行以將資產上傳到Adobe Dynamic Media Classic時，使用批次集預設集可自動建立影像集或迴轉集。

公司管理員首先會針對他們想要分組到一組中的資產定義命名慣例。 然後，您可以建立批次集預設集來參考這些影像。 每个预设都是单独命名的、自成体系的指令集，指令集可定义如何使用与预设方法中定义的命名约定匹配的图像构建集。

“上载作业选项”对话框会列出公司的所有活动批量集预设，以便您指定要在每个上载会话期间应用的预设。公司管理员将看到所有活动和非活动的批量集预设。上傳檔案時，Adobe Dynamic Media Classic會自動建立一個集合，其中包含與作用中預設集中定義的命名慣例相符的所有檔案。

### 默认命名 {#default-naming}

公司管理员创建在任何批量集预设方法中使用的默认命名约定。在批次集預設集定義中選取的預設命名慣例可能是貴公司批次產生所有網站集所需的一切。 要使用您定义的默认命名约定，需创建批量集预设。如果公司定义的默认命名有例外情况，您可以为一组特定内容根据需要使用备用的自定义命名规则创建任意数量的批量集预设。

使用批次集預設集功能不需要設定預設命名慣例。 不過，Adobe最佳實務建議您使用預設命名慣例來定義要在集合中分組的命名慣例元素。 這麼做有助於簡化批次集的建立。

1. 前往 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 批次集預設集]** > **[!UICONTROL 預設命名]**.
1. 选择“**[!UICONTROL 查看表单]**”或“**[!UICONTROL 查看代码]**”，以指定您希望如何查看和输入有关每个元素的信息。

   您可以選取 **[!UICONTROL 檢視程式碼]** 核取方塊，以檢視表單選取專案旁的規則運算式值建置。 如果表单视图因某种原因对您构成限制，您可以输入或更改上述值，以帮助定义命名约定的元素。如果無法在表單檢視中剖析您的值，則表單欄位會變成非作用中。

   >[!NOTE]
   >
   >停用的表单字段并不表示正则表达式无效。没有针对正则表达式正确性的验证措施。您会在“结果”行的后面看到您为每个元素构建的正则表达式的结果。完整的正则表达式显示在页面底部。

1. 根据需要展开每个元素，并输入您要使用的命名约定。
1. 視需要選取 **[!UICONTROL 新增]** 為元素新增其他命名慣例。 或者，選取 **[!UICONTROL 移除]** 刪除元素的命名慣例。
1. 選取 **[!UICONTROL 另存為]** 並輸入預設集的名稱。 或者，選取 **[!UICONTROL 儲存]** 如果您正在編輯現有的預設集。

另外，您还可以使用没有表单字段的“查看代码”。在此檢視中，您完全使用規則運算式來建立命名慣例定義。

有两个元素可用于定义，即“匹配”和“基本名称”。在这些字段中，您可以定义命名约定的所有元素，并指定用于命名它们所在的集的约定部分。公司的個別命名慣例可能會對這些元素中的每一個使用一或多行定義。 可以在您的特有定义中使用所需数量的行，并将它们分组到不同的元素中，例如，用于主图像、颜色元素、备选视图元素和样本元素。

### 创建批量集预设 {#creating-a-batch-set-preset}

Adobe Dynamic Media Classic使用批次集預設集來組織共用某些常見資訊或內容的資產，使其成為影像集並在檢視器中顯示。 批次集預設集配方會自動與您在Adobe Dynamic Media Classic中排程的資產匯入作業一起執行。

可以使用“批量集预设”创建、编辑和管理批量集预设。您可以視需要建立儘可能多的預設集，以涵蓋所需的所有資產擷取工作。 批次集預設集定義有兩種形式：一種是您已設定的預設命名慣例，另一種是您立即建立的自訂命名慣例。

您可以使用表單欄位方法來定義批次集預設集，或使用程式碼方法來讓您使用規則運算式。 如在 **[!UICONTROL 預設命名]**，您可以選取 **[!UICONTROL 程式碼檢視]** 同時，您要在表單檢視中定義，並使用規則運算式來建置定義。 或者，您可以取消选中任一视图，只使用其一个视图。

另請參閱 [建立批次集預設集以自動產生2D迴轉集](application-setup.md#creating_a_batch_set_preset_for_the_auto_generation_of_a_2d_spin_set).

另請參閱 [2D迴轉集](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/537_2d-spin_converted%20renamed_Done-AVS) 訓練影片。

**创建批量集预设:**

1. 前往 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 批次集預設集]** > **[!UICONTROL 批次集預設集]**. 默认视图为“**[!UICONTROL 查看表单]**”（在“详细信息”页面的右上角设置）。
1. 在「預設集清單」面板中，選取 **[!UICONTROL 新增]** 以啟動頁面右側「詳細資訊」面板中的定義欄位。
1. 在“详细信息”面板的“预设名称”字段中，键入预设的名称。
1. 在“批量集类型”下拉菜单中，选择预设类型。

   要自动生成 2D 旋转集，请在“批量集类型”下拉列表中选择“**[!UICONTROL 多轴旋转集]**”。

1. 执行以下任一操作：

   * 如果您使用先前在下設定的預設命名慣例 **[!UICONTROL 應用程式設定]** > **[!UICONTROL 批次集預設集]** > **[!UICONTROL 預設命名]**，展開 **[!UICONTROL 資產命名慣例]**，然後在「檔案命名」下拉式清單中，選取 **[!UICONTROL 預設]**.
   * 若要在設定預設集時定義命名慣例，請展開 **[!UICONTROL 資產命名慣例]**，然後在「檔案命名」下拉式清單中，選取 **[!UICONTROL 自訂]**.

1. 在「序列順序」中，定義影像集在Adobe Dynamic Media Classic中分組後的順序。 默认情况下，将按字母数字顺序对您的资源排序。不过，可以使用逗号分隔的正则表达式列表来定义顺序。
1. 对于设置命名和创建约定，为您在“资源命名约定”中定义的基本名称指定后缀或前缀。也定義在Adobe Dynamic Media Classic資料夾結構中建立影像集的位置。

   如果您定義大量影像集，請將這些影像集與包含資產本身的資料夾分開。 许多客户会创建一个“图像集”文件夹，并让应用程序将批量集生成的集合放在此处。

1. 選取 **[!UICONTROL 儲存]** 在「詳細資訊」面板中。

### 建立批次集預設集以自動產生2D迴轉集 {#creating-a-batch-set-preset-for-the-auto-generation-of-a-d-spin-set}

您可以使用批量集类型“**多轴旋转集**”来创建用于自动生成 2D 旋转集的“方法”。对图像进行分组时采用“行”和“列”正则表达式，以便图像资源在多维数组的对应位置中正确对齐。

另請參閱 [建立批次集預設集](application-setup.md#creating_a_batch_set_preset).

多軸旋轉集中沒有最小或最大列數或欄數。

例如，假設您要建立名為的多軸旋轉集 *spin-2dspin*. 有一组旋转集图像包含 3 行，每行 12 个图像。这些图像命名如下：

```as3
spin-01-01
spin-01-02
… 
spin-01-12
spin-02-01
… 
spin-03-12
```

您可以使用此資訊來建立「批次集型態」配方，如下所示：

![批次集配方影像](assets/se_batch_set_recipe.png)

迴轉集之共用資產名稱部分的分組會新增至「比對」欄位（反白顯示）。 将包含行和列的资源名称的变量部分分别添加到“行”和“列”字段。

在上载和发布旋转集时，将激活在“上载作业选项”对话框的“**[!UICONTROL 批量集预设]**”下面列出的 2D 旋转集方法名称。

**创建用于自动生成 2D 旋转集的批量集预设:**

1. 前往 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 批次集預設集]** > **[!UICONTROL 批次集預設集]**. 默认视图为“**[!UICONTROL 查看表单]**”（在“详细信息”页面的右上角设置）。
1. 在「預設集清單」面板中，選取 **[!UICONTROL 新增]** 以啟動頁面右側「詳細資訊」面板中的定義欄位。
1. 在“详细信息”面板的“预设名称”字段中，键入预设的名称。
1. 在“批量集类型”下拉菜单中，选择“**[!UICONTROL 资源集]**”。
1. 在“子类型”下拉列表中，选择“**[!UICONTROL 多轴旋转集]**”。
1. 展開 **[!UICONTROL 資產命名慣例]**，然後在「檔案命名」下拉式清單中，選取 **[!UICONTROL 自訂]**.
1. 使用“**[!UICONTROL 匹配]**”和（可选）“**[!UICONTROL 基本名称]**”属性定义用于对构成分组的图像资源进行命名的正则表达式。

   例如，您的常值Match規則運算式可能如下所示：

   `(\w+)-\w+-\w+`

1. 展开“**[!UICONTROL 行列位置]**”，然后为 2D 旋转集数组中图像资源的位置定义名称格式。

   使用圆括号将文件名中的行或列位置括起来。

   例如，針對列規則運算式，其外觀可能如下所示：

   `\w+-R([0-9]+)-\w+`

   或者

   `\w+-(\d+)-\w+`

   對於欄規則運算式，它可能會如下所示：

   `\w+-\w+-C([0-9]+)`

   或者

   `\w+-\w+-C(\d+)`

   請記住，這些運算式只是範例。 您可以创建任何满足自己需要的正则表达式。

   >[!NOTE]
   >
   >如果列和欄中的規則運算式組合無法判斷資產在多維度迴轉集陣列中的位置，則該資產不會新增到集合中，並會記錄錯誤。

1. 对于设置命名和创建约定，为您在“资源命名约定”中定义的基本名称指定后缀或前缀。也定義在Adobe Dynamic Media Classic資料夾結構中建立影像集的位置。

   如果您定義大量影像集，請將這些影像集與包含資產本身的資料夾分開。 许多客户会创建一个“图像集”文件夹，并让应用程序将批量集生成的集合放在此处。

1. 選取 **[!UICONTROL 儲存]** 在「詳細資訊」面板中。
1. 照常上载和发布您的旋转集，同时确保您在“作业加载选项”对话框中的“批量集预设”下激活 2D 旋转集的名称。

>[!MORELIKETHIS]
>
>* [預覽資產](previewing-asset.md#previewing_an_asset)
>* [設定影像預設集](setting-image-presets.md#setting_up_image_presets)
>* [檢視、新增和匯出中繼資料](viewing-adding-exporting-metadata.md#viewing_adding_and_exporting_metadata)
>* [檢查工作檔案](checking-job-files.md#checking_job_files)

