# 使用电视遥控器调暗客厅的灯光

> 原文：<https://hackaday.com/2012/11/20/dimming-the-living-room-lights-using-your-tv-remote/>

![](img/fba7f69aeb7d2ec776e26e1642e9df7d.png "dim-the-lights-using-your-TV-remote")

作为完整家庭影院系统的一部分，[Andy]希望能够在沙发上控制灯光。当他意识到他的电视遥控器上有他从来不用的按钮时，他开始思考最好的方法。这些控件适用于与电视由同一制造商生产的其他组件。因为他手头没有那个设备，[他自己做了一个红外接收器，用那些不用的按钮来开关灯](http://handya.co.nz/post/36127381687/remote-controlled-home-theatre-lights)。

他使用 AVR 微控制器监控和红外接收器。它通过内置的壁式电源供电。该项目还包括一个固态继电器，能够将主电源切换到照明电路。[Andy]提到使用固态器件意味着您不会听到与机械继电器相关的咔嗒声。一个电气盒扩展被用来给他更多的空间来安装红外接收器和放置他的 DIY 电路板。