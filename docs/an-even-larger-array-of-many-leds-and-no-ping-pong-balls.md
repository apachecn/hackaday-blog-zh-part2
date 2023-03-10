# 一个更大的 led 阵列，没有乒乓球

> 原文：<https://hackaday.com/2013/12/20/an-even-larger-array-of-many-leds-and-no-ping-pong-balls/>

![Color Led Matrix](img/f275702bdb20aecd6445730acb7680b3.png)

[乔治]用他最新的 RGB LED 面板走上了职业道路。几年来，我们已经记录了[乔治]迈向 led 涅槃之地的旅程。他从一个由许多乒乓球组成的 [8×8 彩虹板](http://hackaday.com/2012/01/08/rainbow-board-of-many-ping-pong-balls/)开始。当这还不够时，他把赌注增加到一个 [32×16 的乒乓球阵列](http://hackaday.com/2012/07/27/a-much-larger-rainbow-board-of-many-ping-pongs/)。仍然不满意，[George]现在已经将尺寸增加到两个 20×15 的面板，总共 600 个 led。虽然这只是一个适度的规模增加，从以前的化身，这里的主要变化已经在阵列的设计和建设。

[George]发现自己在一些专业场合使用 LED 面板。移动和装配面板的压力暴露了几个设计缺陷。点对点分立 LED 设计容易短路，导致通过在黑暗的俱乐部中拨弄电线来排除故障。控制代码也是 solderlab 代码、[George]代码和各种脚本的混合体。甚至商标乒乓球光扩散也是一个问题，因为它们造成了火灾隐患。[George]吸取了第一个和第二个 LED 阵列的所有经验，开始了新的设计 MX3。板框是由一家专业金属商店建造的。从一个方形钢管骨架开始，和铝板外壳焊接就位。钢管为任何数量的索具选项提供了一个挂载点。前面板是经过防火涂料处理的[中密度纤维板](http://en.wikipedia.org/wiki/Medium-density_fibreboard)。

电子设备也发生了变化。单个的 RGB 发光二极管不见了。[George]已改用常见的 WS2812 LED 灯串。安装在面板上的 Raspberry Pis 控制 LED 灯串。通信是通过 [Art-Net](http://en.wikipedia.org/wiki/Art-Net) 进行的，这是舞台灯光中常用的 [DMX512](http://en.wikipedia.org/wiki/DMX512) 协议的以太网实现。最后的结果[看起来棒极了](http://www.youtube.com/watch?v=ql9tu1-xCWI)。我们对[乔治]在如此年轻的年龄(去年六月他才 16 岁)所取得的成就印象深刻。

[https://www.youtube.com/embed/orFe21x2iiU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/orFe21x2iiU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[https://www.youtube.com/embed/ql9tu1-xCWI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/ql9tu1-xCWI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

【谢谢特里！]