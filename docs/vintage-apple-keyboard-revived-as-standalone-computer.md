# 老式苹果键盘作为独立电脑复活

> 原文：<https://hackaday.com/2014/12/10/vintage-apple-keyboard-revived-as-standalone-computer/>

我们的许多读者都熟悉经典 PC 键盘的黄金标准——带有开关的碉堡，即 IBM 型键盘。M 型键盘的 Apple contemporary 是 Apple Extended Keyboard，它们同样受到各自发烧友的追捧。尽管这款代号为“Saratoga”的键盘在近 25 年前就已经停产，而且与过去 15 年里生产的任何产品都不兼容，但它被广泛认为是苹果有史以来最好的键盘。

[以斯拉]有一个爱好，使这些古老的心脏现代化，并挽救他们过早过时。在[一个有极好记录的教程](http://straypoetry.com/project/raspberry-pi-inside-a-vintage-mechanical-apple-extended-keyboard/)中，他不仅展示了如何将它们转换成 USB(一个[流行的](http://hackaday.com/2011/03/10/keyboard-converter-2-pack/)和琐碎的黑客)，还教你如何以及在哪里走私一个树莓派。

拆卸后，该项目只需要一点点凿和 Dremel 工作之前，烙铁出来。[Ezra]相当细致地移除或重定向 Pi 的连接器，并硬连线内部。只需要从原始键盘上追踪 3 个引脚，而[Ezra]选择的 ADB –> USB Rosetta Stone 是运行在 Atmega 32u4 克隆版上的 [Hasu 转换器](http://github.com/tmk/tmk_keyboard/tree/master/converter/adb_usb)。在权衡成本、范围和 Pi 功耗后，他选择了 TP-LINK WN722N 作为他的 WiFi 解决方案，该解决方案也藏在箱子里。一个上拉电阻就完成了，当[Ezra]第一次插上电源时，他很高兴地发现它工作了。

这个时代的键盘使用真正的瞬时开关，每次按键可以听到两次滴答声。在我们这个屏幕为钥匙庆祝触觉约束缺失的世界里，使用像 M 型或 AEK 这样的野兽来迫使晶体管执行你的命令，就像在玩激光游戏时打散弹枪一样——可笑的迟钝，但令人愉快的机械。

如果你想扩大[Ezra]的修补范围，他已经列出了一个愿望清单:一个切换开关，将 Pi 切换回普通的 USB 键盘，一个内部 USB 集线器和一个电源开关。

休息后听听 AEK 的视频(或者在你午睡时循环播放，让它听起来更有效率)。

[https://www.youtube.com/embed/qxSz9IdjTWw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/qxSz9IdjTWw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)