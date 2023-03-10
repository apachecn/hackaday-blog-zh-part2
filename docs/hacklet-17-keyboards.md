# hacklet 17–键盘

> 原文：<https://hackaday.com/2014/09/26/hacklet-17-keyboards/>

本周在 Hacklet 上，我们将展示 Hackaday.io 中一些最好的键盘技巧！

黑客对他们的键盘很着迷。每个人都有自己的喜好，而这些喜好千差万别。机械、触感柔软、符合人体工程学、QWERTY、DVORAK、chorded，凡是你能想到的，都有一个黑客、创客或者工程师喜欢它，或者绝对讨厌它。对一些人来说，没有一个商业产品是完美的。尽管如此，一切都没有失去，因为自定义键盘只是一个黑客了！

[![ergo60](img/7a16730eb51e09790c4a0f41131f9a4e.png)](https://hackaday.io/project/448)

[沃伦扬森斯]用他的 60 键人体工程学键盘 [Ergo60](https://hackaday.io/project/448) 开始工作。[Warren's]布局是一对 25 个键的手簇，每个键有一个匹配的 5 个键的拇指簇。这种布局最大限度地减少了手腕的横向运动。通过减少的键数和堆叠的键，用户的手永远不会离开主行。[Warren]为 Ergo60 生产他自己的 PCB。一个运行 [TMK](https://github.com/tmk/tmk_keyboard) 分叉的 Teensy 2.0 充当 Ergo60 的控制器。[沃伦的]是运行樱桃黑色开关和他的键帽是从签名塑料。[Warren]目前正在使用 Ergo60 作为他的日常驱动程序，所以他设置“已完成项目”标签也就不足为奇了。

[![keycaps](img/c7387a5d4979600212f8c4de0aa9d571.png)](https://hackaday.io/project/1506)

有人说他根本不需要键盘，他的心跳听起来就像 IBM 的 m 型电脑。我们只知道他叫布莱恩·本切夫。[布莱恩的]创造了一对极简键盘项目。[不开心的黑客键盘](https://hackaday.io/project/1265)带我们回到基础。毕竟，计算机运行在 1 和 0 上，对吗？一个人还需要什么？显然只是一个空格和回车。不开心黑客键盘用的是一个带 V-USB 的 ATtiny85 作为控制器和接口。钥匙是樱桃 MX 蓝调。键帽是由 Shapeways 打印的【布莱恩的】自己的 [Hackaday Cherry MX 键帽](https://hackaday.io/project/1506)。

[![zxkeyboard](img/0a66d14c69b0dc20423055418d87c6b1.png)](https://hackaday.io/project/2076) 整整一代黑客不知道在小小的橡胶键盘上打字的快乐。(Alistair MacDonald)旨在解决这个问题，所以他用他的 [ZX 键盘](https://hackaday.io/project/2076)把一台旧电脑变成了一个键盘。[Alistair]从一个破碎的 ZX 光谱开始。他去掉了原来的电子设备，添加了一个运行 V-USB 库的 Ardunio Pro Mini。[Alistair]直接将键盘的行和列 I/O 线连接到他的 Arduino。其结果是一个键盘，这是完美的手机，树莓派和类似的大小。

[![chordkey](img/8c332ada6181086203a6f57878f7fab2.png)](https://hackaday.io/project/2115) 【伺服】教我们用[和弦键](https://hackaday.io/project/2115)打字的新方法，他的和弦键盘项目。和弦键应该用在左手上。五个手指按钮和三个拇指按钮就可以调出 64 个不同的字母和符号。[Servo]利用 ATmega32U4 供电的 Sparkfun pro micro 来控制他的键盘。Chordy Key 是一个概念证明，但随着[Servos]使用 3D 打印部件，Chordy Key 看起来已经为你的下一个可穿戴计算项目做好了准备！

[![chord2](img/fb096a145470c5cc5a2c7f6204ca0070.png)](https://hackaday.io/project/1321)【jmptable】也在致力于和弦键盘的设计。[和弦键盘](https://hackaday.io/project/1321)仅使用 7 个键来发送整个 ASCII 字符集和一些控制组合。[jmptable]使用 ATmega328P 作为他的处理器。不过和弦键盘没有连线。RN-42-HID 模块提供了与世界的蓝牙连接。

[jmptable]提供了他的研究的大量细节，包括他的目标之一是在 Gameboy Advance 中添加和弦键盘。键盘本身将被安装在游戏盒的脊柱上。我们希望看到这个想法实现，[伺服]！

[![mighty](img/80f98e659b0217eb4dbb7b84380f606a.png)](https://hackaday.io/project/203) 最后我们有了【Gertlex】，他只想在键盘上嵌入一个滚轮。他在苹果大老鼠的帮助下到达那里。[苹果鼠标滚动球键盘](https://hackaday.io/project/203)是那些看起来像它原始设备的黑客之一。[Gertlex]在 Targus 超薄 USB 键盘上钻了一个洞，正好在 ESC 和 F1 键之间。他把他的苹果鼠标上的滚动球放进了洞里。电子产品就像将鼠标和键盘插入同一个 USB 集线器一样简单。这种设计的唯一缺点是[Gertlex 的]键盘识别速度不够快，无法在启动过程中发送按键。

对于这一集的黑客攻击来说，这已经足够了。一如既往，下周见。同样的黑客时间，同样的黑客频道，带给你最好的 Hackaday.io！

*更新——点击这里查看我们的[键盘列表](http://hackaday.io/list/3097-Keyboards)！*