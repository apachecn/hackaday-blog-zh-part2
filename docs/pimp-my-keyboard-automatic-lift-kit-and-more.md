# 皮条客我的键盘:自动升降套件和更多

> 原文：<https://hackaday.com/2013/11/24/pimp-my-keyboard-automatic-lift-kit-and-more/>

![Cherry-keyboard-with-lifts](img/5de7c679df8c2289ee7b2153de722b08.png)

想知道什么是起重工具吗？你知道那些能弹跳的低轮车吗？这就是这个黑客的想法。[Justblair]在他的樱桃色 G80 上增加了自动高度调节功能，同时还隐藏了其他一些额外功能。由于这个模型的机箱内有相当大的空间，他可以隐藏所有东西，只保留一根线来运行它。

当然，吸引你眼球的是键盘自动上升到打字高度的能力。这是通过几个伺服电机和一些 3D 打印的替代脚来完成的。有一些打嗝的方式与动力不足的伺服系统，但膨胀到一些 HXT 900 9G 模型提供更多的权力比目前必要的。自动功能归功于一个电容传感器，该传感器由一根环绕键盘周边的导线构成。

当然，要监控传感器和驱动伺服系统，你需要某种大脑。为此，[Justblair]配备了一个 ATmega32U4 分线板。因为他无论如何都必须接入 USB 来供电，所以他添加了一个 USB 集线器，并将其中一个端口路由到键盘的左侧，作为连接其他外围设备的便捷方式。甚至有空间包括一个 RFID 阅读器，他用它来解锁他的会话(类似于今年早些时候的桌面安装)。硬件方面仍有很大潜力。为了使未来的改进更容易，黑客包括一个 IDC 插座作为辅助端口。

[Justblair]很好地分享了他的作品。他的帖子链接到一个 Github repo 的代码和一个 Thingiverse 的 3D 打印腿项目。没有下面的演示视频，它是不完整的。

[https://www.youtube.com/embed/yMt1YARdvRQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/yMt1YARdvRQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)