# 树莓派车库门开启器

> 原文：<https://hackaday.com/2015/02/15/a-raspberry-pi-garage-door-opener/>

在这里，我们似乎永远找不到足够的车库门黑客。坦纳的项目是这个类别中最近的一个项目。他设法在他的车库门开启器上安装了一个覆盆子。这大大扩展了他的活动范围……任何有网络连接的地方。

他的黑客技术相对简单。他从车库门遥控器开始。他拆下了通常用来开门的瞬时开关。他桥接了电连接，创造了一个总是闭合的电路。这意味着只要遥控器有电，开关就会被激活。现在[坦纳]所要做的就是取下电池，把电源插头接到他的树莓派上。由于遥控器的工作电压为 3.3V，消耗的电流很少，因此他可以直接从 Pi 为遥控器供电。Pi 只需瞬间将其引脚变为高电平即可激活遥控器。

从世界任何地方切换车库门状态的能力也伴随着偏执。当他不在家时，他想知道门是向上的，向下的，还是停在中间的某个地方。他还想使用尽可能少的设备。由于他在车库里已经有了一个 IP 摄像头，他决定使用[计算机视觉](http://www.tannr.com/2015/02/12/raspberry-pi-garage-door-opener-part-2/ "OpenCV to detect garage door state")来进行检测。

他在普通的白色电脑纸上打印出两个巨大的黑色图形。一个贴在门的顶部，一个贴在底部。一个定制脚本在 Pi 上运行，它从相机中抓取最新的图像，并使用 [OpenCV](http://hackaday.com/2012/05/13/getting-started-with-opencv/ "Getting started with OpenCV") 来检测形状。如果两个形状都可见，那么脚本可以假定门是关着的。否则，它可能是打开的。这使得[坦纳]更容易知道门是开着还是关着，而不必亲自检查摄像机。

找不到足够的车库门黑客？试试[这些](http://hackaday.com/2014/05/25/arduino-garage-door-opener-is-security-minded/ "Arduino garage door opener")的[尺寸](http://hackaday.com/2013/10/13/raspberry-pi-garage-door-automation/ "Garage door automation")。

[https://www.youtube.com/embed/fCRlvkibfxc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/fCRlvkibfxc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)