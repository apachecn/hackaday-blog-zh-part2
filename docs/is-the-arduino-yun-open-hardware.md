# Arduino 云是开放硬件吗？

> 原文：<https://hackaday.com/2015/02/24/is-the-arduino-yun-open-hardware/>

根据[Squonk42]，[没有](http://www.wifi4things.com/arduino-yun-what-is-under-the-hood/)。我们认为他可能是对的。

Yun 是一款 Arduino Leonardo，内置 Atheros AR9331 WiFi SoC。这是一个好主意，将 Arduino 与一个能够运行 OpenWRT 的微型 WiFi 路由器配对。但这怎么就不再是开源硬件了呢？尝试获得一个可编辑的板布局。你不能。

或者至少[Squonk42]不能。2013 年 9 月，[Squonk42] [在 Arduino 论坛](http://forum.arduino.cc/index.php?topic=187766.0)上发帖请求 Arduino Yun 的原理图和可编辑的设计文件，他仍然没有收到这些文件，甚至没有得到回复。

现在这家伙不懒散了。他负责 TP-Link TL-WR703N 袖珍路由器的[最完整的逆向工程，这并非巧合，它是基于 Atheros AR9331 的参考设计。这就是 Arduini 人遇到麻烦的地方。](http://squonk42.github.io/TL-WR703N/)

[Squonk42]的假设是，在这种情况下，当面对一个超级复杂的硬件和一个潜在的棘手的无线电布局时，Arduino 一定会做任何“理智的”工程师都会做的事情:只需使用参考设计(Atheros AP-121)。业内其他人都是这么做的。这很聪明，只有消费电子行业的其他公司没有声称自己是开源硬件，而参考设计受到 NDA 的保护。

所以看起来 Arduino 的手被绑住了。他们，或者他们的伙伴[狗猎人](http://www.doghunter.org/?portfolio=arduino-yun)，要么签署了 NDA，要么下载了在互联网上流传的参考设计的 PDF 文件。不管怎样，[都很难在知识共享署名共享许可下发布设计文件。](http://arduino.cc/en/Main/FAQ)

对于 Arduino 人来说，这是一个策略的改变还是他们只是犯了一个错误？在他们回复之前我们不会知道，而答案将在一年半后揭晓。让我们看看我们能做些什么。谁知道呢，也许 Arduino 可以依靠 Atheros 来打开他们的参考设计？这已经是公开的秘密了。

但是，在你点亮你的开源硬件的干草叉，磨亮你的火把之前，通读一下[Squonk42]的案例，然后挖掘他所链接的主要来源，以做出你自己的决定。如果你自己做，你会让你的情况更有说服力。

祝你好运，[Squonk42]！我们希望你至少能得到你的答案。即使你已经知道了。