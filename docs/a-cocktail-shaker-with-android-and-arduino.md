# 装有 Android 和 Arduino 的鸡尾酒调酒器

> 原文：<https://hackaday.com/2014/03/08/a-cocktail-shaker-with-android-and-arduino/>

![drinks](img/fe7cfd64c7a635a5314f44875160895d.png)

任何项目中最有回报的部分一定是坐下来第一次看到你的劳动成果开始发挥作用，然后喝一杯好酒放松一下。[托尼·迪科拉]真的展示了他提前思考的能力，因为他的[智能鸡尾酒调酒器](http://learn.adafruit.com/smart-cocktail-shaker/overview)负责建造后的庆祝活动，精确计量饮料。

该建筑借助于一个从港口货物中捡来的小型电子秤(Tony)精确地测量出任何液体的量。他没有尝试与秤中的电子设备接口，而是将一个 INA125 仪表放大器连接到称重传感器。Arduino micro 在称重传感器上测量重量，根据已知的杜松子酒、苦艾酒和卡鲁瓦的密度，[Tony]可以很好地了解鸡尾酒调酒器中有多少液体。

这个版本真正出色的部分是界面:[Tony]为他的平板电脑编写了一个 Android 应用程序，它可以通过一个蓝牙适配器与 Arduino 进行对话。该应用程序接收称重传感器上的当前重量，显示鸡尾酒调酒器中的当前酒量，并提供制作任何鸡尾酒的分步说明。

这是一个方便的小装置，可以放在酒柜周围，加上大量的泵和阀门，可以很容易地成为非常酷的鸡尾酒机器人的基础。

[https://www.youtube.com/embed/gkc7QWlxNpc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/gkc7QWlxNpc?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)