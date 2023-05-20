---
title: 创建模板参数
description: 瞭解如何在Adobe Dynamic Media Classic中建立範本引數。
uuid: d17168a8-4776-4761-b022-8258d5997604
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: d263f041-5a0d-4c4f-9266-aeff51a5a7e2
feature: Dynamic Media Classic
role: User
exl-id: 118806ea-c8a7-4aaf-9ae3-739c6b04ea77
source-git-commit: cb55e09a997b9d36002c4ac429603576d52fb8bd
workflow-type: tm+mt
source-wordcount: '846'
ht-degree: 54%

---

# 创建模板参数{#creating-template-parameters}

您可以通过参数尽可能灵活地使用模板；可以通过参数来动态自定义模板图像。您可以确定模板中要包括哪些文本图层和图像图层，以及每个图层中要显示哪些参数。例如，若要吸引客戶注意正在銷售的產品，您可以建立「正在銷售」文字圖層。 日后可以删除“待售”参数来删除该图层，但仍保留模板图像的其余部分。

创建模板参数时，实际上是声明要在 URL 字符串中调用模板的哪些部分。使用参数构造的 URL 会在 URL 字符串中列出相关项目。通过列出的参数，您可以按照模板图像从图像服务器动态构造的方式来创建自定义结果，从而动态更改模板（因为您可以调用 URL 中的部分或全部参数）。

在文本图层参数中，还可以将文本字符串设置为链接到数据库值的动态字段。将文本链接到数据库的功能非常有用（例如在促销活动中）。您可以自定义模板图像，使其显示客户端或客户姓名。您也可以將文字層引數連結至價格資料庫，以在範本影像中顯示專案的價格。

您可以多次引用一个参数。对参数对话框中的每个命令使用组合框，以选择匹配该特定命令的参数。例如，所有大小引數都可用於 `size=` 命令。 可以将参数引用再分配给已存在于组合框中的任何参数，并重命名为组合框中不存在的名称。在後一種情況下，名稱必須是唯一的。 否則，錯誤會指出引數存在。 當您刪除引數參照時，如果引數未在其他任何地方參照，則會從URL中移除。 當您變更文字引數的預設值時，該引數的所有參照都會更新。 您可以在圖層表格、範本演算和URL中看到更新。 當您藉由操控調整大小控點或在屬性面板中輸入值來變更圖層屬性時，引數值會更新，且引數的所有參照都會更新。 例如，如果使用一个参数对两个图层的大小进行了参数化，则在更改其中一个图层大小时，两个图层的大小均会更新。在您预览模板并更改参数时，该参数的所有引用均会更新。

另請參閱 [範本基本需知](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/553_Template%20Basics_converted%20renamed_Dynamic%20Banners-AVS) 訓練影片。

## 將圖層引數化 {#parameterizing-a-layer}

对于模板中的每个图层，请根据以下步骤创建模板参数：

1. 在“图层”列表中，选择要创建参数的图层名称旁边的“参数”按钮 。将打开“参数”屏幕。它会列出图层上每个参数的名称、值及类型。
1. 選取要包含在範本影像中的每個引數名稱旁的「開啟」選項。
1. 選取 **[!UICONTROL 關閉]** 以結束「引數」畫面。

>[!NOTE]
>
>可以在“参数”屏幕中重命名参数。重命名参数使得参数更易于在 URL 字符串中标识，且更易于作为数据库值使用。若要重新命名引數，請選取其 **[!UICONTROL 開啟]** 選項，選取其名稱，然後在「名稱」欄位中輸入新名稱。

若要檢視您為範本建立的引數清單，請選取「範本」畫面上的「引數摘要」按鈕。 将打开“参数摘要”屏幕。它会列出每个图层的名称，如果已为图层创建参数，则还会显示参数名和参数值。

## 建立動態文字引數 {#creating-dynamic-text-parameters}

對於文字圖層，您也可以將文字字串設為連結至資料庫值的動態欄位。 请遵循以下步骤：

1. 在“模板”屏幕上，选择要为其创建动态文本参数的文本图层名称旁边的“参数”按钮 。「引數」頁面隨即開啟。
1. 選取 **[!UICONTROL 開啟]** 文字屬性名稱(textAttr)旁的選項。
1. 選取 **[!UICONTROL 文字]** 索引標籤中。
1. 選取 **[!UICONTROL 新增引數]**. 将显示默认的参数名。选择该名称并覆盖键入新名称，可以替换此名称。当前键入的文本字符串将成为参数的新名称。
1. 選取 **[!UICONTROL 關閉]** 以關閉「引數」頁面。

要使参数名使用数据库值，请将以下字符串附加到模板 URL：

```as3
?$_2(parameter name)=(database value)
```

引數名稱會由資料庫欄位中的名稱或Java™程式碼取代，例如指出目前專案價格或客戶名稱。
