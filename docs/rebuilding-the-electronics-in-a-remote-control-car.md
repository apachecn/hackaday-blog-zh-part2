# 重建遥控车中的电子设备

> 原文：<https://hackaday.com/2012/08/30/rebuilding-the-electronics-in-a-remote-control-car/>

![](img/ccf6a25411be6da85aaccce7b649fc00.png "car")

受到许多自主漫游车如*好奇号*和自动驾驶谷歌汽车的启发，[Rohit]决定通过购买现成的遥控车并添加自己的电子设备来建造自己的车。不幸的是，他找不到用于接收无线电信号和驱动电机的芯片的数据表，所以他最终[制造了自己的电子设备](http://rkrishnan.me/?p=343)并把它们放在汽车里。

[Rohit]的汽车 Thunder Rumbler RC 汽车——是通过向两个电机供电来驱动的。这是一个容易控制的系统，因为只需要两个通道来使汽车向前、向左、向右或向后行驶。为了驱动这两个电机，[Rohit]在他的各种电子元件箱中找到了一个 SN754410 四路半 H 桥驱动器芯片。多亏了一个[有用的指令](http://www.instructables.com/id/Duel-Motor-Driver-with-Arduino-using-a-SN754410NE-/step3/Arduino-Sketch/)，这个芯片很容易用 Arduino 控制。

这就留下了向 Arduino 发送无线信号的问题。[Rohit]通过依赖 Android 手机提供远程控制来实现这一点。

[Rohit]在他的桌面上运行了一个小程序，允许他向 Android 手机发送“L”、“R”、“U”或“D”，以指示汽车应该向左、向右、向前或向后行驶。Android 手机通过互联网接收这些命令，并通过耳机端口发送音频信号。该音频信号连接到 Arduino 的两个模拟引脚。通过一点软件和对[频移键控](http://en.wikipedia.org/wiki/Frequency-shift_keying)的一点了解，【Rohit】能够让他的车向任何方向移动。

尽管[Rohit]实现了自己控制遥控汽车的目标，但制造工作还远未完成。他计划添加一些超声波传感器，并使用机器人的摄像头进行物体检测。