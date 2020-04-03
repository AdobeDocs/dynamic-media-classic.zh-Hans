---
title: 将模板链接到网页
seo-title: 将模板链接到网页
description: 'null'
seo-description: 了解如何将模板链接到网页。
uuid: f111ef06-4afc-454c-86ce-5d640236d40b
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: 989dba07-448a-45b1-b157-af50abb5359a
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# 将模板链接到网页{#linking-a-template-to-a-web-page}

您的网站和应用程序通过URL字符串访问Dynamic Media Image Server内容。 发布模板后，Dynamic Media Classic会激活引用Dynamic Media Image Server上的模板的URL字符串。 可以将该 URL 粘贴到 Web 浏览器中进行测试。

要将 URL 字符串放置在网页和应用程序中，请从 Scene7 Publishing System 中复制这些字符串。要获取使用图像预设生成的模板 URL 字符串，请转至“预览”屏幕或浏览面板（在“细节”视图中）。然后选择“图像预设”并选择“复制 URL”按钮。

>[!NOTE]
>
>在发布资源之前，URL 处于非激活状态。

## 获取模板 URL {#obtaining-a-template-url}

您可以在“模板预览”屏幕上获取使用图像预设生成的模板 URL 字符串。复制 URL 后，该字符串将放置在剪贴板上，以便在必要时进行粘贴。请按照以下步骤在“模板预览”屏幕上获取使用图像预设生成的模板 URL 字符串：

1. 单击模板的变换“预览”按钮或选择“文件”>“预览”。“预览”屏幕随即打开。
1. 使用“预设”菜单，选择要用于发送模板图像的图像预设。“预览”屏幕可显示从服务器发送后的模板效果。
1. 单击“复制 URL”按钮，将 URL 复制到剪贴板。

## 将模板 URL 添加到网页中 {#adding-template-urls-to-your-web-page}

To add a template to your web page, consult with your web page development team to modify the `<IMG>` tag in your HTML web page code using the Dynamic Media Classic URL string to make a request to Dynamic Media Image Servers. 商业引擎或动态网页代码插入的模板图像符合为模板选择的图像预设所定义的大小及格式规格。

>[!MORELIKETHIS]
>
>* [将动态图像添加到网页中](linking-urls-web-application.md#adding_dynamic_images_to_your_web_page)

