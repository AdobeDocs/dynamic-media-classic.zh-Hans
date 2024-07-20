---
title: 创建模板参数
description: 了解如何在Adobe Dynamic Media Classic中创建模板参数。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
feature: Dynamic Media Classic
role: User
exl-id: 118806ea-c8a7-4aaf-9ae3-739c6b04ea77
topic: Development
level: Experienced
source-git-commit: 00591bdbe721035e25d3dea245a2110f978d19aa
workflow-type: tm+mt
source-wordcount: '791'
ht-degree: 45%

---

# 创建模板参数{#creating-template-parameters}

通过参数，您可以最灵活地使用模板；通过参数，您可以动态自定义模板图像。 您可以确定模板中要包括哪些文本图层和图像图层，以及每个图层中要显示哪些参数。例如，要吸引客户注意正在销售的产品，您可以创建一个“正在销售”文本层。 日后可以删除“待售”参数来删除该图层，但仍保留模板图像的其余部分。

创建模板参数时，实际上是声明要在 URL 字符串中调用模板的哪些部分。使用参数构造的 URL 会在 URL 字符串中列出相关项目。通过列出的参数，您可以按照模板图像从图像服务器动态构造的方式来创建自定义结果，从而动态更改模板（因为您可以调用 URL 中的部分或全部参数）。

在文本图层参数中，还可以将文本字符串设置为链接到数据库值的动态字段。将文本链接到数据库的功能非常有用（例如在促销活动中）。您可以自定义模板图像，使其显示客户端或客户姓名。您还可以将文本层参数链接到价格数据库，以在模板图像中显示项目的价格。

您可以多次引用一个参数。对参数对话框中的每个命令使用组合框，以选择匹配该特定命令的参数。例如，所有大小参数都可用于`size=`命令。 可以将参数引用再分配给已存在于组合框中的任何参数，并重命名为组合框中不存在的名称。在后一种情况下，名称必须是唯一的。 否则，错误会声明参数存在。 删除参数引用时，如果参数未在其他任何位置引用，则会从URL中删除该参数。 当更改文本参数的缺省值时，对该参数的所有引用都将更新。 您可以在图层表、模板的渲染和URL中查看更新。 当通过操作调整大小句柄或在属性面板中键入值来更改图层属性时，参数值将更新，所有对该参数的引用都将更新。 例如，如果使用一个参数对两个图层的大小进行了参数化，则在更改其中一个图层大小时，两个图层的大小均会更新。在您预览模板并更改参数时，该参数的所有引用均会更新。

另请观看[模板基础知识](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/553_Template%20Basics_converted%20renamed_Dynamic%20Banners-AVS)培训视频。

## 参数化图层 {#parameterizing-a-layer}

对于模板中的每个图层，请根据以下步骤创建模板参数：

1. 在“层”列表中，选择要为其创建参数的层名称旁边的“参数”按钮。 将打开“参数”屏幕。它列出了层上每个参数的名称、其值及其类型。
1. 选择要包含在模板图像中的每个参数的名称旁边的“开启”选项。
1. 选择&#x200B;**[!UICONTROL 关闭]**&#x200B;以退出“参数”屏幕。

>[!NOTE]
>
>可以在“参数”屏幕中重命名参数。重命名参数使得参数更易于在 URL 字符串中标识，且更易于作为数据库值使用。要重命名参数，请选择其&#x200B;**[!UICONTROL On]**&#x200B;选项，选择其名称，然后在“名称”字段中输入一个新名称。

要查看为模板创建的参数列表，请选择“模板”屏幕上的“参数摘要”按钮。 在“参数摘要”屏幕中，列出每个层的名称，如果已为层创建了参数，则列出参数名称和值。

## 创建动态文本参数 {#creating-dynamic-text-parameters}

对于文本图层，您还可以将文本字符串设置为链接到数据库值的动态字段。 请遵循以下步骤：

1. 在“模板”屏幕上，选择要为其创建动态文本参数的文本图层名称旁边的“参数”按钮。 此时将打开“参数”页。
1. 选择文本属性(textAttr)的名称旁边的&#x200B;**[!UICONTROL On]**&#x200B;选项。
1. 在“参数”屏幕中选择&#x200B;**[!UICONTROL 文本]**&#x200B;选项卡。
1. 选择&#x200B;**[!UICONTROL 添加参数]**。 将显示默认的参数名。选择该名称并覆盖键入新名称，可以替换此名称。当前键入的文本字符串将成为参数的新名称。
1. 选择&#x200B;**[!UICONTROL 关闭]**&#x200B;以关闭“参数”页。

要使参数名使用数据库值，请将以下字符串附加到模板 URL：

```as3
?$_2(parameter name)=(database value)
```

数据库字段或Java™代码中的名称将替换参数名称。 例如，此类功能指示项目的当前价格或客户名称。
