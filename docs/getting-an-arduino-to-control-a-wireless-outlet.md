# 让 Arduino 控制无线插座

> 原文：<https://hackaday.com/2013/01/31/getting-an-arduino-to-control-a-wireless-outlet/>

[Reza]对这个遥控插座的系统调查让他[使用 433 MHz 发射机](http://rezaalihussain.blogspot.com/2013/01/controlling-smart-outlet-with-arduino.html)接入 Arduino。这是一个单设备单元，但这里使用的技术应该允许您控制无线钻机，这些钻机有多个模块来控制许多设备。

我们已经看到本地黑客空间的一些人试图接入遥控器本身。这使用了某种奇怪的按钮扫描(不只是连接一个引脚到地面或电压)，没有成功。[Reza]甚至没有打开上面看到的任何一个单元的外壳。相反，他径直走向手边的无线接收器，用逻辑分析仪捕捉来自遥控器的信号。

一旦他对按下遥控器的开或关按钮时发出的信号有了一个很好的快照，他就开始在他的 Arduino 代码中复制它。他的函数 setStateWithDelay 有三个参数:传输引脚、电平(高或低)和延迟的毫秒数。每个信号都会多次调用这个函数，但是解决这个问题非常容易；只要用逻辑嗅探器捕捉信号，并与股票遥控器进行比较。