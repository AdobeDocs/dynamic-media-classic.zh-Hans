---
title: 发布设置
description: 通过“发布”设置设置，可决定默认情况下如何将资源从Adobe Dynamic Media Classic服务器传递到网站或应用程序。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic
role: Admin
exl-id: 699d4c12-e47b-4c6b-86f3-dc7aaaa56c1e
topic: Administration, Content Management
level: Intermediate
source-git-commit: 51c05c62448b39a75facb2e90cc9da5d0f26ab45
workflow-type: tm+mt
source-wordcount: '2408'
ht-degree: 41%

---

# 发布设置 {#publish-setup}

“发布设置”页面设置可确定默认情况下，如何将资源从Adobe Dynamic Media Classic服务器传递到网站或应用程序。 如果未指定设置，则Adobe Dynamic Media Classic服务器会根据发布设置页面上的默认设置交付资源。 例如，发送不包含分辨率属性的图像的请求会生成一个图像，该图像具有“图像服务器”页面上的“默认对象分辨率”设置。

管理员可以更改图像服务器、图像渲染器和晕影页面上的默认设置，以便建立用于从服务器交付资产的默认设置。

要打开“发布设置”页面，请转到 **[!UICONTROL 设置]** > **[!UICONTROL 应用程序设置]** > **[!UICONTROL 发布设置]**.

>[!NOTE]
>
>发布设置页面可供经验丰富的网站开发人员和程序员使用。 Adobe Dynamic Media Classic假定在这些页面上更改设置的用户熟悉Adobe Dynamic Media Classic、HTTP协议标准和惯例，以及基本成像技术。

## 图像服务器 {#image-server}

“映像服务器”页建立了从映像服务器传送映像的默认设置。 设置位于这五个类别中（有关设置的详细说明，请参阅“图像服务器”页面）。

仅在Adobe Dynamic Media Classic支持人员的协助下更改这些设置。

* **[!UICONTROL 目录管理]**  — 这些设置确定Adobe Dynamic Media Classic和目录的交互方式。 与大多数Web服务器不同，Dynamic Media图像服务器URL调用转到清单或目录文件，而不是真正的图像文件。 目录文件（不要与 eCatalog 混淆）中包含发布到图像服务器的所有内容的列表，以及每个图像的路径。如果您有 Digimarc ID，请在“Digimarc 用户信息”部分中输入您的用户信息。

* **[!UICONTROL 请求属性]**  — 这些设置对可以从服务器传送的图像施加限制。 例如， *最大值* **[!UICONTROL 回复图像大小限制]** 是 **[!UICONTROL 宽度]** 5000和 **[!UICONTROL 高度]** 5000

* **[!UICONTROL 默认请求属性]**  — 这些设置与图像的默认外观相关。

* **[!UICONTROL 常用缩略图属性]**  — 这些设置与缩略图图像的默认外观和对齐有关。

* **[!UICONTROL 目录字段的默认值]**  — 这些设置与图像的分辨率和默认缩略图类型有关。

* **[!UICONTROL 颜色管理属性]**  — 这些设置确定使用哪些ICC颜色配置文件。

* **[!UICONTROL 兼容性属性]**  — 此设置允许将文本图层中的前导段落和尾随段落视为版本3.6中的前导段落和尾随段落，以便向后兼容。

