---
title: '"定义可变性：参数化与 DOM 处理"'
seo-title: '"定义可变性：参数化与 DOM 处理"'
description: 'null'
seo-description: 了解如何使用参数化与DOM操作定义可变性。
uuid: dce424f2-07d8-4703-aa3 a-40d2 eee12 f74
contentOwner: admin
content-type: 引用
products: SG_ EXPERIENCE MANAGER/Dynamic-Media-Scene-7
geptopics: SG_ SCENESELEFERENDER_ PK/类别/模板发布
discoiquuid: 5b844afe-ac55-4dd2-125a9 b8125 a9 c9 af948
translation-type: tm+mt
source-git-commit: d5bf894d56687561c93ef08762bc19d3597225e6

---


# 定义可变性：参数化与 DOM 处理{#defining-variability-parameterization-versus-dom-manipulation}

动态媒体经典提供两种用于管理模板中的可变内容的技术。通过这两种技术，您都可以在Illustrator中设计初始模板，将模板转换为Dynamic Media经典FXG文件格式，并将它上传到SPS。但在您对变量元素的控制程度以及使用这些元素所需的技巧方面，这两种方法有所不同。

**在Scene Publishing System中参数化** 此技术需要在SPS中的“模板发布构建和预览”屏幕中定义可变性，或在用于Web到打印的Adobe Illustrator插件中定义可变性。这两种方法均提供了工具供您创建参数，分配参数值和测试结果。

**使用DOM操作** 此技术可让您控制XML级别上的设计和模板。Dynamic Media Classic FXG文件为XML。通过该方法，您可以直接通过设计模板的 XML DOM（显示对象模型）编辑设计模板。在 Illustrator 中，使用 s7:elementID 标记变量元素，以便稍后使用 URL 命令处理这些元素。

>[!MORELIKETHIS]
>
>* [在Dynamic Media经典中参数化模板](parameterizing-template-scene7.md#parameterizing_a_template_in_scene7)
>* [DOM 处理](dom-manipulation.md#dom_manipulation)

