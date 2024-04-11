---
title: 通过查看Adobe Analytics报表测试集成
description: 了解如何通过查看Adobe Dynamic Media Classic报表来测试Adobe Analytics中的集成。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 6186fcf0-99b4-447d-ae94-b4124dcb405b
topic: Integrations, Development
level: Experienced
source-git-commit: 5b5dcd1199bd51ec987b5673fce75bc86baad55b
workflow-type: tm+mt
source-wordcount: '339'
ht-degree: 5%

---

# 通过查看Adobe Analytics报表测试集成{#testing-the-integration-by-viewing-an-adobe-analytics-report}

在Adobe Analytics中创建必要的变量、将这些变量链接到Adobe Dynamic Media Classic事件并完成必要的实施步骤后，即可测试设置。 您可以测试和验证Adobe Analytics本身是否正在捕获数据。 如果设置正常，则无需其他步骤。假设您执行上述步骤并将Adobe Dynamic Media Classic事件数据链接到一个或多个自定义流量变量，然后按照此工作流在Adobe Analytics中测试您的数据。

**要通过查看Adobe Analytics报表来测试集成，请执行以下操作：**

1. 从您的帐户启动Adobe Dynamic Media Classic查看器，特别是要广播要获取的量度的帐户，并与该帐户交互以创建一些事件数据。

   例如，如果要测量图像集中的常用替代视图，则预览图像集并单击不同的缩略图图像。

1. 在Adobe Analytics中，转到 **[!UICONTROL 自定义流量]** > **[!UICONTROL 自定义流量1-10]** > [prop的名称]，从菜单选项中选择流量prop名称。

   例如，要访问 **[!UICONTROL LoadAsset]** prop中，正确的菜单选项为 **[!UICONTROL 自定义流量]** > **[!UICONTROL 自定义流量1-10]** > **[!UICONTROL LoadAsset]**. 如果您有十个以上的自定义prop，您也会看到其他菜单选项。

1. 查看 Adobe Analytics 生成的图表。此图表通常只是单个指标的数据。 如果您还想知道此数据与哪个资产相关联，请获取此事件的资产数据。 例如，了解观看了哪个视频的百分比仅为50%或集中的哪个图像受欢迎通常很有用。

>[!NOTE]
>
>所有Adobe Dynamic Media Classic查看器数据都会在Adobe Analytics的自定义流量报表或自定义转化报表中显示和报告。

有关更多信息，请参阅 [AnalyticsTutorials](https://experienceleague.adobe.com/en/docs/analytics-learn/tutorials/overview).