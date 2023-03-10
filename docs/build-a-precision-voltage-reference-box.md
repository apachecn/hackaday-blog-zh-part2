# 构建精密电压基准盒

> 原文：<https://hackaday.com/2015/03/23/build-a-precision-voltage-reference-box/>

所以你刚刚得到了一个老式的测试设备，或者你刚刚买了一个漂亮的新的数字万用表(嗯…我们喜欢新的万用表的味道！)但是它能准确读取电压吗？你怎么能确定？嗯，这就是为什么你应该[给自己建一个电压参考箱](http://www.youtube.com/watch?v=01IBdhcEmOw)的原因。

YouTube[scull com]的最新视频已经覆盖了你。想要一些规格？当然可以。一个精度只有 0.025%的 10v、5v 输出，声音却惊人的 2.5 ppm/℃对于你自己能拼凑出来的东西来说，这很了不起。我们发现有趣的是，他实际上使用了一些易趣部件来完成这个构建。LiPo 电池、USB LiPo 充电电路和升压调节器都来自 ebay。不过不用担心，因为这些器件仅用于为 15 伏线性稳压器供电。真正的奇迹发生在德州仪器 [REF102](http://www.ti.com/product/ref102) 精密基准电压源中。你给它一个相当干净的 12-36 伏，它会给你一个 10 伏的参考输出。这些令人惊叹的芯片能够获得如此高的精度，部分原因是它们在工厂经过校准(或者更具体地说是“激光微调”)。通过使用差分放大器实现 5 伏的次级输出。

警告:休息后的视频有点长(43 分钟)，所以你可能想做一些爆米花。但我们发现(斯卡尔科姆的)教学风格很可爱，他从头到尾都很好地解释了这个项目。

[https://www.youtube.com/embed/01IBdhcEmOw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/01IBdhcEmOw?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)