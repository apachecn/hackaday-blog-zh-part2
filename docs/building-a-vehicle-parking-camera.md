# 构建车辆停车摄像头

> 原文：<https://hackaday.com/2013/04/02/building-a-vehicle-parking-camera/>

![rpi-backup-camera](img/1469321be57acb617d5654d0ac90e7c0.png)

我们从来不知道该怎么称呼这些东西。当我们说“备用摄像机”时，它听起来明显像是主摄像机无法工作时的冗余系统。但是当你在汽车里倒车的时候它会被使用。[Jeremy Blythe] [使用树莓 Pi 板作为大脑构建了距离感测视频系统](http://jeremyblythe.blogspot.co.uk/2013/03/raspberry-pi-parking-camera-with.html)。

Linux 的灵活性和 RPi 板的强大功能最终使得一切都可以很容易地协同工作。他使用的是微软 Lifecam Cinema HD 摄像机，它连接到板上的一个 USB 端口。就在上面，你可以看到红外距离传感器，它使用 Adafruit 的 Pi 鹅卵石分线板之一连接到 RPi 的 GPIO 头。这也有利于连接到 176×220 彩色液晶显示屏。

在休息后的视频中，你可以看到[杰里米]在传感器前移动他的手来测试系统。Python 用于从相机中抓取图像，在其上画一个圆，并在底部覆盖以厘米为单位的距离。一旦他的手在 30 厘米以内，覆盖层变成红色，并显示工作停止。相当整洁！

[https://www.youtube.com/embed/XroxIqcuZeA?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/XroxIqcuZeA?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)