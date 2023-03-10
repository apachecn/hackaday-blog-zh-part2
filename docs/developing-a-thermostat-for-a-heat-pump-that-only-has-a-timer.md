# 为只有定时器的热泵开发恒温器

> 原文：<https://hackaday.com/2012/11/12/developing-a-thermostat-for-a-heat-pump-that-only-has-a-timer/>

![](img/d03340d888f5bf4fbec6b8d924383f2f.png "heat-pump-controller")

给(克里斯·勒布朗)家降温的热泵缺乏他一直在寻找的那种控制。它只有一个计时器，可以自动关闭。他希望能够像自动调温器驱动的装置一样安排冷却循环。他最终建立了自己的控制器来自动化冷却过程。

热泵配备了红外遥控器，为项目提供了接入点。[Chris]开始模拟远程协议，这省去了他打开装置和连接控制器的麻烦。他带着危险原型的红外玩具，因为这个设备能够记录和传输红外信号——它基本上是一个通用的 USB 端口遥控器。他的树莓派，在左边，控制着这个系统。它通过 USB 集线器连接到红色红外玩具板上，USB 集线器也用于连接 WiFi 加密狗。该系统与谷歌日历(Google Calendar)协同工作，让克里斯只需添加一个预约，就能安排他家的制冷时间。Python 脚本查询日历，然后选择并发送适当的 IR 命令。休息之后，他展示了视频中的身材。

[https://www.youtube.com/embed/1RDMPptUeIQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/1RDMPptUeIQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)