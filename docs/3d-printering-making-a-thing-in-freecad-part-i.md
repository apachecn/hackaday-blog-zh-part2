# 3D 打印:在 FreeCAD 中制作一个东西，第一部分

> 原文：<https://hackaday.com/2014/02/05/3d-printering-making-a-thing-in-freecad-part-i/>

![printering](img/f129892b22bffa0dd52c94f9b281e2fb.png)

我写这些关于在流行的 3D 建模程序中制作一个物体的教程已经有一段时间了，每个星期我都会呼吁下一步我应该做什么软件。在所有那些评论线程中有一个常量:FreeCAD。我不知道这些建议反映的是 FreeCAD 的受欢迎程度~~还是难度~~没关系，完全是难度。

FreeCAD 是一个令人惊叹的工具，如果使用正确，它可以用来制造任何零件，并在制造环境中完成。如果你需要一个比原来大三倍的小玩意，FreeCAD 的参数化建模可以很容易地放大它。如果你正在设计一个指旋螺钉，并且想要头部更大，同时保持螺纹不变，FreeCAD 就是为你准备的。基本上，你可以认为这是 [Thingiverse 定制器](http://hackaday.com/2013/02/16/custom-3d-printed-designs-with-makerbots-customizer/)的图形化扩展。非常强大，非常酷，不像外面的许多 CAD 软件，*是免费的。*

我们的内部高薪 SEO 专家(他实际上只是一只受过牛鞭训练的猴子)要求我链接到以前的“制作东西”教程:

*   [OpenSCAD](http://hackaday.com/2013/12/11/3d-printering-making-a-thing-with-openscad/)
*   [AutoCAD 第一部分](http://hackaday.com/2013/12/18/3d-printering-making-a-thing-with-autocad/)
*   [AutoCAD 第二部分](http://hackaday.com/2013/12/22/3d-printering-making-a-thing-in-autocad-part-ii/)
*   [搅拌机第一部分](http://hackaday.com/2014/01/03/3d-printering-making-a-thing-in-blender-part-i/)
*   [搅拌机第二部分](http://hackaday.com/2014/01/08/3d-printering-making-a-thing-with-blender-part-ii/)
*   [SketchUp](http://hackaday.com/2014/01/15/3d-printering-making-a-thing-with-sketchup/)
*   [Autodesk 123D](http://hackaday.com/2014/01/22/3d-printering-making-a-thing-in-autodesk-123d/)

FreeCAD 的教程在下面继续。

* * *

#### 我们的事

和所有的教程一样，我们将复制这个“东西”，摘自一本有 80 年历史的关于制图的教科书。

我们不会完全复制这个东西*—*在带沉孔的标签上有一个小锥度——但我们会足够接近，所以我们完成的模型应该在功能上是等效的。

#### 启动和概述

要使用 FreeCAD，您可能需要[下载 FreeCAD](http://www.freecadweb.org/wiki/index.php?title=Download) 。它适用于 32 位或 64 位版本的 Windows、Linux 和 OS X。选择你的毒药。下载并安装后，您将会看到一个类似如下的“开始中心”:

[![Title](img/6c6e9807c35203687d79ecdcaba200d7.png) ](http://hackaday.com/2014/02/05/3d-printering-making-a-thing-in-freecad-part-i/title-10/) [ ![Orientation](img/6c235e871955ca1ec841095633325357.png) ](http://hackaday.com/2014/02/05/3d-printering-making-a-thing-in-freecad-part-i/orientation/) FreeCAD 在 3D 设计程序中是独一无二的，因为它有[许多不同的工作台](http://www.freecadweb.org/wiki/index.php?title=Workbenches)或模式，可以在其中绘图和建模。对于我们的大部分事情，我们将使用零件设计工作台。在起始页的“启动新项目”选项卡下，单击“部件设计”按钮。点击创建草图，选择 XY 平面，惊叹于你的绘图网格。

在开始之前，您最好将栅格大小更改为 1 毫米，并打开栅格捕捉。

*有一点需要注意:*虽然网格尺寸*说的是*毫米，但是 FreeCAD 并没有真正的单位。它有单位，一个 FreeCAD 单位等于一个 FreeCAD 单位。这很好，因为现在我们可以用八分之一英寸来设计我们的零件，其中八分之一英寸是一个单位。这更简单，为了打印出正确尺寸的零件，我们需要乘以*……*

#### 如果你不读别的，读这两段

FreeCAD 是一个参数化建模器。这意味着所有线、图形和部件都由参数和约束定义。参数是定义零件属性的信息片段——一个 10 厘米的立方体的 X、Y 和 Z 轴的参数等于 10 厘米。约束定义了对象各部分之间的关系。两条线可以被约束为平行；移动直线的一个顶点，受约束直线的一个顶点也会移动。

对一个对象进行参数化建模是公司设计许多相似但大小不同的对象的方法。一家制造鞋子的公司可能只有一种型号的鞋子。有了参数模型，制作 6 号和 10 号鞋的部件可能就像改变一个数字一样简单——从脚趾到脚跟的长度。

#### 最后，建立

对于我们的大多数建模，我们将使用两个工具栏。它们是*几何*和*约束*工具栏:

![Create](img/637f76abc6f76fcddeaba9632ed76a5a.png)

“几何”工具栏几乎是任何 CAD 或绘图软件包中都能找到的。有用于创建点、弧、圆、直线和多段线的按钮，甚至还有圆角和修剪按钮。

![Constraints](img/cd3bba01fc48047995e516c77dcb0e5b.png)

“约束”工具栏上有按钮，用于将对象(直线、圆、多段线等)锁定到垂直轴和水平轴上。此外，可以使直线平行、垂直于圆弧的切线，并且直线的垂直、水平距离以及直线的总长度或圆的半径也可以受到约束。

我们要画的“东西”的第一部分是最大的圆。使用栅格捕捉(或在移动光标时按住 CTRL)，在栅格上 0，0 处绘制一个圆。这个圆的半径为 9.5。我们以八分之一英寸为单位，由于最大圆的直径为 2 3/8 英寸，即 19/8 英寸，半径为 9.5 个单位。同样添加另一个半径为 4 的圆。

![Radius](img/1959ba5c5f34730ebe841a3408a5899f.png)你可以使用几何按钮使这些圆大致符合尺寸，然后使用半径约束使这些圆符合要求的尺寸。

在您绘制并约束了这些圆之后，您应该会看到如下所示的内容:

[![Circles](img/d3536ee03af6ff9096575947535d6a08.png)](http://hackaday.com/2014/02/05/3d-printering-making-a-thing-in-freecad-part-i/circles-2/)

#### 现在来看一些细节

我们的“东西”还有很多要补充的。让我们从 3/8”宽的槽开始。从画两条线开始，大致从圆心穿过较大的圆。将它们约束为平行，其中一个(约束工具栏上最右边的按钮)的角度为 45 度。

使用几何工具栏上的修剪工具，修剪掉所有多余的部分——两条线的末端和两个圆上的剪切部分。现在你应该有类似字母 c 的东西了。

![2](img/ae56ed0501ed3065c28a3b5ffd3e1a0d.png)

使用“固定长度”约束工具，使两条 45 度线之间的距离为 3。最后，用“锁定”约束锁定槽的上部、外部顶点。你应该有一些看起来像右边的图片。你还会注意到在 FreeCAD 的左侧工具栏上,“解算器消息”显示这是一个完全约束的草图。

![Solver](img/6df7d40abe103047cae171feb3b0a41a.png)

这意味着我们已经正确地完成了*。好吧，在这种情况下，这是一个谎言(我们没有保证插槽与圆心对齐)，但它足够接近。在 FreeCAD 中，目标是拥有一个完全受约束的对象。这就是我们在这里所做的。*

 *由于我喜欢将这些教程压缩到 1000 字左右，所以我将在此结束。在本教程的下一部分中，我们将在这个垫圈型零件上添加凸缘，将其挤压到第三维空间，并添加带埋头孔的钻头。

未完待续，我可能会在这里放一个第二部分 [的链接。](http://wp.me/pk3lN-tQq)*