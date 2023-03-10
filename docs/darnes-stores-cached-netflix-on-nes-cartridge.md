# [darNES]将缓存的网飞存储在 NES 墨盒上

> 原文：<https://hackaday.com/2015/03/13/darnes-stores-cached-netflix-on-nes-cartridge/>

我们来玩一个快速的单词联想游戏:花生酱…果冻。拱门…金色的。NES…网飞？最后一个听起来有点牵强，但是[darNES]开发团队有一个黑客日和一个梦想。他们从缓存的网飞数据开始，最后在普通的 NES 上播放。 (YouTube 链接)

数据被预先转换，因此视频帧被存储为 tilesets 并存储在 ROM 图像中。[Guy]使用了 [NES 内存映射器(MMC3)](http://wiki.nesdev.com/w/index.php/MMC3) 来交换帧。[darNES]原本计划在盒式磁带中使用一个 Raspberry Pi 来处理视频转换和联网，但由于时间限制和资源可用性，不得不改变方式，制作一个静态 ROM 映像。

访问网飞的数据就像过去的日子一样——将墨盒装入未经修改的 NES，然后按下电源按钮(他们甚至不需要对它吹气！).一个基本的网飞画廊出现了。你可以用 NES 控制器的 D-pad 移动屏幕上的白色光标。选择了《纸牌屋》,和往常一样，下一个屏幕显示了一个带有静止图像的概要，并提供了游戏选项。推荐也是有的，但是显然在这个设置下是行不通的。尽管如此，我们还是忍不住笑了。[darNES]承认由于时间问题，他们没有优化瓷砖拼板的调色板。他们计划在本周发布更多的技术信息，但是已经给了我们一些关于他们黑客新闻的线索。

休息后查看视频，看看他们适合 256K NES 墨盒的视频。

[https://www.youtube.com/embed/_yn-rNdYZAY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/_yn-rNdYZAY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[https://www.youtube.com/embed/womt2t_GES0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/womt2t_GES0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

【谢谢，bluewraith！]