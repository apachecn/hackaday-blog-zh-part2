# 蓝牙低能耗入门

> 原文：<https://hackaday.com/2013/08/29/primer-on-bluetooth-low-energy/>

我们确信，和我们一样，你至少听说过一些关于蓝牙低能耗(BLE)的事情。蓝牙 4.0 是 BLE 的另一个名字，它已经在一些智能手机上使用；从 iPhone 4S、黑莓 10 开始，并在 4.3 中增加了对 Android 的支持——果冻豆。这是您了解该规范的机会。原始资料(我们将在下面讨论)提供了大量的背景知识。但是如果你想要一个简洁的概述，看看[Gervasi 的] [关于蓝牙低能耗的总结](http://www.element14.com/community/groups/wireless/blog/2013/08/23/bluetooth-low-energy)。

我们不会在这里重新发布技术细节，因为两篇文章在这方面做得很好。以下是你应该从 BLE 带走的东西:它是为依靠微小电源运行的设备而设计的。两篇文章中概述的是一个硬币电池。但是我们更愿意想到能源采集的未来。峰值电流限制为 15 mA。这确实限制了吞吐量，但想想传感器，而不是蓝牙耳机。你不需要从这些设备上推送那么多数据。一个巧妙设计的能量收集电路应该能够在没有任何电池的情况下实现 ble 装置。

我们确实提到了对标准的更深入的探索。上面的图片来自于[这本面向开发者的 BLE 初级读本](http://supportforums.blackberry.com/t5/Native-Development-Knowledge/BlackBerry-10-Bluetooth-LE-primer-for-developers/ta-p/2287377)。把它加入到你的周末阅读中。

[via [Reddit](http://www.reddit.com/r/geek/comments/1l966q/bluetooth_low_energy_the_future_of_bluetooth/)