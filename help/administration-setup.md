---
title: 管理設定
description: 瞭解如何設定Adobe Dynamic Media Classic的管理區域。
uuid: 16ba9fed-b5c6-4991-83b3-8d7d7129013a
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 3c9ee4ec-dd37-498d-98d6-1339b80177ff
feature: Dynamic Media Classic
role: Admin
exl-id: 14e3d8be-f265-4cec-aa8e-19ef71526b68
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '1969'
ht-degree: 33%

---

<!-- UPDATE TOPIC AFTER DECEMBER 31, 2020!!!! -->

# 管理设置{#administration-setup}

「管理設定」畫面可用來管理Adobe Dynamic Media Classic使用者。 使用這些畫面可讓使用者在Adobe Dynamic Media Classic中工作，並透過電子郵件與使用者通訊。

1. 若要存取管理設定選項，請前往 **設定** > **個人設定** > **管理設定**.

## 用户管理 {#user-administration}

所有Adobe Dynamic Media Classic使用者都會獲得一個角色，該角色會決定他們對Adobe Dynamic Media Classic中功能的許可權和存取許可權。 管理员会为自己负责的公司确定不同角色和职责。

通常Adobe Dynamic Media Classic會設定第一組公司並指派公司管理員。 然後，公司管理員會設定和管理Adobe Dynamic Media Classic使用者。

Adobe Dynamic Media Classic支援多個使用者角色。 這些角色可以存取為Adobe Dynamic Media Classic設定的公司：

<!-- **Adobe Dynamic Media Classic Administrator** Can view and administer all features in Adobe Dynamic Media Classic, as well as set up companies and add administrators and users. -->

**Adobe Dynamic Media Classic使用者** 可以存取已指派給他們的公司；無法執行任何管理職責。

**Adobe Dynamic Media Classic公司管理員** 只能檢視和管理自己的公司。 公司管理员还可以执行所有管理功能，包括添加管理员和用户。公司管理員可將使用者新增至DMC公司管理員帳戶。 （该角色是默认用户角色。）

新增使用者後，Adobe Dynamic Media Classic會傳送一封歡迎電子郵件給使用者。 此訊息包含密碼和Adobe Dynamic Media Classic URL。

### 新增使用者或管理員 {#adding-a-user-or-administrator}

1. 前往 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 管理設定]** > **[!UICONTROL 使用者管理]**.
1. 選取 **[!UICONTROL 新增]**.
1. 輸入您要新增的使用者或管理員的名稱和電子郵件地址，然後選取 **[!UICONTROL 下一個]**.

   >[!NOTE]
   >
   >單引號字元(`‘`)不允許出現在電子郵件地址中。

1. 若要將角色指派給使用者，請選擇角色選項。

   另請參閱 [Adobe Dynamic Media Classic使用者角色和許可權](administration-setup.md#user_administration).

1. 若要將使用者新增至公司，請選取公司名稱。
1. 如果您想要將使用者新增至群組（如果您新增Media Portal使用者或貢獻者），請選取「 」 **[!UICONTROL 下一個]** 並新增使用者。
1. 選取 **[!UICONTROL 儲存]** 以完成使用者設定。

   保存之后，系统将提示您是否要将用户添加到其他公司。選取 **[!UICONTROL 新增]** 如果您想要將使用者新增至公司。

   所有新使用者都會獲得隨機產生的密碼；使用者在第一次登入Adobe Dynamic Media Classic案頭應用程式時需要變更密碼。

   在您添加新用户后，会向他们发送欢迎电子邮件。此電子郵件會提供暫時密碼，並說明如何登入Adobe Dynamic Media Classic。

   如果使用者沒有收到歡迎電子郵件，請讓他們前往Adobe Dynamic Media Classic登入頁面(https://s7sps1.scene7.com)，然後選取 **[!UICONTROL 忘記我的密碼]**. 将重置密码并发送新的电子邮件。如果用户未收到电子邮件，并且该电子邮件不在“垃圾邮件”文件夹中，请联系技术支持人员。

   新增Media Portal使用者時，您也可以前往 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 使用者管理]**，然後選取 **[!UICONTROL 上傳使用者清單]** 並選取包含不多於500名使用者的.csv檔案。

### 删除用户 {#deleting-a-user}

您可以讓使用者無效以從Adobe Dynamic Media Classic中刪除使用者。 无效用户会从系统和所有帐户中被删除。

1. 前往 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 管理設定]** > **[!UICONTROL 使用者管理]**.
1. 從清單中選取使用者，然後選取 **[!UICONTROL 編輯]**.
1. 取消选择“有效”。
1. 選取 **[!UICONTROL 儲存]**.

