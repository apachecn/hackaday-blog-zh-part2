# 把树莓派变成 SNES

> 原文：<https://hackaday.com/2013/01/04/turning-a-raspberry-pi-into-an-snes/>

![snes](img/ced23af6a6d413045f59b9aef8d28863.png)

早在世纪之交，将 MiniITX 主板塞进几乎所有的东西在技术人群中风靡一时。[waterbury]的想法是用 SNES 制造一台计算机，但增加了读取 SNES 墨盒的能力。这个想法已经在[沃特伯里]的脑海中漂浮了多年，现在有了一个树莓皮[，他终于可以让他的项目成为现实](http://familab.org/blog/2012/12/snes-super-nintendo-emulated-system/)。

从原来的 SNES 上拆下一个墨盒连接器后，[waterbury]把它插在一块 perf 板上，开始研究如何真正读取墨盒。SNES 盒式磁带需要 16 个地址引脚、8 个数据引脚、8 个存储体控制引脚和 4 个其它控制引脚来读取；在一个简洁的 I/O 扩展器和一大堆电平转换器的帮助下,[waterbury]总共访问了 36 个引脚。

[waterbury]通过 [Raspberry Pi 的 I2C 接口](http://familab.org/blog/2012/12/snes-super-nintendo-emulated-system/5/)访问这些数据、地址和控制线，这是一项不平凡的任务，花了 70 分钟阅读*大金刚国家*，然后他找到了将 Raspi 速度提高两倍的方法。休息之后，你可以看看[沃特伯里]的完整项目——可以阅读磁带，用[模拟器](http://aloshi.com/emulationstation)玩 rom。此外，购物车阅读器的代码可以在[waterbury]的 git
上获得[。](https://github.com/waterbury/SNES-Pi)

[https://www.youtube.com/embed/qEJuDdjkVSc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/qEJuDdjkVSc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)