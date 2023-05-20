---
title: 建立eCatalog
description: 瞭解如何在Adobe Dynamic Media Classic中建立eCatalog。
uuid: 2aff05c2-7052-426c-b61d-7f9091f7ace8
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
discoiquuid: 28889c60-596a-40d2-85d4-f48a4f86b932
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: 51d411b2-b4bc-4cf6-afca-dd0ed0d219a1
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '967'
ht-degree: 56%

---

# 创建 eCatalog {#creating-an-ecatalog}

创建 eCatalog 需要对页面排序、选择页面布局、通过绘制图像映射链接页面以及输入变换和超文本数据。也可以选择自定义目录，以使观众能够在 eCatalog 查看器中看到页面名称而不是页码。

## 建立eCatalog {#create}

您可以在eCatalog中包含影像檔案和PDF檔案。

在创建 eCatalog 时，“**[!UICONTROL 保存后发布]**”选项按以下方式影响集和集成员：

| 是否在保存之前选择了“保存后发布”选项？ | 保存后的集状态 | 保存后的集成员状态 |
| --- | --- | --- |
| 是 | 已发布 | 已发布 |
| 否 | 未发布 | 集成员保持其已发布或未发布状态。 |

另请参阅[手动发布资源](publishing-files.md#manually_publishing_assets)和[手动取消发布资源](publishing-files.md#manually_unpublishing_assets)。

**创建 eCatalog:**

1. 采用以下方法之一开始创建 eCatalog：

   * **先選取檔案**  — 在「瀏覽」面板中，選取檔案，然後前往 **[!UICONTROL 建置]** > **[!UICONTROL eCatalogs]**.

   * **從eCatalog畫面開始**  — 前往 **[!UICONTROL 建置]** > **[!UICONTROL eCatalogs]**. 在资源库中选择一个文件夹，将该文件夹中的文件拖到 eCatalog 页面的“排序页面”选项卡中。

      >[!NOTE]
      >
      >要按照名称而不是缩略图查看资源库中的物品，在“个人设置”的“默认资源库”视图中选择“名称”选项。

1. 为 eCatalog 选择整体布局。選取 **[!UICONTROL 1欄式]** 若為單一頁面， **[!UICONTROL 2欄式]** 適用於雙頁跨頁，或 **[!UICONTROL 自訂]** 適用於超過兩頁的頁面跨頁。 在 **[!UICONTROL 變更eCatalog版面]** 對話方塊中，選取 **[!UICONTROL 所有跨頁]** 選項並選取 **[!UICONTROL 確定]**.
1. 或者，您可以選取個別頁面或頁面跨頁，然後選擇 **[!UICONTROL 1欄式]**， **[!UICONTROL 2欄式]**，或 **[!UICONTROL 自訂]** 按鈕。 在 **[!UICONTROL 變更eCatalog版面]** 對話方塊中，選取 **[!UICONTROL 選取的跨頁]** 選項並選取 **[!UICONTROL 確定]**.
1. 根据需要采用以下方法之一重新排序页面：

   * **拖曳**  — 將頁面或跨頁拖曳到新位置。 垂直栏显示要移动的页面的位置。

   * **移動至按鈕**  — 選取頁面或跨頁，選取 **[!UICONTROL 移至]**，然後在功能表中選擇您想要頁面顯示在其前面的頁面。

   * **序號**  — 在「清單檢視」的「序號」欄位中輸入頁碼。

1. 完成后，确保在页面右下角附近选择了“**[!UICONTROL 保存后发布]**”（默认）。
1. 選取 **[!UICONTROL 儲存]**.
1. 在“保存”对话框中，选择一个文件夹以存储您的 eCatalog。在“文件名”字段中，输入旋转集名称。
1. 選取 **[!UICONTROL 儲存]**.

   儲存eCatalog後，您可以選取 **[!UICONTROL 預覽]**.

## 編輯eCatalog {#editing-an-ecatalog}

無論您是編輯已發佈集還是未發佈集， **[!UICONTROL 儲存後發佈]** 選項會以下列方式影響設定和設定成員：

| 是否已发布集？ | 是否在保存编辑内容之前选择了“保存后发布”选项？ | 保存后的集状态 | 保存后的集成员状态 |
| --- | --- | --- | --- |
| 是 | 是 | 已发布 | 已发布 |
| 是 | 否 | 已发布 | 现有的集成员保持其已发布状态。在编辑期间添加的任何新的集成员保持其已发布或未发布状态。 |
| 否 | 是 | 已发布 | 已发布 |
| 否 | 否 | 未发布 | 现有的集成员以及在编辑期间添加的任何新的集成员保持其已发布或未发布状态。 |

另请参阅[手动发布资源](publishing-files.md#manually_publishing_assets)和[手动取消发布资源](publishing-files.md#manually_unpublishing_assets)。

**编辑 eCatalog:**

1. 選取eCatalog的變換 **[!UICONTROL 編輯]** 按鈕。
1. 根据需要，进行相应的更改。
1. 在完成编辑后，确保在页面右下角附近选择了“**[!UICONTROL 保存后发布]**”（默认）。
1. 選取 **[!UICONTROL 儲存]**，選取儲存資料夾，輸入集名稱，然後選取 **[!UICONTROL 儲存]**.

## 刪除eCatalog {#deleting-an-ecatalog}

在删除集时，集本身将移到垃圾桶中。不过，集中的成员（或“子项”）不受影响；它们分别保持现有的已发布或未发布状态。

另请参阅[手动发布资源](publishing-files.md#manually_publishing_assets)和[手动取消发布资源](publishing-files.md#manually_unpublishing_assets)。

**删除 eCatalog:**

1. 在网格视图、列表视图或详细信息视图中，选择一个或多个 Catalog。
1. 在全域導覽列上，前往 **[!UICONTROL 檔案]** > **[!UICONTROL 刪除]** > **[!UICONTROL 刪除]**.

## 自訂目錄（目錄） {#customizing-the-table-of-contents-toc}

Adobe Dynamic Media Classic會在eCatalog畫面的「訂購頁面」標籤上，提供eCatalog中的預設頁碼。 要自定义页面名称，可以更改构成目录 (TOC) 的页标签。推荐重命名封面和封底。例如，封面可以閱讀「封面」而非「第0-1頁」。

可以采用手动方式或通过从 CSV（仅 Mac）或 XML 文件导入页面名称来为 eCatalog 创建自定义目录 (TOC)。

>[!NOTE]
>
>若要還原預設頁面標題，請在 **[!UICONTROL 排序頁面]** 索引標籤，選取 **[!UICONTROL TOC標籤]**，然後選取 **[!UICONTROL 還原預設值（全部）]**.

### 手动输入页面名称 {#manually-entering-page-names}

要逐个手动输入页面名称，转至 eCatalog 屏幕的“排序页面”选项卡。然後，在頁碼欄位中，為每一個要命名的頁面輸入名稱。

### 匯入頁面名稱 {#importing-page-names}

如果处理包含很多页面的 eCatalog，则推荐使用导入页面名称的方法。可以从制表符分隔的文件或 XML 文件导入名称。

TOC標籤儲存在影像的「使用者資料」欄位中；將此資料格式化為 `name=<value>` ` pairs separated by two question marks “??” `. 例如，要为名为 `tocEN` 的 TOC 字段设置一个标签，可以将图像的“用户数据”设置为：

`tocEN=&lt;EN_page_label>`

若要為命名的TOC欄位設定個別標籤 `tocEN` 和 `tocFR`：

`tocEN=&lt;EN_page_label>??tocFR=&lt;FR_page_label>`

若要匯入Tab字元分隔檔案中的「使用者資料」欄位，請包含該欄位使用者資料：

| IPSID | 使用者資料 |
| --- | --- |
| `<image_IPS_ID>` | `tocEN=<EN_page_label>??tocFR=<FR_page_label>` |

要用 XML 文件导入“用户数据”字段，应包含 `vc_userdata` 属性：

```as3
<ips> 
<ghw_object vc_objectname="<image_IPS_ID>" … vc_userdata=" tocEN=<EN_page_label>??tocFR=<FR_page_label>" … /> 
</ips>
```

若要從定位字元分隔或XML檔案匯入頁面名稱，請選取 **[!UICONTROL TOC標籤]** 按鈕並選取 **[!UICONTROL 匯入]**. 在「上傳中繼資料」對話方塊中，選取 **[!UICONTROL 瀏覽]**，然後匯入CSV檔案(僅限Mac)或將每個頁面與頁面名稱建立關聯的XML檔案。
