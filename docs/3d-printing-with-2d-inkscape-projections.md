# 使用 2D Inkscape 投影进行 3D 打印

> 原文：<https://hackaday.com/2015/08/02/3d-printing-with-2d-inkscape-projections/>

如果你上过正式的制图课，你可能学过制作正交投影——有多个视图的工程图(例如，顶视图、前视图和右视图)。即使你没有上过这门课，你也可能见过这样的画，你从不同的角度把一个三维物体看成一系列 2D 视图。

如今，你更有可能创建一个物体的 3D 模型，尤其是如果你打算 3D 打印它。毕竟，3D 打印机软件需要一个模型。当[茄影]想要一个笔记本电脑支架作为他的工作台时，他开始尝试做一个 3D 模型。然而，他的最终产品是由[在 Inkscape](http://wemakethings.net/2015/06/19/parabol-laptop-stand/) 中创建的两个视图制成的。它们并不完全是最终产品的正投影，但想法是相似的。

Inkscape 是一个矢量图形程序，通常创建 SVG 文件，尽管它也可以保存 EPS 文件。[茄影]使用 pstoedit 将 EPS 输出转换为 DXF 格式。DXF 文件仍然是二维的，但 OpenSCAD 可以将 DXF 文件挤压成三维形状。

然而，仅仅拥有一个视图的 3D 形状是不够的。 [OpenSCAD 脚本](https://github.com/kspi/parabol)将对象旋转到正确的方向，并使它们相交，形成最终的对象。这不同于通常使用 Inkscape 来[跟踪扫描](http://www.thingiverse.com/thing:43387)或生成[简单文本](http://www.thingiverse.com/thing:68195)的情况。

Inkscape 可以直接导出 DXF，但是它有很多限制。如果你不想使用 pstoedit，有一些插件(如[蓝色锯插件](http://www.bigbluesaw.com/saw/big-blue-saw-blog/general-updates/big-blue-saws-dxf-export-for-inkscape.html))工作得更好，可能也适用于这个应用程序。

这种技术远非通用(一些对象需要两个以上的视图，并且轮廓并不是真正的投影)。不过，如果你能理解这两种形状，这仍然是一种生成 3D 物体的有用技术。

我们以前见过 Inkscape 与打印机和切割机一起使用，或者[生成 2D 激光切割图案](http://hackaday.com/2014/01/07/delta-laser-engraver-uses-inkscape-for-g-code/)或者定义[有用的轮廓](http://hackaday.com/2012/07/26/box-maker-extension-for-inkscape/)。不过，在这种情况下，这些形状实际上会混合(通过“相交”命令)形成最终的 3D 对象。当然不一定要用 Inkscape。任何输出 DXF 的 CAD 程序(例如，FreeCAD 或 LibreCAD)都应该使用这种技术。

[https://www.youtube.com/embed/EKOjV63ohJM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/EKOjV63ohJM?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)
[https://www.youtube.com/embed/SIEaoubaipE?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/SIEaoubaipE?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

谢谢[miceuz]的提示！