---
title: 发布设置
seo-title: 发布设置
description: 'null'
seo-description: 发布设置屏幕设置决定了默认情况下如何将资产从Dynamic Media经典服务器传送到网站或应用程序。
uuid: 196f25c8-abf5-4c5 d-8f6 f-bc70007 a0301
contentOwner: admin
content-type: 引用
products: SG_ EXPERIENCE MANAGER/Dynamic-Media-Scene-7
discoiquuid: cba59093-28b6-4490-b838-d942 b72 ad1 ec
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# 发布设置 {#publish-setup}

发布设置屏幕设置决定了默认情况下如何将资产从Dynamic Media经典服务器传送到网站或应用程序。如果未指定任何设置，Dynamic Media经典服务器将根据“发布设置”屏幕上的默认设置提供资产。例如，传送不含分辨率属性的图像的请求会以“图像服务器”屏幕上的“默认对象分辨率”设置生成图像。

管理员可以更改“图像服务器”、“图像渲染器”和“晕影”屏幕上的默认设置，以建立用于从服务器传送资源的默认设置。

要打开“发布设置”屏幕，请单击“设置”&gt;“应用程序设置”&gt;“发布设置”。

>[!NOTE]
>
>“发布设置”屏幕可供有经验的网站开发人员和程序员使用。动态媒体经典假定更改这些屏幕设置的用户熟悉Scene Publishing System、HTTP协议标准和惯例以及基本的图像技术。

## 图像服务器 {#image-server}

“图像服务器”屏幕建立用于从图像服务器传送图像的默认设置。设置分为五个类别（有关设置的详细说明，请参阅“图像服务器”屏幕）。

仅在Dynamic Media经典支持人员的协助下更改这些设置。

**目录管理** 这些设置决定Scene Publishing System和目录交互的方式。与大多数Web服务器不同，动态媒体图像服务器URL调用将转到清单或目录文件，而不是正确的图像文件。目录文件（不要与 eCatalog 混淆）中包含发布到图像服务器的所有内容的列表，以及每个图像的路径。如果您有 Digimarc ID，请在“Digimarc 用户信息”部分中输入您的用户信息。

**请求属性** 这些设置对可从服务器传送的图像施加限制。

**默认请求属性** 这些设置与图像的默认外观相关。

**常用缩略图属性** 这些设置与缩略图图象的默认外观和对齐方式相关。

**目录字段默认值** 这些设置与图像的分辨率和默认缩略图类型相关。

**颜色管理属性** 这些设置确定使用的ICC颜色配置文件。

**兼容性属性** 此设置允许文本层中的前导和尾部段落像在版本3.6中一样对待，以向后兼容性。

**本地化支持** 这些设置允许您管理多个区域设置属性。它还允许您指定区域设置映射字符串，以便定义查看器中的各种工具提示所需的支持语言。

例如，如果您的品牌在多个不同国家/地区销售，您可以确保每个国家/地区都有自己特定区域设置的查看器。要实现该功能，请指定区域设置映射字符串。然后，在查看器预设中编辑工具提示文本，添加所需语言的翻译文本字符串。

>[!NOTE]
> 要设置“本地化支持”选项，请与Adobe Dynamic Media经典技术支持部门联系，或发送电子邮件至s7support@adobe.com请求设置帮助。

