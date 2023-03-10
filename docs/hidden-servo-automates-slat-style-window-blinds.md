# 隐藏伺服自动板条式窗帘

> 原文：<https://hackaday.com/2013/04/18/hidden-servo-automates-slat-style-window-blinds/>

![slat-blind-automation](img/663f62d8f42171e39c729f4bf53d8070.png)

[Home Awesomation]一直致力于自动化他的板条式百叶窗。他的重点是调整板条的角度，而不是完全收起窗帘。由于缝翼角度调整需要很少的扭矩，伺服电机证明是完美的工作。好消息是，他家现有的百叶窗在顶部有空间完全隐藏他的附加硬件。

上面的图片是演示的截图，你可以在休息后观看。百叶窗的顶部外壳正好显示在框架的顶部。这里[哈]展示了一些不同的控制设计，他一直在尝试。你可以看到一个看起来像 Molex 连接器的东西，上面连接着某种类型的组件。这是一个红外运动传感器，他对它的性能非常满意。他对电源线旁边的黑色瞬时按钮开关也有同感。但是他的 DIY 解决方案效果很好，那就是把拉绳系在一片柔韧的金属上。当金属弯曲到足以接触固定导体时，它就完成了电路，告诉 Arduino 开始驱动伺服系统。

这个项目背后的主要想法是轮询一个温度传感器，自动关闭百叶窗，以帮助保持白天的凉爽。我们认为，如果他已经在使用微控制器来驱动这个项目，他可能还会在模块中放一个便宜的蓝牙设备，让它可以用智能手机来控制。

[https://www.youtube.com/embed/4W_H9D2edS8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/4W_H9D2edS8?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[via [Ariccio](http://ariccio.com/2013/04/12/automated-window-blinds-with-arduino/)