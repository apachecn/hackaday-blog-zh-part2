# 滑板车电脑，一体式滑板车电脑

> 原文：<https://hackaday.com/2013/05/21/scooterputer-the-all-in-one-scooter-computer/>

![ScootDisplay-2](img/99231d84848d6d8522394923d1de2dc0.png)

在过去的几个月里，我们已经看到了相当多的 carputer 构建包含了 Raspberry Pi，但是即使 Raspi 的能力也无法与 Arduino 驱动的 scooterputer 的强大相抗衡。

像所有令人敬畏的项目一样，这个版本是大量特性蔓延的产物。最初，[Kurt]只想要一个电池电压监控器。用一个 Arduino Duemilanove，一个分压器和一个晚上的编码，[Kurt]很快就做出了一个简单的设备，它有三个 led 来指示电池的状态:低、好或正在充电。

这个项目完成了，直到他偶然发现了一个很棒的有机发光二极管屏幕。使用触摸屏显示器进行电池监控有点过头了，所以[Kurt]去了趟 Sparkfun，拿到了温度传感器、实时时钟、加速度计、GPS 传感器，甚至蜂窝屏蔽。

由此产生的踏板车是车载显示器的杰作:有一个数字速度计和 GPS 单元，蜂窝盾牌作为一个跟踪设备和一种下载踏板车当前位置的实时地图的方式。

虽然大多数电子产品都藏在摩托车的引擎盖下，但显示器当然需要在户外。为了做到这一点，[Kurt]找到了一个很好的外壳，带有一个非常适合有机发光二极管展示的橡胶套。显示器通过 cat5 电缆连接到 Arduino，只要[Kurt]不在飓风中行驶，一切都应该保持良好。

你可以看看下面的视频。

[https://www.youtube.com/embed/WzzKB-dMWsQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/WzzKB-dMWsQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)