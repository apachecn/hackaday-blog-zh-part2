# 重复使用损坏的喷墨打印机的液晶屏和按钮组件

> 原文：<https://hackaday.com/2014/09/11/re-using-the-lcd-button-assembly-from-a-broken-inkjet-printer/>

喷墨打印机一毛钱一打。你可能已经把旧的打印机拆开来清理像马达、滑轮、皮带、开关、线性杆、电源等部件。这些部件很容易在其他项目中重复使用，不像打印机的控制器部分那样容易使用。[Blaupause]做了一些非常有趣的事情，对于大多数修补者来说，它可能属于“极端困难”类别。他已经从一台无法正常工作的佳能 Pixma 喷墨打印机上取下了前面板，并想出了一种与它连接的方法。

这台打印机的前面板上有你在任何 ole 打印机上都能找到的标准按钮，但是 Pixmas 也有一个小的 LCD 屏幕。[Blaupause]为 Olimexino 微控制器编写了一个库，它可以与重新设计的前面板通信并利用它。这个项目的巧妙之处在于，当涉及到在 LCD 屏幕上显示图像或检查按钮状态时，前面板的板载处理器可以完成繁重的工作，从而解放您的微控制器来做其他任何事情。目前，LCD 屏幕可以显示位图并支持图像透明。该图书馆还不能显示视频，但该选项正在努力。

[Blaupause]在该项目的 Sourceforge 页面上向公众公开他所有的辛勤工作。除了图书馆，他还包括打印机面板引脚和详细信息，如何与按钮和液晶显示屏通信。休息后的视频…

[https://player.vimeo.com/video/49274373](https://player.vimeo.com/video/49274373)

[谢谢帕特]