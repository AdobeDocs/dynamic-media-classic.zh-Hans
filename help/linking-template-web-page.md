---
title: 将模板链接至网页
description: 了解如何在AdobeDynamic Media Classic中将模板链接到网页。
uuid: f111ef06-4afc-454c-86ce-5d640236d40b
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: 989dba07-448a-45b1-b157-af50abb5359a
feature: Dynamic Media Classic
role: User
exl-id: 6305c287-360f-48c2-b456-58be0791c7af
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '339'
ht-degree: 37%

---

# 将模板链接至网页{#linking-a-template-to-a-web-page}

您的网站和应用程序通过URL字符串访问Dynamic Media图像服务器内容。 发布模板后，AdobeDynamic Media Classic会激活一个URL字符串，以在Dynamic Media图像服务器中引用该模板。 可以将该 URL 粘贴到 Web 浏览器中进行测试。

要将URL字符串放置到网页和应用程序中，请从AdobeDynamic Media Classic中复制它们。 要获取通过图像预设生成的模板URL字符串，请转到“预览”屏幕或“浏览”面板（在“详细信息”视图中）。 然后选择“图像预设”并选择“复制 URL”按钮。

>[!NOTE]
>
>在发布资源之前，URL 处于非激活状态。

## 获取模板URL {#obtaining-a-template-url}

您可以在“模板预览”屏幕上获取使用图像预设生成的模板 URL 字符串。复制 URL 后，该字符串将放置在剪贴板上，以便在必要时进行粘贴。要从“模板预览”页面获取通过图像预设生成的模板URL字符串，请执行以下操作：

1. 选择模板的滚动更新&#x200B;**[!UICONTROL 预览]**&#x200B;按钮或转到&#x200B;**[!UICONTROL 文件]** > **[!UICONTROL 预览]**。
1. 使用“预设”菜单，选择要用于发送模板图像的图像预设。“预览”页面显示从服务器传送模板时模板的外观。
1. 选择&#x200B;**[!UICONTROL 复制URL]**，以便将URL复制到剪贴板。

## 将模板URL添加到您的网页 {#adding-template-urls-to-your-web-page}

要向网页中添加模板，请咨询网页开发团队，以修改HTML网页代码中的`<IMG>`标记。 使用AdobeDynamic Media Classic URL字符串向Dynamic Media图像服务器发出请求。 商业引擎或动态网页代码插入的模板图像符合为模板选择的图像预设所定义的大小及格式规格。

>[!MORELIKETHIS]
>
>* [向网页中添加动态图像](linking-urls-web-application.md#adding_dynamic_images_to_your_web_page)

