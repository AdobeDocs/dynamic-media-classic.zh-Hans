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
role: 数据工程师，管理员，业务从业者
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '352'
ht-degree: 39%

---


# 查看 Adobe Analytics 报告以测试集成{#testing-the-integration-by-viewing-an-adobe-analytics-report}

在Adobe Analytics中创建了必要的变量后，将它们链接到Dynamic Media Classic事件并完成了必要的实施步骤，您应该测试设置。 您可以在 Adobe Analytics 中测试和验证是否正在捕获数据。如果设置正常，则无需其他步骤。假定您遵循上述步骤并将Dynamic Media Classic事件数据链接到一个或多个自定义流量变量，则按照此工作流程在Adobe Analytics内测试您的数据。

**通过查看报告测试 Adobe Analytics 集成**

1. 从您的帐户启动Dynamic Media Classic查看器，尤其是广播您要捕获的量度并与它交互以创建某些事件数据的查看器。

   例如，如果您想测量某个图像集中最受欢迎的替代视图，请预览该图像集并单击其他缩略图图像。

1. 在Adobe Analytics中，转到“自定义流量”>“自定义流量1-10”>“prop]的名称”，从菜单选项中选择您的流量prop名称。[

   例如，要访问我们的示例帐户的 LoadAsset 属性，正确的菜单选择顺序是“自定义流量”>“自定义流量 1-10”>“LoadAsset”。如果您的自定义属性超过 10 个，那么还可以看到其他的菜单选择项。

1. 查看 Adobe Analytics 生成的图表。请注意，这通常只是单个量度的数据。如果您还想知道此数据与哪个资产关联（例如，哪个视频被监视到仅50%，或某个视频集中哪个图像最受欢迎），请务必也捕获此事件的资产数据。

>[!NOTE]
>
>所有Dynamic Media Classic查看器数据都会在Adobe Analytics的“自定义流量”报表或“自定义转换”报表中显示和报告。

有关详细信息，请参阅[www.adobe.com/go/learn_sc7_sitecatalystguide_en](https://www.adobe.com/go/learn_sc7_sitecatalystguide_en)。
