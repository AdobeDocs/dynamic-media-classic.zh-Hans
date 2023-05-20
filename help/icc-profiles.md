---
title: ICC （國際色彩聯盟）設定檔
description: 瞭解Adobe Dynamic Media Classic中的ICC設定檔。
uuid: 708ff2ad-9a47-4e3e-b643-5b19648f726b
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/support_files
discoiquuid: 44f1b4c4-6d7f-4e0f-84ce-11d26745e0f0
feature: Dynamic Media Classic
role: User
exl-id: 989f2761-f5d0-4ece-b2a6-f7b4577aa8a2
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '451'
ht-degree: 54%

---

# ICC 配置文件{#icc-profiles}

ICC （国际色彩联盟）配置文件是描述如何正确地将图像文件从一个颜色空间转换到另一个颜色空间的文件。ICC 配置文件有助于为图像获取正确的颜色。例如，到正确地显示用于在计算机显示器上打印的图像，可以选择 ICC 配置文件。该配置文件将图像转换到不同的颜色空间并确保颜色正确地联机显示。

在Adobe Dynamic Media Classic中，您可以選擇ICC設定檔，在上傳影像時將影像轉換為不同的色域。 Adobe Dynamic Media Classic預設提供所有標準Photoshop ICC設定檔。 要在“上载”屏幕中查看颜色配置文件的名称，请选择“颜色配置文件”菜单。然后选择“自定义从>到”，再从“转换至”和“转换到”菜单中选择 ICC 配置文件的名称。

另請參閱 [上傳時的影像編輯選項](image-editing-options-upload.md#image-editing-options-at-upload).

除了使用預設的ICC設定檔之外，您還可以將其他ICC設定檔上傳到Adobe Dynamic Media Classic，並使其可用於色域轉換。 切換至「瀏覽」面板中的「詳細資料檢視」，以調查ICC設定檔的設定檔類別、色域型別和PCS型別。

## 上傳ICC設定檔 {#uploading-icc-profiles}

通过与上载文件时所使用的技术相同的技术上载 ICC 配置文件。您可以將ICC設定檔儲存在任何Adobe Dynamic Media Classic資料夾中。

另請參閱 [上傳您的檔案](uploading-files.md#uploading_your_files).

## 檢查ICC設定檔 {#examining-an-icc-profile}

若要檢查ICC設定檔，請在「瀏覽」面板中選取該設定檔，並在「詳細資料檢視」中顯示它。 「詳細資料檢視」提供下列有關ICC設定檔的資訊：

* **[!UICONTROL 設定檔類別]** - ICC （國際色彩協會）定義每個類別以涵蓋應用程式型別。 例如，输入配置文件应用于数码相机和扫描仪等设备，输出配置文件应用于打印机。

* **[!UICONTROL 色域型別]**  — 此數字是設定檔的「輸入」色彩空間，如ICC所定義。 颜色空间类型定义颜色空间的组件的数量和对这些组件的解释。例如，RGB 是具有三个组件（红色、绿色和蓝色）的颜色空间。颜色空间类型不定义空间的特定颜色特征（例如，原色的色度）。

* **[!UICONTROL PCS型別]**  — 此PCS型別是設定檔的「輸出」色彩空間 — 其設定檔連線空間。 例如，颜色配置文件可以将 RGB 转换成 PCS，然后转化成 CMYK。

对于有助于标记颜色或图像的输入、显示或输出配置文件，PCS 类型是 XYZ 或 Lab。将该配置文件解释成在 ICC 规范中定义的相应的特定颜色空间。
