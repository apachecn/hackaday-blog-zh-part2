# 新鲜集市上的 Furbies 歌唱皇后

> 原文：<https://hackaday.com/2013/11/05/furbies-sing-queen-at-freshers-faire/>

![kent-furby](img/3c42c476e8c0a1539697c72d9bc878ed.png)

肯特大学有自己的黑客空间，叫【创客社】。每年学校都会为新生举办一个名为新生集会的迎新活动。今年新鲜集市上的[创客协会]展示包括一群穿着半裸的皮草歌手演唱皇后乐队的经典波西米亚狂想曲。这不是我们第一次使用[波西米亚狂想曲和黑客硬件](http://hackaday.com/2009/04/19/bohemian-rhapsody-on-old-hardware/)。

[创客协会]开始做一些互联网研究和逆向工程第一代 Furby。Furby 本身就是成本降低的奇迹。玩偶的所有功能都由一个马达和一个凸轮系统控制。当凸轮处于零位时，限位开关会告知机载微控制器。光学编码器在凸轮移动时跟踪它。该协会用 Atmel ATMega328 取代了 Furby 的内部微控制器。这允许他们使用 Arduino 编程环境。

许多经典的电子动画系统使用音频记录动作。一般来说，立体声录音机有双重功能。第一个轨道将包含动画的音频。第二轨道将包含对应于被动画化的玩偶的每个自由度的运动的音频音调。因为两条轨道在同一条磁带上，所以声音和运动总是同步的。多轨磁带录音和回放系统为这种类型的系统增加了更多的灵活性。

[制造者协会]在他们的毛皮上使用了这种经典系统的电脑化扭曲。一组位置和时间以逗号分隔变量(CSV)格式存储。一个 java 程序会播放歌曲并读取文件，在指定的时间向 Furbies 发送移动命令。结果相当不错。不幸的是，集会的声音太大了，我们听不到太多毛皮兽的歌声。

[https://www.youtube.com/embed/H0NAQZcjhpY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&start=26&wmode=transparent](https://www.youtube.com/embed/H0NAQZcjhpY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&start=26&wmode=transparent)

[https://www.youtube.com/embed/GE5ano_8DBY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/GE5ano_8DBY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)