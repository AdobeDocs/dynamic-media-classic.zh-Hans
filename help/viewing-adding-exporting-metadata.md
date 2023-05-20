---
title: 檢視、新增和匯出中繼資料
description: 瞭解如何在Adobe Dynamic Media Classic中檢視、新增和匯出中繼資料。
uuid: a5254c51-9e04-45ae-8236-3eab2925e5fc
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: 5414b4f5-6e05-468c-8725-385423596342
feature: Dynamic Media Classic,Asset Management,Metadata
role: User
exl-id: 2be50cc7-9a8b-4f7b-8ebf-18a3208654f2
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '2261'
ht-degree: 45%

---

# 檢視、新增和匯出中繼資料{#viewing-adding-and-exporting-metadata}

您可以儲存您在Adobe Dynamic Media Classic中處理之檔案的特定資訊；此資訊稱為 *中繼資料*. 您可以在Adobe Dynamic Media Classic中使用中繼資料來組織、搜尋、篩選和排序您的資產。

中繼資料會與Adobe Dynamic Media Classic產生的資訊一起顯示在「詳細資料檢視」中，例如檔案建立日期、發佈日期和關鍵字。 若要檢視中繼資料，請在「詳細資料檢視」中開啟資產，然後選取「中繼資料」面板。 可以在详细信息视图中输入和编辑 元数据。

一些元数据直接嵌入到文件中。如果檔案包含此中繼資料，Adobe Dynamic Media Classic會自動將其與檔案一起上傳。 您可以將中繼資料內嵌至Adobe Photoshop、InDesign、Illustrator和其他應用程式的來源資產；Adobe Dynamic Media Classic可辨識此中繼資料。 您也可以在「詳細資料檢視」的「中繼資料」面板中，將中繼資料新增至個別檔案。 为了确保资源的一致性，公司管理员创建了元数据模板，提供可以填写的元数据字段。

