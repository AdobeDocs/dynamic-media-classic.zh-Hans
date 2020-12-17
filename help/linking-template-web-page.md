---
title: 将模板链接到网页
seo-title: 将模板链接到网页
description: 'null'
seo-description: 了解如何将模板链接到网页。
uuid: f111ef06-4afc-454c-86ce-5d640236d40b
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: 989dba07-448a-45b1-b157-af50abb5359a
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '340'
ht-degree: 70%

---


# 将模板链接到网页{#linking-a-template-to-a-web-page}

您的网站和应用程序通过URL字符串访问Dynamic Media图像服务器内容。 发布模板后，Dynamic Media经典将激活引用Dynamic Media图像服务器上该模板的URL字符串。 可以将该 URL 粘贴到 Web 浏览器中进行测试。

要将URL字符串放置到网页和应用程序中，请从Dynamic Media经典中复制它们。 要获取使用图像预设生成的模板 URL 字符串，请转至“预览”屏幕或浏览面板（在“细节”视图中）。然后选择“图像预设”并选择“复制 URL”按钮。

>[!NOTE]
>
>在发布资源之前，URL 处于非激活状态。

## 获取模板 URL {#obtaining-a-template-url}

您可以在“模板预览”屏幕上获取使用图像预设生成的模板 URL 字符串。复制 URL 后，该字符串将放置在剪贴板上，以便在必要时进行粘贴。请按照以下步骤在“模板预览”屏幕上获取使用图像预设生成的模板 URL 字符串：

1. 单击模板的变换“预览”按钮或选择“文件”>“预览”。“预览”屏幕随即打开。
1. 使用“预设”菜单，选择要用于发送模板图像的图像预设。“预览”屏幕可显示从服务器发送后的模板效果。
1. 单击“复制 URL”按钮，将 URL 复制到剪贴板。

## 将模板 URL 添加到网页中  {#adding-template-urls-to-your-web-page}

要向网页添加模板，请咨询网页开发团队，使用Dynamic Media经典URL字符串修改HTML网页代码中的`<IMG>`标记，以向Dynamic Media图像服务器发出请求。 商业引擎或动态网页代码插入的模板图像符合为模板选择的图像预设所定义的大小及格式规格。

>[!MORELIKETHIS]
>
>* [将动态图像添加到网页中](linking-urls-web-application.md#adding_dynamic_images_to_your_web_page)

