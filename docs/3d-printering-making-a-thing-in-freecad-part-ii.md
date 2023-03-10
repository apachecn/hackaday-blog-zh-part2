# 3D 打印:在 FreeCAD 中制作一个东西，第二部分

> 原文：<https://hackaday.com/2014/02/15/3d-printering-making-a-thing-in-freecad-part-ii/>

![printering](img/f129892b22bffa0dd52c94f9b281e2fb.png)

又到了制作物品教程的另一期了，我在多个 3D 设计软件包中一遍又一遍地设计同一个零件。

上周我们看了一下 FreeCAD，一个免费的开源参数建模器。这是一个令人惊讶的强大工具，而不是最后的时间来完成我们的模型，一个奇怪的物体从一个 80 岁的绘图教科书中撕下来。

这里有一些以前制作东西教程的链接，doe:

*   [OpenSCAD](http://hackaday.com/2013/12/11/3d-printering-making-a-thing-with-openscad/)
*   [AutoCAD 第一部分](http://hackaday.com/2013/12/18/3d-printering-making-a-thing-with-autocad/)
*   [AutoCAD 第二部分](http://hackaday.com/2013/12/22/3d-printering-making-a-thing-in-autocad-part-ii/)
*   [搅拌机第一部分](http://hackaday.com/2014/01/03/3d-printering-making-a-thing-in-blender-part-i/)
*   [搅拌机第二部分](http://hackaday.com/2014/01/08/3d-printering-making-a-thing-with-blender-part-ii/)
*   [SketchUp](http://hackaday.com/2014/01/15/3d-printering-making-a-thing-with-sketchup/)
*   [Autodesk 123D](http://hackaday.com/2014/01/22/3d-printering-making-a-thing-in-autodesk-123d/)
*   [自由 CAD 第一部分](http://hackaday.com/2014/02/05/3d-printering-making-a-thing-in-freecad-part-i/)

请继续阅读我们 FreeCAD 教程的第二部分

* * *

#### 我们的事情，我们上次离开的地方

右边是我们正在制作的东西。这是一本 80 年前的关于起草的书。

一些人向我要这本书的. PDF 文件。我的副本是死树格式，我还没有建立一个图书扫描仪。如果有人有第一版或第二版*工程图*(法国，1911 年或 1918 年)，请扫描它(它的公共领域)并发布链接。 [这是第二版](http://books.google.com/books?id=6R5DAAAAIAAJ&pg=PA78#v=onepage&q&f=false)的谷歌扫描件。

在本教程的最后一期[中，我们复习了安装 FreeCAD，参数化建模的基础，并画了一些圆和线。完成我们的“东西”只是一个绘制线条、圆弧和圆角的过程，约束它们，并且在 FreeCAD 无法向你展示*你草图中的一个不受约束的元素时，你会抓狂，哦，我的上帝。*经过一点点反复试验，我们最终得到了类似下图的东西，这是我们大部分交换机基础的完全受限草图:](http://hackaday.com/2014/02/05/3d-printering-making-a-thing-in-freecad-part-i/)

![Done](img/a1149f17e313d53b999fe261853989f8.png)

是的，很丑，但是很准。现在是时候进入第三维度了，把我们的东西挤出 7/16 英寸。请注意，我真的不在乎我正在设计的东西的绝对尺寸。FreeCAD 只是公制的，所以我设计的都是八分之一英寸左右的东西。切片器可以让你缩放打印*反正……*

* * *

#### 推出

一旦我们绘制并约束了零件，左侧工具栏上的解算器将告诉我们有一个完全约束的草图。现在是挤出我们的物体的时候了。单击任务栏上的“关闭”,您将看到几个选项:创建草图、凸台、凹槽、旋转和凹槽。我们用于挤压的工具是 Pad，所以点击它。切换到等轴测视图，为正确的拉伸深度设置凸台参数，您将获得一个非常棒的填充实体。太棒了。

![close](img/6a873b33d5874ab09608c4fed0ab9d1e.png)

![PAD](img/672b827484e6d697fbb616f65c4c7f87.png)

![Pad2](img/6025ecf0aedebf4643fc59313bac7009.png)

![extrude](img/8edce1dc4ecd8e61deac1aba37683524.png)

虽然我们无法在零件设计工作台中对零件进行“内部”圆角处理，但“圆角”命令仅适用于两条线之间，不适用于直线和圆弧。现在我们已经将我们的东西挤压到 Z 轴上，我们终于可以添加这些圆角了。在 3D 视图中，单击分隔我们零件的大“垫圈”和长凸缘的边。

![fillet3](img/e056196cf1187a8c527ec776a26e6f0d.png)

![fillet2](img/caeb13883fd862c034f3ad30f3e9480e.png)

之后，我们得到一个相当好看的部分。不过，我们还没完。我们还需要制造另一部分，我喜欢称之为“埋头法兰”。

#### 添加另一部分

![Flange1](img/92315e74fdfb7cbc6a4a60f5026f3b75.png)

现在我们已经设计好了底部，但是我们仍然缺少带埋头孔的法兰。要添加这个，我们需要创建我们的东西的“埋头法兰”部分的轮廓。进入零件设计工作台，画一个完全约束的零件，然后像我们对第一个零件做的那样挤压它。当我们完成时，我们将得到类似这样的东西:

![flangeextrude](img/5ae0096f1be7cd1d8da062290b90ac72.png)

做完这些后，就该组装这两个零件了。当我们返回零件工作台时，我们会看到类似右边的图片。我们的零件在那里，但我们需要正确地安排它们，并以某种方式连接它们。之后，我们需要在法兰上打孔。很简单。

* * *

#### 排列零件

![Placement](img/e2c33bd23ae1f9eb0fcd74947dcdb73d.png)

在零件工作台中，选择您刚刚在零件树中为我们的产品制作的法兰。底部有一个标签为“数据”的标签，这是我们将法兰放置在我们的东西的“垫圈”部分末端的地方。不断调整位置，直到一切都正确为止，我们已经完成了 90%的工作。

![flange3](img/f570a2b8235066bb53022b5604b30a77.png)

#### 添加孔

选择法兰上我们要钻孔的面。我们需要为此创建两个草图；一个用于通孔，另一个用于沉孔。画一个较小的孔，然后用袖珍工具移除它。这个工具是非常相反的垫工具；它挤压的是“下”而不是“上”。

在法兰表面的另一个草图中，绘制较大的孔，并将其缩小到适当的深度。

![Holes](img/6ec1016715437ffe8d4043910392fcfc.png)

还有一个完整的部分。导出，如果需要的话做一些布尔运算，我们就完成了。

* * *

#### 包装 FreeCAD

FreeCAD 是一个非常强大的工具，但是在制作这个教程的时候，我确实注意到 FreeCAD 的界面有点不稳定；使用鼠标中键在当前视图中平移草图并不总是有效，添加一条线有时(虽然很少)会导致冻结，并且有几个 UX 只是…很糟糕的例子。

鉴于 FreeCAD 目前的版本是 0.13，以及我可能使用 Windows 版本的事实，这种事情是可以预料的。它仍在改进中，尽管我相信 FreeCAD 最终会成为最好的开源设计和建模软件之一，但它仍需要一些工作。

如果你懂 Python 和 C++，并且正在寻找一个开源项目，我强烈建议[帮助 FreeCAD 开发者](http://www.freecadweb.org/wiki/index.php?title=Help_FreeCAD)。毫无疑问，在我看来，FreeCAD 在几年后最终会像 KiCAD 在电子设计中一样受欢迎。FreeCAD 现在仍然是一个很棒的软件包*，但是在成为主流之前它还需要一点工作。*

 ** * *

这就是制作一个东西的教程。下周，Hackaday 贡献者[Rich]将发布 Solidworks 教程的第一部分。太棒了，你会看的。

在 Soildworks 教程之后，我完全不知道这些制作东西的教程会走向何方。到目前为止，本系列已经介绍了六个软件包，我们已经介绍了创建 3D 打印对象的几乎所有方法——AutoCAD 用于传统制图，FreeCAD 用于参数化建模，OpenSCAD 用于脚本化 3D 建模。

为其他软件包编写更多的教程只会重复本系列已经对不太流行的软件所做的工作。这意味着我有点不知该为这些制作指南写些什么。

如果你知道这一系列教程接下来应该做什么，请在评论中留言。我也考虑过弄一个简单的 Printrbot，展示打印失败的所有原因，以及修复它的方法。如果你有更好的想法，你总是可以在评论中提出建议。*