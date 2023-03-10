# 树莓派超级电容

> 原文：<https://hackaday.com/2014/10/04/supercapacitors-for-the-raspberry-pi/>

尽管 Raspberry Pi 功能多样，但它有一个弱点，那就是需要在断电时能够正常关闭，尤其是在处理数据敏感或工业应用程序时。为了解决这个问题，[Pavol Sedlacek]专门为 Raspberry Pi 创造了一种基于超级电容器的 UPS，如果检测到电源故障，它有足够的时间适当地暂停其进程并关闭。

这个装置叫做 Juice4Halt。它使用 DC-DC 转换器从正常电源向 Pi 供电，并在正常工作期间为超级电容器充电。它是双向的，因此在电源故障的情况下，它会反向工作，从电容器获取电源，并将其反馈给 Pi。第二个 DC-DC 转换器处理来自外部电源的电力。

使用超级电容器作为 UPS 的一个副作用是，它们还可以帮助 Pi 度过限电。该项目网站有大量关于该设备功能的细节，包括电路图和源代码。在之前，我们已经见过其他[基于超级电容器的 UPS 装置，但这个特别的装置更加强大，在任何工业或其他敏感环境下都非常适合。](http://hackaday.com/2014/04/03/raspberry-pi-ups-using-supercapacitors/)