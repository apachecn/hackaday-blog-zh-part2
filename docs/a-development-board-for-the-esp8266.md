# 用于 ESP8266 的开发板

> 原文：<https://hackaday.com/2014/11/05/a-development-board-for-the-esp8266/>

[死灵]准备涉足固件开发领域，为大家最喜欢的 WiFi 芯片 ESP8266 开发固件。在此之前，为这个芯片制作一个漂亮的小分线板是个好主意。[这里是](http://ncrmnt.org/wp/2014/11/04/esp8266-and-pl2303hx-gpio-adventures/)，一个带有 USB 到 UART 转换器的板，具有与墨粉转移过程兼容的板艺术。

由于这只是一个将 USB 转换为 ESP8266 可以理解的东西的板，最合理的行动是在那里扔一个 FTDI 芯片，然后就到此为止。我们不建议你这么做。相反，[死灵]使用的是[多产的 PL2303HX](http://prolificusa.com/portfolio/pl2303hx-rev-d-usb-to-serial-bridge-controller/) 。串行芯片上的 RTS/DTR 引脚没有被使用，只是因为 ESP8266 论坛尚未决定如何将它们连接到 WiFi 芯片。多产系统上的 GPIOs 是为[死灵]考虑的一些其他项目开发的，有一个用户空间驱动程序来使一切工作。

[死灵] [是 Antares](http://hackaday.io/project/1470-antares-linux-kernel-like-buildsystem-for-ucs) 的创造者，Antares 是一个微控制器构建系统，也是 Hackaday 奖的参赛作品。他打算让他的构建系统与这种 WiFi 芯片兼容，只要其他人找到一种简单的方法让它工作。