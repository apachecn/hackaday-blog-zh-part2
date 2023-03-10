# Kindle 天气和回收显示

> 原文：<https://hackaday.com/2013/04/01/kindle-weather-and-recycling-display/>

![kindle-weather-and-recycling-display](img/d4e777dfd8c5aba4cab3dd6a602c5b91.png)

我们已经看到了相当数量的像这样的黑客，他们重用 Kindle 基本上只是为了它的 ePaper 显示屏。[HaHaBird]把这个装置挂在他的冰箱上，用来显示天气并提醒他回收日的到来。这让我们想知道为什么我们没有在业余爱好市场上看到便宜的 ePaper 模块？

这个概念并不新鲜，但[哈哈伯德]确实将它向前推进了一点点。他开始遵循[Matt]在完成最初的 Kindle 天气显示破解后写的指南。它使用一台独立的计算机运行一个脚本，在互联网上查询天气数据，并生成一个如上图所示的矢量图形。然后 Kindle 每五分钟加载一次图像，这要感谢根设备上的 cron 作业。但是为什么就此打住呢？[HaHaBird]调整了剧本，加入了一个关于他的市政当局不规则回收计划的提醒。

不要忽视这个黑客的硬件方面的质量。由于它在厨房中的突出位置，他想要一个完美的外观。这是通过用樱桃做一个框架，并在背面留出通道来为延长线腾出空间(这样它就可以横向悬挂)和一个固定 Kindle 的栓扣来实现的。关于版本[的更多信息请点击](http://www.reddit.com/r/DIY/comments/1b94nf/kindle_weather_recycling_station/c94qfwu)。