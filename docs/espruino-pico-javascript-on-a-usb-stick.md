# Espruino Pico，u 盘上的 Javascript

> 原文：<https://hackaday.com/2014/10/29/espruino-pico-javascript-on-a-usb-stick/>

这方面的官方数字可能很少，但 web 开发人员至少*似乎*超过了经常用 c 进行插针和注册的人数。对他们来说，嵌入式世界肯定是一个可怕和不祥的领域，充满了按位操作和动态类型。[Gordon]发现了另一种方法，并为微控制器构建了一个 Javascript 解释器。围绕这个解释器[构建的最新板在 Kickstarter](https://www.kickstarter.com/projects/gfw/espruino-pico-javascript-on-a-usb-stick) 上运行，它比他的早期版本更小，功能更强。

这不是[戈登]的第一次竞技表演；去年[他推出了(全尺寸)Espruino](http://hackaday.com/2013/09/03/the-javascript-of-things/) ，配备了 ARM Cortex M3 [和他自己的 Javascript 解释器](http://hackaday.com/2012/10/05/a-javascript-interpreter-for-arm-micros/)。大型 Espruino 取得了令人振奋的成功，现在他正转向更小的拇指驱动器大小的 Pico。硬件稍微好一点，依靠的是 RAM 稍微多一点的 ARM Cortex M4 STM32F4，这次的板卡稍微便宜一点。不过，它仍然运行相同的 Javascript 解释器，所以所有代码都与您预期的完全一样。

我们还没有看到很多项目使用这种微小的 Javascript，但新的布局确实使它非常有用。根据众筹活动的结果，[Gordon]可能会添加 socket 和 USB HID 支持，以及内嵌 C 函数。