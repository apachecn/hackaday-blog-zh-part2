# 黑掉一台业余无线电

> 原文：<https://hackaday.com/2013/02/28/hacking-a-ham-radio/>

圣诞节，[Lior]收到了一台宝丰 UV5R 收音机。他没有业余无线电执照，所以他决定用它作为警方的扫描仪。既然图表已经有了，他[打开它，黑了它](http://www.liorelazary.com/index.php?option=com_content&view=article&id=49%3Ahacking-the-baofeng-uv5r&catid=14%3Abaofeng-uv5r&Itemid=17 "Hacking the Baofeng UV5R")。

这种 40 美元的无线电通信在 136-174 兆赫和 400-480 兆赫波段。它使用一次性可编程微控制器和 RDA1846 收发器。切断 MCU 的电源后，[Lior]能够使用 Arduino 通过 I2C 向芯片发送自己的信号。他还记录了股票微控制器在启动时发出的信号，这样他就可以用 Arduino 来模拟它。

一旦 Arduino 上的通信工作正常，[Lior]就决定摆脱现有的微控制器。他拆下芯片，留下暴露的焊盘来焊接引线。将这些设备连接到 Arduino 上，他就可以通过可编程的方式来控制设备。他获得了无线电执照，实现了莫尔斯电码的传输，并在书面报告中提供了 Arduino 草图。

[Lior]指出，他的下一步是制作一个 PCB，将不同的微控制器连接到设备上。这将给他一个 40 美元的完全可编程的收音机。休息之后，看看被黑的无线电的视频。

[https://www.youtube.com/embed/vgPwW9Nn9OY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/vgPwW9Nn9OY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)