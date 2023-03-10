# 小技巧# 7–MIDI

> 原文：<https://hackaday.com/2014/07/11/the-hacklet-7-midi/>

![7](img/03b9a4378fc08d487d9f619986612df8.png)

本周的 Hacklet 都是关于使用 MIDI 的 [Hackaday.io](http://hackaday.io/) 项目，或者为门外汉准备的[乐器数字接口](http://en.wikipedia.org/wiki/MIDI)。MIDI 从一开始就被设计成一种开放的乐器通信标准。几乎每个主要的仪器公司都参与了标准的设计。MIDI 于 1983 年 1 月首次演示，随后在 8 月发布了通信标准文档。黑客、制造商和音乐人立即开始使用它，使用 MIDI 做一些设计者做梦也想不到的事情。

[![SAMSUNG](img/b0eaca9b2f9eb95d5310eef66e99bf62.png)](http://hackaday.io/project/1700-Cosmic-Ray-(Muon)-81-(9x9)-Pixel-Hodoscope) 【罗伯特】 [9×9 像素μ子探测器/速度镜](http://hackaday.io/project/1700-Cosmic-Ray-(Muon)-81-(9x9)-Pixel-Hodoscope)就是一个很好的例子。[罗伯特]正在使用 18 个盖革米勒管来探测宇宙粒子，特别是[μ子](http://en.wikipedia.org/wiki/Muons)。这些管子被堆叠成两排，这使得他能够使用符合探测。除了绘制一些图表或计算撞击概率，[Robert]还黑进了一个 Korg Nanokey 2 MIDI 控制器，通过 USB 输出与探测到的μ介子相对应的 MIDI 消息。查看他的视频[来看看宇宙音乐的样本！](https://www.youtube.com/watch?v=hulW7-2W7OU)

[![diyMPC](img/0d991c7f87180c60e443e5a2599467ef.png)](http://hackaday.io/project/1601-DIY-USB-MIDI-controller-MPC-style) 接下来是【米歇尔的】 [DIY MPC 风格的 MIDI 控制器](http://hackaday.io/project/1601-DIY-USB-MIDI-controller-MPC-style)。[米歇尔]需要一个简单的低成本鼓控制器，不会吵醒他的邻居。他喜欢 Akai MPC 控制器，所以他推出了自己的控制器。[Michele]研究了力敏电阻，但发现它们非常昂贵。以每个 8 美元的成本来看，他的电阻几乎相当于一个低端 MPC 的成本！[Michele]用一层铜带和 3M [Velostat](http://www.adafruit.com/products/1361) 导电片制作了他自己的感应垫。HCF4067 将所有模拟线路路由至 Teensy 3.0 的单个引脚，然后将模拟电阻输出转换为 MIDI 消息。

[![pic-midi-1vo](img/136855523a602faa20de0f9831a379a4.png)](http://hackaday.io/project/1740-MIDI2VC)【Johan】喜欢他的模拟合成器，希望它们也能说 MIDI。他构建了 [MIDI2VC](http://hackaday.io/project/1740-MIDI2VC) ，一个将 MIDI 转换成 1V/八度音程的电路(类似于 [CV/Gate](http://en.wikipedia.org/wiki/CV/Gate) )。1V/八度音程是一些早期合成器以及许多现代模拟创作中使用的模拟控制系统。音高被分配了电压，顾名思义，每个八度音程是 1 伏。键盘上的 A4 用 4 伏表示，A5 是 5 伏。[Johan]使用微芯片 PIC16LF1823 来接收和转换 MIDI 信号。PIC 将 I2C 数据输出到 MCP4725 DAC，后者驱动模拟端。

[![eldance](img/7db38b1405f0dfd3c086caf111587d6b.png)](http://hackaday.io/project/1558-El-Dance) 早在 [DMX512](http://en.wikipedia.org/wiki/DMX512) 登场之前，黑客们就已经在通过 MIDI 控制灯光了。[Artis]用 [El Dance](http://hackaday.io/project/1558-El-Dance) 延续了这一点，这是一种用于控制舞者佩戴的电致发光电线的无线系统。在功能上类似于[【秋叶的】EL wire 系统](http://hackaday.com/2013/12/10/get-tangled-up-in-el-wire-with-freaklabs/)，【Artis】走了一条成本更低的路线，使用了古老的 NRF24L01 无线电模块。他增加了一个天线，使模块的范围达到 30 米左右。运行舞蹈动作音乐的计算机将链接的发送端视为 MIDI 乐器。标准音符开和关命令激活 EL 线串。

[![midi-vibe](img/8e936b688f2e10dd98fcf78d32a8956c.png)](http://hackaday.io/project/1485-MIDI-Vibrator-Inductor-Synth) 我们最后的黑客来自【Jen】，他建造了一个 [MIDI 振动器感应器合成器](http://hackaday.io/project/1485-MIDI-Vibrator-Inductor-Synth)。[Jen]在一个名为“我的妻子”的实验性乐队中表演，乐器多种多样，包括小提琴和缝纫机。[Jen]一定是[范·海伦的磅饼](https://www.youtube.com/watch?v=o1GJxVmYv-E)的粉丝，因为她用了类似的手法，用了 MIDI 的手法。Arduino 将 MIDI 音符转换为模拟值，然后发送到电机控制板。电机控制器使用 PWM 以正在演奏的音符的频率驱动振动器电机。像所有的 DC 汽车一样，振动器产生大量的电磁噪音，很容易被[珍的]电贝司拾取。

这就是本周的 Hacklet！下周敬请关注来自 [Hackday.io 的更多项目！](http://hackaday.io/)