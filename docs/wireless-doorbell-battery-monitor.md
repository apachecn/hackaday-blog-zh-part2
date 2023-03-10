# 无线门铃电池监控器

> 原文：<https://hackaday.com/2013/03/07/wireless-doorbell-battery-monitor/>

![wireless-doorbell-battery-monitor](img/52e8d1c7c3dc2324c17e5d322b9b2f38.png)

我们确切地知道[丹]正在经历什么。我们还买了一个便宜的无线门铃，并为电池快用完而苦恼。当这种情况发生时，你知道的唯一方法是当人们开始敲门，因为你没有按门铃。对[丹]来说没有更多的了。他建造了一个备用系统来监控钟声装置上的电池电压。

你可以看到他用来放置微控制器和用户界面的一小块原型板。这是一个带有绿色发光二极管和一个按钮的装饰品。这个想法是使用芯片的 ADC 来监控为钟声供电的一对电池的电压水平。当电压降至 3V 以下时，绿色 LED 将亮起。

首先，我们希望这些东西配备更好的电源电路。例如，我们刚刚更换了 Apple TV 遥控器中的 CR2032，并测量了 2.7V 的电压。该遥控器和蜂鸣器都是由 3V 电源供电的。不能让它们工作到 1.8V 吗？但是我们跑题了。

除了监测电压之外，丹的装置还能计算钟声响起的次数。每八秒钟，它就会以二进制闪烁计数，除非他按下红色按钮清除计数。休息后的视频中显示了这一点。我们猜测他想知道在电池耗尽之前这东西能使用多少次。

说真的，对于这样一个很少使用的物品，使用环境光采集来帮助节省电池有多难？查看一些室内太阳能采集数据可以发现，只靠光伏发电可能是不可能的，但是如果有一个超级电容器，它可以从太阳能电池板获得涓涓细流，但当它耗尽时仍然会使用电池，那会怎么样？

[https://www.youtube.com/embed/TOxmkhh5-6c?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/TOxmkhh5-6c?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)