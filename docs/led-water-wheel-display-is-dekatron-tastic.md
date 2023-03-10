# LED 水车显示器是 Dekatron-tastic！

> 原文：<https://hackaday.com/2014/08/27/led-water-wheel-display-is-dekatron-tastic/>

![led-ring-final](img/05bc88e8e16ea92aeb7f4bc33cdd0c1c.png)

有时候，是简单的事情让人着迷。[JohnS_AZ]已经[创造了一个简单的 dekatron 风格](http://hackersbench.com/Projects/LEDRing/index.html) LED 戒指，但我们似乎无法停止观看他的视频。[约翰的] LED 环开始作为他的 Hackaday 奖参赛作品的视觉指示器，一个[耗水量显示器](http://hackaday.io/project/1460-Remote-Water-Consumption-Display)。从[的网站](http://hackersbench.com/)、[、【约翰】](http://hackaday.com/2014/07/17/thp-hacker-bio-hackersbench/)来看，他有点像个展示狂。谢妮电子管和巨大的时钟是突出的特色。

我们已经看到许多 LED 项目使用可靠的 74xx595 8 位移位寄存器。[John]个人并不喜欢，因为整个芯片只能驱动大约 50mA 的电流。虽然黑客通常会将芯片推过这一限制几次，【John】在德州仪器 [TLC59282 16 通道恒流 LED 驱动器](http://www.ti.com/lit/ds/symlink/tlc59282.pdf)中找到了一款专为该任务设计的芯片。(PDF 链接)虽然比 595 贵，但 59282 让生活更轻松。芯片的电流检测引脚只需要一个电阻，而不是每个 LED 都需要一个限流电阻。59282 还提供空白输入，非常适合 PWM 驱动。

[John]设计了一个简单的 PCB，用 59282 驱动一个由 16 个 led 组成的环。在等待电路板的时候，他为微芯片 PIC16F1509 编写了一些测试代码。[John 的]代码没有优化，但这使得很容易看到他正在向 led 写入哪些位模式。这一切构成了一个很棒的演示，让我们想起了那些古老的迪卡龙电子管。
正是这个演示视频成就了这个项目。点击休息，给它一个手表。经过几天漫长的参赛作品评审，一个真正漂亮的 LED 戒指可能正是医生想要的。

[https://www.youtube.com/embed/L8Dy9vjY-iE?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/L8Dy9vjY-iE?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)