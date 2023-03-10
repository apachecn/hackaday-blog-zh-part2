# RasPi 备用电池保证您的数据安全

> 原文：<https://hackaday.com/2013/11/17/battery-backup-for-raspi-keeps-your-data-safe/>

我们都对丢失的数据感到愤怒，这通常是不合理的乐观和缺乏规划的结果。[George]分享了他为最坏情况准备的解决方案:[为 RasPi 及其硬盘驱动器提供备用电源的电路](http://www.repairhub.co.uk/content/resources/raspberry-pi-battery-backup)。[George 的] Pi 设置既可以作为 Apple Time Machine 服务器运行，也可以作为网站备份服务器运行，停电可能会破坏 Pi 连接的硬盘上存储的数据。

然而，[George]没有求助于商业解决方案，而是希望利用 Pi 的低功耗优势，创造一种廉价的定制电路，在断电时安全自动地关闭设备。为了检测电源故障，该构建将 Pi 的一个 GPIOs 连接到一个光隔离器，该光隔离器通过一个齐纳二极管连接到 12V 墙壁适配器:尽管[George]欢迎提供安全识别主电源断电的替代方法的建议。电路的其余部分用作两个附加 9V 电池的涓流充电器，并作为调节器向 RasPi 提供正确的电压。连接到 GPIO 的功率 MOSFETs 处理延迟断电。

您可以查看(和编辑！)[电路在线点击这里](http://www.circuitlab.com/editor/#?id=58j88n)并在【乔治的】网站上找到相关源代码。如果你想建立自己的 RasPi 文件服务器，尝试[将所有部件塞进一个旧的光驱外壳](http://hackaday.com/2013/09/01/build-a-file-server-inside-an-old-external-optical-drive-enclosure/)。