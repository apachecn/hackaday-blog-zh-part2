# RGB 无限远镜

> 原文：<https://hackaday.com/2013/09/04/rgb-infinity-mirror/>

如果你一直在等待一个更详细的指南，然后再开始研究你自己的无限镜， [[Ben]的文章可能是你会发现的最平易近人的一篇](http://www.instructables.com/id/Arduino-controlled-RGB-LED-Infinity-Mirror/?ALLSTEPS)。这种构建使用一组四个电位计来控制模拟 RGB LED 条(这些灯不是单独可寻址的:但这使得编码更简单)。[Ben]从 12V 5A DC 适配器为一切供电，这足以与 Arduino 一起运行 12V RGB 条。

镜子有两种不同的“模式”:独立通道颜色控制和颜色淡化。在第一种模式下，三个电位计分别驱动 RGB 通道。颜色淡化模式有自己的想法，在所有可能的颜色之间滑动；您可以旋转第四个电位计来控制过渡的速度。

下面的视频更好地说明了不同的模式。我们强烈推荐[Ben's]这本优秀的指南，对于那些还没有尝试简单的微控制器练习的人来说，它是第一个理想的项目。查看自由边亚特兰大的无限镜子原型以获得更多灵感。

[https://www.youtube.com/embed/IW5E4i0bzAY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/IW5E4i0bzAY?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)