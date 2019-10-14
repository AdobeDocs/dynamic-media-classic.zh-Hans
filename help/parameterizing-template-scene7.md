---
title: 在Dynamic Media Classic中参数化模板
seo-title: 在Dynamic Media Classic中参数化模板
description: 'null'
seo-description: 了解如何在Dynamic Media Classic中参数化模板
uuid: 27c8c8b4-47f3-4270-a6db-d304648ba357
contentOwner: admin
content-type: 引用
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEEVENTONDEMAND_PK/categories/template-publishing
discoiquuid: df1a9ff5-a5ba-4480-ba0d-a19bc665f907
translation-type: tm+mt
source-git-commit: 6fff3699f8a08af433df3f3a7790a11bf9d05b00

---


# 在Dynamic Media Classic中参数化模板{#parameterizing-a-template-in-scene}

在将另存为Dynamic Media Classic FXG的Illustrator模板上传到Scene7 Publishing system后，可以定义其变量元素。 通过在“模板发布构建和预览”屏幕中参数化变量元素执行此操作。Dynamic Media Classic提供了用于定义图层及其相应属性上的文本和对象参数的工具。 您还可以创建模板的不同版本。

参数化 FXG 模板后，即可在模板中自定义文本、图像和图形的可变性。例如，您可以参数化一行文本，以便最终用户可以通过 Web 用户界面修改该文本。您可以将空文本字段定义为变量，以便最终用户可以在这些字段中填充个性化文本。您还可以在“Dynamic Media Classic模板发布构建”屏幕中参数化设计元素的属性和属性。

>[!NOTE]
>
>如果您计划使用DOM操作，则无需在Dynamic Media Classic中参数化模板。

## 定义 FXG 模板中的参数 {#defining-parameters-in-fxg-templates}

按照Dynamic Media Classic中的以下步骤为FXG模板定义参数：

1. 在“浏览”窗口中，选择 FXG 文件。
1. Click **Build** and choose **Template Publishing**, or click the file’s **Edit** button.

   随即打开“模板发布”屏幕。

1. 选择LRCo\FXG\Welcome_Summit_10 （FXG文件），然后单击“ **构建** ”&gt;“ **模板发布”**。</p>

   ![](assets/wp_fxg_edit.png)

1. 在“模板发布”屏幕的“图层”面板中，选择包含要参数化的元素的图层。

   >[!NOTE]
   >
   >连续单击眼睛图标，确保您选择了正确的对象。

1. 在“属性”面板中，单击“名称”列（用于参数化文本）或“参数”列（用于参数化对象）中的参数。

   * **文本**&#x200B;在文本字段中单击（滚动到“属性”列表的底部以查找它）。 此时会出现“参数”对话框。Select the text that you want to parameterize and click **Add**. 您可以通过选择该文本的不同部分并为每个部分添加参数，从同一文本属性创建多个参数。To change the name of the parameter, click it, enter a new name, and click **Close**.

   * **对象**&#x200B;单击“参数”列中的框。 此时会出现“编辑参数”对话框。Enter a name and click **OK**.
   要使用相同值一次自定义多个属性，请对每个属性使用相同的参数名称。例如，如果您的模板包含一个矩形和一个星形，您可以键入 `newcolor` 作为每项的“纯色”颜色属性的参数名称。每当您更改 `newcolor` 值时，矩形和星形就会变为新的颜色。

1. 在“值”或“数据”字段中指定该属性的默认值。设置所选对象的所有属性，以指定所需的外观。
1. （可选）对要参数化的所有对象或图层重复步骤 3 - 5。
1. 单击“**保存**”或“**另存为**”。
1. Click **Preview** to open the FXG Preview window and see the parameters you created with their default values.

## 在 FXG 模板中显示或隐藏对象或图层 {#show-or-hide-an-object-or-layer-in-the-fxg-template}

隐藏的对象和图层不会显示在预览或输出中，但这并不是从文件中删除。您可以根据需要使其再次可见。可见性是一种可以成为变量的属性。连续单击眼睛图标会为对象或图层的可见性设置默认值。

