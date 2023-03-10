# WonderSwan 概念验证闪光推车

> 原文：<https://hackaday.com/2014/10/28/a-proof-of-concept-flash-cart-for-the-wonderswan/>

除非你去过日本或者非常热衷于收集复古游戏，否则你可能从未听说过 WonderSwan。这是一款掌上游戏机，在 Game Boy Color 开始显示其年龄之后发布，比 Game Boy Advance 的推出早一点。它在唯一发行的国家卖得相当好，游戏库给人留下了深刻的印象，并且有相当多的自制游戏。然而，实际上运行这些自制游戏是一个挑战:每个 WonderSwan 都有一个内存控制器，将游戏 ROM 映射到 CPU 的内存中。在不知道这个控制器芯片如何工作的情况下，运行家酿墨盒的唯一方法是用一个真正的购物车打开机器，进入系统菜单，然后将购物车换出来。[事实证明有一个更好的解决方案](http://www.986-studio.com/2014/10/28/finally/)，包括对 CPLDs 编程和查看逻辑分析仪的输出。

[Godzil]努力为 WonderSwan 创建闪存推车的第一步是解决盒式磁带连接器的引脚问题——对于没有自制硬件场景的系统来说，这是没有很好记录的事情。这是以通常的方式完成的；[通过大量的带状电缆和耐心](http://www.986-studio.com/2012/08/01/wonder-project/)，这只提供了 WonderSwan 如何与其手推车交互的不完整画面，但在挖掘出[一个官方开发板](http://www.986-studio.com/2014/07/04/new-wonderswan-information-thanks-wonderwitch/)后，【Godzil】能够理解所有的信号。

在为墨盒端口构建分线板之后，[Godzil]连接了一个 DE0 Nano FPGA 板，并查看了所有信号。只需一点点 VHDL，内存控制器就可以被逆向工程和重新实现。[Godzil]已经实现了他的概念验证——视频如下——他项目的下一步将是把它变成一个合适的闪光推车。

[https://www.youtube.com/embed/-HaSt_DgD5g?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/-HaSt_DgD5g?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)