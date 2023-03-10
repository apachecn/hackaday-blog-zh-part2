# 黑客空间监视器监视黑客空间环境

> 原文：<https://hackaday.com/2014/09/09/hackerspace-monitor-monitors-hackerspace-environment/>

黑客空间发生了什么？如果你不能回答这个问题，也许你的空间需要一个[黑客空间监视器](http://taylanayken.wordpress.com/2013/03/22/hackerspace-monitoring-with-raspberry-pi/)。东京黑客空间想出了一种远程监控所有你想知道的关于空间的东西的方法。

他的项目是基于一个树莓 Pi，一个网络摄像头通过集线器连接到 Pi 的 USB 端口。网络摄像头被设置为每秒 2 帧，这足以判断空间中的活动。WiFi 加密狗也插入 USB 集线器，以便访问互联网，发送视频，并允许 SSH 进入 Pi。

如果你正犹豫是否要去做你最喜欢的项目，但目前的天气让你想知道 hackerspace 的温度会是多少？这个项目也涵盖了这一点。现成的温度和湿度传感器直接插入 Pi 的 GPIO 引脚。[Tayken]使用了基于 Python 的包 RPi。GPIO，用于管理温度和湿度传感器读数，以及一个拨动开关，用于监控主门是打开还是关闭。

为了让所有上述信息都显示在网页上，[泰肯]必须做一些花哨的编程。对我们来说幸运的是，他已经让所有的[代码可供下载](https://github.com/tayken/HackerSpace-Monitor)。这不仅为会员提供了极大的便利，而且还可以告诉非会员什么时候去查看“空间”是否合适。