1. 在“对象”面板中，单击对象或图层名称旁边的眼睛图标，以将其隐藏在文件中。
1. 再单击一次，使该对象可见。

## 创建模板的不同版本 {#create-different-versions-of-a-template}

您可以编辑属性以针对不同用途创建模板的不同版本。

在“模板发布”屏幕中，单击“另存为”将该文件保存为新的 FXG 模板，而不覆盖原始 FXG 模板。

## 使用描边文本 {#using-stroked-text}

描边文本就是如何对属性进行参数化的一个示例。Dynamic Media Classic支持以下描边文本功能：

* 描边宽度
* 虚线描边图案
* 不同结点样式
* 不同端点样式
* 描边叠印
* 单独对描边进行颜色处理，包括专色支持

下表描述支持描边文本的属性。

| 属性 | 说明 |
|--- |--- |
| s7:fill `<Boolean>`(S7FXG Only) | 指定是否为文本启用填充。默认为 true。 |
| s7:stroke `<Boolean>` (S7FXG Only) | 指定是否为文本启用描边。默认值为 false。 |
| s7:weight `<number>` (S7FXG Only) | 以磅为单位指定文本的描边粗细。默认值为 1 磅。 |
| s7:joints `<string>` (miter, round, bevel) (S7FXG Only) | 指定描边的连接类型。默认值为 round。 |
| s7:caps `<string>` (none, round, square) (S7FXG Only) | 指定描边的端类型。默认值为 round。 |
| s7:miterLimit `<number>` (S7FXG Only) | 指定当连接为描边斜接连接时的斜接限制。默认值为 4。 |
| s7:strokeOverprint `<Boolean>` (S7FXG Only) | 指定是否为描边启用叠印。默认值为 false。 |
| s7:strokeColorName（仅限 S7FXG） | 与 s7:colorName 相同，但是它定义描边的颜色名称。 |
| s7:strokeColorValue（仅限 S7FXG） | 与 s7:colorValue 相同，但是它定义描边所用的颜色值。 |
| s7:strokeColorspace（仅限 S7FXG） | 与 s7:colorspace 相同，但是它定义描边的颜色空间。 |
| flm:dashPattern `<array>` (S7FXG Only) | 默认情况下，没有虚线和间隙图案。该属性定义描边的虚线/间隙图案。第一个值是描边的虚线。第二个值是虚线之间的间隙。您可以同样的方式使用指定为虚线和间隙的替代值扩展多个值的数组。 |

## 使用弯曲文本 {#using-warped-text}

利用弯曲文本，可以修改带有波浪、旗帜、拉伸等效果的文字的外观。

富文本对象支持弯曲文本。文本可以是垂直或水平文本，也可以是点文本、区域文本和路径文本。必须先选择整个文本对象，然后才能应用弯曲文本。

可以在 Adobe Illustrator 中创建弯曲文本。

在弯曲文本时，您可以设置以下属性：

* 样式
* 方向
* 弯曲
* 水平扭曲
* 垂直扭曲

每个属性各包含一组值。

| 属性 | 值 | 默认 |
|--- |--- |--- |
| 样式7:warpStyle | nonearcarcLowerarcUpperarchbulgeshellLowershellUpperflagwavefishrisefishEyeinflatesqueezetwist | 无 |
| Directions7:warpDirection | horizontalvertical | 水平 |
| Bends7:warpBend | -1 到 1 | 0.5 |
| 水平扭曲7:warpHorizontalDistortion | -1 到 1 | 0 |
| 垂直扭曲7:warpVerticalDistortion | -1 到 1 | 0 |

>[!NOTE]
>
>For `inflate` and `fishEye`, changing the `s7:warpDirection` flag between horizontal and vertical does not have any effect on the output.

有关创建和使用弯曲文本的更多信息，请参阅 Adobe Illustrator 文档。

>[!MORELIKETHIS]
>
>* [在 Illustrator 中创建初始模板](create-initial-template-illustrator.md#create_the_initial_template_in_illustrator)
>* [Upload files for Template Publishing](upload-files-template-publishing.md#upload_files_for_template-publishing)

