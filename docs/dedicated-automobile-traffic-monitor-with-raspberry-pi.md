# 带树莓派的专用汽车交通监控器

> 原文：<https://hackaday.com/2015/01/06/dedicated-automobile-traffic-monitor-with-raspberry-pi/>

[j3tstream]想要一种更简单的方法来[监控他所在区域道路上的交通](http://www.weirdlab.fr/?p=581 "traffic monitor")。具体来说，他想在开车时从车里监控道路。这意味着它需要易于使用，不要太分散注意力。

[j3tstream]认为他可以使用树莓 Pi 来运行系统。这将使事情变得容易，因为他将拥有一个完整的 Linux 系统。Pi 的功耗相对较低，所以它是通过汽车点烟器适配器运行的。[j3tstream]确实需要在 Pi 中添加一个自定义的电源按钮。这允许系统正常启动和关闭，防止系统文件被损坏。

在搜索了易贝之后，[j3tstream]发现了一款便宜的 3.2 英寸 TFT LCD 触摸屏显示器，可以很好地显示交通数据。显示器很容易与 Pi 一起工作。[j3tstream]使用了 Raspbian linux 发行版。他的项目页面包括一个下载 Raspbian 图像的链接，该图像已经包含了使用 LCD 屏幕的必要模块。一旦图像被加载，所有需要做的就是使用内置的操作系统功能来校准屏幕。

该系统仍然需要数据连接。为了使事情变得简单和便宜，[j3tstream]使用了 USB WiFi 加密狗。然后，Pi 连接到他的 4G 手机内置的 WiFi 热点。要查看交通地图，[j3tstream]只需连接到一个显示他所在区域交通状况的网站。

最后的步骤是尽可能自动化。毕竟，你不想在开车的时候摸索着用一点点触摸屏。[j3tstream]对 LXDE 自动启动文件进行了一些编辑。这些更改会自动将浏览器以全屏模式加载到交通网站。现在，当[j3tstream]启动他的 Pi 时，它会自动连接到他的 WiFi 热点，并加载本地交通地图。