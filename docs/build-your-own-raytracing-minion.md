# 建立你自己的光线追踪工具

> 原文：<https://hackaday.com/2014/11/30/build-your-own-raytracing-minion/>

一个被取消的项目留给了[克雷格]六个基于 Raspberry Pi 的设备，他称之为“小黄人”。minion 是一个小外壳中的树莓 Pi 型号 A，配有 Adafruit 2.2 英寸 320×240 SPI LCD。LCD 位于底座上方的棒棒糖式圆形外壳中。[克雷格]发现他的一个手下可以作为桌面光线追踪器。

Raspberry Pi 非常能够运行视觉光线跟踪器的[持久性，或 POV-Ray](http://en.wikipedia.org/wiki/POV-Ray) 。POV-Ray 是早期基于 PC 的光线跟踪器。POV-Ray 最初发布于 1987 年，是作为一个名为 DKBTrace 的 Amiga 程序的一个端口创建的，它本身也是一个 Unix 光线跟踪器的端口。对于门外汉来说，像 POV-Ray [这样的光线跟踪器可以从字面上跟踪从光源到图像平面的](http://en.wikipedia.org/wiki/Ray_tracing_(graphics))光线。可以想象，Raspberry Pi 的小臂处理器会花费相当多的时间来光线追踪高分辨率图像。不过针对 320×240 的 LCD，还算不错。

(克雷格的)仆人正在运行他自己的软件，他称之为 ArtRays。根据设置文件，ArtRays 可以渲染来自多个来源的图像，包括通过 WiFi 加密狗或本地 SD 卡的互联网。[Craig]提供了一个链接，下载完整的 SD 卡映像来构建您自己的 Minion，而不是浏览设置和软件安装。不过，首先在自己的服务器上进行试验可能是值得的，而不是用 1GB 的下载来毁掉他的服务器。

我们很高兴[克雷格]为他的一个爪牙找到了用武之地，现在我们要看看他对其他五个爪牙做了什么！