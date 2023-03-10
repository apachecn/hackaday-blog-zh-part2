# TightLight:3D 投影贴图助手

> 原文：<https://hackaday.com/2013/08/22/tightlight-a-3d-projection-mapping-assistant/>

![tightLight](img/a1c5b6f52f23c93461c74292b43e45cc.png)

任何人都可以拿起投影仪，插上电源，对着墙放电影。然而，如果你想给你的作品增加一些深度——无论是隐喻的还是物理的——你最好开始投影映射。像这些泡沫聚苯乙烯板一样复杂的表面是令人惊叹的显示器的绝佳候选，但不会给你的设置带来额外的复杂性。[Grady] [希望通过 TightLight](http://vimeo.com/72077681) (警告:“音乐”)来缓解一些沉闷。

视频显示了整个映射过程，Arduino 在其中扮演了一个特定的角色。在进行任何投影仪校准之前，[Grady]需要一个精确的投影表面的 3D 模型，这看起来很复杂。好在他有一个 NextEngine 3D 激光扫描仪，当它行驶时，你会看到它照亮了红色的表面。

进入紧光状态:基本上是 20 个连接到 Duemilanove 的 CdS 光电池，每个光电池被放置在 3D 表面上预先标记的点上。快速校准扫描使来自投影仪的光在 X 轴和 Y 轴上滚动，击中每个传感器以确定其准确位置。[Grady]然后使用 [TouchDesigner](http://www.derivative.ca/) 平台将光电池位置数据与早期的 3D 模型合并，然后嘭:一切都排好队，运行良好。