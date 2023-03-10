# 三传感器邮箱警报真正实现了

> 原文：<https://hackaday.com/2014/11/07/triple-sensor-mailbox-alert-really-delivers/>

我们一般不建议干扰美国邮政。但是如果你像鲍勃一样建立自己的邮箱，你就有更好的机会做你想做的事情，而不用抛出任何旗帜。

说到扔旗子，这个项目最酷的部分之一是房子里的玩具邮箱，它可以监控真实盒子的活动。当有邮件等待时，玩具邮箱上的旗帜就会升起。一旦[Bob]取回邮件，该标志就会自动降下来。如果遵循外发协议中提出的标志，真实盒子标志中的磁铁可以防止玩具箱上的错误警报。最棒的是，他内置了一些遇险处理功能:如果邮箱门开着或者电池电量不足，玩具邮箱就会上下摇旗。

那么，这三个传感器在哪里呢？真实邮箱墙上的磁簧开关与旗子上的磁铁配对。为了确定门是否打开，[Bob]最初在箱子底部使用了另一个磁簧开关。这在潮湿天气下效果不好，所以他改用机械倾斜传感器。天花板上的红外发光二极管和地板上的光电晶体管一起工作来检测邮件的存在。

[Bob]的自制邮箱有一个隐藏 PIC 16F1825 的假背面。当门打开时，PIC 醒来，打开 MOSFET，并检查电池电量。它等了两分钟，让邮递员完成他的工作，然后读取旗州。在比较红外发光二极管和光电晶体管的状态后，它会向玩具邮箱发送一条信息，指示是否有邮件。

玩具邮箱装有一个修改过的接收器板和一个伺服系统来控制它的旗帜。[Bob]在他的网站上发布了代码和图表。演练视频在跳跃之后。

[https://www.youtube.com/embed/GZvhmCDTlu0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/GZvhmCDTlu0?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)