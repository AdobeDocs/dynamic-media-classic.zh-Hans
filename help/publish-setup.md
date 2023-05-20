---
title: 发布设置
description: 發佈設定可讓您決定預設如何從Adobe Dynamic Media Classic伺服器將資產傳送至網站或應用程式。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic
role: Admin
exl-id: 699d4c12-e47b-4c6b-86f3-dc7aaaa56c1e
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '2405'
ht-degree: 42%

---

# 发布设置 {#publish-setup}

「發佈設定」頁面設定會決定預設如何從Adobe Dynamic Media Classic伺服器將資產傳送至網站或應用程式。 如果未指定任何設定，Adobe Dynamic Media Classic伺服器會根據「發佈設定」頁面上的預設設定傳送資產。 例如，傳送不包含解析度屬性的影像的要求會以「影像伺服器」頁面上的「預設物件解析度」設定產生影像。

管理員可以在「影像伺服器」、「影像轉譯器」和「暈映」頁面上變更預設設定，以建立從伺服器傳送資產的預設設定。

若要開啟「發佈設定」頁面，請前往 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 發佈設定]**.

>[!NOTE]
>
>「發佈設定」頁面可供有經驗的網站開發人員和程式設計人員使用。 Adobe Dynamic Media Classic假設在這些頁面上變更設定的使用者熟悉Adobe Dynamic Media Classic、HTTP通訊協定標準和慣例，以及基本影像處理技術。

## 图像服务器 {#image-server}

「影像伺服器」頁面會建立從影像伺服器傳送影像的預設設定。 設定值可用於這五個類別（如需設定的詳細說明，請參閱「影像伺服器」頁面）。

請僅在Adobe Dynamic Media Classic支援人員的協助下變更這些設定。

* **[!UICONTROL 目錄管理]**  — 這些設定會決定Adobe Dynamic Media Classic和目錄互動的方式。 與大部分的網頁伺服器不同，Dynamic Media影像伺服器URL呼叫會前往資訊清單或目錄檔案，而不是一般的影像檔案。 目录文件（不要与 eCatalog 混淆）中包含发布到图像服务器的所有内容的列表，以及每个图像的路径。如果您有 Digimarc ID，请在“Digimarc 用户信息”部分中输入您的用户信息。

* **[!UICONTROL 請求屬性]**  — 這些設定對可從伺服器傳送的影像施加限制。 例如， *最大值* **[!UICONTROL 回覆影像大小限制]** 是 **[!UICONTROL 寬度]** 5000和 **[!UICONTROL 高度]** 5000。

* **[!UICONTROL 預設請求屬性]**  — 這些設定與影像的預設外觀有關。

* **[!UICONTROL 通用縮圖屬性]**  — 這些設定與縮圖影像的預設外觀和對齊有關。

* **[!UICONTROL 目錄欄位的預設值]**  — 這些設定與影像的解析度和預設縮圖型別有關。

* **[!UICONTROL 色彩管理屬性]**  — 這些設定會決定使用哪些ICC色彩設定檔。

* **[!UICONTROL 相容性屬性]**  — 此設定可讓文字圖層中的前導段落和尾隨段落被視為與3.6版相同，以便回溯相容。