### 啟用或停用使用者 {#activating-or-deactivating-users}

已被停用的用户不再具有进入在“选择要访问的帐户”菜单的顶部列出的帐户的权限。

1. 前往 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 管理設定]** > **[!UICONTROL 使用者管理]**.
1. 在使用者清單中，選取或取消選取 **[!UICONTROL 作用中]** 使用者名稱旁的選項。

### 编辑用户信息 {#editing-user-information}

您可以编辑的用户信息取决于您的管理员角色以及要编辑其信息的用户被指定的角色。变暗（不可用）的选项不可编辑。

1. 前往 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 管理設定]** > **[!UICONTROL 使用者管理]**.
1. 從清單中選取使用者，然後選取 **[!UICONTROL 編輯]**.
1. 在表格中選取專案，以顯示您嘗試修改許可權或存取權的公司，然後選取 **[!UICONTROL 管理公司]**.
1. 选择用户角色。
1. 如果您想要變更使用者的群組成員資格（如果您正在編輯或新增Media Portal使用者或貢獻者），請選取「 」 **[!UICONTROL 下一個]** 並編輯群組成員資格。
1. 選取 **[!UICONTROL 儲存]**.

### 对用户列表进行过滤和排序 {#filtering-and-sorting-the-user-list}

您可以通过过滤和排序用户列表来找到用户。无论在“选择要访问的帐户”菜单中选择哪个帐户，您管理的所有帐户中的所有用户都会显示在“用户”列表中。

您可以使用下列使用者清單篩選技術：

* **依群組篩選**  — 選取 **[!UICONTROL 依群組]** 選單並選擇選項以將清單縮小至群組中的使用者。

* **依使用者角色篩選**  — 選取 **[!UICONTROL 依使用者角色]** 選單並選擇選項以將清單縮小至不同型別的使用者或管理員。

* **依欄位名稱篩選**  — 選取 **[!UICONTROL 啟用依欄位篩選]**. 然後選取 **[!UICONTROL 依欄位名稱]** 選單，選擇欄以篩選清單，然後選取「篩選字元」選單並選擇字母。 清單會依您選取的字母在其中一個欄上篩選。 若要檢視完整清單，請取消選取 **[!UICONTROL 啟用依欄位篩選]** 選項。

* **篩選出無效的使用者**  — 取消選取 **[!UICONTROL 包含無效]**. 搜索结果只显示系统中的用户。已從您管理的系統和帳戶中刪除無效的使用者。

* **依欄標題排序**  — 選取標題以依狀態依字母順序、名字、姓氏或電子郵件、使用者角色或有效/無效狀態來排序所有使用者。

如果您有许多用户，可以通过选择“最大列表大小”菜单并选择一个数值来限制列表的大小。

<!-- CQDOC-16690 TOPIC REMOVED AS PER JIRA TICKET INSTRUCTIONS ### Linking an IMS user identity to an Adobe Dynamic Media Classic IPS user account {#linking-an-ims-user-identity-to-a-scene-ips-user-account}

You can link an Adobe IMS user identity to an Adobe Dynamic Media Classic IPS user account so you can use SSO (Single Sign On) to log on and launch Scene7 Publishing System from within Adobe Marketing Cloud.

1. Adobe should already have setup your account with an Adobe Marketing Cloud organization and linked it to your Scene7 Publishing System product context. If this setup is not yet done or you are unsure if it has been done, contact Adobe Customer Care.

   When the setup is complete, you can can log on to Adobe Marketing Cloud and link your Adobe Marketing Cloud identity to your Adobe Dynamic Media Classic user account by doing the following.

