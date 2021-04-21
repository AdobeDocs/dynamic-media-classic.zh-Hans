---
title: 公开资源前测试资源
description: 了解如何在资产公开之前对其进行测试。
uuid: 5e8f3bec-6cf1-408e-8ea1-aebde0012a70
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/upload_and_publish_assets
discoiquuid: 52fadf99-7d11-46f7-8483-a9f87ffc2f67
feature: Dynamic Media Classic，资产管理
role: Business Practitioner
exl-id: fd78d535-391e-43eb-a8aa-25fa6c2885cb
translation-type: tm+mt
source-git-commit: 7456226cf6469f40e66ff327475d4c605b6d6e13
workflow-type: tm+mt
source-wordcount: '1100'
ht-degree: 55%

---

# 公开资源前测试资源 {#testing-assets-before-making-them-public}

安全测试可根据一组可配置的 IP 地址和范围来帮助您定义安全的测试环境并构建可靠的 B2B 解决方案。利用此功能，您可以将Dynamic Media Classic部署与内容管理和商务平台的架构相匹配。

通过安全测试，可以预览包含未发布内容的临时版网站。

基于下列原因，您可能希望创建临时环境，而不是公开资源：

* 在公开发布之前预览网站（临时网站）。
* 提供要求限制访问的资源，如在 B2B Web 应用程序中显示价格的 eCatalog。
* 将防火墙后的资源用作产品信息管理系统、客户服务应用程序、培训站点等的一部分。

>[!NOTE]
>
>安全测试不会影响对Dynamic Media Classic的访问。 Dynamic Media Classic安全性保持一致，并且需要通常的凭据才能访问Dynamic Media Classic和相关Web服务。

## 安全测试的工作原理 {#how-secure-testing-works}

大多数公司在防火墙后运行 Internet。可以通过某些路由，通常是通过限定范围的公共 IP 地址访问 Internet。

从您的公司网络，您可以使用https://whatismyip.com等网站确定您的公共IP地址，或从您的公司IT部门请求此信息。

通过安全测试，Dynamic Media Classic为登台环境或内部应用程序建立了专用的图像服务器。 对此服务器的所有请求都将检查原始 IP 地址。如果传入请求不在获批准的 IP 地址列表中，则返回失败响应。Dynamic Media Classic公司管理员为公司的安全测试环境配置IP地址的已批准列表。

由于必须确认原始请求的位置，因此安全测试服务的流量不会通过内容分发网络(如公共Dynamic Media Image Server流量)路由。 与公共Dynamic Media映像服务器相比，请求安全测试服务的延迟可能稍高一些。

通过安全测试服务，可以立即使用未发布的资源，无需发布。这使您可以在将资源发布到面向公众的图像服务器之前运行预览。

>[!NOTE]
>
>安全测试服务使用以内部发布上下文配置的目录服务器。因此，如果您的公司配置为发布到安全测试，请注意，Dynamic Media Classic中的所有上传资产都会立即在安全测试服务上可用。 无论资源是否在上载时标记为发布，此功能都有效。

安全测试服务当前支持以下资产类型和功能：

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>Added videos to list below 9/11/2012. Moved “Render Server requests” from unsupported to supported, listed below on 3/15/2016 as per email from Cynthia March 11, 2016)</p>

 -->

* 图像.
* 晕影（渲染服务器请求）。
* 渲染服务器请求（支持，但必须由客户明确请求）。
* 集，包括图像集、eCatalog、渲染集和媒体集。
* 标准Dynamic Media Classic富媒体查看器。
* Dynamic Media Classic OnDemand JSP页。
* 静态内容，如 PDF 文件和逐步提供的视频。
* HTTP 视频流。
* 渐进式视频流。

当前不支持以下资源类型和功能：

* RTMP 视频流
* UGC 服务
* Web-to-print
* Dynamic Media Classic Info或eCatalog搜索

## 测试安全测试服务 {#testing-the-secure-testing-service}

您应测试安全测试服务以确保其正常运行。

注意：如果未提及“设置”>“发布设置”>“图像服务器”>“测试图像服务”下的任何IP
如果您只添加一个IP，则IP将能够调用资产，而不允许其他IP进行调用。 只要该部分未提及IP，所有IP都允许对资产发出调用，并且它们将会出现。

**准备帐户**

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>RB: Rewrote entire steps under “Prepare your account” 9/10/2012</p>

 -->

1. 请联系技术支持人员，并请求对您的帐户启用安全测试。
1. 在Dynamic Media Classic中，单击&#x200B;**设置** > **发布设置** > **图像服务器**。
1. 在“图像服务器发布”页中，在“发布上下文”下拉列表中选择“**测试图像服务**”。
1. 在“客户端地址过滤器”中，单击“**添加**”。
1. 选中复选框以启用（打开）地址，然后分别在相应的文本字段中键入 IP 地址和网络掩码。

   >[!NOTE]
   >
   >如果添加单个IP地址和网络掩码，则该地址可进行资产调用。 但是，您添加的任何其他IP地址和网络掩码均不允许进行资产调用。 因此，您可能希望考虑禁用（关闭）上述步骤中的复选框，以关闭指定IP地址和网络掩码的功能。 这样做会有效地允许&#x200B;*所有* IP地址进行资产调用，所有这些IP地址都会显示出来。

1. 执行以下任一操作：
   * 重复前两个步骤以添加更多 IP 地址。
   * 继续执行下一步。
1. 在“图像服务器发布”页面的左下方，单击“**保存**”。
1. 将所需的图像上传到您的Dynamic Media Classic帐户。

   请参阅[上载文件](uploading-files.md#uploading_files)。

1. 请确保部分图像已标记为发布，而其它图像未标记，然后提交发布作业。

   请参阅[发布](publishing-files.md#publishing_files)。

1. 通过单击“**设置**”>“**应用程序设置**”>“**常规设置**”，确定您的安全测试服务的名称。
1. 在“应用程序常规设置”页面上，在“服务器”组下，在“**测试发布上下文服务器名称**”右侧找到该名称。

如果服务器名称缺失或服务器的URL不起作用，请与Adobe关怀联系。

**准备网站变体**

您需要两个网站变体，分别链接已发布和未发布的资源：

* 公共版本 — 使用传统Dynamic Media Classic URL语法链接资源。
* 暂存版本 — 使用相同的语法但使用安全测试站点名称链接资产。

**运行测试**

执行以下测试：

1. 检查是否可从公司网络内部访问资源。

   从公司网络内部（根据以前定义的 IP 地址范围确定）访问时，网站的临时版本应显示所有图像，无论图像是否标记为发布。这使得您在测试时可以避免在预览审批或产品推出前意外地将图像设为可用。

   确认网站的公共版本显示的已发布资产与之前使用Dynamic Media Classic时的体验相同。

1. 从公司网络外部，确认未发布的资源（即未标记为发布）受到保护，第三方无法访问。

   从外部（如从家庭计算机或通过 3G 连接）访问您的网络，然后确认站点的公开版本显示有所已发布的资源，但不显示未发布的内容。

   确认临时版本未显示任何资源，因为您正在从未获批准的 IP 地址访问安全测试服务。
