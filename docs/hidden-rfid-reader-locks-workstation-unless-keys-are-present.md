# 除非有钥匙，否则隐藏的 RFID 阅读器会锁定工作站

> 原文：<https://hackaday.com/2013/09/07/hidden-rfid-reader-locks-workstation-unless-keys-are-present/>

我们不知道[克里斯托佛·马歇尔]是如何在工作中找到空闲时间的，但他利用这些时间来加强他的计算机安全。以上是完成的项目。这里确实没什么可看的。他安装了一个隐藏的 RFID 阅读器，可以锁定和解锁他的工作站。

系统的安全性依赖于 xscreensaver，它已经内置了密码保护锁功能。当标签从阅读器的字段中移除时，它使用 Perl 脚本启动屏幕保护程序。

但是从屏保中醒来有点棘手。该软件包不允许您从命令行唤醒它——很可能是出于安全考虑。他发现 xdotool 在这里非常有用。这是一个命令行工具，模拟键盘和鼠标输入。他的脚本检测 xscreensaver 密码提示何时出现在屏幕上，并使用 xdotool 填写[Kristoffer 的]密码。因为脚本知道什么有焦点，所以它不会不小心泄露你的密码。

休息后，请查看剪辑中的完整设置。

[https://www.youtube.com/embed/IIEdExAOXf0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/IIEdExAOXf0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)