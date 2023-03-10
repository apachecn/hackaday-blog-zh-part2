# THP 参赛作品:数码大幅面相机

> 原文：<https://hackaday.com/2014/07/07/thp-entry-a-digital-large-format-camera/>

[![Click to embiggen. It's seriously worth it.](img/86b728b31f16a4120b446e2f45dd5516.png)](https://hackaday.com/wp-content/uploads/2014/07/largeformatcamera.jpg)

Click to embiggen. It’s seriously worth it.

经过 20 年左右的发展，数码相机可能很快就会在几乎所有方面都优于胶片，但也有一些利基市场，胶片相机占据主导地位。例如，大画幅相机能够拍摄出令人惊叹的图像，但是如果没有一天几千美元的租金，你可能永远也不会得到一台。因为他参加了 Hackaday 奖..alzen]决定建造一台[*数码*大幅面相机](http://hackaday.io/project/1762-Large-Format-Camera)，使用一种如今不常使用的有趣设备——线性 CCD。

[吉米]的相机是围绕一个 [TAOS TS1412S](http://www.mouser.com/ProductDetail/ams/TSL1412S/?qs=3f1SISAG10INP9cTgrIjnw==) 构建的，这是一个能够捕捉 1536 像素宽的光线的线性 CCD。模拟值从这个芯片中按顺序输出，直接进入 Arduino 进行处理、保存和在小屏幕上显示。

在相机内部，传感器位于一对轨道上，并在步进电机的帮助下驱动穿过焦平面。其效果类似于我们过去见过的[平板扫描仪到相机的转换](http://hackaday.com/2009/12/29/panoramic-scanner-camera/)，但是【Jimmy】能够简单地通过改变传感器的积分时间来调整相机的曝光。他还可以改变扫描每列像素之间的延迟，从而创造出一些非常酷的长曝光摄影技术；图像的一面可能是在中午拍摄的，而另一面可能是美丽的日落。如果没有相机外的重要数字操作，这是你做不到的。

* * *

![SpaceWrencher](img/4892437613088ab3882681a2ec04a2bb.png) **本帖介绍的项目是[黑客大奖](http://hackaday.io/prize)中的一个参赛项目。建造一些令人敬畏的东西，赢得太空之旅或数百个其他奖品。**