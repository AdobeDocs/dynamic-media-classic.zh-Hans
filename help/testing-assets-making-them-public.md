---
title: 在公開資產之前先測試資產
description: 瞭解如何先在Adobe Dynamic Media Classic中測試資產，然後再將資產公開。
uuid: 5e8f3bec-6cf1-408e-8ea1-aebde0012a70
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/upload_and_publish_assets
discoiquuid: 52fadf99-7d11-46f7-8483-a9f87ffc2f67
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: fd78d535-391e-43eb-a8aa-25fa6c2885cb
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '1066'
ht-degree: 31%

---

# 在公開資產之前先測試資產 {#testing-assets-before-making-them-public}

Secure Testing可協助您定義安全的測試環境，並根據一組可設定的IP位址和範圍來建立強大的B2B解決方案。 此功能可讓您將Adobe Dynamic Media Classic部署與內容管理和業務系統的架構配對。

通过安全测试，可以预览包含未发布内容的临时版网站。

如有需要，請建立中繼環境，而非讓資產公開可用，理由如下：

* 在公开发布之前预览网站（临时网站）。
* 提供要求限制访问的资源，如在 B2B Web 应用程序中显示价格的 eCatalog。
* 将防火墙后的资源用作产品信息管理系统、客户服务应用程序、培训站点等的一部分。

>[!NOTE]
>
>安全測試不會影響對Adobe Dynamic Media Classic的存取。 Adobe Dynamic Media Classic安全性會維持一致，且需要一般憑證才能存取Adobe Dynamic Media Classic及相關網路服務。

## 安全测试的工作原理 {#how-secure-testing-works}

大多数公司在防火墙后运行 Internet。可以通过某些路由，通常是通过限定范围的公共 IP 地址访问 Internet。

透過公司網路，您可以使用以下網站找出您的公用IP位址： [https://www.whatismyip.com](https://www.whatismyip.com/) 或向您的企業IT組織索取此資訊。

透過安全測試，Adobe Dynamic Media Classic建立了專用的影像伺服器，用於中繼環境或內部應用程式。 对此服务器的所有请求都将检查原始 IP 地址。如果传入请求不在获批准的 IP 地址列表中，则返回失败响应。Adobe Dynamic Media Classic公司管理員會為公司的安全測試環境設定經過核准的IP位址清單。

由於原始請求的位置必須確認，因此Secure Testing服務的流量不會透過內容發佈網路(例如公用Dynamic Media Image Server流量)進行路由。 向安全測試服務提出的請求與公開Dynamic Media影像伺服器的延遲相比，稍微高一些。

通过安全测试服务，可以立即使用未发布的资源，无需发布。透過這種方式，您可以在資產發佈到公開顯示的影像伺服器之前執行預覽。

>[!NOTE]
>
>Secure Testing服務會使用已設定內部發佈內容的目錄伺服器。 因此，如果您的公司設定為發佈至Secure Testing，Adobe Dynamic Media Classic中任何上傳的資產都可立即透過Secure Testing服務使用。 不論資產是否標示為上傳時發佈，此功能皆為true。

Secure Testing服務目前支援下列資產型別和功能：

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>Added videos to list below 9/11/2012. Moved “Render Server requests” from unsupported to supported, listed below on 3/15/2016 as per email from Cynthia March 11, 2016)</p>

 -->

* 图像.
* 晕影（渲染服务器请求）。
* 轉譯器伺服器請求（受支援，但必須由客戶明確請求）。
* 集，包括图像集、eCatalog、渲染集和媒体集。
* 標準Adobe Dynamic Media Classic多媒體檢視器。
* Adobe Dynamic Media Classic OnDemand JSP頁面。
* 静态内容，如 PDF 文件和逐步提供的视频。
* HTTP 视频流。
* 渐进式视频流。

当前不支持以下资源类型和功能：

* Adobe Dynamic Media Classic資訊或eCatalog搜尋
* RTMP 视频流
* Web-to-print
* UGC （使用者產生的內容）服務

