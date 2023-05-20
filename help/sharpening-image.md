---
title: 锐化图像
description: 瞭解如何在Adobe Dynamic Media Classic中銳利化影像。
uuid: d86af74a-89c5-4f2b-96ba-f2e7da600bca
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 11cd5362-d90a-4c1e-bfbd-46a65a554409
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 4b3e8368-f8f5-46d9-9130-361a8273de2c
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '2278'
ht-degree: 41%

---

# 锐化图像 {#sharpening-an-image}

锐化是为了让数字图像的轮廓变得更为清晰的图像处理技术。锐化会增加边缘像素之间的对比度，并强调明暗区域的过渡。锐化将增加局部对比度，展现细节。并没有严格的公式可以正确锐化所有图像。锐化过少会使得图像对比度较弱，但过分锐化会增添光晕、伪影和杂波。

Adobe Dynamic Media Classic強烈建議您為所有影像使用影像預設集。 它們可確保大小一致，而且會強制使用「影像預設集」呼叫的任何影像進行銳利化。 此外，您也可以輕鬆編輯和變更「影像預設集」的銳利化引數。 下次发布时，将为使用该预设调用的所有图像提供新的值。

Adobe Dynamic Media Classic也建議對檢視器預設集新增銳利化，然後使用該預設集呼叫檢視器。 這麼做可確保檢視器內的影像清晰且吸引人。

不過，無論您是使用影像預設集和檢視器預設集，還是其他銳利化方法，最根本的辦法是您必須銳利化影像。 如果沒有這個選項，您的影像（和網站）可能會顯得既柔和又模糊。

>[!NOTE]
>
>“锐化”命令可覆盖图像预设设置，包括锐化效果。影像預設集可控制從Dynamic Media影像伺服器傳送影像的大小和格式。 Adobe Dynamic Media Classic強烈建議使用影像預設集來傳送所有影像，以確保影像是以一致的大小和銳利化方式傳送。 不过，在更改单个图像的锐化设置之后，图像预设锐化设置将不再应用于该图像。该图像在传送时将不使用图像预设锐化设置。

通常锐化图像是必须的。Adobe Dynamic Media Classic和影像伺服器提供數個銳利化選項。 了解锐化对图像的作用以及您所需的锐化程度很重要。大多数图像都需要进行一定程度的锐化，但是所需的锐化程度取决于图像。

图像锐化可增加像素的对比度，从而达到突出边缘的效果。人们将这种增强的边缘对比度视为锐度。尽管通过对图像使用锐化滤镜可以很轻松地提高图像品质，但是也很容易过度锐化图像。

过度锐化将造成光晕效果，或使边缘线生成条纹。

您可以遵循最佳實務，在Adobe Dynamic Media Classic和Dynamic Media Image Server上最佳化影像銳利化。

另請參閱 [在Adobe Dynamic Media Classic和Dynamic Media Image Server上銳利化影像的最佳作法](/help/assets/s7_sharpening_images.pdf).

另請參閱 [銳利化](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/547_sharpening1_converted%20renamed_Done-AVS) 訓練影片。

**锐化图像:**

若要銳利化影像，請選取其滑鼠指向效果 **[!UICONTROL 編輯]** 按鈕並選擇 **[!UICONTROL 銳利化]**，或在「詳細資料檢視」的「瀏覽」面板中將其開啟，然後選取「 」 **[!UICONTROL 銳利化]**. 「銳利化編輯器」頁面隨即開啟，其中包含銳利化指令。 選擇命令，然後選取 **[!UICONTROL 儲存]**.

>[!NOTE]
>
>锐化图像之前，您可以选择“应用预设”菜单，然后选择一种图像预设来查看其锐化效果。影像預設集的銳利化效果適用於您的影像。 此 **[!UICONTROL 套用預設集]** 功能表位於「銳利度編輯器」頁面底部。

**銳利化選項**

图像服务器锐化选项如下表所示。

