# 滚动你自己的 LoJack 克隆

> 原文：<https://hackaday.com/2013/02/13/roll-your-own-lojack-clone/>

![diy-lojack](img/85ce5d59f1a8a88151ae746c7b0f2696.png)

如果你曾经担心你的车被偷，这个软件可以帮你解决一些问题。这是一个支持蜂窝的地理定位设备。这些东西已经使用了一段时间，我们知道的最常见的品牌是 LoJack。那家公司给你一个安装在车上的小盒子，如果它丢失了，他们可以获取坐标并将其转发给当局。这种定制版本在 EFM32 板的附加板上构建了很多插件。

上图显示了附加组件的主要组件:GPS 模块和 GSM 调制解调器。沿着电路板的顶部边缘是电压调节器电路，旨在保持待机功率最小，以免耗尽汽车的电池。你看不到的是位于底部的 SIM 卡插槽。

你可以在上面的链接中找到 Eagle 文件。休息之后我们嵌入了该项目的视频描述。

[https://www.youtube.com/embed/rz5wn8NnoIU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/rz5wn8NnoIU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)