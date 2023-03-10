# 价格低于 100 美元的 led 激光雷达

> 原文：<https://hackaday.com/2014/01/23/lidar-with-leds-for-under-100/>

如果你的机器人、无人机或其他项目需要某种距离传感器，你有两个选择:一个范围有限的廉价超声波传感器，或一个昂贵的激光系统。LIDAR-Lite 填补了这一空白，它将整个激光雷达模块填充到一个小电路板上。

在传统的激光雷达系统中，激光用于测量光束在传感器和物体之间的飞行时间。该系统需要非常精确的时钟和激光模块，这意味着激光雷达模块至少需要几百美元。LIDAR-Lite 通过闪烁带有“签名”的 LED 并寻找该签名的返回来解决这些问题。这项技术封装在一个 SoC 中，降低了传统激光雷达系统的成本和尺寸。

至于 LIDAR-Lite 规格，它可以感应 40 米以外的物体，精确度为 5%和 95%，通过 I2C 总线与任何微控制器通信，并且足够小，可以适合任何项目。

考虑到现有的机器人和四轴飞行器距离测量解决方案，这种传感器肯定会成为一些非常棒的项目。

编辑:这个[背后的一个家伙在评论中发布了他们的规格表和专利](http://hackaday.com/2014/01/23/lidar-with-leds-for-under-100/#comment-1168221)的链接