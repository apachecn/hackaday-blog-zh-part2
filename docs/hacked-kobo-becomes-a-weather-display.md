# 被黑的 Kobo 变成了天气显示器

> 原文：<https://hackaday.com/2012/10/21/hacked-kobo-becomes-a-weather-display/>

[![](img/bf733f2bb4f15a0ab195ad84f5cdcdd2.png "Kobo Weather Display")](http://hackaday.com/2012/10/21/hacked-kobo-becomes-a-weather-display/kobowifiweathersmall/)

Kobo 电子阅读器已经被黑了一段时间了。通过修改一些文件，很容易启用 telnet 访问。一旦[凯文]能够远程登录到设备并绘制到显示器上，他就创建了 [Kobo Wifi 天气预报](http://www.mobileread.com/forums/showthread.php?t=194376 "Kobo Wifi Weather Forecast ")。这个黑客的灵感来自我们过去讨论过的 Kindle 天气显示，但是这个版本完全运行在 Kobo 上。

天气预报软件是用 pygame 库用 Python 写的。将软件包加载到 Kobo 上后，通过 telnet 运行一些命令来设置 Python 并运行显示。由于 Python 和 pygame 在 Kobo 上运行，它允许直接访问电子墨水显示。

联网的电子墨水设备运行定制图形代码有很多可能性。它要求变成你能想象的任何一种展示。你对定制电子墨水显示器有什么想法？请在评论中告诉我们。