# Kickstarter Monitor 将点亮你的一天

> 原文：<https://hackaday.com/2014/10/16/kickstarter-monitor-will-brighten-your-day/>

跟上 kickstarter 活动可能是一项相当艰巨的任务，尤其是如果你的项目是真实的(看看你，涂鸦笔！)而且你要努力跟上产品制造以及将产品推向市场所涉及的所有其他物流。[macetech]目前正在进行一场活动，并建立了一个响亮、明亮的警报系统，通知他们任何新的 kickstarter 支持者。

该项目使用一个 LED 字幕来显示当前的支持者人数，但每当有新的支持者向该项目捐款时，一个耀眼的绿色箭头交通信号就会亮起，压电扬声器会播放庆祝曲。所有这些设备都由 Arduino Yun 控制，Arduino Yun 内置 Atheros 芯片组，可以轻松连接到网络并监控 kickstarter 页面的变化。

[macetech]使用了一些有趣的硬件来让所有东西协同工作。他们使用带 FTDI 芯片的 USB 转 RS232 电缆来驱动 LED marquee，使用 Adafruit 的 PowerSwitchTail 2 来驱动耗电的交通信号。他们的工作室的所有东西都摆放得很整齐，非常棒！所有的源代码都在他们的项目页面上，你也可以查看他们的 [RGB LED 灯罩](https://www.kickstarter.com/projects/macetech/rgb-led-shades) kickstarter 活动。