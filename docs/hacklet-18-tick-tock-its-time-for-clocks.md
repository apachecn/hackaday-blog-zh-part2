# 滴答滴答，该是时钟的时间了

> 原文：<https://hackaday.com/2014/10/10/hacklet-18-tick-tock-its-time-for-clocks/>

![18](img/802375923e859fd85db68b17f2e43821.png)

三个字，黑客爱时钟。我们不仅认为数字手表仍然是一个非常好的想法，我们还喜欢各种各样的钟表。这一集的 Hacklet 主要关注我们在 [Hackaday.io](http://hackaday.io/) 上发现的时钟项目。

[![xkcdHardware](img/4471d213d8cf7c5f53e03a559f57bc0a.png)](http://hackaday.io/project/1074) 我们从【rawe】和【tabascoeye】开始，他们都把著名的 XKCD“now”时钟放到了硬件中。[塔巴斯科耶]在他的 [xkcd 世界时钟](http://hackaday.io/project/1167)中使用了步进电机。[rawe]手边没有任何踏步机，所以他从宜家买了一个便宜的挂钟作为他的硬件[xkcd.com/now 钟](http://hackaday.io/project/1074)。现在时钟需要 24 小时运转。宜家只卖 12 小时机芯，所以[rawe]黑进了一个 555 和一些逻辑将时钟的水晶除以 2。他目前正在使用 EEVblog uCurrent 来验证他改进的时钟消耗大约半毫瓦。

[![touchscreenclock](img/c9c2e9bbfb5e66aef6aa0a11fb81569f.png)](http://hackaday.io/project/2785) 接下来是【Craig Bonsignore】和他的[触摸屏闹钟](http://hackaday.io/project/2785)。[克雷格]厌倦了商店买的闹钟，所以他自己做了一个。然后他修改了一下，加了几个功能，继续建！这款时钟的最新版本有一个非常新颖的界面:在双色 LED 矩阵上有一个触摸屏。时钟的其余部分由 Arduino、Adafruit 波盾和 Macetech Chronodot 组成。[Craig]目前正在混合这些开源设计，并为他的时钟构建一个单一的 Arduino 屏蔽。

[![irisledclock](img/683d28f7f064af359a60965cb43fe5c8.png)](http://hackaday.io/project/1237) 【股神扬森斯】带着[虹膜钟](http://hackaday.io/project/1237)走极简路线。Iris 是一圈 WS2812 RGB LEDs。led 灯安装在一块墙面彩色木板的后面，这样你只能看到它们在钟框和墙后面发光。这有助于 WS2812s 在直接观看时产生灼热的视觉效果，即使使用 PWM 调光也是如此。代码主要是 C 与一些 AVR 大会扔在控制发光二极管。[Warren]给了 Iris 8 种不同的时间模式，从小时/分钟/秒到一天中日出和日落标记的百分比。有这么多模式，唯一困难的部分是知道如何读取 Iris 显示的时间！

[![stargate](img/94efeec8aaf0d2c9f62606b3600f08b1.png)](http://hackaday.io/project/1919) 【大卫·霍普金斯】也建造了一座环形钟。他的[星际之门 LED 钟](http://hackaday.io/project/1919)不仅能报时，而且是电视剧中星际之门的伟大复制品。[David]使用四个 Adafruit WS2812 Neopixel 段构建了一个完整的 60 RGB LED 环。星际之门在 Arduino nano 上运行，带有实时时钟芯片以保持准确的时间。光敏电阻允许星际之门在晚上自动变暗。通过一些巧妙的编程，[David]添加了从可视的每小时“钟声”到从 LED 到 LED 的平滑渐变的所有东西。

[![bendulum](img/086de77c4061e7b8ee873962640bd939.png)](http://hackaday.io/project/185)【dehne 1】给我们带来了与[钟](http://hackaday.io/project/185)完全不同的东西。弯曲器是[dehne 1]自己创造的，由一个没有支点的倒立摆组成。倒立摆通过沿着它的长度弯曲来摆动。在[dehne 1]的设计中，弯曲器是由从汽车挡风玻璃刮水器中抢救出来的弹簧钢条制成的。Bendulum 没有机械擒纵机构，而是由 Arduino 感应和驱动的电磁铁。这个项目令人惊讶的部分是[dehne1]没有使用实时时钟芯片。标准的 8MHz Arduino 谐振器在各种温度下进行校准，然后用于校准 bendulum 本身。结果是每天的时钟可以精确到 1 分钟以内。[dehne1]将他的时钟安装在定制的木箱内。我们认为它看起来很棒，想为 Hackaday 总部买一台！

在这一集的黑客攻击中，我们已经使用了足够多的时钟滴答。一如既往，下周见。同样的黑时间，同样的黑渠道，带给你最好的 [Hackaday.io！](http://hackaday.io/)

还想要更多吗？查看我们的[时计列表！](http://hackaday.io/list/2452)