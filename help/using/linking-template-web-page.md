---
title: 将模板链接到网页
description: 了解如何将模板链接到Adobe Dynamic Media Classic中的网页。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
feature: Dynamic Media Classic
role: User
exl-id: 6305c287-360f-48c2-b456-58be0791c7af
topic: Administration, Content Management, Development
level: Experienced
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '339'
ht-degree: 16%

---

# 将模板链接到网页{#linking-a-template-to-a-web-page}

您的网站和应用程序通过URL字符串访问Dynamic Media图像服务器内容。 发布模板后，Adobe Dynamic Media Classic会激活一个在Dynamic Media图像服务器上引用模板的URL字符串。 可以将此URL粘贴到Web浏览器以进行测试。

要将URL字符串放置到网页和应用程序中，请从Adobe Dynamic Media Classic复制它们。 要获取使用图像预设生成的模板URL字符串，请转到“预览”屏幕或“浏览”面板（在“详细信息视图”中）。 然后选择“图像预设”并选择“复制 URL”按钮。

>[!NOTE]
>
>在发布资源之前，URL 处于非激活状态。

## 获取模板URL {#obtaining-a-template-url}

您可以在“模板预览”屏幕上获取使用图像预设生成的模板 URL 字符串。复制 URL 后，该字符串将放置在剪贴板上，以便在必要时进行粘贴。要从“模板预览”页面获取使用图像预设生成的模板URL字符串，请执行以下操作：

1. 选择模板的滚动更新&#x200B;**[!UICONTROL 预览]**&#x200B;按钮或转到&#x200B;**[!UICONTROL 文件]** > **[!UICONTROL 预览]**。
1. 使用预设的菜单，选择要用于交付模板图像的图像预设。 “预览”页面显示从服务器交付模板时的外观。
1. 选择&#x200B;**[!UICONTROL 复制URL]**，以便将URL复制到剪贴板。

## 将模板URL添加到网页 {#adding-template-urls-to-your-web-page}

若要向网页添加模板，请咨询网页开发团队，以修改HTML网页代码中的`<IMG>`标记。 使用Adobe Dynamic Media Classic URL字符串向Dynamic Media图像服务器发出请求。 商业引擎或动态网页代码将按照您为模板选择的图像预设所定义的大小和格式规范插入模板图像。

>[!MORELIKETHIS]
>
>* [将动态图像添加到网页](linking-urls-web-application.md#adding_dynamic_images_to_your_web_page)
