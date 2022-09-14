---
title: 在将资产公开之前对其进行测试
description: 了解如何在Adobe Dynamic Media Classic中测试资产，然后再将其公开。
uuid: 5e8f3bec-6cf1-408e-8ea1-aebde0012a70
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/upload_and_publish_assets
discoiquuid: 52fadf99-7d11-46f7-8483-a9f87ffc2f67
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: fd78d535-391e-43eb-a8aa-25fa6c2885cb
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '1066'
ht-degree: 31%

---

# 在将资产公开之前对其进行测试 {#testing-assets-before-making-them-public}

安全测试可帮助您定义安全测试环境，并基于一组可配置的IP地址和范围构建强大的B2B解决方案。 此功能允许您将Adobe Dynamic Media Classic部署与内容管理和业务系统的架构相匹配。

通过安全测试，可以预览包含未发布内容的临时版网站。

如果需要，请创建暂存环境，而不是公开提供资产，原因如下：

* 在公开发布之前预览网站（临时网站）。
* 提供要求限制访问的资源，如在 B2B Web 应用程序中显示价格的 eCatalog。
* 将防火墙后的资源用作产品信息管理系统、客户服务应用程序、培训站点等的一部分。

>[!NOTE]
>
>安全测试不影响对Adobe Dynamic Media Classic的访问。 Adobe Dynamic Media Classic安全性保持一致，需要通常的凭据才能访问Adobe Dynamic Media Classic和相关web服务。

## 安全测试的工作原理 {#how-secure-testing-works}

大多数公司在防火墙后运行 Internet。可以通过某些路由，通常是通过限定范围的公共 IP 地址访问 Internet。

从您的公司网络中，您可以使用诸如 [https://www.whatismyip.com](https://www.whatismyip.com/) 或向您的公司IT组织请求此信息。

通过安全测试，Adobe Dynamic Media Classic为暂存环境或内部应用程序建立专用的图像服务器。 对此服务器的所有请求都将检查原始 IP 地址。如果传入请求不在获批准的 IP 地址列表中，则返回失败响应。Adobe Dynamic Media Classic公司管理员为其公司的安全测试环境配置已批准的IP地址列表。

由于必须确认原始请求的位置，因此安全测试服务的流量不会通过内容分发网络(如公共Dynamic Media图像服务器流量)路由。 与公共的Dynamic Media图像服务器相比，对安全测试服务的请求的滞后时间略高。

通过安全测试服务，可以立即使用未发布的资源，无需发布。这样，您就可以在将资产发布到其面向公众的图像服务器之前，运行预览。

>[!NOTE]
>
>安全测试服务使用配置了内部发布上下文的目录服务器。 因此，如果您的公司配置为发布到安全测试，则Adobe Dynamic Media Classic中任何上传的资产都会立即在安全测试服务上可用。 无论资产是否标记为上传后发布，此功能都为true。

安全测试服务当前支持以下资产类型和功能：

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>Added videos to list below 9/11/2012. Moved “Render Server requests” from unsupported to supported, listed below on 3/15/2016 as per email from Cynthia March 11, 2016)</p>

 -->

* 图像.
* 晕影（渲染服务器请求）。
* 呈现服务器请求（支持，但必须由客户明确请求）。
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
>2021年9月30日终止对Adobe Dynamic Media Classic中新的或现有的UGC矢量图像资产的支持。

## 测试安全测试服务 {#testing-the-secure-testing-service}

测试安全测试服务，以确保该服务按预期运行。

<!-- >[!NOTE]
>
>*If you do not mention any IPs under **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Publish Setup]** > **[!UICONTROL Image Server]** > **[!UICONTROL Test Image Service]*** - If you add an IP only, that IP is able to call the assets and no other IP are allowed to make the calls. As long there is no IP mentioned under that section, all IPs are allowed to make the calls for the assets, and they show up. -->

### 准备帐户

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>RB: Rewrote entire steps under “Prepare your account” 9/10/2012</p>

 -->

1. 请联系Adobe客户关怀团队，要求他们在您的帐户中启用安全测试。
1. 在Adobe Dynamic Media Classic的全局导航栏上，转到 **[!UICONTROL 设置]** > **[!UICONTROL 发布设置]** > **[!UICONTROL 图像服务器]**.
1. 在“图像服务器发布”页面上的 **[!UICONTROL 发布上下文]** 下拉列表中，选择 **[!UICONTROL 测试图像提供]**.
1. 对于客户端地址筛选器，选择 **[!UICONTROL 添加]**.
1. 选中此复选框以启用（打开）地址，然后在相应的文本字段中键入IP地址和网络掩码。

   >[!NOTE]
   >
   >如果您添加单个IP地址和网络掩码，则该地址可以发起资产调用。 但是，您添加的任何其他IP地址和网络掩码都不允许进行资产调用。 因此，请考虑禁用（关闭）上述步骤中的复选框，以关闭指定IP地址和网络掩码的功能。 这样做能够有效地 *全部* IP地址进行资产调用，所有这些IP地址都会显示。

1. 执行以下任一操作：
   * 如果必须添加更多IP地址，请重复上述两个步骤。
   * 继续下一步。
1. 在“图像服务器发布”页面的左下角，选择 **[!UICONTROL 保存]**
1. 将所需的图像上传到您的Adobe Dynamic Media Classic帐户。

   请参阅 [上传文件](uploading-files.md#uploading_files).

1. 请确保部分图像已标记为发布，而其它图像未标记，然后提交发布作业。

   请参阅 [发布文件](publishing-files.md#publishing_files).

1. 通过转到 **[!UICONTROL 设置]** > **[!UICONTROL 应用程序设置]** > **[!UICONTROL 常规设置]**.
1. 在“应用程序常规设置”页面上，在“服务器”组下，在“**[!UICONTROL 测试发布上下文服务器名称]**”右侧找到该名称。

如果服务器名称缺失或指向服务器的URL不起作用，请联系Adobe关怀。

### 准备网站变体

您需要两个网站变体，分别链接已发布和未发布的资源：

* 公共版本 — 使用传统的Adobe Dynamic Media Classic URL语法关联资产。
* 测试版本 — 使用相同语法但具有安全测试网站名称的资产链接。

### 运行测试

执行以下测试：

1. 检查是否可从公司网络内部访问资源。

   在由先前定义的IP地址范围标识的公司网络中，网站的暂存版本显示所有图像，无论是否标记为发布。 因此，在预览批准或产品发布之前，您无需意外地使图像可用，即可进行测试。

   确认网站的公共版本显示的是之前使用Adobe Dynamic Media Classic所体验的已发布资产。

1. 从公司网络外部，确认未发布的资源（即未标记为发布）受到保护，第三方无法访问。

   从外部（如从家庭计算机或通过 3G 连接）访问您的网络，然后确认站点的公开版本显示有所已发布的资源，但不显示未发布的内容。

   确认临时版本未显示任何资源，因为您正在从未获批准的 IP 地址访问安全测试服务。
