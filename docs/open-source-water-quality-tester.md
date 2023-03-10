# 开源水质测试仪

> 原文：<https://hackaday.com/2014/10/17/open-source-water-quality-tester/>

水污染在许多第三世界国家是一个大问题。不纯净的水导致许多严重的健康问题，尤其是对儿童而言。安装水净化系统似乎是解决这个问题的简单方法，但选择正确的净化系统取决于水中污染物的水平。

水浊度测试仪通常用于测量水污染的严重程度。不幸的是，大多数商业水浊度测试仪都非常昂贵，所以[Wijnen，Anzalone 和 Pearce]着手开发一种[更实惠的开源测试仪](https://libre3d.com/category/687/Test-Equipment/listings/717/Open-Source-Water-Testing-Platform.html)。他们的测试器性能和商用设备一样好，但成本却低 7-15 倍。

开源水测试仪是用 OpenSCAD 设计的，3d 打印的。它包含一个带有自定义屏蔽的 Arduino，可以测量几个 TSL235R 光频转换器的频率。一个 LED 照亮了水，传感器测量有多少光被水中的颗粒散射和反射。另一个传感器测量 LED 的亮度作为基线参考。根据亮度值计算水的浊度，并显示在字符 LCD 上。关于测试仪的更多细节包含在[一篇相当详尽的论文](https://www.academia.edu/8319858/Open-source_mobile_water_quality_testing_platform)中。

[谢谢安德鲁]