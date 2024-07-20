---
title: 在公开资产之前测试资产
description: 了解如何在发布资源之前在Adobe Dynamic Media Classic中测试资源。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/upload_and_publish_assets
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: fd78d535-391e-43eb-a8aa-25fa6c2885cb
topic: Content Management
level: Intermediate
source-git-commit: 29752cf9eca0fc9bb760c721e1c3dc8e4ef912c3
workflow-type: tm+mt
source-wordcount: '1061'
ht-degree: 19%

---

# 在公开资产之前测试资产 {#testing-assets-before-making-them-public}

安全测试可帮助您定义安全的测试环境，并根据一组可配置的IP地址和范围构建强大的B2B解决方案。 此功能可让您将Adobe Dynamic Media Classic部署与内容管理和业务系统的架构相匹配。

通过安全测试，可以预览包含未发布内容的临时版网站。

如有需要，请创建暂存环境，而不是公开资产，原因如下：

* 在公开发布之前预览网站（临时网站）。
* 提供需要受限访问的资产，如在B2B Web应用程序中显示价格的eCatalog。
* 使用防火墙后的资产作为产品信息管理系统、客户服务应用程序、培训站点等的一部分。

>[!NOTE]
>
>安全测试不会影响对Adobe Dynamic Media Classic的访问。 Adobe Dynamic Media Classic安全性将保持一致，并且需要使用常规凭据来访问Adobe Dynamic Media Classic和相关Web服务。

## 安全测试的工作原理 {#how-secure-testing-works}

大多数公司在防火墙后运行 Internet。可以通过某些路由，通常是通过限定范围的公共 IP 地址访问 Internet。

通过公司网络，您可以使用[https://www.whatismyip.com](https://www.whatismyip.com/)之类的网站确定公共IP地址，或者向公司IT组织请求此信息。

通过安全测试，Adobe Dynamic Media Classic为暂存环境或内部应用程序建立了专用的图像服务器。 对此服务器的所有请求都将检查原始 IP 地址。如果传入请求不在批准的IP地址列表中，则会返回失败响应。 Adobe Dynamic Media Classic公司管理员为公司的Secure Testing环境配置已批准的IP地址列表。

由于必须确认原始请求的位置，因此Secure Testing服务的流量不会像公共Dynamic Media Image Server流量那样通过内容分发网络进行路由。 向Secure Testing服务发出的请求与向公共Dynamic Media图像服务器发出的请求相比，滞后时间稍长一些。

通过安全测试服务，可以立即使用未发布的资源，无需发布。通过这种方式，您可以在将资产发布到面向公众的图像服务器之前运行预览。

>[!NOTE]
>
>Secure Testing Services使用配置了内部发布上下文的目录服务器。 因此，如果贵公司配置为发布到Secure Testing，则在Adobe Dynamic Media Classic中上传的所有资源都可以立即通过Secure Testing服务使用。 不论资源是否标记为在上传时发布，此功能均为true。

安全测试服务当前支持以下资产类型和功能：

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>Added videos to list below 9/11/2012. Moved "Render Server requests" from unsupported to supported, listed below on 3/15/2016 as per email from Cynthia March 11, 2016)</p>

 -->

* 图像。
* 晕影（渲染服务器请求）。
* 渲染服务器请求（受支持，但客户必须明确请求它）。
* 集，包括图像集、eCatalog、渲染集和媒体集。
* 标准Adobe Dynamic Media Classic富媒体查看器。
* Adobe Dynamic Media Classic OnDemand JSP页。
* 静态内容，如 PDF 文件和逐步提供的视频。
* HTTP 视频流。
* 渐进式视频流。

当前不支持以下资源类型和功能：

* Adobe Dynamic Media Classic信息或eCatalog搜索
* RTMP 视频流
* Web-to-print
* UGC（用户生成的内容）服务

>[!IMPORTANT]
>
>对Adobe Dynamic Media Classic中新增或现有UGC矢量图像资源的支持已于2021年9月30日终止。

