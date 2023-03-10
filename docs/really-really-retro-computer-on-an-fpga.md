# 非常非常复古的 FPGA 电脑

> 原文：<https://hackaday.com/2015/06/23/really-really-retro-computer-on-an-fpga/>

[丹尼尔·贝利]用 FPGA 为自己建造了一个早期计算机的缩小版克隆。具体来说，他写了一些 VHDL 代码来描述这台机器，这是一台缩小版的[曼彻斯特小型实验机](https://en.wikipedia.org/wiki/Manchester_Small-Scale_Experimental_Machine)，配有 8 位处理器和巨大的 8 字节 RAM，所有这些都显示在 led 屏幕上。太酷了。

在这样的限制下，他可以让它做任何事情，这让我们感到惊讶。观看他的编程，并在休息时间下面的视频中测试它的速度。

[https://www.youtube.com/embed/LP7s1XPLMyI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/LP7s1XPLMyI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

最初的“曼彻斯特宝贝”最酷的地方是它在一个[威廉姆斯电子管](https://en.wikipedia.org/wiki/Williams_tube)中保留了记忆，这实际上是一个带有覆盖屏幕的电子拾音器板的 CRT。你知道电子束击中旧阴极射线管的表面会产生静电荷吗？事实证明，你可以暂时读取这个电场，并把它作为短期记忆元素。

SSEM 的建造者包括第二个阴极射线管屏幕，这样你就可以在屏幕上看到整个 32×32 位的内存，就像你想的那样。很自然地，[丹尼尔]不得不在他的曼彻斯特婴儿克隆体上复制这个特征，但是使用 8×8 的 LED 矩阵。现在我们想在笔记本电脑上安装一个。

Github 上有 [VHDL，还有机器](https://github.com/danieljabailey/C88)的 [Javascript 模拟器。如果你感兴趣，这里有一个活跃的逆向计算](http://danieljabailey.github.io/c88-js/) [Google+小组](https://plus.google.com/u/0/communities/109052413018437647853)，这个和类似的项目在这里被取笑。看看一些最早的电脑音乐，是由曼彻斯特婴儿的后代制作的。

谢谢你的提示。