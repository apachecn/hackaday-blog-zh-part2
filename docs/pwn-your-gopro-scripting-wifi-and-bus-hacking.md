# Pwn Your GoPro:脚本、WiFi 和总线黑客

> 原文：<https://hackaday.com/2014/06/20/pwn-your-gopro-scripting-wifi-and-bus-hacking/>

![naked-gopro](img/ee1a2daaf7e5e3e9091f36283cae9fdc.png)

GoPro 相机开箱后具有大量功能。大多数人会感到满意，甚至可能被可用的选项所淹没，但是如果你能够做到这些，你将能够进一步扩展你的相机的功能。然而，他们可以使你的保修无效，所以和大多数黑客一样，你要自担风险。

### **使用 Autoexec.ash 编写脚本**

![gopro-hack](img/a933a5ca97af28b6ebe24eda8c2ea03a.png)到目前为止，扩展 GoPro 功能的最简单方法是在 GoPro 相机的根文件夹中放置一个名为 Autoexec.ash 的文本文件。你可以在[chernowee.com](http://chernowii.com/ "chernowii.com")上下载一些脚本，根据【康拉德】的见解，这些脚本应该很容易修改。使用这些脚本是非常强大的，人们可以修改相机的元素，从简单地闪烁 led，到改变视频捕捉属性，到许多其他有用的设置。

你可以在他的页面上查看这些，或者如果你喜欢这种方式，这是他的 Github 账户。他很快指出这将使你的保修失效，所以要小心行事。虽然很想尝试，但我还没有“库存”GoPro 功能无法解决的紧迫情况。风险可能很小，但对我来说回报几乎不存在。

### **通过 WiFi 进行黑客攻击**

![python-script-wifi-gopro](img/7d52686808f4322c342b955f062262f4.png)

如果编写一个驻留在 GoPro 上的脚本不是你的风格，或者感觉风险太大，你总是可以在你的电脑上使用脚本来控制相机。[【Adrian】就是这么做的](http://sitterle.co/removing-gopros-timelapse-frequency-constraints/ "Python script GoPro control over WiFi")，写了一个 Python 脚本来控制超过“库存”60 秒的延时频率。有更多的命令可以通过类似的脚本技术在 WiFi 上执行，[Korad]在他的 [GitHub 页面上列出了这些命令。](https://github.com/KonradIT/goprowifihack/blob/master/WiFi-Commands.mkdn "Github GoPro WiFi Command List")

在[Adrian 的]页面上还概述了用电脑登录 GoPro 并四处浏览实际上非常简单。这种类型的“黑客行为”对于即使是最受时间限制的“脚本小子”来说也是有趣的事情。

这个 WiFi 脚本来自 Reddit 的[，它声称这不是黑客攻击…继续，在评论中随意写“不是黑客”！](http://www.reddit.com/r/goprodiy/comments/279j5r/removing_gopros_timelapse_frequency_constraints/ "WiFI GoPro "No Hack"")

### **BacPac 总线黑客**

如果你对 14 岁的(康拉德的)Autoexec.ash hacking 或他的 WiFi 命令列表印象不够深刻，他还在他的网站上列出了 [BacPac 连接器上的引脚的功能(并拆卸了一个，如第一张图所示)。我从来没有真正想过将它作为更多按钮或输出的接入点，但是很自然地，有很多 IO 功能通过这个端口运行。](http://chernowii.com/hack.html "chernowii.com")

人们可以想象将 Arduino 或 Raspberry Pi 连接到总线上，并通过它控制摄像机。特别是考虑到 RGB 视频输出引脚，很难不想到这种类型的控制可能带来的有趣的黑客攻击。如果你已经在做一些 BacPac 的黑客工作了[，我们想听听它的情况](http://hackaday.com/contact-hack-a-day/)！

### **DIY 安装选项**

![magnetic-gopro-egg-timer-nolg](img/37d44f0c5512b22c2d8097692b6a1bd3.png)切换齿轮，可能是我最喜欢的一类 GoPro“黑客”是人们想出的安装它们的 DIY 方法。其中最有用的，也是最简单的，是厨房定时器 GoPro mount。我们展示了几款有趣的车型，包括这款使用宜家零件的[出色支架。这里有一个](http://hackaday.com/2011/09/21/build-cheap-panning-camera-mounts-for-time-lapse-photography/ "Ikea GoPro timer")[是我用不同风格的带磁性底座的定时器做的](http://hackaday.com/2013/07/18/magnetic-panning-time-lapse-camera-mount-couldnt-be-easier/ "magnetic camera mount GoPro timer")，这带来了一些独特的安装可能性。

在更极端的一端，你可以用弹弓将你的 [GoPro 发射到空中，或者总是有单 GoPro 子弹时间旋转黑客。(哈德)明矾(迦勒)在这里相当成功地演示了这个](http://hackaday.com/2013/08/21/gopro-slingshot/ "Launch a GoPro with a slingshot")，但你可能也看到了使用[吊扇和烟花](http://hackaday.com/2013/07/02/bullet-time-with-a-ceiling-fan/ "bullet time ceiling Fan Gopro fireworks")的出色效果。有火一切都好！

[https://www.youtube.com/embed/qvghDGlrbUo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/qvghDGlrbUo?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

**安装+软件=超级棒**

最后，如果你“碰巧”有 6 台 GoPro 相机，一台 3D [打印机来制作支架](http://www.thingiverse.com/thing:52584 "3D printed 6 GoPro Mount")，以及[软件来将视频拼接在一起](http://www.kolor.com/360-video/autopano-video-360-video-stitcher.html "Kolor Autopano")，你就可以创建一个令人难以置信的[球形全景视频](http://www.jonasginter.de/360-grad-video-mit-6-gopro-kameras/ "Spherical panorama with a 6 GoPro cameras")。看着下面的结果，让我感觉自己就要从地球掉到太空了，但是很难不继续看下去！[通过 [Reddit](http://www.reddit.com/r/gopro/comments/2410v8/3d_printed_a_360_gopro_mount_im_only_2_gopros/ "Reddit comments 360 GoPro mount")

[https://player.vimeo.com/video/90312869](https://player.vimeo.com/video/90312869)

* * *

Jeremy Cook 是一名全职工作 10 年的制造工程师，拥有克莱姆森大学的 BSME。工作之外，他是一个狂热的制造者和实验者，从事各种工作，从业余爱好数控机械，到灯光涂鸦，甚至偶尔 DIY 乐器。当他不忙着创造(或破坏)什么的时候，你可以在 Twitter 上找到他