如需內嵌中繼資料的詳細資訊，請參閱 [可延伸的中繼資料平台](https://www.adobe.com/products/xmp.html).

## 查看元数据 {#view-metadata}

若要檢視資產的中繼資料，請在「詳細資料檢視」中開啟資產，然後點選「中繼資料」面板。 若要選取一組中繼資料欄位，請在「中繼資料檢視」選單中選擇選項。 Adobe Dynamic Media Classic提供下列中繼資料檢視：

* **壓縮檢視**  — 基本值清單。

* **IPTC**  — 國際新聞通訊委員會定義的值。

* **XMP**  — 可延伸中繼資料程式定義的值。

管理员可以创建元数据视图。这些视图也显示在“元数据视图”菜单中。

另請參閱 [中繼資料檢視](application-setup.md#metadata_views) 以取得關於建立中繼資料檢視的資訊。

## 为资源手动输入元数据 {#manually-enter-metadata-for-an-asset}

1. 在「詳細資料檢視」中開啟資產。
1. 打开“元数据”面板并执行以下一项操作或全部操作：

   * 选择一种元数据视图，以确定面板中显示哪些元数据字段。
   * 選擇預設值，然後選取 **[!UICONTROL 套用]** 以使用預設值填入中繼資料欄位。 这些预设值由公司管理员创建。

1. 在“元数据”面板中输入值。

>[!NOTE]
>
>若要一次編輯多個資產的中繼資料，請選取資產並前往 **[!UICONTROL 檔案]** > **[!UICONTROL 編輯資訊]**. 在“编辑信息”窗口中对元数据所进行的编辑会应用于所有选定资源。

## 添加或编辑关键字 {#add-or-edit-keywords}

除了中繼資料之外，您還可以使用關鍵字來協助搜尋和管理您的資產。

如果您在此工作階段期間將關鍵字新增至其他檔案，或者如果您已從清單中移除關鍵字，關鍵字會出現在關鍵字建議表格中。

1. 在详细信息视图中打开文件。
1. 選取 **[!UICONTROL 關鍵字]**.
1. 要添加关键字，请执行以下任意操作：

   * 在文字方塊中輸入關鍵字並選取 **[!UICONTROL 新增]**.
   * 在「 」中選擇關鍵字 **[!UICONTROL 關鍵字建議]** 表格。

1. 若要移除關鍵字，請選取該關鍵字並選取 **[!UICONTROL 移除]**. 该关键字会移到“关键字建议”表中。

>[!NOTE]
>
>您可以將關鍵字上傳至Adobe Dynamic Media Classic時新增至檔案。 在「上載工作選項」對話方塊中，選擇 **[!UICONTROL 其他中繼資料]** 並輸入關鍵字。
>请参阅[上载选项](uploading-files.md#upload_options)。

## 导入元数据 {#import-metadata}

可以从制表符分隔的文件或 XML 文件为多个不同资源导入元数据，而不必每次一个为资源手动输入元数据。在制表符分隔文件或 XML 文件中输入元数据并导入该文件比在各个资源中输入元数据节省时间。在制表符分隔文件的第一行中，输入要为其记录元数据的字段的 ID 和名称。在每个后续行中，输入资源 ID 名称，后跟元数据值。系统不会对制表符分隔文件或 XML 文件中未包括的字段进行修改。要从 XML 文件导入元数据，请确保您符合 DTD。

>[!NOTE]
>
>您可以建立用於輸入中繼資料的範本，以便將其正確匯入至Adobe Dynamic Media Classic。 创建模板之后，可以使用该模板输入元数据。
>请参阅[创建模板以输入要上载的元数据](viewing-adding-exporting-metadata.md#create_a_template_for_entering_metadata_to_upload)。

如需有關標準化屬性的詳細資訊，請參閱 [Adobe XMP開發人員中心](https://www.adobe.com/devnet/xmp.html).

1. 在浏览面板中，选择要从制表符分隔的文件或 XML 文件为其添加元数据的图像。
1. 前往 **[!UICONTROL 檔案]** > **[!UICONTROL 匯入中繼資料]**.
1. 在 **[!UICONTROL 上傳中繼資料]** 對話方塊，選取 **[!UICONTROL 瀏覽]**.
1. 在“**[!UICONTROL 选择要上载的文件]**”对话框中，选择包含元数据的制表符分隔文件或 XML 文件。
1. 输入作业名称。
1. 選取 **[!UICONTROL 上傳]**.

### 識別匯入中的不同中繼資料型別

在识别要导入的不同元数据类型时，请记住以下几点：

* 使用者定義欄位是以在中建立的名稱來識別 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 中繼資料]** > **[!UICONTROL 使用者定義的欄位]**. 使用“生成文件”功能来获取采用正确导入格式的所有已定义 UDF 的列表。
* “XMP 元数据”属性在（属性-）名称之前必须具有相关 XMP- 前缀。前缀和名称之间用冒号分隔。XMP首碼可在以下網址找到： **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 中繼資料]** > **[!UICONTROL 中繼資料結構]** 編輯者。 技术名称可在相关 XMP 架构文档中找到。XMP屬性名稱未出現在「產生檔案」功能中。
* “元数据架构”属性在（属性-）名称之前必须具有相关前缀。前缀和名称之间用冒号分隔。前缀和属性名称是在元数据架构编辑器中定义的。中繼資料結構描述屬性名稱未出現在「產生檔案」功能中。

例如：關鍵字的XMP屬性是首碼為XMP結構描述「Dublin Core」 `dc` 和 `subject` 是技術XMP名稱。 前置詞和技術XMP名稱會合併至 `dc:subject` 完整屬性名稱。 在XML中繼資料匯入格式中， `dc.subject` 必須是屬性名稱。 在以Tab字元分隔的匯入格式中，它必須是欄標題。

### 导入关键字

關鍵字可以匯入為以逗號分隔的清單。 如果逗號出現在任何個別值中，則必須使用反斜線(\)逸出。 反斜杠字母为常见的双反斜杠 (\\)。

例如，包含值的中繼資料匯入檔案 `Hello\, World!,back\\slash,foo` 的 `dc:subject` 在資產上設定三個XMP關鍵字： `Hello, World!,` `back\slash,` 和 `foo`.

### 导入 XMP 和元数据架构元数据 XMP 文件

XML 导入仅接受有效的 XML。匯入XMP或中繼資料結構欄位時，會新增名稱空間前置詞，其行為類似於XMP-namespace。 必須宣告此名稱空間。 例如，在頂層標籤中。

例如：

```as3
<ips> 
    <ghw_object vc_objectname="img_001" dc:subject="word1,word2" 
</ips>
```

### 匯入XMP和中繼資料結構描述資料（以Tab分隔）檔案

必须在导入字段的相关列标题中添加前缀。

## 导入元数据（通过 FTP） {#import-metadata-via-ftp}

您可以在定位字元分隔或XML檔案中輸入中繼資料，然後選取 **[!UICONTROL 處理中繼資料檔案]** 上傳工作選項（透過FTP索引標籤）頁面。

确保制表符分隔文件或 XML 文件中的数据格式正确。在第一行中，输入 ID 字段，随后输入要修改的元数据字段名称。在每个后续行中，输入资源 ID 名称，后跟元数据值。系统不会对制表符分隔文件或 XML 文件中未包括的字段进行修改。

在全域導覽列上，選取 **[!UICONTROL 上傳]**. 若要匯入中繼資料，請在「上傳」頁面上選取 **[!UICONTROL 透過FTP]** 索引標籤，然後選取 **[!UICONTROL 工作選項]**. 在「上載工作選項」對話方塊中，選取 **[!UICONTROL 工作]**，然後選取 **[!UICONTROL 處理中繼資料檔案]** 核取方塊。

## 使用元数据批量重命名 ID {#batch-rename-ids-using-metadata}

您可以使用從定位字元分隔檔案或XML檔案匯入的中繼資料，重新命名Adobe Dynamic Media Classic ID。 导入的元数据仅适用于在元数据文件自身中指定的图像。無論是否在「瀏覽」面板上選取影像。

若要重新命名影像的Adobe Dynamic Media Classic ID，請新增標籤為的欄 *newipsid* 至以Tab分隔的檔案，或新增欄位 `new_vc_objectname` 至XML資料。

例如：

|  | newipsid |
| --- | --- |
| testjacket_1 | Jacket_test_1 |
| testjacket_blue | Jacket_test_2 |

中繼資料工作的工作記錄會顯示哪些ID已成功重新命名，哪些未重新命名。

## 创建模板以输入要上载的元数据 {#create-a-template-for-entering-metadata-to-upload}

Adobe Dynamic Media Classic提供用來建立記錄中繼資料範本的命令。 使用範本可確保中繼資料以正確的格式輸入，以便正確地上傳至Adobe Dynamic Media Classic。 若要建立範本以用於記錄中繼資料並將其匯入至Adobe Dynamic Media Classic，請遵循下列步驟：

1. 選取含有您想要用於範本的中繼資料欄位的影像資產。
1. 前往 **[!UICONTROL 檔案]** > **[!UICONTROL 匯入中繼資料]**.
1. 對於 **[!UICONTROL 資產屬性型別]**，選取 **[!UICONTROL 影像]**.
1. 從 **[!UICONTROL 產生檔案]** 下拉式清單，選擇 **[!UICONTROL Tab字元分隔範本]**， **[!UICONTROL 資產的XML中繼資料]**，或 **[!UICONTROL XML DTD]**.
1. 選取 **[!UICONTROL 產生]**.
1. 在显示的对话框中，复制数据。使用此数据构建模板。

## 使用元数据架构 {#working-with-metadata-schemas}

公司管理员可以查看所有可用的架构的列表。在全域導覽列上，前往 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 中繼資料]** > **[!UICONTROL 中繼資料結構]**.

最初，會隱藏XMP等全域標準結構描述的清單。 通过选中列表底部的复选框，可以显示该列表。

公司管理員可以建立自訂結構，或編輯現有的自訂結構。

您可以使用元数据架构编辑器来执行以下操作：

| 操作 | 说明 |
| --- | --- |
| 添加 | 將屬性新增至結構描述。 強制回應對話方塊會收集資訊：ID、標籤、結構和資料型別。 |
| 添加选项值 | 向结构为开放式选项或限定式选项的属性中添加新的可选择选项。所有选项值的类型相同。選取屬性本身以啟用按鈕。 |
| 编辑 | 编辑属性或选项值的标签。您仅可更改标签、ID，类型信息不可变。 |
| 上移/下移 | 架构的顺序反映在 UI 中。要更改此顺序，请选择属性或选项值，并通过按钮进行移动。目前不支援拖放。 |
| 删除 | 从架构中删除属性或选项值。它不會從XMP區塊或資料庫刪除值。 屬性不再適用於中繼資料檢視，且已從資產詳細資料檢視中移除。 如果屬性已發佈至中繼資料伺服器，請執行強制發佈，從公開的中繼資料伺服器移除資料。 |

系統會自動為使用者定義的欄位產生具有首碼的自訂結構 `s7udf`. 它是現有的使用者定義欄位，並在其自己的設定區段中編輯。

>[!NOTE]
>
>对架构所做的更改永远不会更改资源元数据自身。不過，並非所有Adobe Dynamic Media Classic和中繼資料伺服器功能都能看見這些專案，且無法在變更後加以存取。 同樣地，如果資產的中繼資料存在，建立相符的結構描述會使中繼資料可用於Adobe Dynamic Media Classic和中繼資料伺服器。

中繼資料結構編輯器提供在Adobe Dynamic Media Classic中新增或編輯自訂公司結構的圖形方式。 架构由前缀、命名空间和一系列属性定义。

* **[!UICONTROL 名稱]**  — 結構描述的UI-Name。 用于在元数据视图和高级搜索中识别属性。类似于 XMP 部分，如“基本”、IPTC、PDF。

* **[!UICONTROL 前置詞]**  — 結構描述的技術唯一識別碼。 僅限於字母a-z和A-Z。前置詞不會顯示在Adobe Dynamic Media Classic UI中，但會在資產的中繼資料儲存在XMP區塊和資料庫時使用。 前缀用于在元数据服务器上的元数据搜索查询中或导入时唯一识别元数据字段。

* **[!UICONTROL 名稱空間]**  — 結構描述的技術唯一識別碼，通常為表單中的URL `https://your.company.com/name/version/`. 有关示例，请参阅标准架构列表。名稱空間不會顯示在Adobe Dynamic Media Classic UI中，但會用來將中繼資料儲存在XMP區塊中。

* **[!UICONTROL 說明]**  — 結構描述的自由形式說明。

>[!NOTE]
>
>前缀和命名空间无法编辑。要更改这些属性，您必须删除并重新创建架构。

属性用于描述可与此架构一起存储在 XMP 块中的元数据。属性包括：

| 属性 | 说明 |
| --- | --- |
| ID | 该属性的技术性标识符。ID不會顯示在Adobe Dynamic Media Classic UI中，但會在資產的中繼資料儲存於XMP區塊和資料庫時使用。 ID 用于在元数据服务器上创建搜索查询。ID 具有以下限制： <ul><li>不得包含空格</li><li>不得包含“.”、“:”和“$”</li><li>第一个字符不得为数字</li><li>最好使用 a-z 或 A-Z 作为第一个字符</li></ul> <br>创建后，ID 即无法更改。 |
| 标签 | 该属性的 UI 名称。 |
| 结构 | 与数据类型一起确定属性的类型。结构可能为：<ul><li>简单类型：单个数据类型值</li><li>序列：相同数据类型的值的列表</li><li>开放式选项：从预定义的值列表中选择一项，或随意输入文本。数据类型仅可为字符串型或整型</li><li>限定式选项：从预定义的值列表（弹出窗口或组合框）中选择一项</li></ul> |
| 数据类型 | 从以下可用的类型中选择： <ul><li>字符串型</li><li>整型</li><li>浮点型</li><li>是/否（布尔型）</li><li>日期</li></ul> |

当属性的结构为“开放式选项”或“限定式选项”时，您必须提供至少一个选项值。开放式选项可以更改。限定式选项不可更改。所有选项值都具有属性的数据类型。

| 属性 | 说明 |
| --- | --- |
| ID | 该值的技术性标识符。ID不會顯示在Adobe Dynamic Media Classic UI中，但會用於資產的中繼資料儲存於XMP區塊和資料庫時。 ID 用于元数据服务器上的搜索查询。ID 不可包含空格。创建后，ID 即无法更改。 |
| 标签 | 该值的 UI 名称。 |

>[!MORELIKETHIS]
>
>* [Viewer Presets](application-setup.md#viewer_presets)
>* [Metadata Presets](application-setup.md#metadata_presets)