* **[!UICONTROL 本地化支持]*** — 这些设置允许您管理多个区域设置属性。 它还允许您指定区域设置映射字符串，以便定义查看器中的各种工具提示所需的支持语言。

  例如，如果您的品牌在多个不同国家/地区销售，您可以确保每个国家/地区都有自己特定区域设置的查看器。要实现该功能，请指定区域设置映射字符串。然后，通过添加所需语言的翻译文本字符串在查看器预设中编辑工具提示文本。

  >[!NOTE]
  > 要设置本地化支持选项， [使用Admin Console创建支持案例。](https://helpx.adobe.com/enterprise/using/support-for-experience-cloud.html) 在您的支持案例中，请求设置帮助。

  有关设置“**[!UICONTROL 本地化支持]**”的更多信息，请参阅[设置资源本地化时的注意事项](publish-setup.md#considerations_when_setting_up_localization_of_assets)。

### 设置资源本地化时的注意事项 {#considerations-when-setting-up-localization-of-assets}

>[!NOTE]
>
>如果要在Adobe Dynamic Media Classic中设置本地化支持选项，如“区域设置映射”字段， [使用Admin Console创建支持案例。](https://helpx.adobe.com/enterprise/using/support-for-experience-cloud.html) 在您的支持案例中，请求设置帮助。

使用Adobe Dynamic Media Classic的常见方法是管理电子商务网站上的产品图像。 国际企业面临如下挑战：类似产品的资源在各个国家/地区之间存在一些差异。通常，差异在于整个媒体的几个部分。 通过复制每个国家的所有资产并仅覆盖这些差异来解决这些差异是一项巨大的努力，并且与单一的主要资产隐喻相矛盾。 从包含不同音轨的国家/地区特定视频，到产品所用电源线的细微但重要的差异，此类资源差异可能会持续存在。Adobe Dynamic Media Classic使用基本的查找机制。 您可以从所需的区域设置开始，定义图像服务器查找资源后缀的顺序。

#### 如何本地化资源

IS（图像服务）请求的区域设置通过以下 IS/IR（图像渲染）命令来识别：

`locale=`

此命令接受区域设置 ID (locId) 字符串，不区分大小写。区域设置ID通常是由字母和“_”组成的2-6字符串。

IS支持任意可打印的ASCII字符串。 此 `locale=` 命令具有全局范围，这意味着它适用于整个请求，包括所有嵌套的IS和IR请求、引用的模板以及图像图层。 不支持每个请求应用多个区域设置，如每个图层应用不同的区域设置。但是，允许在嵌套的请求中显式覆盖区域设置。

如果 `locale=` 未指定， `attribute::DefaultLocale` 传递给翻译引擎。 有限输入验证应用于 `locale=` 值。 空 `locale=` 值是允许的。 因为 `locale=` 具有全局范围， `attribute::DefaultLocale` 由主目录为整个请求提供。

使用的一些好处 `locale=` 和 `attribute::DefaultLocale` 包括以下内容：

* 针对多个区域设置共享内容。
* 使用通用 ID 访问区域设置特定的内容。
* 在区域设置特定内容的命名约定和管理方面具有相当大的灵活性，如区域设置前缀与后缀或单独目录中的区域设置特定内容。
* 支持访问特定于区域设置的版本。
* 聚合对象（如图像集）有时可以包含对可能特定于区域设置的内容的通用引用。
* 支持由需要本地化的目录管理的所有内容，包括图像、图像集、晕影、材料和查看器配置记录。
* 最大程度地减少对 IPS 数据库和 IS 清单机制的更改。
* 在实施RFC IS-63时，添加了对静态内容（如视频和外观）的支持。
* 默认区域设置是可配置的。

#### 应用程序方案

| 应用程序 | 方案 |
| --- | --- |
| 查看器本地化 | 在实施静态内容目录后，本地化可完全通过 locale= 参数控制，该参数会附加到对 IS 的所有请求后面。配置记录、外观和启动画面等可以具有区域设置特定的变量，也可以没有。正确内容由 IS 提供，查看器无需知道哪些内容进行了本地化以及其 ID 是什么。 |
| 图像和视频 | 跨国公司通常同时拥有通用内容和区域设置特定的内容。通过这种机制，对图像或视频的引用可以是泛型引用，并且 IS 会提供区域设置特定的内容（如果可用）。 |
| 图像集和媒体集 | 对于某些区域设置（例如当eCatalog不同时），整个图像集可以不同，即从通用图像集转换为由查看器处理的特定于区域设置的图像集。 更常见的是，通用集中的单个ID可以引用本地化的内容。 例如，除控制面板照片外，设备的大多数照片在所有语言中都可能相同。 IS 会自动转换 ID，因此无需生成区域设置特定的图像集。 |

#### 实施资产本地化

Adobe Dynamic Media Classic和图像服务具有允许本地化的图像和静态内容的界面。

当没有本地化版本时，图像服务器 URL 如下所示：

`https://server/is/image/company/image`

在本地化过程中，图像服务器URL会添加 `locale=` 参数到路径，如下所示：

`https://server/is/image/company/image?locale=de_DE`

当图像服务器收到http调用时， `locale=` 参数是通过 `localeMap` 在以下位置找到字段： **[!UICONTROL 设置]** > **[!UICONTROL 应用程序设置]** > **[!UICONTROL 发布设置]** > **[!UICONTROL 图像服务器]** > **[!UICONTROL 本地化支持]** 组。

“区域设置映射”字段包含一个用管道符号 (|) 分隔的条目列表。

每个条目由一个以逗号分隔的值列表组成。第一个值是由传递的搜索值 `locale=` 参数。 其余值是后缀/替换值，然后尝试这些值，直到产生现有图像为止。

具体应用后缀值还是应用替换值，取决于“**[!UICONTROL 设置]**”>“**[!UICONTROL 应用程序设置]**”>“**[!UICONTROL 发布设置]**”>“**[!UICONTROL 图像服务器]**”>“**[!UICONTROL 本地化支持]**”组中的“全局区域设置”。

>[!NOTE]
>
>“全局区域设置”设置只有在您通过API进行设置时才可用，不能在Adobe Dynamic Media Classic界面中进行设置。

**后缀示例:**

| URL | localeMap ID | 结果 |
| --- | --- | --- |
| `https://server/is/image/company/image?locale=de_DE` | `de_DE,_DE,|fr_FR,_FR,` | 请注意，这里没有定义 GlobalLocale。区域设置参数de_DE与 `localeMap`. 第一个对应值 _DE 将添加为资源 image_DE 的后缀，并尝试在图像服务器上查找该资源。如果在服务器上找到该资源，则会将其返回。否则，第二个值“”将用作后缀，从而导致图像本身被返回。 |

**替换示例:**

| URL | `GlobalLocale` 和 `localeMap` ID | 结果 |
|--- |--- |--- |
| `https://server/is/image/company/image-main-01?locale=de_DE` | `GlobalLocale=mainlocaleMap -` <br><br/> `de_DE,de,main|fr_FR,fr,main` | 在以上替换示例中，GlobalLocale 被设置为 main。区域设置参数de_DE与 `localeMap`. 找到GlobalLocale子字符串并将其替换为第一个相应值 `de` 在 `localeMap`： `image-de-01`. 如果在图像服务器上找到，则会将其返回。否则，替换第二个值，最终生成 `image-main-01`。 |

如果 URL 中没有定义区域设置，则图像服务器会采用 DefaultLocale（如果定义）并将其应用到 URL。

如果提供了未知或空的区域设置参数 `locale=`，然后 `localeMap` 将扫描空值“starting with”。 为未知区域设置应用默认区域设置很重要。

#### 关于默认图像

图像服务器会为请求的区域设置逐个试用选项。如果未找到匹配项，则区域设置选项将应用于defaultImage，并返回匹配的版本。 因此，每个区域设置都必须包含一个未进行本地化的图像选项，或者本地化的defaultImage版本在Adobe Dynamic Media Classic中可用。

#### 用于查找 localeMap 的方案

假定您要支持以下区域设置：

`en, en_us, en_uk, de, de_at, de_de, fr`

将这些区域设置映射到后缀 `_E`， `_G`、和 `_F`，分别表示英语、德语和法语。 对于所有示例，通用输入图像 ID 为 `myImg`。

##### 用于查找 localeMap 的标准行为

区域设置 ID 会被映射到其对应的后缀。如果在目录中找不到区域设置特定的 ID，则尝试使用通用 ID。请注意映射到通用 ID 的空 locSuffix 值。

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,`

| locale= | 要搜索的输出 ID |
| --- | --- |
| en,en_us, en_uk | myImg_E,myImg |
| de,de_de,de_at | myImg_D,myImg |
| fr | myImg_F,myImg |
| 所有其他区域设置 | - |

##### 区域设置未知时查找 localeMap

您可以将未知的区域设置映射到特定 ID 或通用 ID。例如，您可以将未知的区域设置映射到英文ID，如果没有未知的区域设置，则映射到通用ID。

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,|,_E,`

| locale= | 要搜索的输出 ID |
| --- | --- |
| de,de_de,de_at | myImg_D,myImg |
| fr | myImg_F,myImg |
| 所有其他区域设置 | myImg_E,myImg |

您还可以具有专用的locSuffix，例如U，以用于未知区域设置，如果没有，则强制使用默认图像 `_U` 存在，如下所示：

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,|,U`

或者，可以直接映射到通用 ID，如下所示：

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,|,`

##### 使用多层查找查找查找区域设置映射

通常，最好对区域设置（如欧洲、中东和北美）进行分组以应对区域标准，如外观曝光。可以使用多层查找来实现这种效果。

对于本示例，假定您要支持供西方和中东使用的集合。这两个集合都基于通用图像集合，而且都添加或修改某些图像。然后，针对特定的区域设置，进一步优化这两个收藏集，例如 `m1, m2` 两个中东变体的，以及 `w1, w2,` 和 `w3` 三种西式区域设置，但图像共享用于 `w1` 和 `w3`. 未知区域设置仅映射到通用集合，而且无法访问区域设置特定的图像。该映射如下所示：

`attribute::LocaleMap=w1,-W,|w2,-W2,-W,|w3,-W,|m1,-M1,-M,|m2,-M2,-M,|,`

| locale= | 要搜索的输出 ID |
| --- | --- |
| w1, w3 | myImg-W, myImg |
| w2 | myImg-W2, myImg-W, myImg |
| m1 | myImg-M1, myImg-M, myImg |
| m2 | myImg-M2, myImg-M, myImg |
| 所有其他区域设置 | mylmg |

##### 通过搜索特定的ID来查找区域设置映射

某些图像命名约定不支持通用图像ID。 必须将请求中的通用 ID 映射到目录中的特定 ID。但是，在某些情况下，确切的特定ID未知。

以第一个示例为基础，所有语言的图像都可以有后缀 `_1`， `_2`，或 `_3`. 特定于法语区域设置的图像可以具有后缀 `_22` 或 `_23` 后缀。 而特定于德国区域设置的图像可以具有后缀 `_470` 或 `_480`.

`attribute::LocaleMap=,_1,_2,_3|fr,_22,_23,_1,_2,_3|de,_470,_480,_1,_2,_3|de_at,_470,_480,_1,_2,_3|de_de,_470,_480,_1,_2,_3`

| locale= | 要搜索的输出 ID |
| --- | --- |
| fr | myImg_22, myImg_23, myImg_1, myImg_2, myImg_3 |
| de, de_at, de_de | myImg_470, myImg_480, myImg_1, myImg_2,myImg_3 |
| 所有其他区域设置 | myImg_1, myImg_2, myImg_3 |

##### 实施本地化支持时的重要注意事项

* 本地化仅限基于 ID 的资源调用，无法用于基于路径的资源调用。因此，在调用具有区域设置的视频时，必须以 company/assetID 的形式调用，而不采用视频的完整路径。您不能将rtmp与本地化一起使用，因为此方法仅用于基于路径的视频调用。
* 当 localeMap 处于活动状态时，无法使用包含单个视频的“混合媒体集”，否则对媒体集内容的调用会失败。要解决此问题，可以将单个视频添加到自适应视频集。 然后，将自适应视频集添加到混合媒体集。
* 某些请求没有本地化，例如针对自适应视频集内容的请求。因此，如果您打算将自适应视频集与本地化一起使用，请将自适应视频集放置在混合媒体集中。 然后，使用将集调入混合媒体查看器 `locale=` 参数。

## 图像渲染器 {#image-renderer}

“图像渲染器”页面建立了从图像渲染服务器交付图像集的默认设置。 有以下五种类别的设置可用（有关这些设置的详细说明，请参阅“图像服务器”页）：

* **[!UICONTROL 目录管理]**  — 这些设置确定Adobe Dynamic Media Classic和目录文件如何交互。 Adobe Dynamic Media Classic渲染服务器URL调用会发送到目录，然后目录会调用从服务器传送图像。 仅在Adobe Dynamic Media Classic支持人员的协助下更改这些设置。

* **[!UICONTROL 会话属性]**  — 这些设置可建立错误参数、相对图像URL的URL以及是否允许对象重叠。

* **[!UICONTROL 默认材质属性]**  — 这些设置建立图像的默认分辨率和锐化设置。

* **[!UICONTROL 响应图像属性]**  — 这些设置与图像的默认外观相关。

* **[!UICONTROL 颜色管理属性]**  — 这些设置与图像的默认颜色设置相关。

## 晕影 {#vignette}

“晕影”页提供了用于建立晕影默认外观的设置（有关选项的详细说明，请参阅页面本身）。
