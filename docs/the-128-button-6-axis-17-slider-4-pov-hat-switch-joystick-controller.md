# 128 按钮，6 轴，17 滑块，4 视点帽子开关操纵杆控制器

> 原文：<https://hackaday.com/2014/02/14/the-128-button-6-axis-17-slider-4-pov-hat-switch-joystick-controller/>

![stick](img/66203e6cd681f0282040c867a54013b8.png)

Teensy 系列开发板的创造者[Paul Stoffregen]之前为 Teensyduino 实现了一个六轴操纵杆，这是 Teensy 的 Arduino 库。他最初尝试了 8 轴，但是出现了一些问题，最后期限临近了，他就让它保持原样。最近的几个项目让他对如何实现一个超过六轴的操纵杆作为 USB HID 设备有了一些了解，所以他开始研究如何读取 USB 操纵杆的大量罐子和按钮。

到目前为止，最大的问题是弄清楚什么软件实际上可以使用这么多控制的 HID 操纵杆。这个问题的答案是没有。基于 Linux 的 jstest-gtk 能够读取 6+17 个 pots，四个帽子开关，但只能读取 128 个按钮中的 64 个。Teensy 论坛上的一名用户[Pointy]一直在为[开发他自己的游戏杆测试应用程序](http://www.planetpointy.co.uk/joystick-test-application/)，该程序可以在 ~~Linux~~ Windows 上运行，但是在 Windows 上测试游戏杆是一项徒劳的工作，原因无人知晓。

至于为什么有人*想要*一个六轴、17 个滑块、128 个按钮的操纵杆，想想这个:有了这么多的控制，建立 MIDI 控制器来结束所有的 MIDI 控制器，或者为从 C172，737 到 Kerbal 星际巡洋舰的所有东西建立一个驾驶舱模拟器将是相对简单的。这是一个令人印象深刻的控制量，而且都来自一个 20 美元的 Teensy 开发板。

迫切需要对这个小小的操纵杆进行进一步的测试，所以如果你能帮忙，可以在论坛的帖子里留言。