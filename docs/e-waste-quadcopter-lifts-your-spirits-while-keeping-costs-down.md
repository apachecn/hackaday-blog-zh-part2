# 电子垃圾四轴飞行器让你精神振奋，同时降低成本

> 原文：<https://hackaday.com/2014/04/01/e-waste-quadcopter-lifts-your-spirits-while-keeping-costs-down/>

在过去的几年里，四轴飞行器及其性能的进步是惊人的。不幸的是，价格点进入运动与体面的大小，非玩具，车辆仍然是数百美元。如果能造出来，买一个又有什么意思呢？！？资金紧张，也有同样的感受，hackerspace Knackatory 的[Hans]决定用电子垃圾制造一架[四轴飞行器。](http://www.youtube.com/watch?v=RmuydYJ-9b8)

+形框架由轻质胶合板制成。很明显，主转子是 PC 风扇，在这种情况下为 140 毫米。通常情况下，除非机载 24v Dewalt 无绳工具电池将风扇速度提升至 15，000 rpm，否则这些风扇无法产生足够的升力以脱离自己的方式。一个橙色风扇允许操作员保持目视参考，以确定直升机的哪一侧向前。

一个运行 [MultiWii](http://www.multiwii.com/) 控制软件的 Arduino 是这架无人机的大脑。MultiWii 软件使用任天堂 Wii 遥控器上的传感器来感知方向和运动。虽然这种四轴飞行器本身没有手持发射器，但与主机的通信由运行 [OpenWRT](http://www.openwrt.org) 的无线路由器处理。路由器是网关，允许 Arduino 和以太网 Shield 组合通过黑客空间的 wifi 网络进行通信。飞行计划是预先编好的。诚然，通过计算机键盘命令进行实时控制需要做一些工作。该团队计划将常规的 USB 游戏控制器与该软件连接起来。

用电子垃圾制造东西是一种很好的回收方式。还记得这个[电子垃圾 3D 打印机](http://hackaday.com/2013/10/13/3d-printer-made-from-e-waste-in-africa/)吗？

![quad-fly](img/35e510b0106d0c2564a0c229a560c301.png)