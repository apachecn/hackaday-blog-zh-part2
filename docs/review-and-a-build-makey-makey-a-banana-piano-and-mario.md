# 回顾和构建:Makey Makey，香蕉钢琴和马里奥

> 原文：<https://hackaday.com/2012/05/25/review-and-a-build-makey-makey-a-banana-piano-and-mario/>

![](img/87d9d3b6e707da6c7e8b10600669b33d.png "Makey")

我们在黑客热线上收到了很多关于 Makey Makey T1 的邮件。这种名片大小的电路板将一切——香蕉、培乐多、水和人——都变成了触摸界面。

已经有[吨](http://www.wired.com/geekdad/2012/05/makey-makey/)[博客](http://www.geek.com/articles/gadgets/makey-makey-play-mario-with-a-banana-20120516/)写了关于 [Makey Makey Kickstarter](http://www.kickstarter.com/projects/joylabs/makey-makey-an-invention-kit-for-everyone) 并在湾区 Maker Faire 上首次亮相，但 Hackaday 对 Makey Makey 的即将发布保持沉默。这是有原因的:[Jay]和[Eric]，麻省理工学院媒体实验室的老鼠，他们想出了 Makey Makey，提供了一个演示板给 Hackaday 的人。好吧，这是你可以用 Makey Makey 做的所有酷东西的评论。

Makey Makey 是一款简单的设备，旨在让每个人都成为发明家。在电路板的前面是一对鳄鱼夹插入孔，背面是一个 USB 插头。将鳄鱼夹插入任何导电物体，将“地线”连接到你的身体上，将任何物体变成触摸传感器。在背面有一堆易于试验的接头，将正面的 6 个输入扩展到 16 个输入，可以将任何输入发送到 PC。

#### 你能用它做什么

用 Makey Makey 做的标准“第一件事”就是香蕉钢琴。事实上，这是[Jay]和[Eric]发给我的包中包含的测试版说明手册中列出的第一个例子。甚至 Hackaday 自己的电路之神[Sprite_tm] [也建造了一架克隆的 Makey Makey 香蕉钢琴](http://hackaday.com/2012/05/17/bananaphone-lets-you-use-fruit-and-other-things-as-switches/)，所以我想我应该试一试。

[https://www.youtube.com/embed/pfjWdoW7pt4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/pfjWdoW7pt4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

是的，沙基·坎姆。

为了装配这架香蕉钢琴，我所做的只是在一只香蕉手上连接几根导线，将它们插入 Makey Makey，并用铝箔制成的简易 ESD 脚踝带将自己接地。加载 Makey Makey [演示钢琴页面](http://scratch.mit.edu/projects/jay/2530241)我的桌子上有一架香蕉钢琴。在这一点上，我真的不得不佩服[杰伊]和[埃里克]。这东西太棒了。

在那之后，我决定更进一步，用铝箔做一个巨大的超级任天堂控制器:

[https://www.youtube.com/embed/KN6vhSsGq2c?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/KN6vhSsGq2c?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

我有一个成长的起源。很明显。

老实说，我不能说 Makey Makey 有多酷。这是一个完全开放的工具箱，可以构建你想要的任何东西。当我把香蕉钢琴放在一起时，我感到头晕，我敢肯定，在我对超级马里奥世界的许多初步测试中，我的血压都在上升。

#### 硬件规格

如果没有至少一段关于硬件的内容，这就不是一篇黑客评论了。Makey Makey 加载了 ATMega32U4(与全新的 [Arduino Leonardo](http://arduino.cc/en/Main/ArduinoBoardLeonardo) 中的微控制器相同)，与 Arduino IDE 兼容，并可通过 6 引脚 AVR 接头完全重新编程。USB 端口的操作就像任何其他 USB HID 设备一样，所以如果您的计算机可以使用 USB 键盘，它就可以使用 Makey Makey。

在 Makey Makey 的背面，有 16 个母接头，这些母接头插入传感器以获得额外的钥匙。目前，Makey Makey 会向您的计算机发送 WASDFGHJ、up、down、left、right、left click 和 right click，但当 Makey Makey 源代码发布时，这可以很容易地在 Arduino 环境中重新映射([Jay]说他们至少会在发布时发布源代码，如果不是更早的话)。这位进取型制造商总共有 18 个触摸感应输入，可以映射到任何 USB 输入。

#### 最后…

Makey Makey 棒极了。想想你想做的任何项目，比如音乐啤酒。你可以用 Makey Makey 来做。这是一个神话般的玩具，对于你负责的好奇的小学生来说是一个完美的介绍，足以让最疲惫的青少年对制作一些很酷的东西感兴趣。这比门票的价格更值得，尤其是当你可以在 T2 做这么多事情的时候。