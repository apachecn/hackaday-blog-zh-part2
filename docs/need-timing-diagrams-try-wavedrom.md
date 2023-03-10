# 需要时序图吗？试试 Wavedrom

> 原文：<https://hackaday.com/2015/05/25/need-timing-diagrams-try-wavedrom/>

当处理任何数字事物时，你很快就会开始阅读或书写时序图。对我们来说，这意味着记笔记，在餐巾纸上画点什么，或者使用像 Inkscape 这样的工具。这些都不理想。

一个下午寻找更好的工具最终以 [Wavedrom](http://wavedrom.com/) 结束。

为了让你知道我们从何而来，下面是我们对时序图绘制解决方案的需求列表:

*   图表有一个基于文本的表示，因此它们的生成可以很容易地编写脚本，结果可以在整个项目开发过程中进行版本化和跟踪
*   图像的命令行渲染，因为我们喜欢自动化一切
*   看起来不错
*   在普通情况下使用简单，但是足够灵活，可以在需要时做一些奇怪的事情
*   绝对必要时输出可修改:SVG 会很好

基本上，我们想要的是时序图的 graphviz。

Wavedrom 目前锁定了这五个中的四个，并承诺覆盖所有的基础。给[在线编辑器](http://wavedrom.com/editor.html)试玩一下。我们发现它足够直观，我们甚至不需要阅读精美的手册就可以制作简单的图表。[教程](http://wavedrom.com/tutorial.html)已经为您介绍了更深奥的用例。

[![foo](img/31bb51c18e056c92c727764a053328c9.png)](https://hackaday.com/wp-content/uploads/2015/05/foo.png)

显然，波形描述语言 [WaveJSON](https://github.com/drom/wavedrom/wiki/WaveJSON) 中已经加入了一些好的想法；它的可读性很强，使要点变得简单快捷。因为您也可以直接进入 SVG，所以它为全面的疯狂敞开了大门。

Wavedrom 是用 JavaScript 写的，为嵌入网页而建；这是他们希望我们使用它的方式。另一方面，如果你想运行你自己的本地版本的在线编辑器，你可以[下载它](https://github.com/wavedrom/wavedrom.github.io/releases)并在本地安装。

我们唯一的缺点是，如果没有 Arch 系统上的 GUI，独立的命令行应用程序不会生成图像。(貌似有一些谷歌 Chrome 的依赖？)否则，我们认为我们已经找到了解决方案。

还有其他的应用。Drawtiming 看起来不错，但是我们不能完全理解文件格式，图形输出也没有我们希望的那么灵活:它只输出 GIF，我们更喜欢 SVG，因为它可以在事后很容易地编辑。

有一些基于字体的解决方案可以让你“输入”时序图。我们找到了 [Xwave](http://www.josephpalmer.com/cgi-local/View_Permalink.cgi?entry=2004/6/30/02:31:40:163) 和[时序图字体](http://www.pcserviceselectronics.co.uk/fonts/index.php)。这些工作，但不是特别灵活；如果你希望某件事在奇怪的时间发生，你就不走运了。此外，这感觉就像一个肮脏的黑客，好像这是一件坏事。

Latex 用户可以使用 [tikz-timing](http://www.ctan.org/tex-archive/graphics/pgf/contrib/tikz-timing/) ，这使得绘制时序图就像在 Latex 中设计一个非常复杂的表格一样有趣(也就是说:一点也不有趣)。另一方面，它看起来很好，非常灵活，输出 PDF，如果有人花时间写一个漂亮的前端，它是可脚本化的。

所以在接下来的一小段时间里，我们将尝试 Wavedrom。

你用什么做时序图？