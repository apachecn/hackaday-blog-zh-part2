# 黑客空间:传输 2 解谜

> 原文：<https://hackaday.com/2014/04/30/hackaday-space-transmission-2-puzzles-explained/>

![transmission-2-explanation](img/d111ad8883bec3b32a70bc15387c1c09.png)

所以昨天我们给了你一个 4 月 1 日发布的 1 号传输的摘要。我们很快就从不得不为 4 月 1 日准备一些有趣的东西变成了运行整整一个月的 ARG，让 SupplyFrame 总部的事情变得非常繁忙。让我们来看看在第二周的虚拟现实游戏中隐藏了哪些数据。如果你被困在某个没有网络的地方几天，这个游戏是宣布[黑客日奖](http://hackaday.io/prize)的前奏。

传播 2 始于出现在 Hackaday 博客顶部的以下视频:

[https://www.youtube.com/embed/GarHflTVGyQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/GarHflTVGyQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

汤姆少校随后在一个名为 [Transmission 2](http://hackaday.io/page/314) 的页面上发布了以下图片。

[![Transmission 2 image](img/c310af0fe5af8020614f112e60aa0aee.png)](http://hackaday.com/wp-content/uploads/2014/04/status.jpg) 因为每个人都认为之前传输的图像中使用了隐写术，所以我们决定在这次传输中使用这种方法来隐藏一些数据。为了做到这一点，我们需要你找到一些密钥和适当的隐写术方法来解码数据。所以我们决定在视频中隐藏一些线索。

该视频主要是由我们在 [IcoEx](http://icoex.co.uk/) 的朋友们制作的，但我们想在其中加入一些信息。在视频中(如果你仔细看的话)有两个隐藏在噪音中的几乎潜意识的图像，这些图像因[鲍勃·威德拉]而出名。作为额外的线索，我们张贴了[Alek 的] [关于[Bob]](http://hackaday.com/2014/04/08/heroes-of-hardware-revolution-bob-widlar/) 和他声名狼藉的职业生涯的史诗般的文章。

[![Widlar current source](img/cd3cb839e78be97bd4c7268970f14259.png) ](http://hackaday.com/wp-content/uploads/2014/04/widlar_source.png) [ ![Widlar sheep](img/bdd5765b30cf5e69af55f6e7d7b62eae.png)](http://hackaday.com/wp-content/uploads/2014/04/widlar_sheep.jpg)

此外，在视频中，你会听到我们自己的[Brian Benchoff]以老派[数字站](http://en.wikipedia.org/wiki/Numbers_station)的风格读出一系列数字。音频中的数字序列是 921763865，这是 IP 地址【54.241.0.25[的十进制表示。如果您尝试在 web 服务器中加载它，您会得到一个包含以下文本的简单响应:](http://54.241.0.25)

> `DO AUTHENTICATION WILL ENCRYPT DO TERMINAL TYPE DO TSPEED DO XDISPLOC DO NEW-ENVIRON DO ENVIRON WILL SUPPRESS GO AHEAD DO ECHO DO LINEMODE DO NAWS WILL STATUS DO LFLOW DO TIMING-MARK`

这看起来有点奇怪，没有换行符(这是它在浏览器中呈现的方式)，但实际上是 telnet 服务器在您第一次连接到它时发出的选项语句。这是一个足够的线索，每个人都找到了 telnet 服务器，它给了他们提示:“地面控制登录:”。这个用户名和密码有点晦涩，但是很快就被发现了。这是“鲍勃:威德拉”,当你弄清楚潜意识的图像时，这是非常明显的。

一旦进入 telnet 服务器，您发现自己在一个非常受限制的帐户中，有一个包含 2 个文件和一个文件夹的主文件夹。这个文件夹完全是一个障眼法，我们在本周早些时候寻找可能的谜题想法时发现了阿波罗制导计算机源代码，并最终将其放入主文件夹中，只是为了好玩。我们曾经考虑过让你使用令人难以置信的 [MoonJS](http://svtsim.com/moonjs/agc.html) 端口对 AGC 进行编程，但结果证明它相当复杂，我们决定改用其他的方法。然而，令我们印象深刻的是，有几个人下载了源代码，检查了它与原始版本的差异，甚至设法让它编译了！Hackaday 读者再一次展示了他们的坚持和独创性。

主文件夹中的另外两个文件是名为“keyfile”的文件和名为“reminder.txt”的文本文件。密钥文件包含 3 组字符串:

`9186743BFDA92EE261752C138EBCD
FD332A7F1B1347BAFBA673B13EE3D
2D34FBA5FFBC69D2FBC1C1C25C484`

第二个文件包含由莱纳德·利普顿和彼得·雅柔创作的流行歌曲《噗噗，魔龙》的文本。这是对流行的隐写加密工具 [Open Puff](http://embeddedsw.net/OpenPuff_Steganography_Home.html) 的暗示。有了钥匙和打开的泡芙，就有可能知道钥匙文件中的 3 个字符串代表了你可以打开泡芙的 3 个钥匙。一旦您拨入正确的设置，您将获得一个包含以下消息的文本文件:

```
Current Status
Inclination 52.3
Altitude 439km
O2 76.2%
```

一旦一些人将此张贴到 Transmission 2 页面上，我们就让地面控制关闭这一轮的谜题，并告知:

> 汤姆少校，这是地面控制中心。
> 消息已收到。
> 救援任务已计划，船员选拔正在进行。
> 下一次通信在 T-18180

这标志着第二次传输的结束，并指向下一次传输，该次传输将在 T=0 时间的 18180 分钟。这对我来说是一个小错误，因为我仍然没有完全理解如何使用 T 符号，但已经看到有人试图用分钟来解决它，所以这次我改用分钟。这引起了一点混乱，但最后大家还是到了。

我认为拼图的这一阶段进行得非常顺利，很多人都为解决方案做出了贡献，我们这一方也没有出现重大错误，这使得一切进行得更加顺利。此时，一个围绕这些谜题的社区开始萌芽，一个新的黑客日 IRC 频道于[# #黑客日](http://webchat.freenode.net/?channels=##hackaday)在 freenode 上诞生。后来，这里成了从事拼图工作的人的非正式的家和聚会场所，而且非常有趣。也有一些令人愤慨的巧合，“噗噗，神龙”线索与其他空间事物有着意想不到的关系，这是我们没有考虑到的。一些人认为我们指的是由 SpaceX 开发的[龙飞船](http://en.wikipedia.org/wiki/Dragon_(spacecraft))，其他人认为它可能是指[龙头部星云](http://www.space.com/23750-dragon-s-head-nebula-explored-with-very-large-telescope-video.html)。这种巧合在整个争论中不断出现，但我认为它们增加了乐趣。

传输 3 是一切开始有点不对劲的地方，但那是另一天的故事。明天见！

#### 未完待续…