---
title: 查看 Adobe Analytics 报告以测试集成
description: 了解如何通过查看Adobe Analytics报告来测试集成。
uuid: 937375e0-6dea-4baa-a2b0-4f3e461c9ee2
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: 1ddc89ff-d2e9-42eb-a442-aa6b9871c991
feature: Dynamic Media Classic
role: Data Engineer,Administrator,Business Practitioner
exl-id: 6186fcf0-99b4-447d-ae94-b4124dcb405b
translation-type: tm+mt
source-git-commit: 1beb30b9eda4487dcd549034906079dee0b3149a
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 15%

---

# 查看 Adobe Analytics 报告以测试集成{#testing-the-integration-by-viewing-an-adobe-analytics-report}

在Adobe Analytics中创建了必要的变量，将它们链接到Dynamic Media Classic事件，并完成了必要的实施步骤后，您可以测试设置。 您可以在 Adobe Analytics 中测试和验证是否正在捕获数据。如果设置正常，则无需其他步骤。假定您遵循上述步骤并将Dynamic Media Classic事件数据链接到一个或多个自定义流量变量，则按照此工作流程在Adobe Analytics内测试您的数据。

**要通过查看Adobe Analytics报告测试集成，请执行以下操作：**

1. 从您的帐户开始Dynamic Media Classic查看器，尤其是广播您要获取的量度并与它交互以创建某些事件数据的查看器。

   例如，如果要测量图像集中常用的替代视图，请预览图像集，然后单击不同的缩略图图像。

1. 在Adobe Analytics中，转到&#x200B;**[!UICONTROL 自定义流量]** > **[!UICONTROL 自定义流量1-10]** > [prop]的名称，从菜单选项中选择您的流量prop名称。

   例如，要访问示例帐户中的&#x200B;**[!UICONTROL LoadAsset]**&#x200B;属性，正确的菜单选项是&#x200B;**[!UICONTROL 自定义流量]** > **[!UICONTROL 自定义流量1-10]** > **[!UICONTROL LoadAsset]**。 如果您有十多个自定义prop，您还会看到其他菜单选项。

1. 查看 Adobe Analytics 生成的图表。此图表通常仅是单个量度的数据。 如果您还想了解此数据与哪个资产关联，请获取此事件的资产数据。 例如，了解哪个视频的观看率仅为50%，或者集合中的哪个图像比较受欢迎，这通常很有用。

>[!NOTE]
>
>所有Dynamic Media Classic查看器数据都会在Adobe Analytics的“自定义流量”报表或“自定义转换”报表中显示和报告。

有关详细信息，请参阅[分析Tutorials](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/overview.html)。