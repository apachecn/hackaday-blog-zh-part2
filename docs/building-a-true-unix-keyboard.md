# 构建真正的 Unix 键盘

> 原文：<https://hackaday.com/2014/07/28/building-a-true-unix-keyboard/>

![keyboard](img/7c4272bb79249ef88797d16eb962a62d.png)

紧凑型键盘去掉了普通键盘三分之一的按键，现在非常流行，但对[jonhiggs]来说，它们还不够好。这些紧凑的键盘没有注意到 Unix 快捷键的悠久传统——CTRL-A 是 Home 键，CTRL-D 是 Page Down 键。为了修复 Unix 历史上这一可怕的疏忽，[jon]拆开了这些紧凑键盘中的一个，重新连接了开关矩阵，[并制作了他自己的完美键盘](https://github.com/jonhiggs/ml62)。

[jon]使用的键盘是 Filco Minila，这是一款非常好的高质量键盘。在绘制出开关矩阵后，[jon]将所有的开关连接到一个 Teensy 2.0，上面加载了 [TMK 固件](https://github.com/tmk/tmk_keyboard)。这是构建定制键盘的一种非常标准的方式，而[jon]可以只切割一个开关板，安装面板安装开关，然后点对点地连接矩阵和二极管。键盘的外壳是由乐高积木制成的。

因为这是一个真正的现代 Unix 键盘，[jon]需要将这个键盘连接到一个运行他选择的*nix 的机器上。他尽可能用未来的方式来做这件事，用的是 Amazon EC2 实例。这个项目尚未完成，[乔恩]希望添加一个 ARM 开发板、一个 iPad Retina 显示屏、电池和固态硬盘，将它变成一个完全根据[乔恩]的需求设计的自制笔记本电脑。