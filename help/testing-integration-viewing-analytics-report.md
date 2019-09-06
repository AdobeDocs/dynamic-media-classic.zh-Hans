---
title: 查看 Adobe Analytics 报告以测试集成
seo-title: 查看 Adobe Analytics 报告以测试集成
description: 'null'
seo-description: 了解如何通过查看Adobe Analytics报告测试集成。
uuid: 937375e0-6dea-4baa-a2 b0-4f3 e461 c9 ee2
contentOwner: admin
content-type: 引用
products: SG_ EXPERIENCE MANAGER/Dynamic-Media-Scene-7
geptopics: SG_ SCENEESFERENONDAND_ PK/categories/adobe_ analytics_ contracting_ kit
discoiquuid: 1ddc89ff-d2 e9-42eb-a442-aa6 b9871 c991
translation-type: tm+mt
source-git-commit: a1722c15d3c049f05959d895e85297d47d730872

---


# 查看 Adobe Analytics 报告以测试集成{#testing-the-integration-by-viewing-an-adobe-analytics-report}

在Adobe Analytics中创建必要变量后，将其链接到Dynamic Media经典活动并完成必要的实施步骤，然后您应该测试设置。您可以在 Adobe Analytics 中测试和验证是否正在捕获数据。如果设置正常，则无需其他步骤。假定您遵循上述步骤，然后将Dynamic Media经典事件数据链接到一个或多个自定义流量变量，然后按照此工作流程在Adobe Analytics中测试数据。

**通过查看报告测试 Adobe Analytics 集成**

1. 从您的帐户启动Dynamic Media经典查看器，尤其是广播要捕获的量度并与它交互以创建某些活动数据的查看器。

   例如，如果您想测量某个图像集中最受欢迎的替代视图，请预览该图像集并单击其他缩略图图像。

1. Inside Adobe Analytics, go to Custom Traffic &gt; Custom Traffic 1-10 &gt; [Name of prop], selecting your traffic prop name from the menu choices.

   例如，要访问我们的示例帐户的 LoadAsset 属性，正确的菜单选择顺序是“自定义流量”&gt;“自定义流量 1-10”&gt;“LoadAsset”。如果您的自定义属性超过 10 个，那么还可以看到其他的菜单选择项。

1. 查看 Adobe Analytics 生成的图表。请注意，这通常只是单个量度的数据。如果您还希望了解此数据与哪个资产相关联(例如，将哪个视频监视到50%，或一个集合中的哪个图像最受欢迎)，请务必同时捕捉此事件的资产数据。

>[!NOTE]
>
>所有动态媒体经典查看器数据在自定义流量报告或Adobe Analytics的自定义转换报告中显示和报告。

有关更多信息，请参阅 [www.adobe.com/go/learn_sc7_sitecatalystguide_en](https://www.adobe.com/go/learn_sc7_sitecatalystguide_en)。
