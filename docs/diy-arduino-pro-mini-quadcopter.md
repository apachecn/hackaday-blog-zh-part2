# DIY Arduino Pro 迷你四轴飞行器

> 原文：<https://hackaday.com/2013/03/19/diy-arduino-pro-mini-quadcopter/>

[execUc]买了一架 V929 四轴飞行器，然后[开始做一些巧妙的定制。](http://www.youtube.com/watch?v=8ePVVkbjizY)主要变化–控制电子设备被 Arduino Pro Mini (16Mhz 型号)取代。他将所有的模块焊接在原型板上，虽然不可否认有点重，但这个小家伙飞行起来没有任何问题。

在其他细节中，HMC5883L(磁力计)和 MPU6050(加速度计/陀螺仪)用作传感器。LiPo 7.4V 电池组提供电源。有刷电机由带附加二极管的 SI2302 MOSFET 的脉宽调制控制。他计划将微控制器换成 ARM7 stm32F103 以获得额外的计算能力，并需要调整 PID 值来纠正他在旋转时似乎遇到的一个小问题。

休息之后，请观看试飞视频。[execUc]有他在视频描述中所做的所有改动的完整列表，一定要看完。

[via [被黑的小工具](http://hackedgadgets.com/)

[https://www.youtube.com/embed/8ePVVkbjizY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/8ePVVkbjizY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)