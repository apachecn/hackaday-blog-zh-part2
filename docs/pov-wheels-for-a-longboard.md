# 用于长板的 POV 轮子

> 原文：<https://hackaday.com/2012/11/16/pov-wheels-for-a-longboard/>

![](img/2d984ef31079237f9fea4c5331a74c7c.png "pov-wheels-for-a-longboard")

如果你不介意使用非常小的组件[，这个针对长板](http://ch00ftech.com/2012/11/15/lonboard-wheel-display/)的 POV wheel 项目肯定会吸引一些注意力。

这里的游戏名称是小而便宜。小是因为轮子直径只有 72 毫米(约 2.8 英寸)。便宜是因为[Ch00f]想在当地生产和销售。他带了一个驱动 15 个发光二极管的 ATtiny24 微控制器。显然，这将带来一个问题，因为 uC 使用 14 引脚 SOIC 封装，这不足以单独驱动 led。再加上存储要显示的模式的问题，你会很快耗尽程序内存。

但很明显他成功了。上图显示了显示 CT 标志(ch00ftech.com)的车轮，在广告之后的剪辑中还展示了其他几个图案。发光二极管是多路复用的，但轮子转得足够快，这证明是没问题的。通过瞄准固定轴的红外反射传感器测量旋转。CR2032 为该设备提供动力，并添加了一些配重以保持车轮平衡。

我们唯一担心的是暴露在外的电子设备的脆弱性。但是，如果你击中了正确的 BOM 价格，我们猜测你可以只更换所需的董事会。

[https://www.youtube.com/embed/y8d0f4nB7Qs?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/y8d0f4nB7Qs?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[via [Reddit](http://www.reddit.com/r/ECE/comments/13916v/led_longboard_wheel_display/)