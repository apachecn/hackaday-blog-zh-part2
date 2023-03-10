# 用树莓皮制作一个测斜仪

> 原文：<https://hackaday.com/2014/12/16/create-an-inclinometer-using-a-raspberry-pi/>

你可以用便宜又简单的树莓派做出最新的小发明，这是由[马克·威廉姆斯]提供的。他将惯性测量单元(IMU)连接到 Pi 上，并建造了一个[倾角仪，用于测量越野车的各种角度](http://ozzmaker.com/2014/12/12/inclinometer-using-raspberry-pi-imu/)。

这个特殊的指南通过设置 [SDL](http://en.wikipedia.org/wiki/Simple_DirectMedia_Layer) 来控制小屏幕的视频输出。然后，创建一个函数，根据 IMU 的输入旋转图像，以便车辆位置可以在屏幕上以图形方式显示。现在，当你的卡车要翻上坡时，你会得到提前警告！

当然，整个项目的前提是首先安装 IMU 并在 Raspberry Pi 上运行。[Mark]你是否也在[上介绍了设置指南](http://ozzmaker.com/2014/12/11/berryimu/)。这深入研究了在 I2C 上设置 IMU，让它与 Raspberry Pi 对话，然后将来自 IMU 的原始数据转换为更有用的数据。请务必查看[Mark]的页面，了解所有代码和详细信息！