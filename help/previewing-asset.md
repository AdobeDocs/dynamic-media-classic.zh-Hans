---
title: 預覽資產
description: 瞭解如何在Adobe Dynamic Media Classic中預覽資產。
uuid: 4a01be21-e37f-4d79-9220-f4e177e9179a
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: 17d0bfd6-fc62-4ed6-8a51-7ac1a6bb96cc
feature: Dynamic Media Classic,Asset Management,Viewers
role: User
exl-id: 7e6f652c-b197-4171-b11b-f532795f7cf2
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '1012'
ht-degree: 36%

---

# 預覽資產{#previewing-an-asset}

您可以使用預覽來檢視客戶檢視時數位資產的顯示方式。 “预览”使用分配给资源的默认查看器。默认查看器在“应用程序设置”中进行配置。

另請參閱 [設定預設檢視器](application-setup.md#configuring_default_viewers).

如果您使用引數圖層預覽範本資產，可以變更引數或影像預設集。 因为您所做的更改是嵌入式的，所以可以立即从相同的“预览”窗口查看结果。

另請參閱 [Adobe檢視器參考資料庫範例](https://landing.adobe.com/en/na/dynamic-media/ctir-2755/live-demos.html).

**预览资源:**

1. 在左侧“资源库”面板中，导航到包含要预览的资源的“资源”文件夹。
1. 执行以下任一操作：

   * 在「資產」視窗上方、工具列右側，選取「 」 **[!UICONTROL 格點檢視]**.
   * 在「資產」視窗上方、工具列右側，選取「 」 **[!UICONTROL 清單檢視]**.
   * 在「資產」視窗上方、工具列右側，選取「 」 **[!UICONTROL 詳細資料檢視]**.

1. 根據您使用的檢視，執行下列任一項作業：

   * 在「網格檢視」或「清單檢視」的「資產」視窗中，選取單一資產，然後選取 **[!UICONTROL 預覽]** 在縮圖影像附近。
   * 在「網格檢視」、「清單檢視」或「詳細資料檢視」的「資產」視窗上方的工具列上，選取 **[!UICONTROL 預覽]**.

## 根據檢視器平台型別預覽資產 {#previewing-an-asset-based-on-viewer-platform-type}

可以使用“查看器列表”预览资源在特定查看器平台类型（如 HTML5）上的显示情况。并不是所有平台都可在查看器列表中找到，这取决于您选择要预览的资源类型和关联的查看器。

您也可以使用查看器列表来复制查看器的 URL 或者查看和复制查看器代码以嵌入到网页中。

對於指定的檢視器平台，「檢視器清單」視窗可讓您檢視哪些裝置（例如平板電腦和智慧型手機）可供檢視器使用。

**基于查看器平台类型预览资源:**

1. 在左侧“资源库”面板中，导航到包含要预览的资源的“资源”文件夹。
1. 执行以下任一操作：

   * 在「資產」視窗上方、工具列右側，選取「 」 **[!UICONTROL 格點檢視]**. 在「資產」視窗中，選取單一資產，然後前往縮圖影像下方 **[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**.
   * 在「資產」視窗上方、工具列右側，選取「 」 **[!UICONTROL 清單檢視]**. 在「資產」視窗中，選取單一資產，然後在縮圖影像右側，前往 **[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**.
   * 在「資產」視窗上方、工具列右側，選取「 」 **[!UICONTROL 詳細資料檢視]**. 在相同工具列上，前往 **[!UICONTROL 預覽]** > **[!UICONTROL 檢視器清單]**.

1. （選擇性）在「檢視器清單」視窗中，選取欄標題 **[!UICONTROL 名稱]** 或 **[!UICONTROL 平台型別]** 以遞增或遞減順序來排序欄。
1. 在「檢視器清單」視窗中，在表格的「動作」欄下選取 **[!UICONTROL 預覽]** 檢視所選檢視器和平台型別中資產的顯示方式。

   關閉顯示的預覽。

1. （可选）在“查看器列表”窗口底部的“用于生成副本 URL 的 URL 编码”下拉列表中，选择要在复制资源的 URL 时应用的 URL 编码。
1. （可选）请执行下列操作之一：

   * 在「檢視器清單」視窗中，在表格的「動作」欄下選取 **[!UICONTROL 複製URL]** 適用於選取的檢視器和平台型別。

      當您選取 **[!UICONTROL 複製URL]**，其相關URL會自動複製到剪貼簿。

   * 在「檢視器清單」視窗中，在表格的「動作」欄下選取 **[!UICONTROL 內嵌程式碼]**.

      當您選取 **[!UICONTROL 內嵌程式碼]**，內嵌程式碼視窗隨即開啟，供您檢閱檢視器程式碼。 不允许在该窗口中编辑代码。您也可以将代码复制到剪贴板中，以便可以将其粘贴到网页中。

      關閉顯示的預覽。

1. 在「檢視器清單」視窗的右下角，選取 **[!UICONTROL 關閉]** 以返回「資產」畫面。

## 根據影像預設集預覽影像資產 {#previewing-an-image-asset-based-on-its-image-preset}

您可以基于图像预设来预览图像资源，从而查看在图像以不同大小动态地传送到网站或应用程序时的显示情况。

图像预设是一组预定义的设置，用于更改图像在导出时的外观大小、图像质量、格式、分辨率以及其他方面。

另請參閱 [設定影像預設集](setting-image-presets.md#setting_up_image_presets).

另請參閱 [建立和啟用影像預設集](creating-enabling-image-presets.md#creating_and_enabling_image_presets).

**基于图像预设预览图像资源:**

1. 在左侧“资源库”面板中，导航到包含要预览的图像资源的“资源”文件夹。
1. 执行以下任一操作：

   * 在「資產」視窗上方、工具列右側，選取「 」 **[!UICONTROL 格點檢視]**. 在「資產」視窗中，選取單一影像資產，然後前往縮圖影像下方 **[!UICONTROL 預覽]** > **[!UICONTROL 影像預設集清單]**.
   * 在「資產」視窗上方、工具列右側，選取「 」 **[!UICONTROL 清單檢視]**. 在「資產」視窗中，選取單一影像資產，然後在縮圖影像的右側，前往 **[!UICONTROL 預覽]** > **[!UICONTROL 影像預設集清單]**.
   * 在「資產」視窗上方、工具列右側，選取「 」 **[!UICONTROL 詳細資料檢視]**. 在相同工具列上，前往 **[!UICONTROL 預覽]** > **[!UICONTROL 影像預設集清單]**.

1. 在“图像预设列表”窗口的表中，选择您要嵌入右侧窗格预览其图像资源的预设类型名称。
1. （選擇性）在「影像預設集清單」視窗的 **[!UICONTROL 用於產生復本URL的URL編碼]** 從底部的下拉式清單中，選取複製影像資產時，要套用至其URL的URL編碼。
1. （可選）在「影像預設集清單」視窗中，在預覽窗格的右上角區域選取 **[!UICONTROL 複製URL]** 選取的預設集型別。

   當您選取 **[!UICONTROL 複製URL]**，其相關URL會自動複製到剪貼簿。

1. 在「影像預設集清單」視窗的右下角，選取 **[!UICONTROL 關閉]** 以返回「資產」畫面。
