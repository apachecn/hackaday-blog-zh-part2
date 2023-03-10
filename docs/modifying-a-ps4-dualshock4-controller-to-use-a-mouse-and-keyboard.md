# 修改 PS4 Dualshock4 控制器以使用鼠标和键盘

> 原文：<https://hackaday.com/2013/12/12/modifying-a-ps4-dualshock4-controller-to-use-a-mouse-and-keyboard/>

[Mori]想用他的键盘和鼠标在 PS4 上玩他最喜欢的游戏，所以[他决定修改他的 Dualshock4 控制器，为它提供自定义输入信号](http://www.softfactory.com.br/index.php/blog/entry/carbon-project-hardware-stuff)。

这种构建的核心是 STM32F407 发现板，它连接到 USB 集线器。为了进行这次黑客攻击，[Mori]撕开了 Dualshock4 控制器，找到了来自操纵杆和按钮的 PCB 痕迹。然后，他使用 STM32F407 和 2 个数模转换器(DAC)来创建类似的信号。对我们来说不幸的是，[森]只公布了原理图，而没有固件。我们猜测，他必须将微控制器配置为 USB 主机，枚举鼠标/键盘，解析 HID 报告，并向控制器提供相应的输入。

休息之后，我们嵌入了黑客攻击的视频。如果你有一台 PS4，你可能也想看看如何[禁用双电击 led](http://hackaday.com/2013/11/29/ps4-controller-leds-suck-the-battery/)。

[https://www.youtube.com/embed/jOj65-Za77Y?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/jOj65-Za77Y?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)