| 名称 | URL 协议 | 值 | 示例 |
| --- | --- | --- | --- |
| 简单锐化 | `op_sharpen` | `0` 或者 `1` | `op_sharpen=1` |
| 重新采样模式 | `resMode` | `bilin`， `bicub`， `sharp2`， `trilin`<br><br>`bilin`：選取標準雙線性內插。 最快速的重新取樣方法；會產生一些鋸齒狀不自然感。<br>`bicub`：選取雙三次方內插。 对 CPU 比 bilin 更敏感，但会产生更清晰且锯齿伪影不太明显的图像。<br><br>`sharp2`：選取修改過的Lanczos Windows®函式作為內插演演算法。 可以產生比雙立方體稍微銳利的結果，但CPU成本較高。<br><br>`trilin`：选择改进的三线式插值法，它同时使用更高和更低的分辨率（如果可用）。建议仅当存在锯齿问题时使用。由于减少高频数据而缩小 JPEG 大小。 | `resMode=sharp2` |
| USM 锐化 | `op_usm` | `amount`， `radius`， `threshold`， `monochrome`<br><br>`amount`：濾鏡強度係數（實數0...5）<br><br>`radius`：濾鏡核心半徑，以畫素為單位（實數0...250） <br><br>`threshold`：濾鏡臨界值層級（整數0...255）<br><br>`monochrome`：設為 `0` 若要分別取消銳利化遮色片銳利化每個顏色元件，請將設為 `1` 銳利化遮色片影像亮度（強度） | `op_usm=1,1,10,0` |

選取 **[!UICONTROL 銳利化]** 功能表並選擇一個選項：

* **無**  — 停用銳利化。

* **銳利化**  — 在調整檔案大小後，對檔案執行簡單的銳利化傳遞。 它類似於Adobe Photoshop中的「銳利化」篩選器，不支援任何使用者引數。 通常您會使用此篩選器或 **[!UICONTROL 不銳利化遮色片]**，但不是兩者皆有。 最佳做法不建议使用此方法，但是它有助于补偿模糊。(URL: `op_sharpen`)

* **不銳利化遮色片**  — 可讓您微調最終縮減取樣影像的銳利化濾鏡效果。 您可以控制效果的強度、效果半徑（以畫素測量），以及忽略的對比度臨界值。 此效果使用与 Photoshop 的“USM 锐化”滤镜相同的选项。(URL: `op_usm`)

選擇下列選項，即可使用「不銳利化遮色片」微調銳利化：

* **數量**  — 控制套用至邊緣畫素的對比量。 默认值为 0.0。对于高分辨率图像，可将该值增加到 5.0。数量用于衡量滤镜强度。此 **[!UICONTROL 數量]** Adobe Dynamic Media Classic中的設定與Adobe Photoshop中的金額設定不同。 Adobe Photoshop使用的量介於1%到500%之間，而Adobe Dynamic Media Classic的範圍為0.0到5.0。 （5.0 大致相当于 Photoshop 中的 500%，0.9 类似于 90%，以此类推。）

* **半徑**  — 決定邊緣畫素周圍影響銳利化的畫素數量。 此效果应用于图像中的所有像素并向四面八方辐射。

最佳半径值取决于图像的大小。低值仅锐化边缘像素。高值锐化像素的范围更广一些。

例如，若要針對2000 x 2000畫素影像和500 x 500畫素影像取得類似的銳利化效果，您可以在2000 x 2000畫素影像上設定兩個畫素的半徑值。 然后，在 500 x 500 像素图像上设置 1 个像素的半径值（具有较多像素的图像具有较大的值）。

* **臨界值**  — 決定套用遮色片銳利化調整濾鏡時要忽略的對比範圍。 此选项确定锐化的像素必须与周围区域相差多少，才被滤镜看作边缘像素并被锐化。

