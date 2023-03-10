# 为多普勒运动传感器制作电子设备

> 原文：<https://hackaday.com/2013/08/14/making-the-electronics-for-a-doppler-motion-sensor/>

有许多不同的传感器可用于检测给定环境中的运动。被动红外(PIR)传感器是目前使用最多的，因为它们通过检测移动的热信号来工作。然而，在天气越热的时候，它们就越不可靠，而且显然只对动物和人类有效。

如上图所示的传感器开始出现在互联网上，它们使用多普勒效应来检测运动。我(limpkin) [设计了你需要添加的电子设备](http://www.limpkin.fr/index.php?post/2013/08/09/Making-the-electronics-for-a-%247-USD-doppler-motion-sensor)以便让它们工作。

下面是多普勒效应的一个简单解释:如果你以给定的频率向一个移动的目标发送一个射频信号，那么反射信号的频率就会发生偏移。当一辆汽车鸣响警笛或喇叭接近、经过或远离观察者时，通常会听到这种声音。在接近时，接收频率较高(与发射频率相比),在经过时相同，在后退时较低。

我买的多普勒运动传感器只输出几微伏的非放大信号，其频率代表物体靠近或远离传感器的速度。输出可能非常嘈杂，所以除了放大信号，我还需要过滤掉与普通物体不匹配的频率。

我甚至制作了一个简单的视频来展示结果:

[https://www.youtube.com/embed/q0HEF08JTtI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/q0HEF08JTtI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

所有的文件都可以从我的网站上下载，我还做了一个[募捐活动](https://www.tindie.com/products/limpkin/hb100-doppler-module-with-backpack-1/)，在那里我提到了预计的费用。