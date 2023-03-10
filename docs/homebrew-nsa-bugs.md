# Homebrew NSA Bugs(美国国家安全局)

> 原文：<https://hackaday.com/2014/07/10/homebrew-nsa-bugs/>

![NSA](img/28f883f5adb758d4b670c4bc214027e0.png)

多亏了(爱德华·斯诺登),我们有了一个巨大的、公开的目录，里面有美国国家安全局使用的非常非常有趣的电子窃听工具。从不到一便士的极其复杂的 ARM/FPGA/Flash 模块到可以在 8 英里外安装 Windows 系统后门的机器，这个国家的间谍都可以获得，现在，[装备充足的电子爱好者可以建造自己的](https://www.youtube.com/watch?v=EOD1yHnerXg)。

[GBPPR2]最近几个月一直在查看 NSA 的 ANT 目录，构建一些更简单的基于无线电的 bug。上面链接的窃听器代号为 LOUDAUTO，这是一个相对简单(和便宜)的雷达反射器，允许任何人用硬件照亮一个简单的电路来获得音频。

在[GBPPR2]的构建列表上还有 [RAGEMASTER](https://www.youtube.com/watch?v=DDlsbNjqBOc) ，这是一种适合 VGA 电缆的设备，允许远程查看单个 VGA 颜色通道。

这两个错误背后的基本原理是逆反射，被美国国家安全局描述为一种光电设备。这些器件背后的基本原理是 bug 中的 FET，以及连接到漏极的天线。光电二极管照亮这个天线，发送到 FET 栅极的 PWM 信号调制返回的信号。在接收端有一点软件定义的无线电，您就有了自己的个人安全管理。

这些都是非常酷的东西，但在美国国家安全局的目录中有一些条目根本不涉及无线电。一种叫做 IRATEMONK 的设备在硬盘控制器芯片中安装了后门。有趣的是，Hackaday favorite 和现任 Hackaday Prize 评委[Sprite_TM] [做了一件非常相似的事情](http://hackaday.com/2013/08/02/sprite_tm-ohm2013-talk-hacking-hard-drive-controller-chips/)，只是没有，你知道，真的很粗略。

虽然我们不喜欢任何人实际使用这些设备的想法，但国家安全局的蚂蚁目录仍然是项目想法的沃土。

[https://www.youtube.com/embed/EOD1yHnerXg?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/EOD1yHnerXg?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[https://www.youtube.com/embed/DDlsbNjqBOc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/DDlsbNjqBOc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[https://www.youtube.com/embed/rPQmIYb5E2o?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/rPQmIYb5E2o?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)