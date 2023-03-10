# 1768 个发光二极管，因为 96 个还不够

> 原文：<https://hackaday.com/2015/04/17/1768-leds-because-96-just-wasnt-enough/>

有些人会看着挂在墙上播放动画的巨大的 6 ' x4 ' LED 矩阵，并对结果感到满意。但是[本]不是这样的人。最初的 FLED(神奇的 LED 玩意儿)是八排十二个可寻址的 LED，总共 96 个像素。今年春天，他升级了游戏，用 1768 个发光二极管改装了显示屏。

这不仅仅是一个躁动不安的问题，最初的构建遭受了 led 死亡。事实上，我们[因为这个原因](http://hackaday.com/2014/03/06/fail-of-the-week-ws2811-pixel-failure-on-fled/)把它作为本周的*败笔。严格来说，这不是一个业余爱好项目，它挂在 Supplyframe 办公室的墙上，所以经常把它拉下来修理坏掉的零件并不理想。*

为了使 FLED 更加可靠，[Ben]采购了新的 APA102 发光二极管的条带，我们在去年 12 月看到了这些条带。他们使用 SPI 总线，而不是 WS2812 奇怪的时序方案。乍一看，你会认为这意味着比焊接每个原始 96 像素的两面更容易组装。这些确实是带状的，但布局 52×34 仍然意味着焊接到每一行的末端。

为了确保这些行的布局完美，我们投入了很多心血。一片白色泡沫聚氯乙烯作为基底。成排的两端都有接地编织物，一个是电压总线，另一个是地线。它适合原来的丙烯酸外壳，在漫射光线方面做得很好。我亲眼见过，它看起来非常完美！

挑战不仅仅在于这么多像素的物理布局。将数据推送给所有人比用 96 更难。[Ben]从 RaspberryPi 过渡过来。他考虑过使用 Teensy 3.1 和 ESP8266，但这些廉价模块的 WiFi 太慢，无法从远程设备推送帧信息。最终，是比格犬骨黑推动了重生的展示。这是一个很好的选择，因为引擎盖下有足够的电力，可以使用传统的(更快的)WiFi 加密狗。

不要错过休息后的动画演示。

[https://www.youtube.com/embed/ITjyiKbT2sY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/ITjyiKbT2sY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)