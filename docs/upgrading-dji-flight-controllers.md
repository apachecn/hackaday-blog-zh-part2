# 升级 DJI 飞行控制器

> 原文：<https://hackaday.com/2015/01/04/upgrading-dji-flight-controllers/>

DJI 公司给了我们太受欢迎的幻影系列四轴飞行器，不仅仅是制造最受欢迎的 FPV 系列四轴飞行器。他们的顶级飞行控制器 Naza V2 非常好，能够连接到飞行规划软件，该软件将设置航路点，通过 CAN 总线与外围设备对话，并改进了飞行算法。另一方面，他们的“低价”型号 Naza Light 不能连接到这些漂亮的 can 总线外设，并且在从一侧或另一侧漂移 quad 时有点问题。

纳扎 V2 售价约 300 美元，纳扎灯售价约 170 美元，两者都带有 GPS 模块。V2 和灯里面的硬件完全一样。我们都知道接下来会怎样，对吧？

RC 小组论坛上的[udnham]想出了一种在 Naza Light 上加载更强大的 Naza V2 固件的方法，提供了更便宜的飞行控制器功能，直到现在，只有在更昂贵的 V2 硬件中才能找到。升级包括更好的 GPS 位置和高度保持算法，连接 DJI 外围设备的能力，包括[蓝牙模块](http://www.dji.com/product/btu)、 [iOSD](http://www.dji.com/product/iosd-mark-ii) 和[相机万向节](http://www.dji.com/product/zenmuse-z15-bmpcc)，Octocopter 支持，DJI 数据链调制解调器，以及一系列其他功能。

尽管 DJI 在 170 美元的 Naza Light 和 300 美元的 Naza V2 中使用了相同的硬件，但升级固件需要连接到 DJI 服务器的互联网。[udnham]编写了一个实用程序，可以修改您计算机上的/etc/hosts 文件，运行一个服务，并允许您在 Naza Light 上升级固件。这基本上是一个 130 美元的 DJI 飞行控制器固件升级，只需下载一次。

[udnham] [建立一个网站](http://naza-upgrade.com/)，您可以在这里下载固件更新工具，并通过几个视频展示升级过程和对现有固件的改进。你可以看看下面这些。

[https://www.youtube.com/embed/zmisgphhR8c?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/zmisgphhR8c?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[https://www.youtube.com/embed/E11WtBlkQvA?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/E11WtBlkQvA?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)