## 测试Secure Testing服务 {#testing-the-secure-testing-service}

测试Secure Testing服务，以确保该服务按预期运行。

<!-- >[!NOTE]
>
>*If you do not mention any IPs under **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Publish Setup]** > **[!UICONTROL Image Server]** > **[!UICONTROL Test Image Service]***: If you add an IP only, that IP is able to call the assets and no other IP are allowed to make the calls. As long there is no IP mentioned under that section, all IPs are allowed to make the calls for the assets, and they show up. -->

### 准备帐户

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>RB: Rewrote entire steps under "Prepare your account" 9/10/2012</p>

 -->

1. 请联系Adobe客户关怀部门，要求他们在您的帐户上启用安全测试。
1. 在Adobe Dynamic Media Classic的全局导航栏上，转到&#x200B;**[!UICONTROL 设置]** > **[!UICONTROL Publish设置]** > **[!UICONTROL 图像服务器]**。
1. 在“图像服务器Publish”页面的&#x200B;**[!UICONTROL `Publish Context`]**&#x200B;下拉列表中选择&#x200B;**[!UICONTROL 测试图像服务]**。
1. 对于客户端地址筛选器，选择&#x200B;**[!UICONTROL 添加]**。
1. 选中该复选框以启用（打开）地址，然后在相应的文本字段中键入IP地址和网络掩码。

   >[!NOTE]
   >
   >如果添加单个IP地址和网络掩码，则该地址可能会进行资产调用。 但是，不允许您添加的任何其他IP地址和网络掩码进行资产调用。 因此，请考虑禁用（关闭）上述步骤中的复选框，以关闭指定IP地址和网络掩码的功能。 这样做会有效地允许&#x200B;*所有*&#x200B;个IP地址进行资产调用，并且这些地址都会显示。

1. 执行以下任一操作：
   * 如果必须添加更多IP地址，请重复前两步。
   * 继续下一步骤。
1. 在“图像服务器Publish”页面的左下方，选择&#x200B;**[!UICONTROL 保存]**
1. 将所需的图像上传到您的Adobe Dynamic Media Classic帐户。

   查看[上载文件](uploading-files.md#uploading_files)。

1. 请确保某些图像已标记为发布，而其他图像已取消标记，然后提交发布作业。

   查看[Publish文件](publishing-files.md#publishing_files)。

1. 通过转到&#x200B;**[!UICONTROL 设置]** > **[!UICONTROL 应用程序设置]** > **[!UICONTROL 常规设置]**&#x200B;来确定您的Secure Testing服务的名称。
1. 在“应用程序常规设置”页面上，在“服务器”组下，在“**[!UICONTROL 测试发布上下文服务器名称]**”右侧找到该名称。

如果Adobe名称缺失或指向服务器的URL不起作用，请联系服务器关怀团队。

### 准备网站变体

您需要两个网站变体，分别链接已发布和未发布的资源：

* 公共版本：使用传统的Adobe Dynamic Media Classic URL语法链接资源。
* 暂存版本：使用相同的语法但使用安全测试站点名称链接资产。

### 运行测试

执行以下测试：

1. 检查是否可从公司网络内部访问资源。

   在从先前定义的IP地址范围标识的公司网络中，网站的暂存版本会显示所有图像，无论是否标记为发布。 因此，您可以在测试时避免在预览批准或产品发布之前意外使图像可用。

   确认您的网站的公共版本显示了与Adobe Dynamic Media Classic之前体验过相同的已发布资源。

1. 在公司网络外部，验证未发布的资产（即未标记为发布的资产）是否受第三方访问的保护。

   从外部访问您的网络（例如，从您的家庭计算机或通过3G连接），然后验证公共版本的网站是否显示所有已发布的资产，但不显示任何未发布的内容。

   确认临时版本未显示任何资源，因为您正在从未获批准的 IP 地址访问安全测试服务。
