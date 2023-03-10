# 比格犬骨黑+斜坡

> 原文：<https://hackaday.com/2014/04/19/beaglebone-black-ramps/>

![CRAMPS](img/48403bcaf8e424ea75678a8f7a5e5bf8.png)

BeagleBone Black 拥有令人印象深刻的计算能力和一大堆 I/O，可以成为令人印象深刻的 CNC 控制器，除了两个缺点:BBB 在任何地方都没有库存，CNC 斗篷有点贵。[马克·珀耳帖]无法为你找到一个没有 BeagleBone 的分销商，但他确实为非常受欢迎的 RAMPS-FD 3D 打印机控制器板提供了一个适配器[(论坛，法语，](http://www.usinages.com/emc2/linuxcnc-tourne-sur-carte-beaglebone-black-t59348-30.html#p720591)[这里是谷歌翻译矩阵](http://translate.google.com/translate?sl=fr&tl=en&js=y&prev=_t&hl=en&ie=UTF-8&u=http%3A%2F%2Fwww.usinages.com%2Femc2%2Flinuxcnc-tourne-sur-carte-beaglebone-black-t59348-30.html%23p720591&edit-text=&act=url))。

RAMPS-FD 是 RAMPS 板的扩展，也是 Arduino Due 的屏蔽。Due 和 BBB 都在 3.3 V 下工作，这意味着控制 RAMPS-FD 只需在 BeagleBone 上找到正确的布线图和引脚分配。[Marc]通过使用来自 [BeBoPr cape](http://elinux.org/Beagleboard:BeBoPr_Cape) 的设置和使用现有的 BeBoPr LinuxCNC 配置解决了这个问题。

[马克]修补的最终结果很像[查尔斯·斯坦库勒]为我们在中西部 RepRap 节上看到的 beagle bone Black[设计的 CNC 斗篷。[查尔斯]不卖他的斗篷，但似乎也没有其他人卖比格波恩黑人。](http://hackaday.com/2014/03/17/mrrf-arm-based-cnc-controllers/)

[https://www.youtube.com/embed/GQGVZTl_gy8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/GQGVZTl_gy8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)