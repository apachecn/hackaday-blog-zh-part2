# 在浏览器中学习 3D 建模

> 原文：<https://hackaday.com/2015/09/03/learn-3d-modeling-in-your-browser/>

如果你有一台 3D 打印机，很有可能你至少见过或听说过 [Tinkercad](http://www.tinkercad.com) 。在网络浏览器中进行设计有利有弊，但是 Tinkercad 非常容易使用，非常适合制作简单的对象。但是，您也可以在浏览器中使用其他 3D 对象设计器。Tinkercad 只是大家似乎都知道的一个。

关于 Tinkercad 我就不多说了，但是如果你没有尝试过，很值得一看。它有一个简单的绘图系统。当你把洞和东西融合在一起时，你可以做出很多形状。校准工具很好，自从 Autodesk 收购了它们(它的 [123d 应用套件](http://www.123dapp.com/)的一部分)，它们不太可能很快倒闭(你可能记得，这几乎发生了)。

如果你正在设计一些伟大的新秘密发明，你可能会回避基于云的设计程序。但是如果你打印出的钥匙链上有你同事的猫的名字，你真的在乎吗？这些基于云的程序大多可以在任何电脑上运行，所以你可以在咖啡店里快速设计，然后回家打印。

[https://www.youtube.com/embed/KCaenAGeK_Q?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/KCaenAGeK_Q?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

生成 3D 对象的程序可以分为两类:可视化的和参数化的。可视化工具强调用鼠标绘制形状，而参数化工具倾向于让你用数字描述你想要的东西。这是你的直觉可能让你误入歧途的事情之一。看起来视觉绘画是一条出路，对吗？人是视觉的。但是大部分人也不精确。例如，如果你想为一个定制的测试设备设计一个前面板，很难让所有的东西都完美的排列在一起，并且间隔均匀。

当然，像 Tinkercad 这样的工具有对齐和间隔工具，这很好。但是对于复杂的设计来说，做一个改变可能会引起一阵鼠标活动。专业 CAD 程序通常通过允许您设置约束来解决这一问题，但这通常不容易学习，而且据我所知，在基于浏览器的工具中是闻所未闻的(Onshape 除外，您将在下面看到)。

与纯视觉方法相反的是像 OpenSCAD 这样的程序。你什么也没画。你用一种看起来像编程语言的东西来描述你的形状，然后你可以看到它的可视化表示，你不能用图形编辑它。你可能认为 OpenSCAD 不是一个基于浏览器的程序。你说得对，但是网上有好几个版本。一个是名副其实的[openscad.net](http://openscad.net)，它可能是最接近桌面体验的。

如果你正确地编写了 OpenSCAD 代码，在这里或那里做些调整没什么。前面板上还需要一个洞吗？添加它和所有其他孔移动调整。然而，并不是每个人都编写灵活的代码。如果你只是硬编码所有的数字，结果甚至比使用可视化工具还要糟糕。

许多可视化工具(包括 Tinkercad)为您提供了至少进行一些参数输入的方法(提示:使用标尺并单击尺寸)，例如，如果您需要制作尺寸完全相同的孔，这可能会有所帮助。但是，设置一组孔的 X 和 Y 坐标，使它们对齐并隔开，仍然是你必须做的事情，要么盯着它，使用一次性对齐工具，要么直接输入数字。

我想收集一些我所知道的基于网络的 3D 设计工具。这个列表并不详尽，我相信评论会指出一些我不知道的。

# OpenSCAD 及相关

我已经提到一些网站在你的浏览器中提供 OpenSCAD。如果您已经在使用 OpenSCAD，当您不在自己的计算机前时，这真的很方便。但是，如果你完全属于视觉阵营，你就不会被打动。OpenSCAD 语言并不是一种完全的编程语言(尽管最新版本越来越近了)。如果你是一个更传统的程序员，有像 [OpenJSCad](http://openjscad.org/) 或 [CoffeeSCAD](http://coffeescad.net/) 这样的选项，这两个选项都提供了类似 OpenSCAD 的功能，更多地针对实际编程的人。

如果你有在 web 服务器上托管自己的 OpenSCAD 私有副本的冲动，看看 [cloudscad](https://github.com/tbuser/cloudscad) 。不过，最近没有更新。

[https://www.youtube.com/embed/XNghpq9sKRc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/XNghpq9sKRc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

# 两全其美？

我对开源并且在浏览器中运行良好的 Shapesmith 印象深刻。好的是，虽然它是可视化的，但有一个检查器窗口，让您可以轻松地直接输入参数。如果你不喜欢创建帐户，你可以尝试不注册的网站，尽管如果你不创建一个帐户，你会丢失你的工作。
像 Tinkercad 一样，Shapesmith 允许你设置一个工作平面。然而，如果它有工具来对齐或分隔对象，我找不到它们。左图显示了导入 Shapesmith 并进行调整的 STL 文件。

[https://www.youtube.com/embed/gcw4bHAp55o?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/gcw4bHAp55o?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

# 3dmitn(三聚氰胺)

我第一次了解到 [3D Tin](http://www.3dtin.com) 是因为它出现在 Chrome 商店。它看起来真的很好，它能够绘制 3D 打印项目或只是做一般用途的 3D 建模。它有一个有点古怪的用户界面，试图在视觉和参数之间架起一座桥梁。
当你创建一个形状时，你可以输入尺寸，例如，数字。调整大小时，使用滑块而不是抓取对象手柄。这需要一些时间来适应，但它的工作。它确实提供了方便的对齐和分组工具。右图显示了一个简单的 3Dtin 对象。

[https://www.youtube.com/embed/m8dt0ZEd8CE?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/m8dt0ZEd8CE?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

# 光猪六壮士:昂沙佩

虽然这篇综述中的大多数工具都很容易使用，但 Onshape(目前处于测试阶段)是一个成熟的专业 CAD 软件包。如果你需要那种力量，那很好。但是，如果“填充草图”这个术语对你来说没什么意义，那就做好陡峭的学习曲线的准备吧。

我之前提到过，专业的 CAD 工具使用约束和参数来获得与你在正确编写的 OpenSCAD 脚本中获得的效果相同的效果。Onshape 支持约束和参数。观看他们的[视频](https://www.onshape.com/videos/tutorial-parametric-and-feature-based-modeling)可能会给你一个使用这种设计技术的学习曲线的想法。当然，如果你已经习惯了其他软件包的这种建模方式，你会发现 Onshape 对于一个基于浏览器的应用程序来说非常令人印象深刻。
虽然可以用 Onshape 进行 3D 打印，但是完全可以。免费计划给你有限数量的私人绘画，但实际上无限数量的公共绘画。左图显示了 Onshape 中的一个复杂零件。

[https://www.youtube.com/embed/fPTCgWc3Ouw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/fPTCgWc3Ouw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

# 打破桌面

这些工具中有任何一个能与桌面解决方案相媲美吗？看情况。如果你愿意花时间去学习，Onshape 是非常强大的。浏览器中的 OpenSCAD 与桌面上的 OpenSCAD 非常相似。

也许其他工具确实缺少一些功能。然而，对于你通常 3D 打印的东西，这些工具中的任何一个都可以完成这项工作。我知道外面还有其他人。请在评论中说出你最喜欢的(甚至是最不喜欢的)。

我会在实际项目中使用在线 CAD 吗？也许吧。我现在使用在线邮件应用程序。我偶尔也会使用文字处理等在线办公应用。我觉得主要归结于我对后端的信任程度。如果我拥有后端(这些工具中的一种可能性)或者我信任的公司(可能有点愚蠢)拥有它，并且有合理的隐私控制，为什么我不应该使用在线工具呢？另外，我认为巴顿斯先生的钥匙链落入坏人之手的可能性不大。