>[!IMPORTANT]
>
>Adobe Dynamic Media Classic已於2021年9月30日停止支援新的或現有的UGC向量影像資產。

## 測試Secure Testing service {#testing-the-secure-testing-service}

測試Secure Testing服務，確保該服務可如預期般運作。

<!-- >[!NOTE]
>
>*If you do not mention any IPs under **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Publish Setup]** > **[!UICONTROL Image Server]** > **[!UICONTROL Test Image Service]*** - If you add an IP only, that IP is able to call the assets and no other IP are allowed to make the calls. As long there is no IP mentioned under that section, all IPs are allowed to make the calls for the assets, and they show up. -->

### 准备帐户

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>RB: Rewrote entire steps under “Prepare your account” 9/10/2012</p>

 -->

1. 請聯絡Adobe客戶服務，要求他們在您的帳戶上啟用安全測試。
1. 在Adobe Dynamic Media Classic中的全域導覽列上，前往 **[!UICONTROL 設定]** > **[!UICONTROL 發佈設定]** > **[!UICONTROL 影像伺服器]**.
1. 在「影像伺服器發佈」頁面的 **[!UICONTROL 發佈內容]** 下拉式清單，選取 **[!UICONTROL 測試影像伺服]**.
1. 對於使用者端位址篩選器，請選取 **[!UICONTROL 新增]**.
1. 選取核取方塊以啟用位址（開啟），然後在各自的文字欄位中輸入IP位址和網路遮罩。

   >[!NOTE]
   >
   >如果您新增單一IP位址和網路遮罩，該位址可能會進行資產呼叫。 不過，您新增的任何其他IP位址和網路遮罩都不得進行資產呼叫。 因此，請考慮停用（關閉）上述步驟中的核取方塊，以關閉指定IP位址和網路遮罩的功能。 這麼做實際上允許 *全部* 進行資產呼叫的IP位址，這些位址都會顯示。

1. 执行以下任一操作：
   * 如果您必須新增更多IP位址，請重複前兩個步驟。
   * 繼續下一步驟。
1. 在「影像伺服器發佈」頁面的左下方，選取「 」 **[!UICONTROL 儲存]**
1. 將所需的影像上傳至您的Adobe Dynamic Media Classic帳戶。

   另請參閱 [上傳檔案](uploading-files.md#uploading_files).

1. 请确保部分图像已标记为发布，而其它图像未标记，然后提交发布作业。

   另請參閱 [發佈檔案](publishing-files.md#publishing_files).

1. 請前往「 」，判斷Secure Testing服務的名稱 **[!UICONTROL 設定]** > **[!UICONTROL 應用程式設定]** > **[!UICONTROL 一般設定]**.
1. 在“应用程序常规设置”页面上，在“服务器”组下，在“**[!UICONTROL 测试发布上下文服务器名称]**”右侧找到该名称。

如果伺服器名稱遺失或伺服器的URL無法運作，請聯絡Adobe服務。

### 准备网站变体

您需要两个网站变体，分别链接已发布和未发布的资源：

* 公開版本 — 使用舊版Adobe Dynamic Media Classic URL語法連結資產。
* 測試版本 — 使用相同語法但具有安全測試網站名稱的連結資產。

### 运行测试

执行以下测试：

1. 检查是否可从公司网络内部访问资源。

   從先前定義的IP位址範圍所識別的公司網路中，網站的測試版本會顯示所有影像，無論是否標籤為發佈。 因此，您可以在測試時避免在預覽核准或產品上市之前意外提供影像。

   確認您的網站公開版本是否顯示已發佈的資產，如同先前使用Adobe Dynamic Media Classic時的情形。

1. 从公司网络外部，确认未发布的资源（即未标记为发布）受到保护，第三方无法访问。

   从外部（如从家庭计算机或通过 3G 连接）访问您的网络，然后确认站点的公开版本显示有所已发布的资源，但不显示未发布的内容。

   确认临时版本未显示任何资源，因为您正在从未获批准的 IP 地址访问安全测试服务。
