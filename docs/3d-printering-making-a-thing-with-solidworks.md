# 3D 打印:用 Solidworks 制作一个东西，第一部分

> 原文：<https://hackaday.com/2014/02/19/3d-printering-making-a-thing-with-solidworks/>

![printering1](img/10470cd52b8ac04c2ab10ded944c611c.png)

Brian 很大方地允许我加入 3D 打印潮流，为 Solidworks 的美妙世界写一个简短的介绍。我们将制作与之前的“制作物品”教程相同的“物品”:

![engineeringdrawingblack1](img/aa3b34e53bae14e2b6262656649cf336.png)

*   [OpenSCAD](http://hackaday.com/2013/12/11/3d-printering-making-a-thing-with-openscad/)
*   [AutoCAD 第一部分](http://hackaday.com/2013/12/18/3d-printering-making-a-thing-with-autocad/)
*   [AutoCAD 第二部分](http://hackaday.com/2013/12/22/3d-printering-making-a-thing-in-autocad-part-ii/)
*   [搅拌机第一部分](http://hackaday.com/2014/01/03/3d-printering-making-a-thing-in-blender-part-i/)
*   [搅拌机第二部分](http://hackaday.com/2014/01/08/3d-printering-making-a-thing-with-blender-part-ii/)
*   [SketchUp](http://hackaday.com/2014/01/15/3d-printering-making-a-thing-with-sketchup/)
*   [Autodesk 123D](http://hackaday.com/2014/01/22/3d-printering-making-a-thing-in-autodesk-123d/)
*   [自由 CAD 第一部分](http://hackaday.com/2014/02/05/3d-printering-making-a-thing-in-freecad-part-i/)
*   [F reeCAD 第二部](http://hackaday.com/2014/02/15/3d-printering-making-a-thing-in-freecad-part-ii/)

诚然，大多数黑客读者可能没有 Solidworks，因为它是一个非常昂贵的程序。我们发布这个教程的主要原因是为了让你能够理解工作流程，并将其与一些免费/开放的软件包进行比较。

正如 Brian 在他的 [FreeCAD 帖子](http://hackaday.com/2014/02/05/3d-printering-making-a-thing-in-freecad-part-i/)中提到的，参数模型的零件特征可以随时修改。例如，假设我制作了一个实体块，然后在一个面的中心添加了一个特定大小的孔。后来，如果我想改变块的大小或形状，无论物体的其他部分如何变化，洞都会保持相同的大小，并保持在该面的中心。见下图，所有的变化是块的大小，洞保持不变的大小和位置(面的中心)。这与“缩放”整个对象是不同的，因为洞也会随着块一起被拉伸。

![parametric](img/6fb63bf96858042478cd93391a86d106.png)

#### 入门指南

在学校和工作之间，我有机会使用几个专业的参数化建模软件，包括 ProE(现在叫做 Creo)，NX(曾经是 Unigraphics)，当然还有 Solidworks。工作流程都差不多。如果你记得这四个步骤，你会做得很好:平面，草图，尺寸，拉伸。

在本例中，我们将使用两个主要选项卡，即特征选项卡和草图选项卡。他们有我们制作样品所需的所有工具。

![tabs](img/e39e089b366210c9d05df9add668aef8.png)

让我们创建一个新零件，文件，然后新建。将弹出一个窗口，询问制作什么类型的文件。我们正在制作一个零件，因此我们将选择“零件”。

![open](img/f1a7609e47e4d5308a4296cb3b690327.png)

#### 飞机

您将从一个显示空白空间的屏幕开始，这是将创建对象的地方。有 3 个平面，在下图中，我点击了顶部的平面来选择它。为什么？因为“平面”是我们 4 个步骤中的第一步！我们正在选择将在其上绘制草图的平面(或曲面)。

![planes](img/7cc0f0dfd0647bf6f0255fad268737e3.png)

#### 素描

在平面仍处于选中状态的情况下，单击草图选项卡，然后选择草图。视图将垂直于顶部平面移动。我们现在处于草图模式，将能够绘制零件的一部分草图。我决定先画出零件的底部，有孔和槽的那部分。从零件的后部开始也很容易。

在参数化程序中绘制草图的最大好处是，您可以直接绘制草图，而不用担心尺寸或比例。我们将在草图完成后标注尺寸。为了向你展示我的意思，我打算故意画一个比例失调的草图。

草图所需的所有工具都在“草图”选项卡上。对于这个草图，我将使用直线、中心线、圆、修剪和[圆角](http://en.wikipedia.org/wiki/Fillet_(mechanics))命令。在这一点上绘制草图非常类似于任何 2D CAD 软件，除了你不必担心这个时候的尺寸。只要让它看起来很近。

![sketch1](img/073038550cd2a12811256a0c0e8bb487.png)

嗯，那不是一个丑陋的部分！丑但是完全可以接受。请注意，我故意将内部和外部圆角从零件的右下腿中去掉。我这样做是为了在零件挤压成实体后添加它们，只是为了展示另一种方法。另请注意，我使圆形特征与前平面和右平面的相交处同心。这是个人偏好，但我认为这使标注变得更容易，因为我可以标注与这两个平面相关的特征，这也恰好是圆的中心。来自孔中心的虚线是中心线，将定义槽的角度。中心线不会成为零件的特征，它只是一个参考。稍后，我将使槽边平行于这条中心线，并保持一定的距离。

你可以在草图上看到一堆绿色的小方框。这些是每个特征的关系。每个符号都有意义。垂直线意味着相邻要素将始终是垂直的。带直线的圆表示圆弧与直线相切，并且永远相切。两条线和一个红点意味着两条相邻的线共享一个端点或中点。

#### 尺寸

我们的草图现在需要尺寸。在“草图”选项卡上有一个名为“智能尺寸”的工具。选择此项开始标注零件特征。你可以这样做:

*   要指定两条平行线之间的距离，请单击一条线，然后单击另一条线。将出现一个尺寸，将鼠标移动到需要尺寸标签的位置，然后单击以放置它。在弹出的对话框中输入距离，线将移动以满足新的尺寸要求。
*   要指定圆弧的半径或圆的直径，点击曲线并放置尺寸。然后键入值。
*   要指定两条非平行线之间的角度，点击一条线，然后点击另一条线。放置尺寸标注并输入所需的角度值。
*   要添加一个关系，如指定槽边与中心线平行，选择一个槽边，然后按住 SHIFT 键选择中心线。添加关系选项将出现在屏幕左侧。选择并行。您可以看到所有可用的关系选项。请注意，在完成该命令后，两条线现在是平行的，并且显示了两个绿色的平行关系指示框。仅供参考，添加关系时，您不能在智能维度功能中。

![relation](img/5009f60322b19ba17401fb52542fcb8d.png)

继续标注尺寸，你会得到类似下图的结果。请注意，一些草图线以前是蓝色的，但现在是黑色的。黑线表示其位置和大小已完全确定。这是一件好事，可以防止将来发生意外的几何形状变化。完全黑色的草图可以被称为“完全约束”。

![sketch1dimensioned](img/ece2918b5bfba1b9739f69079439c6f8.png)

草图完成了。单击“草图”选项卡上的“退出草图”。

#### 挤压出

这是有趣的部分。现在，您可以在顶部平面上看到草图，并在左侧的模型树中看到一个名为 Sketch1 的新行项目。如果我们需要改变草图上的任何东西(甚至在模型创建之后),我们可以通过返回并编辑 Sketch1 来完成。

单击“模型树”中的“草图 1 ”( sketch 1)来选择草图。然后在“特征”选项卡上，选择“拉伸凸台/基座”。将弹出一个对话框，询问草图要拉伸多少。输入所需的数量，然后单击绿色复选标记。

![sketch1extruded](img/d39c0bb31459dbbdf85647ce79127aad.png)

成交。….至少在这一部分。在第 2 部分(尚未出版)中，我们将继续其余部分。

如果你愿意浪费生命中的 4 分钟，这里有一个视频:

[https://www.youtube.com/embed/Ouzhg6OI1JY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/Ouzhg6OI1JY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

**3D 打印是一个每周专栏，深入挖掘所有与 3D 打印相关的事物。如果您对未来的分期付款有任何问题或想法，请[将您的想法发送给我们](mailto:tips@hackaday.com?Subject=[3D%20Printering])。**