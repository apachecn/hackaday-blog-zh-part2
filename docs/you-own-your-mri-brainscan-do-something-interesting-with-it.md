# 你拥有你的核磁共振脑扫描；用它做一些有趣的事情

> 原文：<https://hackaday.com/2015/08/25/you-own-your-mri-brainscan-do-something-interesting-with-it/>

你将拥有的最复杂、最迷人的小玩意是你的大脑。为什么不通过创建一个可以自己打印的 3D 比例模型来向这一奇迹致敬呢？如果你有一个全头部磁共振扫描，很容易获得这些数据，并创建一个三维模型，你可以打印出任何三维打印机。以下是如何打印你的大脑。

首先，你需要做核磁共振扫描。不幸的是，【彼得·詹森】正在研究的 [低场磁共振成像](https://hackaday.io/project/5030-low-field-mri) (还)不太管用:你必须让专业人士来做。扫描的类型也很重要，因为我们希望扫描聚焦于大脑本身，而不是它周围的部分。你得到什么类型取决于你的医生想知道什么，因为放射科医生可以运行许多不同的扫描和数据分析，以显示不同类型的组织。在浏览了我得到的扫描后，我选定了一个标记为 eB1000i(大脑)的，有对比和无对比的。对于放射科医生来说，这些信息意味着很多，告诉你这是什么类型的扫描，它是用造影剂完成的，这是一种金属染料，注射它是为了让富含水的组织(如我的大脑)更加可见。这个数字指的是一种叫做 [的扩散加权](http://radiopaedia.org/articles/diffusion-weighted-imaging-1) 的东西，它可以帮助医生寻找可以表明中风、肿瘤等疾病的肿胀。这里有一个关于一些行话 [的很好的指南](http://radiopaedia.org/articles/mri-pulse-sequence-abbreviations) 。

## 请求您的 DICOM 数据

 [![A good scan: the brain stands out from the other bits (skull, etc)](img/e20c0541422f2ebe91050cf670bc6af3.png "scan2")](https://hackaday.com/2015/08/25/you-own-your-mri-brainscan-do-something-interesting-with-it/scan2/) A good scan: the brain stands out from the other bits (skull, etc) [![A bad scan: although you can see a lot of interesting stuff (like my eyes, teeth, etc), this will make it harder for the software to separate my brain from the rest of me.](img/2f26920c38de677bc8e5c7ca04cbce09.png "scan1")](https://hackaday.com/2015/08/25/you-own-your-mri-brainscan-do-something-interesting-with-it/scan1/) A bad scan: although you can see a lot of interesting stuff (like my eyes, teeth, etc), this will make it harder for the software to separate my brain from the rest of me.

如果您正在进行核磁共振成像，您可以在扫描后立即申请 CD，或者联系您的医生:作为患者，您有权获得这些数据的副本。您将收到一张 CD，其中包含格式为 DICOM 的 MRI 图像。这是医学数字图像和通信的缩写，是大多数医疗系统使用的开放格式。光盘将包括一个 Windows 程序，允许您查看这些文件，这是值得一试的，因为滚动浏览自己的大脑是一种相当超现实的体验。如果你没有做过核磁共振，有很多扫描样本可供你使用。Osirix 提供了一个[](http://www.osirix-viewer.com/datasets/)(以及其他位)，并且有多个扫描可用 [这里](http://www.jannin.org/mritemplate/) 。

![Phillips MRI](img/d3bf74b8293ce223391776c78bb3a9b7.png)

菲利普核磁共振成像仪[图片由简·艾纳利](https://commons.wikimedia.org/wiki/File:MRI-Philips.JPG#/media/File:MRI-Philips.JPG)CC BY】

磁共振成像是一门令人着迷的科学，它使用非常强的磁场来激发你体内的水分子。这些分子中的氢原子被这个场激发后，会发出一个无线电信号，由核磁共振仪检测。通过形成磁场，MRI 逐渐绘制大脑地图，找出哪些组织含有大量水分(如血管)，哪些组织水分较少，如骨骼。该设备逐渐将这些信息结合到你体内的图像中，而不必真的进去戳它们。如果你对这个过程的物理和数学感兴趣，这里有一篇 [的深度指南](https://www.cis.rit.edu/htbooks/mri/inside.htm) 。

为了处理和转换这些图像，有几个免费的开源程序可用，如[Slicerweb](http://www.slicer.org/pages/Introduction)，[Osirix](http://www.osirix-viewer.com/Downloads.html)，[3d slicer](http://www.slicer.org/)和 Invesialus。这些都有各自的优点和缺点，但我将在本教程中使用[Invesalius](http://www.cti.gov.br/invesalius/)，因为它最容易使用，可用于 windows、mac 和 Linux。

## 软件中的大脑

安装程序后，打开程序并选择导入 DICOM 图像。如果你做了几个不同系列的扫描，你可以一次全部加载:只需选择 CD 的顶层目录，程序将进入每个目录并对它们进行排序，这样你就可以选择最佳的扫描。加载文件后，它会显示每次扫描的预览。选择显示大脑最清晰的一张，尽可能少地显示你的其他部分。要加载这些图像进行分析，请选择导入。

![After loading the scans into Invesalius, you create the masks (in green)](img/608903c3a4b72860dbaa6b3be4fd56c7.png)

After loading the scans into Invesalius, you create the masks (in green)

这将加载扫描图像，并显示四个窗口。其中三张是从不同角度(从顶部(轴向)、侧面(矢状)和前面(冠状)看到的你的头部视图(专业人士称之为切片)。第四个将会是空白的:那是 3D 模型将会出现的地方。您可以使用窗口侧面的滚动条浏览每个视图的图像。

接下来，我们将挑选出我们感兴趣的部分。这是通过使用一个遮罩来完成的，您可以选择好的部分并丢弃其余的部分。这个遮罩就像一个窄通滤波器:你可以创建一个你想要的窄波段，而忽略其他的。左边是一个带有滑块的窗口。当您更改此滑块的上下边界时，您会看到扫描的选定区域(显示为绿色)发生了变化。你要设置这个，以便尽可能多地选择大脑，尽可能少地选择其他东西。该程序确实从下拉菜单中为不同类型的组织提供了许多预设，但我发现自定义预设更有效。同样，您可以使用每个窗口左侧的滚动条滚动浏览图像，以查看不同的切片是如何被屏蔽的。如果你在制作一个干净的面具时遇到了问题，点击手动编辑，用擦除刷去掉那些不是大脑的部分。

![The 3D surface has been created (bottom right)](img/5220bc4348000b3a4d342dbc2313a419.png)

The 3D surface has been created (bottom right)

完成后，点击创建表面按钮。经过一番思考后，程序将从遮罩中创建 3D 表面，并在第四个窗口中显示它。如果有一些不属于大脑的奇怪的部分，不要担心:我们稍后会去掉它们。要旋转曲面，请单击并按住鼠标左键。如果你对这个表面满意，点击下一步并选择导出三维表面。将此表面另存为. STL 文件。

![Editing the model in MeshLab. The red bit is a scanning error, about to be deleted.](img/ea6122bf305f1ec766f951ae3c43aa0e.png)

Editing the model in MeshLab. The red bit is a scanning error, about to be deleted.

我们现在有了一个 STL 文件。然而，它还不能印刷。接下来，我们将使用 [MeshLab](http://meshlab.sourceforge.net/) 清理模型，并为打印做好准备。运行 MeshLab 并加载 STL 文件与文件>导入网格。MeshLab 将允许我们移除模型中我们不需要的部分。我发现最简单的方法是旋转模型，使用选择矩形区域的面和删除点、垂直和面工具来删除我们不需要的部分。MeshLab 在处理像这样的复杂模型时会使用大量内存，所以如果它没有响应也不要感到惊讶。如果你真的很挣扎，尝试减少模型上的面数的过滤器，如过滤器>重新网格化，简化和重塑>二次边折叠抽取。但是要小心:过多的过滤会从模型中移除细节，这正是我们想要的。

一旦你移除了模型的所有无关部分，选择过滤器>重新网格化、简化和重新建模>关闭孔。这将密封模型中的任何漏洞，并为打印做好准备。

最后，选择文件>导出网格并将文件保存为 STL 文件。现在，您已经准备好加载模型进行打印了！任何 3D 打印程序都应该能够加载程序并对其进行处理以打印出来。我在 TAZ 5 打印机上用 Cura 打印了我的。

## 3D 打印你的大脑

 [![The final 3D model in Cura, ready for printing.](img/0cdae30bba6879fa69d82eb5440dd9cf.png "cura1")](https://hackaday.com/2015/08/25/you-own-your-mri-brainscan-do-something-interesting-with-it/cura1/) The final 3D model in Cura, ready for printing. [![brainprint1](img/7c9f3d398fafd66f5fda721b77129f67.png "brainprint1")](https://hackaday.com/2015/08/25/you-own-your-mri-brainscan-do-something-interesting-with-it/brainprint1/) 

我对我的印刷品的效果非常满意。我的灰质错综复杂的结构被很好地捕捉并印在了大脑的顶部，但侧面类似的结构却不太清晰。这可能是因为扫描的处理方式。通过使用其他扫描并结合结果，我可以得到更多的细节。

 [![brainprint3](img/86fb6e89a90690789c5f2bc1c3a9879a.png "brainprint3")](https://hackaday.com/2015/08/25/you-own-your-mri-brainscan-do-something-interesting-with-it/brainprint3/)  [![brainprint2](img/6940f48e18016840e3d6528f3d291c22.png "brainprint2")](https://hackaday.com/2015/08/25/you-own-your-mri-brainscan-do-something-interesting-with-it/brainprint2/) 

现在我有了 3D 模型，可能性是无限的。我可以用柔性塑料把它打印出来，给我的猫一个有趣的玩具。我可以用激光在木头上切割出一个有趣的装饰品。或者，我可以打印一些小字体，以便下次有人要求与这个组织的大脑交流时使用。