---
title: “快速入门：模板发布”
seo-title: “快速入门：模板发布”
description: 'null'
seo-description: 模板发布和快速入门，帮助您快速上手和运行。
uuid: 101b6211-2421-4565-8635-94315a5c512
contentOwner: admin
content-type: 引用
products: SG_ EXPERIENCE MANAGER/Dynamic-Media-Scene-7
geptopics: SG_ SCENESELEFERENDER_ PK/类别/模板发布
discoiquuid: 03671fc1b-4fae-ad1 f-53c99 ababad
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# Quick Start: Template publishing{#quick-start-template-publishing}

Adobe Dynamic Media Classic Web-to-Print可让您创建专业品牌的印刷内容，便于客户、客户和员工进行自定义和个性化。您可以在整个发布过程中维护企业内容和品牌标识。最终用户可以自定义印刷内容，但仅限于您允许他们自定义的部分内容。例如，个性化信纸、名片、海报、贺卡、标签、支票、礼物、衣服、日历、贴粘簿以及相册都是您可以传送的自定义印刷产品。公司可以在其标志中维护通用的品牌标识，可以针对不同地区、特许经营权、商店以及分支机构自定义这些标识。

首先，在Adobe Illustrator中设计模板。在此模板中，详细定义了常量和变量（变量组件是可以自定义的组件）。例如，在对 Illustrator 文件中的文本进行参数化之后，最终用户可以输入自己的文本。同样，在将背景颜色参数化为一个变量组件之后，可以变换不同的背景颜色。

动态媒体经典提供两个模板发布工作流程，一个用于基本用例，另一个用于高级用例。基本用例在Adobe Illustrator中创建设计，将其上传至Dynamic Media经典，并使用SPS中的参数定义变量元素。高级使用案例需要更全面地定义可变性。高级用例在Adobe Illustrator中创建变量元素，将文件上载到Dynamic Media经典，并使用URL调用直接处理XML级别上的那些元素。调用此方案 *`*DOM manipulation*`*。

>[!NOTE]
>
>For more information about Dynamic Media Classic web-to-print workflows, template creation, parameterization, DOM manipulation, and more, see the Web-to-Print Workflow Guide here: [www.adobe.com/go/learn_s7_webtoprint_en](https://www.adobe.com/go/learn_s7_webtoprint_en) . 将Zip文件下载到本地硬盘并提取其内容(Dynamic Media经典Web到打印教程文档和教程资源)。

**快速入门**

本快速入门介绍了使用 Illustrator 文件创建高质量的可自定义的打印产品的基本工作流程。

**1. 设计 Illustrator 文件以发布模板**

在 Illustrator 中，设计您的模板。如果要使用高级 DOM 处理方法自定义模板，请在 Illustrator 中定义变量元素的 s7:elementID。

请参阅[在 Illustrator 中创建初始模板](create-initial-template-illustrator.md#create_the_initial_template_in_illustrator)和 [DOM 处理](dom-manipulation.md#dom_manipulation)。

**2. Convert your template to Dynamic Media Classic FXG and upload it to Scene7 Publishing System**

Adobe Creative Cloud 用户可以使用用于 Web-to-Print 的 Adobe Illustrator 插件。此插件可将模板转换为Dynamic Media经典FXG。如果模板包含字体，则在上载 FXG 文件之前必须先将相应的字体文件上载到 Scene7 Publishing System。

请参阅[上载用于模板发布的文件](upload-files-template-publishing.md#upload_files_for_template_publishing)。

**3. 在Dynamic Media经典中查看、定义或调整参数**

在“模板发布预览”和“模板发布构建”屏幕中，您可以通过参数定义和优化变量元素，预览结果以及对结果进行测试。在这些屏幕中，您可以执行以下操作：

* 创建和修改参数。
* 为参数属性和特性指定默认值。
* 单击“复制 URL”，将预览 URL 复制到剪贴板，并在浏览器窗口中预览结果。

请参阅 [在Dynamic Media经典中参数化模板](parameterizing-template-scene7.md#parameterizing_a_template_in_scene7)。

**4. 发布 FXG 模板**

在您完成参数和属性的定义和测试之后，发布该文件。发布FXG模板可将其放置在动态媒体图像服务器上并激活URL。

请务必发布 FXG 模板关联的所有图像和字体。

请参阅[发布 FXG 模板](dom-manipulation.md#publish_fxg_templates)。

**5. 获取 URL**

现在，模板可以通过其 URL 嵌入到您的网站中，以供最终用户创建个性化的变量内容。

请参阅[将 FXG 模板链接到网页](linking-fxg-template-web-page.md#linking_an_fxg_template_to_a_web_page)。