* **[!UICONTROL 本地化支援]*** — 這些設定可讓您管理多個地區設定屬性。 它还允许您指定区域设置映射字符串，以便定义查看器中的各种工具提示所需的支持语言。

   例如，如果您的品牌在多个不同国家/地区销售，您可以确保每个国家/地区都有自己特定区域设置的查看器。要实现该功能，请指定区域设置映射字符串。然後，您新增所需語言的翻譯文字字串，以在檢視器的預設集中編輯工具提示文字。

   >[!NOTE]
   > 若要設定本地化支援選項， [使用Admin Console建立支援案例。](https://helpx.adobe.com/enterprise/using/support-for-experience-cloud.html) 在您的支援案例中，要求設定說明。

   有关设置“**[!UICONTROL 本地化支持]**”的更多信息，请参阅[设置资源本地化时的注意事项](publish-setup.md#considerations_when_setting_up_localization_of_assets)。

### 设置资源本地化时的注意事项 {#considerations-when-setting-up-localization-of-assets}

>[!NOTE]
>
>如果您想在Adobe Dynamic Media Classic中設定本地化支援選項，例如「地區設定地圖」欄位， [使用Admin Console建立支援案例。](https://helpx.adobe.com/enterprise/using/support-for-experience-cloud.html) 在您的支援案例中，要求設定說明。

使用Adobe Dynamic Media Classic的常見方式是管理電子商務網站上的產品影像。 国际企业面临如下挑战：类似产品的资源在各个国家/地区之间存在一些差异。通常差異在於整體媒體的一些部分。 複製每個國家的所有資產，並只覆寫這些差異，以解決這些差異是一項巨大的努力，並且與單一主要資產的比喻相悖。 从包含不同音轨的国家/地区特定视频，到产品所用电源线的细微但重要的差异，此类资源差异可能会持续存在。Adobe Dynamic Media Classic使用基本查詢機制。 您可以从所需的区域设置开始，定义图像服务器查找资源后缀的顺序。

#### 如何本地化资源

IS（图像服务）请求的区域设置通过以下 IS/IR（图像渲染）命令来识别：

`locale=`

此命令接受区域设置 ID (locId) 字符串，不区分大小写。区域设置 ID 通常是由 2-6 个字母和“_”组成的字符串。

IS支援任意可列印的ASCII字串。 此 `locale=` 命令具有全域範圍，這表示它會套用至整個請求，包括所有巢狀IS和IR請求、參照的範本和影像圖層。 不支持每个请求应用多个区域设置，如每个图层应用不同的区域设置。但是，允许在嵌套的请求中显式覆盖区域设置。

若 `locale=` 未指定， `attribute::DefaultLocale` 會傳遞至翻譯引擎。 有限的輸入驗證套用至 `locale=` 值。 空白 `locale=` 允許使用值。 因為 `locale=` 具有全域範圍， `attribute::DefaultLocale` 由主目錄提供，以供整個請求使用。

使用的一些優點 `locale=` 和 `attribute::DefaultLocale` 包含下列專案：

* 针对多个区域设置共享内容。
* 使用通用 ID 访问区域设置特定的内容。
* 在区域设置特定内容的命名约定和管理方面具有相当大的灵活性，如区域设置前缀与后缀或单独目录中的区域设置特定内容。
* 支援地區設定特定版本的存取。
* 彙總物件（例如影像集）有時可以包含對潛在地區設定特定內容的一般參照。
* 支援由需要本地化的目錄管理的所有內容，包括影像、影像集、暈映、素材和檢視器組態記錄。
* 最大程度地减少对 IPS 数据库和 IS 清单机制的更改。
* 實作RFC IS-63時，新增對靜態內容（例如視訊和外觀）的支援。
* 默认区域设置是可配置的。

#### 应用程序方案

| 应用程序 | 方案 |
| --- | --- |
| 檢視器本地化 | 在实施静态内容目录后，本地化可完全通过 locale= 参数控制，该参数会附加到对 IS 的所有请求后面。配置记录、外观和启动画面等可以具有区域设置特定的变量，也可以没有。正确内容由 IS 提供，查看器无需知道哪些内容进行了本地化以及其 ID 是什么。 |
| 影像和視訊 | 跨国公司通常同时拥有通用内容和区域设置特定的内容。通过这种机制，对图像或视频的引用可以是泛型引用，并且 IS 会提供区域设置特定的内容（如果可用）。 |
| 影像集和媒體集 | 某些區域設定的整個影像集可能不同（例如當eCatalog不同時），而由檢視器處理的影像集是從一般環境轉譯為區域設定的特定影像。 更常見的情況是，一般集中的個別ID可以參照本地化的內容。 例如，除控制面板的像片外，裝置的大部分像片在所有語言中都可能相同。 IS 会自动转换 ID，因此无需生成区域设置特定的图像集。 |

#### 實施資產本地化

Adobe Dynamic Media Classic和「影像伺服」有一個介面，可將影像和靜態內容本地化。

当没有本地化版本时，图像服务器 URL 如下所示：

`https://server/is/image/company/image`

透過本地化，影像伺服器URL會新增 `locale=` 路徑引數，如下所示：

`https://server/is/image/company/image?locale=de_DE`

影像伺服器收到http呼叫時， `locale=` 引數是透過 `localeMap` 欄位位於 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 發佈設定]** > **[!UICONTROL 影像伺服器]** > **[!UICONTROL 本地化支援]** 群組。

“区域设置映射”字段包含一个用管道符号 (|) 分隔的条目列表。

每个条目由一个以逗号分隔的值列表组成。第一個值是由下列專案傳遞的搜尋值 `locale=` 引數。 其餘的值是字尾/取代值，然後嘗試這些值，直到其中一個值產生現有影像為止。

具体应用后缀值还是应用替换值，取决于“**[!UICONTROL 设置]**”>“**[!UICONTROL 应用程序设置]**”>“**[!UICONTROL 发布设置]**”>“**[!UICONTROL 图像服务器]**”>“**[!UICONTROL 本地化支持]**”组中的“全局区域设置”。

>[!NOTE]
>
>全域地區設定只有在您透過API (而非Adobe Dynamic Media Classic介面)設定時才可行。

**后缀示例:**

| URL | localeMap ID | 结果 |
| --- | --- | --- |
| `https://server/is/image/company/image?locale=de_DE` | `de_DE,_DE,|fr_FR,_FR,` | 请注意，这里没有定义 GlobalLocale。地區設定引數de_DE與 `localeMap`. 第一个对应值 _DE 将添加为资源 image_DE 的后缀，并尝试在图像服务器上查找该资源。如果在服务器上找到该资源，则会将其返回。否则，使用第二个值“”作为后缀，返回图像本身。 |

**替换示例:**

| URL | `GlobalLocale` 和 `localeMap` ID | 结果 |
|--- |--- |--- |
| `https://server/is/image/company/image-main-01?locale=de_DE` | `GlobalLocale=mainlocaleMap -` <br><br/> `de_DE,de,main|fr_FR,fr,main` | 在以上替换示例中，GlobalLocale 被设置为 main。地區設定引數de_DE與 `localeMap`. 找到GlobalLocale子字串並取代為第一個對應值 `de` 在 `localeMap`： `image-de-01`. 如果在图像服务器上找到，则会将其返回。否则，替换第二个值，最终生成 `image-main-01`。 |

如果 URL 中没有定义区域设置，则图像服务器会采用 DefaultLocale（如果定义）并将其应用到 URL。

如果提供未知或空白的地區設定引數 `locale=`，然後 `localeMap` 會掃描「開頭為」的空白值。 為未知地區設定套用預設地區設定是很重要的事。

#### 關於defaultImage

图像服务器会为请求的区域设置逐个试用选项。如果找不到相符專案，則區域設定選項會套用至defaultImage，並傳回相符版本。 因此，每個地區設定都必須包含影像的選項，但不提供本地化，或是在Adobe Dynamic Media Classic中提供本地化的defaultImage版本。

#### 用于查找 localeMap 的方案

假定您要支持以下区域设置：

`en, en_us, en_uk, de, de_at, de_de, fr`

將這些區域設定對應到尾碼 `_E`， `_G`、和 `_F`，分別代表英文、德文和法文。 对于所有示例，通用输入图像 ID 为 `myImg`。

##### 用于查找 localeMap 的标准行为

区域设置 ID 会被映射到其对应的后缀。如果在目录中找不到区域设置特定的 ID，则尝试使用通用 ID。请注意映射到通用 ID 的空 locSuffix 值。

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,`

| locale= | 要搜索的输出 ID |
| --- | --- |
| en,en_us, en_uk | myImg_E,myImg |
| de,de_de,de_at | myImg_D,myImg |
| fr | myImg_F,myImg |
| 所有其他区域设置 | - |

##### 区域设置未知时查找 localeMap

您可以将未知的区域设置映射到特定 ID 或通用 ID。例如，您可以將未知的地區設定對應至英文ID，或將其不存在，對應至一般ID。

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,|,_E,`

| locale= | 要搜索的输出 ID |
| --- | --- |
| de,de_de,de_at | myImg_D,myImg |
| fr | myImg_F,myImg |
| 所有其他区域设置 | myImg_E,myImg |

您也可以具有專用的locSuffix （例如U），以用於未知的區域設定，如果沒有，則強制預設影像 `_U` 存在，如下所示：

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,|,U`

或者，可以直接映射到通用 ID，如下所示：

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,|,`

##### 使用多層查閱來尋找localeMap

通常，最好对区域设置（如欧洲、中东和北美）进行分组以应对区域标准，如外观曝光。可以使用多层查找来实现这种效果。

对于本示例，假定您要支持供西方和中东使用的集合。这两个集合都基于通用图像集合，而且都添加或修改某些图像。然後針對特定地區設定進一步調整這兩個集合，例如 `m1, m2` 兩個中東變體的，以及 `w1, w2,` 和 `w3` 三種西方語言環境，但共用的影像除外 `w1` 和 `w3`. 未知区域设置仅映射到通用集合，而且无法访问区域设置特定的图像。该映射如下所示：

`attribute::LocaleMap=w1,-W,|w2,-W2,-W,|w3,-W,|m1,-M1,-M,|m2,-M2,-M,|,`

| locale= | 要搜索的输出 ID |
| --- | --- |
| w1, w3 | myImg-W, myImg |
| w2 | myImg-W2, myImg-W, myImg |
| m1 | myImg-M1, myImg-M, myImg |
| m2 | myImg-M2, myImg-M, myImg |
| 所有其他区域设置 | mylmg |

##### 搜尋特定ID以尋找localeMap

有些影像命名慣例不支援一般影像ID。 必须将请求中的通用 ID 映射到目录中的特定 ID。但在某些情況下，確切的特定ID會不明。

以第一個範例為基礎，所有語言的影像都可以有尾碼 `_1`， `_2`，或 `_3`. 法語地區設定的特定影像可以有尾碼 `_22` 或 `_23` 字尾。 而德文地區設定的特定影像可以有尾碼 `_470` 或 `_480`.

`attribute::LocaleMap=,_1,_2,_3|fr,_22,_23,_1,_2,_3|de,_470,_480,_1,_2,_3|de_at,_470,_480,_1,_2,_3|de_de,_470,_480,_1,_2,_3`

| locale= | 要搜索的输出 ID |
| --- | --- |
| fr | myImg_22, myImg_23, myImg_1, myImg_2, myImg_3 |
| de, de_at, de_de | myImg_470, myImg_480, myImg_1, myImg_2,myImg_3 |
| 所有其他区域设置 | myImg_1, myImg_2, myImg_3 |

##### 实施本地化支持时的重要注意事项

* 本地化仅限基于 ID 的资源调用，无法用于基于路径的资源调用。因此，在调用具有区域设置的视频时，必须以 company/assetID 的形式调用，而不采用视频的完整路径。您無法將rtmp用於本地化，因為此方法僅適用於以路徑為基礎的視訊呼叫。
* 当 localeMap 处于活动状态时，无法使用包含单个视频的“混合媒体集”，否则对媒体集内容的调用会失败。若要解決此問題，您可以將單一視訊新增至最適化視訊集。 然后，将自适应视频集添加到混合媒体集。
* 某些请求没有本地化，例如针对自适应视频集内容的请求。因此，如果您打算使用自我調整視訊集進行本地化，請將自我調整視訊集放在混合媒體集中。 然後，使用呼叫集到混合媒體檢視器中 `locale=` 引數。

## 图像渲染器 {#image-renderer}

「影像轉譯器」頁面會建立從影像轉譯伺服器傳送影像集的預設設定。 設定值可用於這五個類別（如需設定的詳細說明，請參閱「影像伺服器」頁面）：

* **[!UICONTROL 目錄管理]**  — 這些設定決定Adobe Dynamic Media Classic和目錄檔案的互動方式。 Adobe Dynamic Media Classic轉譯器伺服器URL會呼叫目錄，然後目錄會呼叫從伺服器傳送影像。 請僅在Adobe Dynamic Media Classic支援人員的協助下變更這些設定。

* **[!UICONTROL 工作階段屬性]**  — 這些設定會建立錯誤引數、相對影像URL的URL，以及是否允許物件重疊。

* **[!UICONTROL 預設材料屬性]**  — 這些設定會建立影像的預設解析度和銳利化設定。

* **[!UICONTROL 回應影像屬性]**  — 這些設定與影像的預設外觀有關。

* **[!UICONTROL 色彩管理屬性]**  — 這些設定與影像的預設色彩設定有關。

## 晕影 {#vignette}

「暈映」頁面提供建立暈映預設外觀的設定值（請參閱頁面本身以取得選項的詳細說明）。
