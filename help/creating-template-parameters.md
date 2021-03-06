---
title: 创建模板参数
description: 了解如何在Adobe Dynamic Media Classic中创建模板参数。
uuid: d17168a8-4776-4761-b022-8258d5997604
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: d263f041-5a0d-4c4f-9266-aeff51a5a7e2
feature: Dynamic Media Classic
role: User
exl-id: 118806ea-c8a7-4aaf-9ae3-739c6b04ea77
source-git-commit: 352b1c383195fa03294ad3501207d63f3cfe3e42
workflow-type: tm+mt
source-wordcount: '844'
ht-degree: 59%

---

# 创建模板参数{#creating-template-parameters}

您可以通过参数尽可能灵活地使用模板；可以通过参数来动态自定义模板图像。您可以确定模板中要包括哪些文本图层和图像图层，以及每个图层中要显示哪些参数。例如，要引起对正在销售的产品的注意，您可以创建On Sale文本层。 日后可以删除“待售”参数来删除该图层，但仍保留模板图像的其余部分。

创建模板参数时，实际上是声明要在 URL 字符串中调用模板的哪些部分。使用参数构造的 URL 会在 URL 字符串中列出相关项目。通过列出的参数，您可以按照模板图像从图像服务器动态构造的方式来创建自定义结果，从而动态更改模板（因为您可以调用 URL 中的部分或全部参数）。

在文本图层参数中，还可以将文本字符串设置为链接到数据库值的动态字段。将文本链接到数据库的功能非常有用（例如在促销活动中）。您可以自定义模板图像，使其显示客户端或客户姓名。您还可以将文本层参数链接到价格数据库，以显示模板图像中项目的价格。

您可以多次引用一个参数。对参数对话框中的每个命令使用组合框，以选择匹配该特定命令的参数。例如，所有大小参数都可用于`size=`命令。 可以将参数引用再分配给已存在于组合框中的任何参数，并重命名为组合框中不存在的名称。在后一种情况下，名称必须唯一。 否则，错误会声明参数存在。 删除参数引用时，如果该参数未在其他位置引用，则会从URL中删除该参数。 当更改文本参数的默认值时，对该参数的所有引用都会更新。 您可以在层表、模板渲染和URL中查看更新。 当通过在属性面板中调整控制滑块大小或键入值来更改层属性时，将更新参数值并更新对参数的所有引用。 例如，如果使用一个参数对两个图层的大小进行了参数化，则在更改其中一个图层大小时，两个图层的大小均会更新。在您预览模板并更改参数时，该参数的所有引用均会更新。

另请参阅[模板基础知识](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/553_Template%20Basics_converted%20renamed_Dynamic%20Banners-AVS)培训视频。

## 参数化图层 {#parameterizing-a-layer}

对于模板中的每个图层，请根据以下步骤创建模板参数：

1. 在“图层”列表中，选择要创建参数的图层名称旁边的“参数”按钮 。将打开“参数”屏幕。它会列出图层上每个参数的名称、值及类型。
1. 对于要包括在模板图像中的每个参数，选择其名称旁边的“开”选项。
1. 选择&#x200B;**[!UICONTROL Close]**&#x200B;以退出“参数”屏幕。

>[!NOTE]
>
>可以在“参数”屏幕中重命名参数。重命名参数使得参数更易于在 URL 字符串中标识，且更易于作为数据库值使用。要重命名参数，请选择其&#x200B;**[!UICONTROL On]**&#x200B;选项，选择其名称，然后在“名称”字段中输入新名称。

要查看已为模板创建的参数列表，请在“模板”屏幕上选择“参数摘要”按钮。将打开“参数摘要”屏幕。它会列出每个图层的名称，如果已为图层创建参数，则还会显示参数名和参数值。

## 创建动态文本参数 {#creating-dynamic-text-parameters}

对于文本层，您还可以将文本字符串设置为链接到数据库值的动态字段。 请遵循以下步骤：

1. 在“模板”屏幕上，选择要为其创建动态文本参数的文本图层名称旁边的“参数”按钮 。此时将打开“参数”页面。
1. 选择文本属性名称(textAttr)旁边的&#x200B;**[!UICONTROL On]**&#x200B;选项。
1. 在“参数”屏幕中选择&#x200B;**[!UICONTROL Text]**&#x200B;选项卡。
1. 选择&#x200B;**[!UICONTROL 添加参数]**。 将显示默认的参数名。选择该名称并覆盖键入新名称，可以替换此名称。当前键入的文本字符串将成为参数的新名称。
1. 选择&#x200B;**[!UICONTROL Close]**&#x200B;以关闭“参数”页面。

要使参数名使用数据库值，请将以下字符串附加到模板 URL：

```as3
?$_2(parameter name)=(database value)
```

参数名称由数据库字段或Java™代码中的名称替换，这些名称指示例如项目的当前价格或客户名称。
