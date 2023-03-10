# 由 Arduino 驱动的手持游戏系统

> 原文：<https://hackaday.com/2014/06/22/handheld-game-system-powered-by-arduino/>

![DIY Handheld Game System](img/b653550a1e18de17a9ea5bf4a3cf4a1d.png)

如今，在旅途中玩游戏已经很容易了。如果你有一部智能手机，你就已经准备好了。不过，这并不意味着你不能享受设计和构建自己的便携式游戏系统的乐趣。

就这么做了。他首先从 Adafruit 购买了一个小型的液晶显示屏。就屏幕而言，他选择的屏幕是低功耗的，因此它非常适合这个项目。用快速演示程序测试完屏幕后，就该开始设计电路板了。

[randrews]用 Eagle 设计电路。他手动路由所有的跟踪，以避免自动路由有时可能导致的任何奇怪的问题。他通过将屏幕安装在 ATMega 芯片和其他支持组件的顶部，有效地利用了电路板上的空间。屏幕被设计成可以插入和拔出插座，这样它就可以被移除以接触到芯片。[randrews]需要能够接触到芯片，以便为不同的游戏重新编程。

电路板设计完成后，[randrews]用他的 Shapeoko CNC 铣床从覆铜板上切割下来。他警告说，你需要小心这样做，因为吸入玻璃纤维粉尘对健康长寿有害。一旦板被铣出，[randrews]使用一个小 Dremel 钻床钻所有的孔。

谜题的最后一部分是弄清楚电力状况。[randrews]为此设计了第二个更小的 PCB。电源板装有两节 3V 纽扣电池。Arduino 需要 5V 电压，所以[randrews]必须使用电压调节器。该电源板还包含整个系统的电源开关。

电源板经过打磨和组装。然后是做一些测量的时候了。[randrews]测量了电流消耗，计算出使用两个 3V 纽扣电池，他应该能够获得大约 15 小时的游戏时间。考虑到尺寸，还不错。

[via [Reddit](http://www.reddit.com/r/electronics/comments/28tfnw/i_made_a_handheld_game_system_this_weekend_xpost/ "Reddit.com")