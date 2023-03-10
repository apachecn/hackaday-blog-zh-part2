# 宜家 LED 餐桌 Mod 不缺牛逼

> 原文：<https://hackaday.com/2014/02/03/ikea-led-table-mod-doesnt-lack-awesome/>

有些人将宜家 LACK 拉克餐桌视为廉价家具。我们的读者将它们视为一张空白的画布。[Klaas]将 LACK 拉克边桌变成了一个[互动 LED 桌](https://sites.google.com/site/klaasdc/led-table)，配有 144 个 RGB LEDs。在参加了学生 IEEE 分会关于 WS2801 像素字符串的课程后，[Klaas]受到启发，设计了自己的东西。他坐在宜家的拉克餐桌上，开始画草图。他手头实际上没有桌子，所以他不得不根据网站图片和尺寸来推断大小。他计算出的可用尺寸约为 45 厘米，非常接近标准。在进行了一些测试后，[Klaas]确定一个边长为 35mm 的 12×12 的正方形网格将提供足够的分辨率来玩简单的游戏。35mm x 35mm 的网格也足够小，可以让 LEDS 照亮。他用激光切割机从 3 毫米的 MDF 上切割出一个联锁网格。一个带有 144 个 12 毫米 LED 孔的基板也被切割出来，整个组件被粘合在一起。

在照明方面，[Klaas]选择了 WS2812B LEDs，因为它们比 WS2801 couterparts 便宜。WS2812B 还可以轻松插入 12 毫米的孔中。此时,[Klaas]实际上购买了他的宜家桌子，并开始在上面切一个大洞。网格粘在一起，一些铝 L 型清理顶部边缘。驱动所有这些 led 需要一点处理能力，[Klaas]选择了一个 [Teensy](http://www.pjrc.com/teensy/teensy31.html) 3，和众所周知的 [OctoWS2811](http://www.pjrc.com/teensy/td_libs_OctoWS2811.html) 库。他还添加了一个 USB 主机盾，允许他使用 Xbox 360 USB 游戏手柄作为他的控制器。对于软件，他创建了一个简单的俄罗斯方块克隆，并从 Arduino 游戏盾移植了 snake。一个菜单和一些滚动文本将一切联系在一起。唯一需要添加的是一个玻璃面。[Klaas]还没有选定透明或漫射玻璃。我们建议清除，以避免隐藏这个伟大的建设的任何细节。

[https://www.youtube.com/embed/dCHSTi-dWRY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/dCHSTi-dWRY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)