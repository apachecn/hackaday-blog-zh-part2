# Hackaday 68k:一个新的 Hackaday 项目

> 原文：<https://hackaday.com/2014/02/20/hackaday-68k-a-new-hackaday-project/>

众所周知，黑客喜欢复古电脑、经典硬件和复古技术。既然我们已经有了一个展示长篇项目的好方法，我们把我们的爱和一个新的构建结合起来才是有意义的。在接下来的几个月里，我将开发一台基于摩托罗拉 68000 CPU 的自制电脑，记录过程中的一切，并构建一个非常强大的硬件，最终托管一些黑客网页。我已经让[在项目](http://hackaday.io/project/5-MC68000-Backplane-Computer)上有了一个坚实的开端，并将在我们的首页上发布，讨论已经在进行的主要部分，以及那些尚未到来的部分。

我们接手这个项目有几个原因。除了少数例外，我们看到的大多数自制项目都是基于 8 位微处理器，特别是 6502 和 Z80。16 位和 32 位 CPU 实际上并不难使用，如果我们能够引领 68k、65816 甚至 386(！)，我们都赞成。此外，有人建议我们在复古硬件上托管[hack aday 复古站点](http://retro.hackaday.com/)，还有什么更好的方法可以通过在我们的新项目托管站点上记录构建来做到这一点呢？

这是对这个项目的一个非常简短的介绍。让我们仔细看看我们将使用什么样的硬件，我们将运行什么样的软件，以及您能提供什么帮助。

虽然这篇文章只是想对这个项目的未来做一个大致的概述，但是有一些细节是板上钉钉的:

#### 首先，硬件

你可能想知道这个新项目将采用什么样的硬件，以及我打算如何将想法和原理图快速转化为功能电路。为此，现在是要点时间:

*   ##### Backplane and winding design

[![Backplane for Hackaday 68k](img/c140742d3bfb908458d36e4dac505f8b.png)](http://hackaday.com/wp-content/uploads/2014/02/backplane-design.png)

Backplane for Hackaday 68k

这台计算机将被构建在单独的板上，分别用于 CPU、RAM、ROM 和我们想出的任何其他外围设备。所有的连接都是绕线的。这有几个原因。首先，*如果你有绕线插座* *、电线和工具*，这是一种比面包板更好、更容易的电路原型制作方法。第二，就是这么经典；68000 于 1979 年发布，当时这是制造一次性电脑的方式。是的，我们最终会制造一些 PCB，但你不能为了原型制作的方便而采用绕线设计。

*   ##### Motorola 68000 CPU

为什么是 68k？我们看到许多复古和自制计算机出现在 tip line 上，但除了少数例外，它们都是 8 位 CPU，如 6502、6809 和 Z80。68k 是 16 位时代第一款受欢迎的 CPU，最终进入了 Amigas，最初的 Mac，Sega Genesis/Megadrive，大量的街机游戏和早期的 UNIX 工作站。这是一个令人惊讶的，优雅的芯片，可以用作现实世界中计算机的大脑，做一些有用的事情。

*   ##### Four megabytes of memory

[![Ram Bank Design](img/6f730badc3f0945c6c7ae5616974f1a7.png)](http://hackaday.com/wp-content/uploads/2014/02/ram-bank.png)

Ram Bank Design

是的，你没看错。很疯狂，不是吗？凭借 24 位地址空间，68k 可以寻址高达 16 兆字节的 RAM，而无需存储体切换。与 6502 和 Z80 的 64 *千*字节的地址空间相比，很容易看出 68k 的能力要大得多。此外，对于现代 SRAMs，获得零等待状态是小菜一碟。

*   ##### Yamaha V9938 video display processor

当然，这台电脑将需要某种视频输出，为此我们已经使用了在 [MSX2 家用电脑](http://en.wikipedia.org/wiki/MSX2)中找到的相同视频芯片。我预计这主要用于 80×24 文本模式，但这种芯片也给我们一些非常体面的 16 位图形的能力。

*   ##### Ethernet

*   ##### Compact flash memory /IDE hard disk

*   ##### PS/2 keyboard

*   ##### Maybe it's a 6581 SID chip?

这个项目的最终目标是建造一台非常酷的复古电脑，能够托管 [Hackaday 的复古网站](http://retro.hackaday.com/)。只有放置以太网和某种形式的存储才有意义。很明显，我们需要一个键盘，如果没有 Commodore 64 的声音芯片，任何现代的改装电脑都是不完整的。

#### 一些软件怎么样？

TL；软件的 DR 是:“UNIX 风格的东西，带 C 编译器。”

在这台计算机上安装 68k C 编译器并不难，但 UNIX 很难。第一批 UNIX 工作站使用了*两个*68000 CPU——一个用于正常处理，另一个用于在发生页面错误时重置第一个 CPU。把一个*NIX 放在没有虚拟内存或 MMU 的东西上当然是可能的，但是这是一个很大的工程，我不想进入。一个更好的解决方案是 [uCLinux](http://www.uclinux.org/) 。它是为嵌入式系统设计的，有几乎所有的端口，包括 68000。一个 C 编译器和一个文本编辑器是一台功能齐全的计算机所需要的。

#### 我们将何去何从

这只是最终会成为一篇非常非常长的构建日志的第一篇文章。这也是对我们新的 [Hackaday 项目网站](http://hackaday.com/2014/02/18/hackaday-launches-our-own-hosting-site/)的一个巨大考验，大部分开发将在这里进行。你可以在这里查看当前的构建日志，当然也可以使用非常酷的侧边栏评论功能来指出更好的解决方案、电路和代码。

#### 你能做什么

如果你想在现在和下一篇文章之间提供帮助，[看看 Hackaday 项目的构建日志](http://hackaday.io/project/5-MC68000-Backplane-Computer)，留下评论，如果有什么事情真的让你很烦，给我发电子邮件。如果你真的很有野心，那就克隆一个吧！我正在把所有的图表[放到 Github](https://github.com/bbenchoff/BackplaneComputer) 上。最后一件事。我想为 [Apex 电子](http://hackaday.com/2014/01/21/apex-electronics-your-souce-for-oscilloscopes-and-drop-tanks/)提供一吨绕线插座而欢呼。

此外，我很想制作几个视频，展示我如何解决在线仿真器不可避免的问题。如果有人知道哪里可以买到福禄克 9010a，9000-68000 pod，或者有更好的冰的想法，请在评论中留言。

为接下来的几篇文章做好准备:查看 Hackaday 68k 的机械设计，并闪烁带有 24 位地址总线的 LED。