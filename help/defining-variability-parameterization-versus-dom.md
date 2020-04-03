---
title: '"定义可变性：参数化与 DOM 处理"'
seo-title: '"定义可变性：参数化与 DOM 处理"'
description: 'null'
seo-description: 了解如何通过参数化与DOM操作来定义可变性。
uuid: dce424f2-07d8-4703-aa3a-40d2eee12f74
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template-publishing
discoiquuid: 5b844afe-ac55-4dd2-8fe8-125a9c9af948
translation-type: tm+mt
source-git-commit: 6fff3699f8a08af433df3f3a7790a11bf9d05b00

---


# 定义可变性：参数化与 DOM 处理{#defining-variability-parameterization-versus-dom-manipulation}

Dynamic Media Classic优惠了两种管理模板中可变内容的技术。 使用这两种技术，您可以在Illustrator中设计初始模板，将模板转换为Dynamic Media Classic FXG文件格式，然后将其上传到SPS。 但在您对变量元素的控制程度以及使用这些元素所需的技巧方面，这两种方法有所不同。

* **在Scene7 Publishing System中参数化此技术需要在SPS中的“模板发布构建”和“预览”屏幕或Web到打印的Adobe Illustrator插件中定义可变性。**&#x200B;这两种方法均提供了工具供您创建参数，分配参数值和测试结果。

* **使用DOM操**&#x200B;作此技术可让您在XML级别控制设计和模板。 Dynamic Media Classic FXG文件是XML文件。 通过该方法，您可以直接通过设计模板的 XML DOM（显示对象模型）编辑设计模板。在 Illustrator 中，使用 s7:elementID 标记变量元素，以便稍后使用 URL 命令处理这些元素。

>[!MORELIKETHIS]
>
>* [在Dynamic Media Classic中参数化模板](parameterizing-template-scene7.md#parameterizing_a_template_in_scene7)
>* [DOM 处理](dom-manipulation.md#dom_manipulation)

