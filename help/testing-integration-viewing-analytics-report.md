---
title: 查看 报告以测试 Adobe Analytics 集成
description: 瞭解如何檢視Adobe Analytics報表，以測試Adobe Dynamic Media Classic中的整合。
uuid: 937375e0-6dea-4baa-a2b0-4f3e461c9ee2
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: 1ddc89ff-d2e9-42eb-a442-aa6b9871c991
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 6186fcf0-99b4-447d-ae94-b4124dcb405b
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '339'
ht-degree: 15%

---

# 查看 报告以测试 Adobe Analytics 集成{#testing-the-integration-by-viewing-an-adobe-analytics-report}

在Adobe Analytics中建立必要的變數、將其連結至Adobe Dynamic Media Classic事件，並完成必要的實作步驟後，您就可以測試設定。 您可以在 Adobe Analytics 中测试和验证是否正在捕获数据。如果设置正常，则无需其他步骤。假設您依照上述步驟進行，並將Adobe Dynamic Media Classic事件資料連結至一或多個自訂流量變數，然後依照此工作流程在Adobe Analytics中測試您的資料。

**若要檢視Adobe Analytics報表以測試整合：**

1. 從您的帳戶啟動Adobe Dynamic Media Classic檢視器，尤其是廣播您要取得的量度的帳戶，並與該帳戶互動以建立一些事件資料。

   例如，如果您想要測量「影像集」中常用的替代檢視，請預覽「影像集」並按一下不同的縮圖影像。

1. 在Adobe Analytics中，前往 **[!UICONTROL 自訂流量]** > **[!UICONTROL 自訂流量1-10]** > [prop的名稱]，從功能表選項中選取流量prop名稱。

   例如，若要存取 **[!UICONTROL LoadAsset]** 在範例帳戶中的prop中，正確的功能表選擇為 **[!UICONTROL 自訂流量]** > **[!UICONTROL 自訂流量1-10]** > **[!UICONTROL LoadAsset]**. 如果您有十個以上的自訂Prop，您也會看到其他選單選項。

1. 查看 Adobe Analytics 生成的图表。此圖表通常只是單一量度的資料。 如果您也想知道此資料與哪個資產相關聯，請取得此事件的資產資料。 例如，知道觀看了哪個視訊的比例只有50%，或一組中的哪個影像受到歡迎，通常會有幫助。

>[!NOTE]
>
>所有Adobe Dynamic Media Classic檢視器資料都會顯示在Adobe Analytics的「自訂流量」報表或「自訂轉換」報表中並彙整成報表。

如需詳細資訊，請參閱 [AnalyticsTutorials](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/overview.html).