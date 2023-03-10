# USB 控制的视点荧光棒

> 原文：<https://hackaday.com/2014/11/20/a-usb-controlled-pov-light-stick/>

为了展示他们的 USB LED 条形控制器，[mania cal Labs 的人这个周末制作了一个 POV LED 棒](http://maniacallabs.com/2014/11/19/weekend-project-povstick/)。是的，它与你见过的任何其他 POV LED 显示屏都非常相似；将相机设置为长时间曝光，挥动 POV 荧光棒，在半空中获得一个酷炫的像素图像。不过，这个版本有点不同:它是通过 WiFi 控制的，有一个连接到 WiFi 网络的 Raspberry Pi。

问题中的 USB LED 灯条控制器[是 AllPixel](https://www.kickstarter.com/projects/1101128588/allpixel-usb-interface-for-all-your-led-needs/) ，一个通过 USB 控制 NeoPixels、WS2801、LDP8806 和一系列其他 LED 灯条控制器的小电路板。这个项目使用的棒由两米长的 LPD8806 LEDs 组成，水平分辨率为 96 像素。一个大电池和树莓皮完成了其余的电子设备。

构建 LED POV 显示器与构建 LED 矩阵显示器并没有太大的不同；你所要做的就是将图像分解成单独的列，并按顺序显示它们。为了做到这一点，Maniacal Labs 的人创建了一个 LEDPOV 类。要获得图像，只需打开相机的快门，挥动操纵杆，如果你拍对了，你就会得到一张伟大的 nyan 猫或彩虹扳手的精灵图像。