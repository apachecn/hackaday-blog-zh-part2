# PVC 管无线水位传感器

> 原文：<https://hackaday.com/2015/02/13/wireless-water-level-sensor-from-pvc-pipe/>

[鲍勃]很难跟上他的水槽。他必须不断地检查它们，以确保它们不是空的，他总是发现水位比他想象的要低。他决定是时候为这个问题建立自己的解决方案了。他最终得到的是一个由 PVC 管和一些其他部件制成的水位传感器。

物理组装非常简单。整个结构由 1/2″ PVC 管和配件制成，并分成四个几乎相同的传感器模块。传感器的两侧各有一个电极。电极由聚氯乙烯端盖制成，顶端打磨平整。然后在盖子上钻一个孔，以容纳一个小的机器螺钉。在将螺钉打入孔中之前，在螺钉螺纹上涂上接合剂，形成自己的螺纹。这些盖子被放置在 PVC 管的小部分上，这些小部分依次连接到一个四通 PVC 十字接头上。

在电极帽的内侧，两个垫圈放在螺钉上。将绞合线放在垫圈之间，然后用螺母夹紧到位。所有的模块都用几英寸长的管子连接在一起。[Bob]量出了尺寸，使其正好适合他的食槽，但是尺寸可以很容易地改变，以适合任何尺寸的容器。电线都穿过管道向上延伸。聚氯乙烯管粘在一起防水。接合剂防止电极处的任何泄漏。

一根 CAT 5 电缆将电极连接到防水控制器盒内部的电子设备。电子设备很简单。它只是一块简单的 perfboard，带有一个 [XBee](http://hackaday.com/2011/12/18/xbee-remote-sensors-tell-you-when-someone-enters-your-home/ "Xbee sensor") 和几个晶体管。XBee 可以通过测试任何传感器模块的两个电极之间的闭合电路来检测水位。水就像一种开关，关闭电路。当水位过低时，电路断开，[鲍勃]知道水位降低了。XBee 连接到一个 2.4GHz 的定向天线，以确保信号到达几英亩以外的笔记本电脑。

[https://www.youtube.com/embed/rH8x2E_lbng?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/rH8x2E_lbng?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)