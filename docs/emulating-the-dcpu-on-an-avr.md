# 在 AVR 上模拟 DCPU

> 原文：<https://hackaday.com/2012/07/25/emulating-the-dcpu-on-an-avr/>

[![](img/58149a4612c9680e1fb475b94072413d.png "DCPU")](http://hackaday.com/wp-content/uploads/2012/07/dcpu.jpeg)

[skywodd]刚刚完成[他自己的 DCPU 模拟器](http://skyduino.wordpress.com/2012/07/25/avr-emulateur-dcpu-16/)(法语，[翻译](http://translate.google.fr/translate?sl=fr&tl=en&js=n&prev=_t&hl=fr&ie=UTF-8&layout=2&eotf=1&u=http%3A%2F%2Fskyduino.wordpress.com%2F2012%2F07%2F25%2Favr-emulateur-dcpu-16%2F&act=url))基于[notch]即将推出的游戏，0x10c。[skywodd]构建的巧妙之处在于，他的仿真器使用的是低端的 ATMega328，与(某些)Arduinos 中的微控制器相同。

DCPU 规范介绍了任何 DCPU 仿真器所需的操作。这里有很多疯狂的东西——除法指令只需要 3 个时钟周期，使用溢出作为进位条件，完全没有 JMP 指令——但[skywodd]能够从 [DCPU 工作室](http://badsector.github.com/dcpustud/)和 [VGA 接口](http://microvga.com/)中梳理出一些东西

这个仿真器中的一切都是建立在无焊试验板上的，但是 ROM 和 RAM 还没有完成。到目前为止，一切都由 328 处理，在微处理器上使用 478 字节的 RAM。

当我们听到 0x10c 的风声时，我们承诺将举办一场 DCPU [最佳物理实现的竞赛，而[skywodd]的构建开始看起来像是获奖作品的开始。老实说，我们不知道*什么时候会举办这场比赛，但它可能会在第一个可玩版本发布后不久。如果你想加快进度，就去 bug [notch]*](http://hackaday.com/2012/04/08/getting-12-year-olds-to-learn-assembly-programming/#comments) 吧，因为显然滥用 Twitter 会加速软件开发。