# 老式啤酒厂

> 原文：<https://hackaday.com/2013/01/23/vintage-kegerator/>

[![Vintage Kegerator](img/8a1b0022c4d21d7160f32a9fd3c69a4d.png)](http://hackaday.com/2013/01/23/vintage-kegerator/kegerator/)

[Kerber]得到了一台经典的 20 世纪 50 年代的通用电气冰箱，并把它改装成了这台经典的[vintage kegerator](http://imgur.com/a/pcHto "Vintage Kegerator")。

正如他的建造日志所示，这需要一个密集的修复过程才能让这台冰箱恢复原状。他把它完全拆了下来，刮掉了六十年的绝缘材料、玻璃纤维和胶水。然后底盘被打磨光滑，并涂成黑色。添加了 R-19 绝缘材料来代替旧材料。

接下来是电子产品。Arduino、DS18B20 温度传感器和固态继电器用于调节温度和防止啤酒冻结。还有一个每分钟从 Arduino 读取数据的 Guruplug 服务器。它使这些数据可以通过网页访问，因此可以从任何地方监控小桶的温度。[Kerber]承认这是矫枉过正，但为未来的扩张留有余地。

kegerator 消耗约 180 瓦，每小时运行约 6 分钟以保持温度可控。考虑到冰箱的年龄，这是相当可观的。最终的修复看起来很棒，并且和啤酒一起提供数据。