有关设置“**本地化支持**”的更多信息，请参阅[设置资源本地化时的注意事项](publish-setup.md#considerations_when_setting_up_localization_of_assets)。

### 设置资源本地化时的注意事项 {#considerations-when-setting-up-localization-of-assets}

>[!NOTE]
>
>如果要在Scene Publishing System(如“区域设置映射”字段)中设置“本地化支持”选项，请与Adobe Dynamic Media经典技术支持联系。或者，向 s7support@adobe.com 发送电子邮件寻求设置帮助。

Scene7 Publishing System (SPS) 的一种常见用法是管理电子商务网站上的产品图像。国际企业面临如下挑战：类似产品的资源在各个国家/地区之间存在一些差异。通常，这些差异仅出现在整体媒体的极少部分。通过复制每个国家/地区的所有资源，并仅覆盖其中的差异可以处理此类差异，但这项工作非常艰巨，而且可能会使单个主要资源发生冲突。从包含不同音轨的国家/地区特定视频，到产品所用电源线的细微但重要的差异，此类资源差异可能会持续存在。动态媒体经典使用基本的查找机制。您可以从所需的区域设置开始，定义图像服务器查找资源后缀的顺序。

**如何本地化资源**

IS（图像服务）请求的区域设置通过以下 IS/IR（图像渲染）命令来识别：

`locale=`

此命令接受区域设置 ID (locId) 字符串，不区分大小写。区域设置 ID 通常是由 2-6 个字母和“_”组成的字符串。

IS supports arbitrary printable ASCII strings.The `locale=` command has a global scope, meaning that it is applied to the entire request, including all nested IS and IR requests, referenced templates, and image layers. 不支持每个请求应用多个区域设置，如每个图层应用不同的区域设置。但是，允许在嵌套的请求中显式覆盖区域设置。

If `locale=` is not specified, `attribute::DefaultLocale` is passed to the translation engines. Limited input validation is applied to the `locale=` value. Empty `locale=` values are permitted. Because `locale=` has a global scope, `attribute::DefaultLocale` is provided by the main catalog for the entire request.

Some of the benefits of using `locale=` and `attribute::DefaultLocale` include the following:

* 针对多个区域设置共享内容。
* 使用通用 ID 访问区域设置特定的内容。
* 在区域设置特定内容的命名约定和管理方面具有相当大的灵活性，如区域设置前缀与后缀或单独目录中的区域设置特定内容。
* 支持直接访问区域设置特定的版本。
* 复合对象（如图像集）可以包含对区域设置特定的潜在内容的泛型引用。
* 支持目录管理的可能需要本地化的所有内容，包括图像、图像集、晕影、材料和查看器配置记录。
* 最大程度地减少对 IPS 数据库和 IS 清单机制的更改。
* 实施 RFC IS-63 时，将添加对静态内容（如视频和外观）的支持。
* 默认区域设置是可配置的。

**应用程序方案**

| 应用程序 | 方案 |
|--- |--- |
| 查看器本地化 | 在实施静态内容目录后，本地化可完全通过 locale= 参数控制，该参数会附加到对 IS 的所有请求后面。配置记录、外观和启动画面等可以具有区域设置特定的变量，也可以没有。正确内容由 IS 提供，查看器无需知道哪些内容进行了本地化以及其 ID 是什么。 |
| 图像和视频 | 跨国公司通常同时拥有通用内容和区域设置特定的内容。通过这种机制，对图像或视频的引用可以是泛型引用，并且 IS 会提供区域设置特定的内容（如果可用）。 |
| 图像集和媒体集 | 某些区域设置的整个图像集可能有所不同—如当eCatalog完全不同时—将从通用到特定于区域设置的图像集的翻译转换为查看器处理的特定于区域设置的图像集。更常见的是，通用的ID中的单个ID可能引用本地化的内容。例如，某设备的大部分照片在所有语言中都是相同的，但控制面板的照片除外。IS 会自动转换 ID，因此无需生成区域设置特定的图像集。 |

**实施资源本地化**

Scene7 发布和图像服务的界面允许对图像和静态内容进行本地化。

当没有本地化版本时，图像服务器 URL 如下所示：

`https://server/is/image/company/image`

With localization, an Image Server URL adds the `locale=` parameter to the path, as in the following:

`https://server/is/image/company/image?locale=de_DE`

On receipt of the http call by the Image Server, the `locale=` parameter is parsed through the localeMap field found in **Setup** &gt; **Application Setup** &gt; **Publish Setup** &gt; **Image Server** &gt; **Localization Support** group.

“区域设置映射”字段包含一个用管道符号 (|) 分隔的条目列表。

每个条目由一个以逗号分隔的值列表组成。The first value is the search value that is passed by the `locale=` parameter. 其余的值为后缀/替换值，随后将尝试搜索这些值，直到找到现有图像为止。

具体应用后缀值还是应用替换值，取决于“**设置**”&gt;“**应用程序设置**”&gt;“**发布设置**”&gt;“**图像服务器**”&gt;“**本地化支持**”组中的“全局区域设置”。

>[!NOTE]
>
>“全局区域设置”目前只能通过 API 进行设置，而无法在 Scene7 Publishing System 界面中设置。

**后缀示例**

| URL | localeMap ID | 结果 |
|--- |--- |--- |
| `https://server/is/image/company/image?locale=de_DE` | `de_DE,_DE,|fr_FR,_FR,` | 请注意，这里没有定义 GlobalLocale。区域设置参数 de_DE 与 localeMap 中的第一个条目匹配。第一个对应值 _DE 将添加为资源 image_DE 的后缀，并尝试在图像服务器上查找该资源。如果在服务器上找到该资源，则会将其返回。否则，使用第二个值“”作为后缀，返回图像本身。 |

**替换示例**

| URL | GlobalLocale 和 localeMap ID | 结果 |
|--- |--- |--- |
| `https://server/is/image/company/image-main-01?locale=de_DE` | `GlobalLocale=mainlocaleMap -` <br><br/> `de_DE,de,main|fr_FR,fr,main` | 在以上替换示例中，GlobalLocale 被设置为 main。区域设置参数 de_DE 与 localeMap 中的第一个条目匹配。将查找 GlobalLocale 子字符串，并将其替换为 localeMap 中的第一个对应值 de：image-de-01。如果在图像服务器上找到，则会将其返回。否则，替换第二个值，最终生成 image-main-01。 |

如果 URL 中没有定义区域设置，则图像服务器会采用 DefaultLocale（如果定义）并将其应用到 URL。

If an unknown or empty locale parameter is supplied with `locale=`, then the localeMap is scanned for the empty value “starting with,”. 请务必将此配置为对未知区域设置应用默认区域设置，这一点非常重要。

**关于 defaultImage**

图像服务器会为请求的区域设置逐个试用选项。如果找不到匹配项，则会对 defaultImage 应用区域设置选项，并返回匹配版本。因此，每个区域设置都应包含一个针对未本地化图像的选项，或者应在 Scene7 Publishing System 中提供本地化的 defaultImage 版本。

**用于查找 localeMap 的方案**

假定您要支持以下区域设置：

`en, en_us, en_uk, de, de_at, de_de, fr`

You map these locales to the suffixes `_E`, `_G`, and `_F`, for English, German, and French, respectively. 对于所有示例，通用输入图像 ID 为 `myImg`。

*用于查找 localeMap 的标准行为*

区域设置 ID 会被映射到其对应的后缀。如果在目录中找不到区域设置特定的 ID，则尝试使用通用 ID。请注意映射到通用 ID 的空 locSuffix 值。

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,`

| locale= | 要搜索的输出 ID |
|--- |--- |
| en,en_us, en_uk | myImg_E,myImg |
| de,de_de,de_at | myImg_D,myImg |
| fr | myImg_F,myImg |
| 所有其他区域设置 | - |

*区域设置未知时查找 localeMap*

您可以将未知的区域设置映射到特定 ID 或通用 ID。对于我们的示例，可以将未知区域设置映射到英语 ID，或者，如果英语 ID 不存在，则映射到通用 ID。

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,|,_E,`

| locale= | 要搜索的输出 ID |
|--- |--- |
| de,de_de,de_at | myImg_D,myImg |
| fr | myImg_F,myImg |
| 所有其他区域设置 | myImg_E,myImg |

You could also have a dedicated locSuffix, such as U, just for unknown locales, and force to the default image if no `_U` exists, as in the following:

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,|,U`

或者，可以直接映射到通用 ID，如下所示：

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,|,`

*使用多层查找来找到 localeMap*

通常，最好对区域设置（如欧洲、中东和北美）进行分组以应对区域标准，如外观曝光。可以使用多层查找来实现这种效果。

对于本示例，假定您要支持供西方和中东使用的集合。这两个集合都基于通用图像集合，而且都添加或修改某些图像。Both collections are then further refined for specific locales, such as `m1, m2` for two middle-eastern variants, and `w1, w2,` and `w3` for three Western locales, except that images are shared for `w1` and `w3`. 未知区域设置仅映射到通用集合，而且无法访问区域设置特定的图像。该映射如下所示：

`attribute::LocaleMap=w1,-W,|w2,-W2,-W,|w3,-W,|m1,-M1,-M,|m2,-M2,-M,|,`

| locale= | 要搜索的输出 ID |
|--- |--- |
| w1, w3 | myImg-W, myImg |
| w2 | myImg-W2, myImg-W, myImg |
| m1 | myImg-M1, myImg-M, myImg |
| m2 | myImg-M2, myImg-M, myImg |
| 所有其他区域设置 | mylmg |

*通过搜索特定 ID 查找 localeMap*

有些图像命名约定可能不支持通用图像 ID。必须将请求中的通用 ID 映射到目录中的特定 ID。但是，可能存在确切的特定 ID 未知的情况。

Using the first example as a basis, images for all languages may have the suffixes `_1`, `_2`, or `_3`. Images that are specific to French locales may have the suffixes `_22` or `_23` suffix. And images that are specific to German locales may have the suffixes `_470` or `_480`.

`attribute::LocaleMap=,_1,_2,_3|fr,_22,_23,_1,_2,_3|de,_470,_480,_1,_2,_3|de_at,_470,_480,_1,_2,_3|de_de,_470,_480,_1,_2,_3`

| locale= | 要搜索的输出 ID |
|--- |--- |
| fr | myImg_22, myImg_23, myImg_1, myImg_2, myImg_3 |
| de, de_at, de_de | myImg_470, myImg_480, myImg_1, myImg_2,myImg_3 |
| 所有其他区域设置 | myImg_1, myImg_2, myImg_3 |

**实施本地化支持时的重要注意事项**

* 本地化仅限基于 ID 的资源调用，无法用于基于路径的资源调用。因此，在调用具有区域设置的视频时，必须以 company/assetID 的形式调用，而不采用视频的完整路径。这意味着无法使用本地化的 rtmp，因为该方法仅用于基于路径的视频调用。
* 当 localeMap 处于活动状态时，无法使用包含单个视频的“混合媒体集”，否则对媒体集内容的调用会失败。要解决此问题，可以将单个视频添加到自适应视频集。然后，将自适应视频集添加到混合媒体集。
* 某些请求没有本地化，例如针对自适应视频集内容的请求。因此，如果要使用本地化的自适应视频集，则应将自适应视频集放置在混合媒体集中。Then, call the set into a Mixed Media viewer with the `locale=` parameter.

## 图像渲染器 {#image-renderer}

“图像渲染器”屏幕建立用于从图像渲染服务器传送图像集的默认设置。设置分为五个类别（有关设置的详细说明，请参阅“图像服务器”屏幕）：

**目录管理** 这些设置决定Scene Publishing System和目录文件交互的方式。对目录发出Dynamic Media Classic渲染服务器URL调用，该目录依次调用从服务器传送图像。仅在Dynamic Media经典支持人员的协助下更改这些设置。

**会话属性** 这些设置建立错误参数、相对图像URL的URL以及是否允许对象重叠。

**默认材质属性** 这些设置为图像建立默认分辨率和锐化设置。

**响应图像属性** 这些设置与图像的默认外观相关。

**颜色管理属性** 这些设置与图像的默认颜色设置相关。

## 晕影 {#vignette}

“晕影”屏幕提供了用于确定晕影的默认外观的设置（有关选项的详细说明，请参阅屏幕本身）。