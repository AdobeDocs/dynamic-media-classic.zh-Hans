---
title: 查看 Adobe Analytics 报告以测试集成
description: 了解如何通过查看Adobe Analytics报表来测试集成。
uuid: 937375e0-6dea-4baa-a2b0-4f3e461c9ee2
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: 1ddc89ff-d2e9-42eb-a442-aa6b9871c991
feature: Dynamic Media Classic
role: Data Engineer,Administrator,Business Practitioner
exl-id: 6186fcf0-99b4-447d-ae94-b4124dcb405b
source-git-commit: 1beb30b9eda4487dcd549034906079dee0b3149a
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 15%

---

# 查看 Adobe Analytics 报告以测试集成{#testing-the-integration-by-viewing-an-adobe-analytics-report}

在Adobe Analytics中创建必需的变量，将它们链接到Dynamic Media Classic事件，并完成必要的实施步骤后，您可以测试设置。 您可以在 Adobe Analytics 中测试和验证是否正在捕获数据。如果设置正常，则无需其他步骤。假定您按照上述步骤操作并将Dynamic Media Classic事件数据链接到一个或多个自定义流量变量，然后按照此工作流在Adobe Analytics中测试您的数据。

**要通过查看Adobe Analytics报表来测试集成，请执行以下操作：**

1. 从您的帐户启动Dynamic Media Classic查看器，尤其是用于广播您要获取的量度的查看器，并与其交互以创建一些事件数据。

   例如，如果要测量图像集中的常用替代视图，请预览图像集并单击不同的缩略图图像。

1. 在Adobe Analytics中，转到&#x200B;**[!UICONTROL Custom Traffic]** > **[!UICONTROL Custom Traffic 1-10]** > [Name of prop]，从菜单选项中选择您的流量prop名称。

   例如，要访问示例帐户中的&#x200B;**[!UICONTROL LoadAsset]**&#x200B;属性，相应的菜单选项将为&#x200B;**[!UICONTROL Custom Traffic]** > **[!UICONTROL Custom Traffic 1-10]** > **[!UICONTROL LoadAsset]**。 如果您有十个以上的自定义prop，则还会看到其他菜单选项。

1. 查看 Adobe Analytics 生成的图表。此图表通常只是单个量度的数据。 如果您还想知道此数据与哪个资产关联，请获取此事件的资产数据。 例如，通常有用的信息是：哪个视频的观看率仅为50%，或者某个视频集中的哪个图像很受欢迎。

>[!NOTE]
>
>所有Dynamic Media Classic查看器数据都在Adobe Analytics的自定义流量报表或自定义转化报表中显示和报告。

有关更多信息，请参阅[AnalyticsTutorials](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/overview.html)。