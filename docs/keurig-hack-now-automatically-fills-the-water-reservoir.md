# Keurig Hack 现在会自动注满水

> 原文：<https://hackaday.com/2013/06/03/keurig-hack-now-automatically-fills-the-water-reservoir/>

![keurig-automatic-water-fill](img/573adf27427a4ef45d69a3bf2507d28c.png)

这个黑客让你的 Keurig 体验完全自动化。对于那些不熟悉硬件的人来说:这种类型的咖啡机包括一个储水器。一次煮一杯咖啡，方法是从水中汲取，快速加热，然后迫使它通过装有咖啡渣和过滤器的一次性容器。这使用户友好的设计更进一步，通过[自动保持水满](http://forums.parallax.com/showthread.php/148203-Keurig-Auto-Fill-with-BS1-and-Milone-eTape)。

这超越了我们上次看到的水库黑客攻击。那台机器连接了一条水管，但包括一个手动阀门。【Eod_punk】在这个项目中增加了一个电磁阀和液位传感器。液位传感器浸没在水箱中，由基本的 Stamp 微控制器监控。当水位低时，BS1 通过晶体管驱动螺线管，让水流动。这在下面的视频中都有展示。

[https://www.youtube.com/embed/f-w_Y_e3z-Y?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/f-w_Y_e3z-Y?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)