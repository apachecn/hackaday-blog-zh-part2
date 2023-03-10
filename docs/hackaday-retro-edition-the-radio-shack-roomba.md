# 黑客日复古版:无线电黑客 Roomba

> 原文：<https://hackaday.com/2015/06/01/hackaday-retro-edition-the-radio-shack-roomba/>

几年前，roomba——每个人最喜欢的机器人垃圾桶——带着崇敬之情登上了 Hackaday 的页面。除了爬楼梯，这个小机器人没有什么不能做的。从那以后，Roomba hacks 逐渐消亡，这些小垃圾桶也被垃圾箱吞噬了。真的很令人难过。

[Mike]有一个这样的 Roombas 已经有一段时间了，放在壁橱里，等待有人使用它。他最近把它挖了出来，看了一遍，发现电池出现问题后，led 灯亮了起来。然后问题是如何控制它。

他曾想将其连接到 VIC-20，但 Roomba 上方便的串行端口只接受 19.2k 和 57.6k 之间的波特率。带有老式 6522 VIA 的 VIC-20 只能以高达 2400bps 的速度连接串行端口。然后他突然想到了这个主意。在他古老技术的衣柜里，[迈克]有一个 Tandy 102，一个稍微升级的[TRS-80 型号 100](http://en.wikipedia.org/wiki/TRS-80_Model_100)，可以轻松驱动 19.2k 的串行端口

说到移动复古机器人平台，[Mike]不可能找到更好的计算机了。Tandy 102 有一个显示器，一个基本的解释器，足够运行 Roomba 的内存，由几节 AA 电池供电。他确实需要对串行端口进行一点电平转换，但 MAX232 可以轻松完成这项工作。

把所有的东西放在一起，[迈克]有了一个机器人和一台至少和旧的希斯基特英雄机器人一样好的电脑。你可以看看下面这个 Tandy 机器人的视频。

[https://www.youtube.com/embed/xU51bOgNfp8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/xU51bOgNfp8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)