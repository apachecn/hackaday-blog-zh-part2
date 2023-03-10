# 3D 打印:用 SketchUp 制作一个东西

> 原文：<https://hackaday.com/2014/01/15/3d-printering-making-a-thing-with-sketchup/>

![printering](img/f129892b22bffa0dd52c94f9b281e2fb.png)

想象一下，现在是 20 世纪 80 年代中期，你正在研究桌面出版系统。那些新的 LaserJets 和 LaserWriters 非常酷，但是想象一下桌面出版世界，如果你不能创建自己的文档。是的，拥有一台不会创造独特文档的印刷机似乎很荒谬。

现在让我们回到 30 年前的桌面制造和快速原型制作的世界。有几十个 3D 可打印对象的仓库，但对于每个购买塑料章鱼和开瓶器 3D 打印机的人来说，制作自己设计的东西显然是一门黑暗的艺术和神秘的知识。

本周，应大众要求，我们将在 [SketchUp Make](http://www.sketchup.com/products/sketchup-make) 中制作一个“东西”。尽管它的工具集有限，但它是免费的、简单的，而且用途惊人地广泛。常识和谷歌算法决定了我在下面链接到本系列以前的教程:

*   [OpenSCAD](http://hackaday.com/2013/12/11/3d-printering-making-a-thing-with-openscad/)
*   [AutoCAD 第一部分](http://hackaday.com/2013/12/18/3d-printering-making-a-thing-with-autocad/)
*   [AutoCAD 第二部分](http://hackaday.com/2013/12/22/3d-printering-making-a-thing-in-autocad-part-ii/)
*   [搅拌机第一部分](http://hackaday.com/2014/01/03/3d-printering-making-a-thing-in-blender-part-i/)
*   [搅拌机第二部分](http://hackaday.com/2014/01/08/3d-printering-making-a-thing-with-blender-part-ii/)

现在开始表演。你需要点击“阅读更多”链接。

#### 我们的事

[![engineering drawing](img/bfd122a8c7a67079efd82a91a693fada.png)](//hackaday.com/wp-content/uploads/2014/01/engineeringdrawingblack1.png)

正如所有这些制作一个东西的教程，我们将使用这个开关基地的权利。单击以嵌入。

感谢一些读者，上周带来了一些有趣的观察结果。我现在不会用这个来烦你，但是我已经在这篇文章的底部添加了一些关于这个事情的注释。

#### 设置事物

SketchUp 有两个版本；SketchUp Pro 售价约 600 美元。SketchUp Make 是免费软件，能够制作你能想象的任何机械零件。

安装并启动 SketchUp Make 后，会要求您选择一个模板。我们可以使用“产品设计和木工”模板。令人惊讶的是，SketchUp 的人很友好，给了我们使用英寸和毫米之间的选择。因为我们的“东西”是以英寸为单位的，所以选择那个模板并点击“开始使用 SketchUp”

[![title1](img/d1dabd730c5657eb690d1d17a89a41ad.png)](http://hackaday.com/wp-content/uploads/2014/01/title1.png)

#### 开始我们的事

[![Circle1](img/fa1a675a1c59bf0d8a1290668a2f9d4a.png)](http://hackaday.com/wp-content/uploads/2014/01/circle1.png)Sketchup 背后的基本思想是能够在二维空间中绘制，并使用推/拉工具将形状挤压到 Z 轴(或者在 Sketchup 的情况下，挤压到蓝色轴)。在窗口顶部的工具栏上，选择圆形工具。单击红色、绿色和蓝色线交叉点附近的任意点。

如果你按照 AutoCAD 教程来做，制作这个圆所需的尺寸会看起来很熟悉。要得到一个直径为 2 3/8 英寸的圆，只需在键盘上输入半径。对于不在美国、利比里亚或缅甸的人来说，那是 1 3/16 英寸。

我们的第一项任务是在我们的东西的“大圆圈部分”制作 3/8”槽，并钻出中心。我们先从插槽开始。

SketchUp 有一个很棒的 snap-to 功能，我们即将试用。在工具栏上，使用铅笔或“线条”工具。在圆心周围挥动它，最终它会在圆心处折断。点按中心，沿着红色轴画一条 3/16 英寸长的线(请记住，您可以在数字小键盘上输入尺寸)。再次单击中心，沿相反方向绘制另一条相同长度的线。从这些线的末端，一直向下画，在我们的部分做一个槽。接下来，拿起橡皮擦工具。擦掉我们刚刚画的槽之间的一点点圆的周长。

![Gif1](img/27d36697094846c961ee0a1b69003b11.png)现在该打洞了。选择圆形工具，悬停在你认为是大圆的中心，等待它捕捉。画一个半径为 1/2 英寸的圆。使用橡皮擦工具，明智地使用键盘上的 delete 键，你会得到一些看起来很像我们的东西的东西。剩下唯一要做的就是旋转它。

从“工具”菜单中，选择“旋转”(或只使用“Q”热键)。在零件的紫色区域选择一个点，然后沿着绿色或红色轴选择第二个点。根据您点击的位置，您需要输入 45、135 或 225。或者键盘上的 315 度。

#### 继续…

![Trap1](img/6ffa8461b533d5375e29983aced1ca98.png)

现在，插槽都排好了 45 度角，我们可以开始工作的两个小法兰脱落的圆形部分。较宽的凸缘——除了角上的圆角——留给读者练习。这同样适用于该器件的另一侧，除了设计中的这个小“陷阱”，见右图。

如果我们向下延伸这个凸缘的边，它不会在我们的槽的末端相交。别担心，真的。就像你平常那样画线，点击我们的槽的内部，然后试着延伸这条线。SketchUp 的捕捉非常棒，你可以很容易地在你想要的地方画一条线。之后，用橡皮擦清理干净。

[![trap2](img/60922d707d1bfad4ef034839e0100e60.png)](http://hackaday.com/wp-content/uploads/2014/01/trap2.png)

#### 鱼片

我们需要在我们的东西上绕四个角，所有的角都在我们的大而宽的凸缘上，凸缘从我们的部分底部伸出来。首先我们要做外角。

[![GIF2](img/c707299f9b788d362840e957079eb053.png)](http://hackaday.com/wp-content/uploads/2014/01/gif2.gif)

我们需要在每个角上有 1/8 英寸的半径。首先沿着我们的东西的边画两条 1/4 英寸的线。在。上面的 gif，我在行尾加了两个哈希标记。在这两个端点之间画一条线，然后在这个三角形斜边的中点画一个 1/8”半径的圆。用橡皮擦擦干净，在另一面做同样的动作。

[![GIF3](img/3da2ebf2aec573f2235ddb264583623a.png)](http://hackaday.com/wp-content/uploads/2014/01/gif3.gif)

内侧弯道有点棘手。如果我们使用 AutoCAD，我们只需使用 FILLET 命令在内角制作一个完美的圆角。SketchUp 没有 AutoCAD 高级，但是我们可以用现有的东西来造假。

SketchUp 有一个名为 Offset(热键 F)的工具，允许你“环绕”任何对象，并指定线之间的距离。如果我们将几条线从我们的零件偏移 1/8 英寸，它们交叉的地方就是 1/8 英寸圆角的中心。一旦我们知道圆角的中心在哪里，我们就可以画一个圆，在内角上得到一个完美的半径。很圆滑，是吧？

这是我们最终得到的，没有橡皮擦工具:

![fillet](img/a82b6397be341a2bbc627cd19892ee28.png)

#### 向上挤压

![push](img/9b8a2b3f317a5dd0112e44a24392f6b5.png)现在是时候开始我们的“高”的部分了。离开小凸缘，画一个 1/2 英寸 x 1 1/2 英寸的矩形。使用推/拉工具，将该矩形向上挤出到通孔的中心，或 1 5/16 英寸(即底座厚度的 7/16 英寸，再超出 7/8 英寸)。

现在，使用圆形工具，悬停在我们的新三维实体的顶部前侧的中点。创建一个矩形宽度的圆，向后挤压半英寸。

![GIF4](img/40d6f39bbab7025f1e96ce91940699d1.png)

使用相同的过程，您可以轻松地在零件上创建钻孔和沉头孔。这很简单，只需使用推拉工具和橡皮擦。

#### 哇哦。这种事。多维度。

给你。SketchUp 做的东西。剩下的就是把这个模型发送到你的 3D 打印机上。SketchUp 不支持导出到。虽然是 STL 文件，但这是“制作东西”系列的最后一篇文章。

![thingdone](img/4c870d3bff332d3d8427a7f9716c560c.png)

* * *

这就是本期制作一个东西的全部内容，但是我想说一些关于我们刚刚制作的部分的事情。

就像其他制作东西的教程一样，我们的“东西”取自一本 85 年前的制图教科书《工程制图》(法语，1929)。这是这本书的第四版，上周我问是否有人有第一版(1919 年的)。[【雅各布】很牛逼](http://hackaday.com/2014/01/08/3d-printering-making-a-thing-with-blender-part-ii/#comment-1159021)找到了第一版，但是这部分不在里面。

此外，有史以来第一次，有人注意到我一直在做的这些部分是非常错误的。看较薄法兰的宽度。它有一英寸半宽。现在看看高的部分的“圆顶”的半径。半径为 5/8 英寸，直径为 10/8 英寸。八分之十二不等于八分之十。那个高的部分实际上有一个锥形。

在我看来，如果我做了这个部分的作业——画一个三视图——我就会发现这个锥形。

尽管成千上万的人看到了这些教程，但只有[tarasbot]一个人注意到了这一点。他给我发了邮件，现在他收到了一件 Hackaday t 恤，一些贴纸，以及下周 Hackaday 派对后我能找到的任何东西。需要你的衬衫尺寸。

现在就这样，下周是 Autodesk 123D，和往常一样，欢迎您对用什么软件来构建“东西”提出建议。