「臨界值」會使用0到255之間的值，也就是灰階影像中的亮度階數。 0=黑色，128=50% 灰色，255=白色。例如，阈值 12 忽略肤色亮度的细微变化以避免增加杂色，但仍会在对比强烈的区域中添加边缘对比度，例如，睫毛与皮肤交接的位置。

例如，假定有一张某人脸部的照片。USM 锐化影响具有最大对比度的图像部分和光滑皮肤本身。甚至最平滑的皮肤也会展现亮度值的细微更改。如果您不使用阈值，滤镜将强调皮肤像素的这些细微更改，从而创建杂色效果（很可能不需要此效果），同时还将增加睫毛的对比度，增强锐度（很可能需要此效果）。为了避免出现该问题，请使用此类阈值：可使滤镜忽略未显著更改对比度的像素（如平滑的皮肤）。為了避免引入雜訊或帶有肉色色調的後置影像，例如，嘗試實驗 **[!UICONTROL 臨界值]** 值2到20。 預設 **[!UICONTROL 臨界值]** 0值會銳利化影像中的所有畫素。

* **套用至**  — 選擇 **[!UICONTROL 每種顏色]** 如果您想要個別套用銳利化至每個色彩元件，請選擇 **[!UICONTROL 亮度]** 如果要將銳利化套用至影像亮度區域。

**重新取样**

選取 **[!UICONTROL 重新取樣]** 選單並選擇選項。 当图像缩减像素取样时，以下选项锐化该图像：

* **[!UICONTROL 無]**  — 關閉重新取樣。

* **[!UICONTROL 雙線性式]**  — 最快速的重新取樣方法；會產生某些明顯的鋸齒狀不自然感。

* **[!UICONTROL 雙三次]**  — 增加影像伺服器上的CPU使用量，但產生較銳利的影像，且鋸齒狀不自然感較不明顯。

* **[!UICONTROL 銳利化2]**  — 產生的結果會比 **[!UICONTROL 雙三次]**，但影像伺服器的CPU成本更高。

* **[!UICONTROL 三線性]**  — 如果可用，同時使用較高和較低解析度；僅在出現鋸齒問題時才建議使用。 由于减少了高频数据，此方法会减小 JPEG 的大小。

**銳利化和影像預設集**

您可以合併所有三種銳利化效果，以獲得最終結果。 不過，不建議使用此方法。 Adobe Dynamic Media Classic建議您將銳利化效果儲存為影像預設集的一部分。 影像預設集可讓您封裝最常使用的影像修飾元，以小型文字字串建立動態調整大小的影像。 影像預設集包含檔案格式(通常是網頁的JPEG)、畫素計數和影像銳利化的值。 您應先建立具名影像預設集，例如「縮圖」，而不是將URL附加至您必須用來建立特定影像大小型別的每個影像修飾元。 然後，使用適當的大小、檔案格式和銳利化選項來設定縮圖「影像預設集」。 使用影像預設集名稱呼叫影像。 影像預設集可縮短整體URL的長度。 這兩個URL會以銳利化產生相同的350x350JPEG影像：

* `https://sample.scene7.com/is/image/S7train/Backpack_A?wid=350&hei=350&fmt=jpeg&qlt=85,0&resMode=sharp2&op_usm=0.9,1.0,8,0`
* `https://sample.scene7.com/is/image/S7train/Backpack_A?$!_s7product$`

图像预设随时都可以更改和更新。您會在發佈後和URL的快取清除後，看到影像預設集變更的結果。

如果您为一个大小类别中的每个图像使用一个预设，则任何公司管理员都可以更新该图像预设的定义、重新发布，并影响使用该格式的每个图像，而无需更改任何 Web 代码。作为最佳做法，请在您的网站针对每个特定大小使用一个图像预设。若要新增影像預設集，請在全域導覽列上，前往 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 影像預設集]**. 然後，選取 **[!UICONTROL 新增]** 或選取 **[!UICONTROL 編輯]** 以變更現有的預設集。 唯一的必填字段是预设自身的名称。不過，最好在每個預設集中加入某種程度的銳利化。