1. In Adobe Marketing Cloud, navigate to your account settings.
1. Select **Manage Organizations**.
1. Select **Link Account** or **Get Access**.
1. Select **Experience Manager**, and then type your credentials.

   Your credentials include your IPS company region, email address, and password.

1. Select **Link**.
1. When the link is set, you can launch Scene7 Publishing System from within Adobe Marketing Cloud, or you can launch it directly.

   Do one of the following:

    * To launch Adobe Dynamic Media Classic from within Adobe Marketing Cloud, in the left rail of Adobe Marketing Cloud, select **Solutions** > **Experience Manager**. Under the Adobe Dynamic Media Classic card, select **Launch**.
    * To log on to Scene7 Publishing System directly using your IMS credentials, use the following website:

      https://s7spsN.scene7.com/IpsWeb?ims=1

      Replace “N” in the above path with the number for your IPS company region. That is, N = 1 for North America; 3 for EMEA; or 5 for JAPAC.
 -->

## 頻寬與儲存空間 {#bandwidth-storage}

Adobe Dynamic Media Classic管理員可以為他們管理的公司產生頻寬、儲存空間和其他型別的報表。 這些報告可在頻寬與儲存頁面取得。

若要開啟此頁面，請前往 **[!UICONTROL 設定]** > **[!UICONTROL 個人設定]**. 展開 **[!UICONTROL 管理設定]**，然後選取 **[!UICONTROL 頻寬與儲存]**.

### 报告类型 {#types-of-reports}

下表說明可從「頻寬與儲存」頁面產生的報表：

