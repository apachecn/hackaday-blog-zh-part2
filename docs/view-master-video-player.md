# 查看-主视频播放器！

> 原文：<https://hackaday.com/2013/11/13/view-master-video-player/>

![view master 3d video player](img/d7000ef544653aca54b159fee32254c7.png)

[Alec]刚刚给我们发来了他正在做的这个伟大的项目。将一台 50 年代早期的古董 View-Master 转变成一台能够读取迷你 CD 的现代 3D 视频播放器。

大多数 View-master 都没有太多的空间进行修补，更不用说添加一个树莓 Pi、两个显示器和一个 CD 驱动器了，所以[Alec]发现这个模型时真的很幸运——配有灯和 D-cell 电池组。巨大的空间！他最初打算从中国购买一些便宜的数码相框液晶显示器，但很快意识到制造这些东西不值得，所以他从 Adafruit 购买了一些 0.9 英寸的有机发光二极管显示器。尽管如此，他仍然忘记检查他们是否有树莓 Pi 的驱动程序，并最终走上了另一条弯路[修改 FBTFT 驱动程序](https://github.com/notro/fbtft/pull/50)以使其全部工作。

头痛过后，他进入了有趣的部分——把所有的硬件都塞进去。他在易贝买了一个便宜的笔记本电脑 CD 驱动器，发现使用 80 毫米迷你 CD 标准，光盘正好可以放在 View-Master 中，只突出一点点，有点像原来的照片轮！

经过一番摆弄之后，他成功地将整个东西层层组装起来，没有损坏 View-Master 的外壳。因为它是一件古董，所以对他来说，他的黑客攻击是可逆的是很重要的——在很大程度上，它是可逆的！休息后留下来看一小段视频解释！

[https://www.youtube.com/embed/JcoaqvPsSI8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/JcoaqvPsSI8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)