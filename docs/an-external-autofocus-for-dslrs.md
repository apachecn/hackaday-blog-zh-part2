# 单反相机的外置自动对焦

> 原文：<https://hackaday.com/2014/11/12/an-external-autofocus-for-dslrs/>

大多数现代 DSLR 相机支持拍摄全高清视频，这使它们成为视频制作的一个非常便宜的选择。然而，如果你曾经使用过 DSLR 拍摄视频，你可能会遇到一些限制，包括缓慢的自动对焦。

Sensopoda 通过为 DSLR 增加外部自动对焦来解决这个问题。当相机处于手动对焦模式时，该设备驱动镜头上的对焦环。这允许在外部控制器上实现定制的聚焦控制代码。

要聚焦一个物体，需要知道距离。Sensopoda 使用 [HRLV-MaxSonar-EZ](http://www.maxbotix.com/Ultrasonic_Sensors/High_Resolution_Sensors.htm) 超声波传感器来完成这项任务。Arduino 运行一个控制回路，实现一个[卡尔曼滤波器](http://en.wikipedia.org/wiki/Kalman_filter)来平滑输入。然后用它来控制连接在聚焦环上的步进电机。

这个设计很有趣，因为它相当通用；它可以在几乎任何 DSLR 上运行。完整的文章( [PDF](http://files.julian-h.de/sensopoda.pdf) )给出了构建的所有细节。