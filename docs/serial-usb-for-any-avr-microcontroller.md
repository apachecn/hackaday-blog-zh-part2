# 任何 AVR 微控制器的串行 USB

> 原文：<https://hackaday.com/2013/10/23/serial-usb-for-any-avr-microcontroller/>

如果你正在使用 AVR 微控制器，并且想在项目中增加 USB 接口，有很多选择等着你。LUFA 和 V-USB 都为几乎每个 AVR micro 添加了一些 USB 功能，但如果你想要一个原生串行端口，你唯一的选择是寻找 USB 兼容的 Atmel micros。

[Ray]查看了添加 USB 串行端口的选项，不喜欢他看到的内容；看起来，如果没有第二个更强大的微控制器，这是不可能完成的任务。[然后他有了一个想法](http://rayshobby.net/?p=7363):如果目标只是在计算机和微控制器之间来回传输数据，为什么不写一个 HID 级的 USB 串口呢？

[Ray]将他的项目建立在 V-USB 库的基础上，并创建了一个新的 HID 描述符来在微处理器和计算机之间传输数据。虽然它不能与 Putty 等合适的终端一起工作，但[Ray]设法在处理过程中创建了一个与 Windows、Linux 和 OS X 兼容的串行监控程序。

在下面的视频中，你可以看到[Ray]使用 ATmega328p 和标准的 V-USB 设置。作为概念验证，他正在传输光敏电阻的模拟值，但几乎所有适用于普通串行端口的东西都将适用于[Ray]的库。

[https://www.youtube.com/embed/bTlM27jzOIQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/bTlM27jzOIQ?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)