**JPG 品质**

JPG 品质选项控制 JPG 压缩等级：

* **JPG品質**  — 如果您想要控制壓縮等級和色度縮減取樣，請選取此選項。

* **滑桿**  — 決定JPG壓縮等級。 此设置既影响文件大小，又影响图像质量。JPG品質比例為1-100。

* **啟用JPG色度縮減取樣**  — 由於眼睛對高頻色彩資訊的敏感度低於高頻亮度，因此JPEG影像會將影像資訊劃分為亮度和色彩分量。 压缩 JPEG 图像时，通过将各组像素放到一起平均，亮度分量为全分辨率，颜色分量为缩减像素取样。缩减像素采样会将数据量减少二分之一或三分之一，而对于用户所能感知到的质量而言却几乎没有任何影响。缩减像素采样不适用于灰度图像。这种方法会减少对于高对比度图像有用的压缩的数量（例如，包含覆盖文本的图像）。

**設定全公司銳利化選項**

如果您不使用图像预设，或未通过 URL 字符串传送特定的图像服务器锐化协议，在缩减像素采样时，不会对您的图像进行锐化。不過，如果發生這種缺乏銳利化的情況，您可以設定預設銳利化值，然後任何影像都會有一些銳利化。

若要設定貴公司的預設銳利化選項，請前往 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 發佈設定]** > **[!UICONTROL 影像伺服器]**. 如果您將「預設重新取樣模式」設定為 **[!UICONTROL 銳利化2]**&#x200B;時，縮減取樣一律會銳利化影像。

**新增銳利化至檢視器預設集**

除非您将锐化图像修饰符添加到预设，否则较小的初始加载图像会看起来对比度较柔和，因为它在未进行锐化的情况下被缩减像素采样以适合查看器窗口。

檢視器預設集（如影像預設集）可讓您將許多選項集中到一個位置，包括外觀和檢視器選項（例如包括「列印」按鈕或控制縮放動畫的速度）。 檢視器預設集位於與影像預設集相同的區段中，位於 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 檢視器預設集]**.

另請參閱 [檢視器預設集](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/550_viewer-presets_converted%20renamed_Done-AVS) 訓練影片。

可在所有“eCatalog”、“旋转”和“自定义缩放查看器预设”的“核心设置”部分下找到“修饰符”选项。通过将 URL 锐化命令添加到“修饰符”框中，每次使用该查看器预设调用该查看器时，您都可以添加锐化。

若要呼叫檢視器預設集，請使用 `config=` 命令來編輯檢視器URL。 以下是呼叫含有檢視器預設集的影像集（鞋子）的範例(`FantasticoZoom2022`)：

`https://s7d9.scene7.com/s7viewers/html5/ZoomViewer.html?asset=Scene7SharedAssets/ImageSet-Views-Sample&config=S7train/FantasticoZoom2022`

此处的预设将锐化并更改查看器的默认外观。

**建立影像特定覆寫**

最后一个最不推荐的锐化方法是在基于图像创建锐化覆盖。此方法會以影像預設集自己的特定值來覆寫銳利化。 不過，此方法也會取代任何其他任何大小的銳利化方法。 此方法最好用于以下情况：如果您的某些图像分辨率不高，而图像预设的值对于这些小图像而言太高。在此情況下，可能需要針對個別影像進行某些銳利化。

在Adobe Dynamic Media Classic中，選取任何影像，前往「詳細資料檢視」（按兩下或按） **[!UICONTROL 詳細資料檢視]** 按鈕)，然後選取 **[!UICONTROL 銳利化]**. 變更任何引數，然後選取 **[!UICONTROL 儲存]**. 此程式會告訴影像伺服器使用這些銳利化引數，而不是您在URL中呼叫的任何命令，例如銳利化修飾元或影像預設集。 請確定您已發佈，變更才會生效。
