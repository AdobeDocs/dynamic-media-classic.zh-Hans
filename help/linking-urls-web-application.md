---
title: 將URL連結至您的網頁應用程式
description: 瞭解如何從Adobe Dynamic Media Classic將URL連結至您的網路應用程式。
uuid: 1179bdd3-9b39-47f9-945d-1c1ca186bf96
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
discoiquuid: 71299640-676d-49b7-841d-6118f31044e8
feature: Dynamic Media Classic
role: User
exl-id: ca629427-da33-4bab-9d08-6d9368042f7e
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '843'
ht-degree: 37%

---

# 將URL連結至您的網頁應用程式{#linking-urls-to-your-web-application}

您的網站和應用程式可透過URL字串存取Dynamic Media影像伺服器內容。 發佈影像後，Adobe Dynamic Media Classic會啟用參照Dynamic Media影像伺服器上影像預設集的URL字串。 可将这些 URL 粘贴至 Web 浏览器进行测试。

若要將這些URL字串放入您的網頁和應用程式中，請從Adobe Dynamic Media Classic複製它們。 若要取得影像預設集產生的URL字串，請前往「預覽」畫面或「瀏覽」面板（在「詳細資料檢視」中）。

## 取得影像預設集URL {#obtaining-an-image-preset-url}

可从“预览”或详细信息视图中获得由图像预设生成的 URL 字符串。复制 URL 后，该字符串将放置在剪贴板上，以便在必要时进行粘贴。

>[!NOTE]
>
>在发布资源之前，URL 处于非激活状态。

### 從預覽取得影像預設集URL {#obtaining-an-image-preset-url-from-preview}

1. 在左侧“资源库”面板中，导航到包含要预览的图像资源的“资源”文件夹。
1. 执行以下任一操作：

   * 在「資產」視窗上方、工具列右側，選取「 」 **[!UICONTROL 格點檢視]**. 在「資產」視窗中，選取單一影像資產，然後前往縮圖影像下方 **[!UICONTROL 預覽]** > **[!UICONTROL 影像預設集清單]**.
   * 在「資產」視窗上方、工具列右側，選取「 」 **[!UICONTROL 清單檢視]**. 在「資產」視窗中，選取單一影像資產，然後在縮圖影像的右側，前往 **[!UICONTROL 預覽]** > **[!UICONTROL 影像預設集清單]**.
   * 在「資產」視窗上方、工具列右側，選取「 」 **[!UICONTROL 詳細資料檢視]**. 在相同工具列上，前往 **[!UICONTROL 預覽]** > **[!UICONTROL 影像預設集清單]**.

1. （可選）在「影像預設集」清單的「產生複製URL的URL編碼」下拉式清單中，選取您要在複製影像資產的URL時套用的URL編碼。
1. 在「影像預設集清單」視窗中，在預覽窗格的右上角區域選取 **[!UICONTROL 複製URL]** 選取的預設集型別。
1. 在「影像預設集清單」視窗的右下角，選取 **[!UICONTROL 關閉]** 以返回「資產」畫面。

### 從瀏覽面板取得影像預設集URL {#obtaining-an-image-preset-url-from-the-browse-panel}

1. 在左侧“资源库”面板中，导航到包含要预览的图像资源的“资源”文件夹。
1. 在「資產」視窗上方、工具列右側，選取「 」 **[!UICONTROL 格點檢視]**. 在“资源”窗口中，选择单个图像资源。
1. 在「資產」視窗上方、工具列右側，選取「 」 **[!UICONTROL 詳細資料檢視]**.
1. 選取 **[!UICONTROL URL]** 位於畫面右側的面板上，方便您展開影像預設集清單。
1. 選取 **[!UICONTROL 複製URL]** 影像預設集名稱旁的連結，以及您要複製到剪貼簿的URL。

## 关于图像预设 URL 字符串 {#about-image-preset-url-strings}

Dynamic Media影像伺服器的影像大小調整URL呼叫有以下基本語法：

*路径*/*图像服务器名称*/*帐户名称*/*图像名称*?*修饰符1*&amp;*修饰符2*&amp;...

在Dynamic Media影像伺服器URL中，伺服器的影像顯示指示會出現在問號(？)之後。 例如，以下 URL 调用将传送一个名为“backpack”宽度为 250 个像素的图像：

```as3
https://s7d1.scene7.com/is/image/S7learn/backpack?wid=250
```

图像预设 URL 包含按相应大小和格式规范显示图像的所有修饰符指令。对于没有图像预设的情况，请注意此 URL 字符串中问号 (?) 之后的所有修饰符指令：

```as3
https://s7d1.scene7.com/is/image/S7learn/backpack?wid=250&fmt=jpeg&qlt=80,0&resMode=sharp&op_usm=1.1,0.5,1,0
```

然而，在图像预设生成的 URL 字符串中，图像预设的名称将代替图像预设定义的指令。例如，对于上面的长 URL，此 URL 字符串为：

```as3
https://s7d1.scene7.com/is/image/S7learn/backpack?$Large$
```

在 URL 中图像预设名称用美元符号 ($) 括起。當Dynamic Media影像伺服器遇到URL的影像預設集部分時( `Large` 在此情況下)，使用「大」影像預設集定義的大小和格式設定指示。

## 將動態影像新增至網頁 {#adding-dynamic-images-to-your-web-page}

若要將動態影像新增至網頁，請 `<IMG>` HTML網頁程式碼中的標籤通常會使用Adobe Dynamic Media Classic URL字串進行修改，以向Dynamic Media影像伺服器提出要求。 该字符串会按图像预设定义的大小和格式规范生成图像。

例如，与以下用于打开静态图像的典型调用不同

```as3
img src="/company_images/products/backpack_thumbnail.jpg"
```

您現在使用 `<IMG>`標籤上的標籤，以使用對Adobe Dynamic Media Classic平台的影像預設集呼叫來取代靜態影像的參考。 示例调用如下所示：

```as3
img src="https://s7d2.scene7.com/is/image/S7learn/backpack_trns?$thumbnail$”
```

在此範例中，Dynamic Media影像伺服器「查詢」定義 `$thumbnail$` 並透過以下專案所定義的大小與格式規格，動態產生適當的影像： `thumbnail`影像預設集。 在 URL 字符串中，除产品图像文件名称（本例中为`backpack_trns` ）之外的所有项目都由网页模版所固定。唯一可从商业服务器自动插入到网页模版的元素是 IPS ID 或图像名称。
