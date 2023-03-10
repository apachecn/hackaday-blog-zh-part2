# 伴侣立方圣诞灯改进了新像素

> 原文：<https://hackaday.com/2014/02/20/companion-cube-christmas-lights-improved-with-neopixels/>

![cubes](img/f36867a0d7208790ef0827457f0a0d1b.png)

[Crenn]从 Valve 获得了一系列官方配套立方体灯，但在澳大利亚无法在不使用降压变压器的情况下将它们置于非判断性的荣耀中。他们在工作台上坐了几个月，直到一个想法被孵化出来:[用 Adafruit Neopixel 带](https://www.youtube.com/watch?v=k-oGhfnh02I)代替灯泡，让这些奇妙的无生命朋友成为一串可单独寻址的 RGB LEDs。

转换这些立方体的过程需要在内部填充一个非常小的 9.4 毫米 PCB。感谢墨尔本黑客空间的一些课程，这个 PCB 是用 KiCAD 设计的。电路板文件被发送出去，PCB 被接收，焊接起来，塞进立方体。

使用[新像素库](https://github.com/adafruit/Adafruit_NeoPixel)通过带有单个 IO 引脚的 Duemilanove 进行控制。所有的代码、电路板文件和原理图都可以在[的 gits](https://github.com/crenn/Companion_Cube_WS2812Bs/) 上找到。未来的改进可能包括 3D 打印电缆浮雕和将 PCB 安全安装到立方体内部的方法。

视频如下。

[https://www.youtube.com/embed/k-oGhfnh02I?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/k-oGhfnh02I?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)