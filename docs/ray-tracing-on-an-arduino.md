# Arduino 上的光线跟踪

> 原文：<https://hackaday.com/2014/11/25/ray-tracing-on-an-arduino/>

[Greg]为 Arduino 实现了一个简单的光线跟踪器，作为一个有趣的练习和对处理器进行基准测试的一种方式。他从 [Moller-Trumbore](http://en.wikipedia.org/wiki/M%C3%B6ller%E2%80%93Trumbore_intersection_algorithm) 算法开始，这是一种常见的光线跟踪算法，它计算光线与三角形平面的交点，而不需要预先计算平面。他的代码支持一个静态灯光和一个静态相机，足以渲染一个简单的场景。

[Greg]从一个由几个多边形组成的小场景开始，但是刚刚完成了一个有 505 个顶点，901 个面和反射面的场景(如上图所示)。他在他的电脑模拟器上做了上面的渲染，但是估计在 Arduino 上渲染需要 4 天多一点的时间。[Greg]的项目支持光线的多次反射，这使得他的光线跟踪器不同于我们在之前介绍过的一些[(这也解释了为什么渲染需要这么长时间)。](http://hackaday.com/2012/09/09/3d-games-for-the-arduino-with-raycasting/)

光线跟踪器完全由双精度浮点实现。这意味着大量的软件浮点仿真指令，因为 Arduino 没有浮点单元。虽然由于微控制器的缓慢，这种光线跟踪器不能渲染任何接近实时的图形，但它仍然是一个很好的概念证明。

这篇文章的标题图片是在现代电脑上渲染的，耗时 263 秒。同样的场景以 64×64 的分辨率在 Arduino 上渲染，耗时 4008 秒完成。该渲染在下面。

![ardu](img/e589b0aab011ad0f6c0babb8a9ac0f16.png)