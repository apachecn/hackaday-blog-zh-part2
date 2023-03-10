# 在浏览器中呈现 OpenSCAD

> 原文：<https://hackaday.com/2012/08/20/rendering-openscad-in-the-browser/>

如果你没有听说过，OpenSCAD 是一个非常棒的 3D 建模工具。虽然它没有 AutoCAD 的传统图形界面——它基本上是一种用于 3D 模型的编程语言——但 OpenSCAD 能够只用几行代码创建非常复杂的零件。

这很好，但是如果您想在浏览器中编辑 OpenSCAD 部件呢？[进入 OpenJsCAD](http://joostn.github.com/OpenJsCad/) ，完全用 Javascript 编写的 OpenSCAD 解释器，能够嵌入网页。

[OpenSCAD](http://www.openscad.org/) 允许两种类型的建模——构造实体几何图形，或获取 3D 图元并拉伸、缩放和相交它们以创建 3D 形状，或从 2D 轮廓中挤出。相当多的 RepRap 部分是在 OpenSCAD 中设计的，轻量级的接口和开源特性意味着它非常适合设计在 Makerbot 上打印的内容。

向[Gordon]致敬，他发来了这个，我们真的要赞扬他在发现 OpenJsCAD 之前编写了自己的在线脚本化 CAD 导出器。他可能对在线 OpenSCAD 派对有点晚，但我们不得不同意他的观点，在线 3D 实体编辑器将是 [Thingiverse](http://www.thingiverse.com/) 推出的一个令人敬畏的功能。