| 报告 | 信息 | 用途 |
|:--- |:--- |:--- |
| 带宽 | 公司的带宽使用情况 | 跟踪公司在特定日期范围内的带宽使用量，以确定流量模式。 |
| 存储 | 存储使用情况 | 跟踪公司上载的数据量。 |
| 图像内容 | 按类型划分的图像请求数目 | 跟踪不同图像类型的请求数量和容量。 |
| 域 | 按域划分的 URL 请求数目 | 根据特定公司的图像请求的域，跟踪图像使用情况。(Adobe Dynamic Media Classic可為每個帳戶提供一個以上的網域。 有关更多信息，请联系技术支持。） |
| 视频流 | 流视频的带宽使用情况 | 跟踪公司在特定日期范围内的流视频使用情况，以确定流量模式。 |
| 视频内容 | 不同视频的播放时间 | 确定哪些是最常观看和最少观看的视频。 |

“图像内容”报告提供了对以下图像类型所发出的请求的信息：

* **影像要求**  — 影像要求。

* **縮圖要求**  — 在檢視器中要求色票或替代影像。

* **遮罩要求**  — 要求影像傳回灰階遮色片。

* **檢視器圖磚請求**  — 檢視器載入的影像要求。

* **Vnt物件要求**  — 影像演算要求，傳回要求暈映中具有指定物件的影像。

* **Vnt資訊要求**  — 傳回請求暈映相關資訊的影像演算請求。

>[!NOTE]
>
>“视频流”报告仅应用于流视频。它不跟踪对渐进式视频的观看情况。

### 產生報表 {#generating-a-report}

生成带宽、存储、图像内容、域、视频流或视频内容报告：

1. 前往 **[!UICONTROL 設定]** > **[!UICONTROL 個人設定]**.
1. 展開「管理設定」，然後選取 **[!UICONTROL 頻寬與儲存]**.
1. 選取索引標籤： **[!UICONTROL 頻寬]**， **[!UICONTROL 儲存]**， **[!UICONTROL 影像內容]**， **[!UICONTROL 網域]**， **[!UICONTROL 視訊串流]**，或 **[!UICONTROL 視訊內容]**.

   请参阅[报告类型](administration-setup.md#types_of_reports)。

### 以不同方式檢視資料 {#viewing-data-in-different-ways}

在“带宽与存储”页面上生成报告后，您可以选择用于查看信息的选项。您可以选择如何显示信息，如何在图表或数据网格中查看信息，以及指定用于捕获信息的时间段。在“数据”视图中，您还可以排序信息并重新排列各个列。

* **在圖表或資料網格中檢視資料**  — 選取 **[!UICONTROL 圖表檢視]** 若要在圖表中檢視資料；請選取「 」 **[!UICONTROL 資料檢視]** 以檢視資料網格中的資料。

* **選擇報表簡報型別**  — 在「報表型別」功能表上，選取 **[!UICONTROL 摘要]**， **[!UICONTROL 每日]**，或 **[!UICONTROL 每月]** 以摘要形式、按日期或按月組織資料。 并非所有报告都提供该选项。

* **指定時段**  — 選擇選項以定義報表的時間期間，然後選取 **[!UICONTROL 更新]** 定義時段後：

* **預先定義的時間段**  — 在「預先定義報表」功能表中選擇選項。 例如，选择“上月”以捕获上月的数据。

* **自訂時段**  — 在預先定義報表功能表中，選取 **[!UICONTROL 自訂]**. 然後選擇日期 **[!UICONTROL 開始月份]** (或 **[!UICONTROL 開始日期]**)功能表，以及「月數」 （或「天數」）功能表上的日期。 对于域报告和视频内容报告，您可以为捕获报告信息选择特定的开始和结束日期。

* **排序資料（僅限資料檢視）**  — 若要排序欄上的資訊，請選取欄的標題。 再次選取「 」可依遞減順序排序。

* **重新排列欄（僅限資料檢視）**  — 若要將欄移動到資料網格上的不同位置，請拖曳其標題。

### 匯出和列印報告 {#exporting-and-printing-reports}

在生成报告后，您可以导出其数据，在电子表格和其他应用程序中使用。您还可以打印报告。

* **匯出報表資料**  — 在資料檢視中，視需要排序和排列資料。 然後開啟 **[!UICONTROL 匯出]** 功能表並選擇格式： **[!UICONTROL 定位字元分隔]**， **[!UICONTROL 逗號分隔]**，或 **[!UICONTROL HTML已格式化]**. 資料會以您選擇的格式複製到剪貼簿。 现在，您可以将数据粘贴到电子表格或应用程序中。

* **列印報表**  — 選取 **[!UICONTROL 列印]**，在「列印」對話方塊中選擇所需的選項，然後選取 **[!UICONTROL 確定]**.

## 图像错误 {#image-errors}

Adobe Dynamic Media Classic管理員可以產生影像錯誤報告。 “图像错误”报告针对您当前登录的公司，提供了过去 24 小时内 20 个最常见的图像错误。若要產生「影像錯誤」報表，請執行下列動作：

1. 前往 **[!UICONTROL 設定]** > **[!UICONTROL 個人設定]**.
1. 展開「管理設定」，然後選取 **[!UICONTROL 影像錯誤]**.
1. （可选）请执行下列操作之一：

   * 若要依標題資訊排序錯誤，請選取標題。 默认情况下，按发生次数，从最高到最低排序错误。
   * 将光标移动到错误的“响应”字段上，可查看具体的错误消息。
   * 若要檢視影像或反向連結網頁的連結，請將游標移至URL欄位或反向連結欄位上方。
   * 若要複製實際影像的連結，請選取 **[!UICONTROL URL複製URL]**. 您可以在浏览器窗口中粘贴此链接，以转到该图像并检查错误。
   * 若要複製反向連結網頁的連結，請選取 **[!UICONTROL 反向連結複製URL]**.

顯示的錯誤適用於您目前登入的公司。 每个错误都包括以下信息：

* **影像識別碼**  — 違規影像的ID。

* **時間**  — 首次回報錯誤到上次回報錯誤的時間範圍（在過去24小時內）。

* **計數**  — 影像上報告的錯誤數。

* **回應**  — 特定錯誤訊息。 错误是 4xx 或者 5xx。

* **URL**  — 列出Adobe Dynamic Media Classic上影像的URL。

* **反向連結**  — 指定初始請求來自的網站URL。 引用网站可以是具有指向图像的链接的任何网站。

“URL”和“引用网站”列都有与之相关的“复制 URL”以简化测试。
