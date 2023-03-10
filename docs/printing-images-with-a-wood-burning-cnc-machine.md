# 用燃木数控机床打印图像

> 原文：<https://hackaday.com/2013/01/11/printing-images-with-a-wood-burning-cnc-machine/>

![printing-images-with-a-wood-burning-cnc-machine](img/01ed85b2f87d21934eff84e0a0ddd3c2.png)

为了澄清标题中的任何混淆，[这台燃烧木材的数控机床](https://github.com/grantbrown/Wood-Burning-Robot)靠电力运行。木材燃烧器充当打印头。就是场地右上方那个看起来有点像烙铁的东西。在这种情况下，它被用来像一个点阵打印机。

我们认为这是半色调印刷的一种形式，尽管它不会产生我们在基于工厂的半色调技术中看到的均匀性。[随机样本]用木头、抽屉滑轨和带齿带的步进电机制造机器。他的 Python 脚本获取一幅图像并将其转换成一个文件，该文件可用于引导机器的三个轴。Arduino 通过 USB 连接接收这些命令。每幅图像打印在一个网格中，较暗的像素是通过让热尖端与木材接触更长时间而产生的。

不要错过跳转后嵌入的示例视频。

[https://www.youtube.com/embed/i0HE7dAw2ns?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/i0HE7dAw2ns?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[感谢伊恩通过 [Reddit](http://www.reddit.com/r/arduino/comments/16bwrt/arduino_wood_burning_robot/)