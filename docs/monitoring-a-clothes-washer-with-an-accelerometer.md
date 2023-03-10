# 用加速度计监控洗衣机

> 原文：<https://hackaday.com/2012/07/07/monitoring-a-clothes-washer-with-an-accelerometer/>

![](img/4c800a34ccbbb63821bcb489f9d5fc98.png "accelerometer-based- washing-machine-alert")

[维克多的]洗衣机很好地清洗了他的衣服，但它有点太安静了。机器没有声音警报来让他知道循环已经结束。他决定自己制造一个可以放在机器侧面的闹钟。

你可以看到一对磁铁将电路板固定在洗衣机的金属外壳上。该板实际上没有连接到机器的任何电路，因此这应该对任何单元都同样有效。由于采用了 Freescale MMA7361 三轴加速度计，检测是基于运动的。当他开始洗衣服时，他打开了洗衣板的电源开关。驱动设备的 PIC 12F683 开始监控加速度计的变化。如果超过一分钟没有读数，压电蜂鸣器开始发出蜂鸣声。这是一个有趣而简单的解决方案，与[烤箱预热警报附加功能](http://hackaday.com/2012/03/07/preheat-alarm-added-to-a-basic-kitchen-oven/)一脉相承。