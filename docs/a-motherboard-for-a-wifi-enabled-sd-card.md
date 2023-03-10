# 支持 WiFi 的 SD 卡的主板

> 原文：<https://hackaday.com/2013/10/09/a-motherboard-for-a-wifi-enabled-sd-card/>

在过去的几个月里，一些非常有能力的黑客参与破解了一个支持 WiFi 的 SD 卡，这个 sd 卡恰好运行一个小型的 Linux 系统。无线 Linux 设备的可能性是巨大的，但是到目前为止，还没有人在这个整洁的硬件上启用任何 IO。[CNLohr]刚刚用[他的主板为这些超越 WiFi SD 卡](http://www.youtube.com/watch?v=-Z9TrZQw16s)帮了我们一个忙，允许小型 Linux 系统与 I2C 设备通信。

该版本基于[【Dmitry】为 Transcend WiFiSD 卡定制的内核](http://hackaday.com/2013/09/19/advanced-transcend-wifi-sd-hacking-custom-kernels-x-and-firefox/)。[CNLohr]对这个系统做了一些探索，发现他可以使用 AVR 以其自定义的 4 位协议与卡对话。

“主板”由某种 ATMega、AVR 编程头、电源和 I2C 总线插座组成。[Lohr]在通过 WiFi 连接到 WiFi 卡并直接向卡上的 Linux 系统发出命令之前，将 LED 阵列连接到 I2C 总线，并使用它来显示 WiFi 卡的一些配置设置。显然，最终的结果是一束闪烁的发光二极管。

虽然这是迄今为止我们见过的最复杂和过度紧张的 LED 闪烁方式，但这是一个很好的概念证明，使超越卡*对各种硬件项目非常有趣。如果你想要你自己的创见主板，【CNLohr】[把所有的文件放到](https://cnlohr.net/pubsvn/electrical/SDComputer/)给任何想蚀刻自己主板的人。*