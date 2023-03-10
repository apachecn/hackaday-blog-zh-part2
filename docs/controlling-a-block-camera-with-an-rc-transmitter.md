# 用 RC 发射器控制块摄像机

> 原文：<https://hackaday.com/2014/11/04/controlling-a-block-camera-with-an-rc-transmitter/>

无人机和 FPV 遥控飞机的世界正在迅速扩大，机身越来越大，对更酷的 AV 设备的需求也比以往任何时候都高。[elad]得到了一台能够放大场景的索尼块状摄像机——如果你想近距离拍摄，同时又能保持安全距离，这是一个很好的选择。控制这些相机的变焦通常是通过 RS232 来完成的，[但是【elad】让它与 RC 发射器](http://diydrones.com/profiles/blogs/sony-camera-controlled-trough-rc-transmitter)一起工作。

[elad]正在使用的相机是一台带有标准 SD 分辨率传感器的索尼 FCB-EX11D 块相机。这款相机拥有 10 倍的光学变焦，是空中监控的绝佳解决方案，唯一的问题是 RS232 连接和[VISCA 协议](http://en.wikipedia.org/wiki/VISCA_Protocol)。[elad]使用 Arduino 监听来自 RC 接收器的电梯频道，将其转换为摄像头可以理解的内容。其结果是一个可控变焦的相机，可以很容易地拍摄到天空。

包括 Arduino 和电子设备在内的整个相机包重约 100 克。这与 GoPro 差不多，可以完美地安装在相机的万向节上。唯一的问题是要有一个有足够频道的发射机或其他人在飞行时操作摄像机。下面视频。

[https://www.youtube.com/embed/nPf2kdS5ksQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/nPf2kdS5ksQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)