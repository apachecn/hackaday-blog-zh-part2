# L3D 立方体消除了建造 LED 立方体的工作

> 原文：<https://hackaday.com/2014/11/29/l3d-cube-takes-the-work-out-of-building-an-led-cube/>

建造一个 LED 立方体通常意味着大量精细的焊接工作。弯曲夹具、装配夹具和大量的耐心是这个游戏的名字。如果你想用 RGB LEDs 来建造，这个问题会更加复杂。[肖恩和亚历克斯]希望用他们的 [L3D 魔方](https://www.kickstarter.com/projects/lookingglass/l3d-cube-the-3d-led-cube-from-the-future)改变这一切。是的，L3D 是一个 Kickstarter 活动，但它有足够多的好东西，我们很乐意在 Hackaday 上展示它。[Shawn 和 Alex]所做的是用 WS2812b 表面贴装 led 取代立方体中常用的 5 毫米或 3 毫米通孔 led。不利的一面是，这个立方体在各个方向上都不可见。好的一面是组装变得很容易。

L3D 魔方是开源硬件。源文件可以从独立的[软件](https://github.com/enjrolas/L3D-Software)和[硬件](https://github.com/enjrolas/L3D-Hardware) Github 库获得。不是下周，不是他们达到资金目标的时候，而是现在。我们非常喜欢这一点，希望所有的众筹活动都走这条路。

L3D 魔方使用开源的 [Spark Core](https://www.spark.io/) 作为其处理器和 WiFi 接口。使用 WS2812b 意味着 I/O 引脚减少，并且不需要 LED 驱动芯片。这使得它非常适合像 Spark 或 Arduino 这样的电路板。在软件方面，该团队已经创建了一个[处理库](https://github.com/enjrolas/L3D-library)，这使得无需编码即可轻松创建动画。

L3D 拥有人们期待的 LED 立方体的所有功能——用于环境声音可视化的麦克风和大量内置动画。似乎[Shawn 和 Alex]也创造了某种同步系统，同时允许多个立方体在堆叠时一起工作。该团队希望有人能拿出一个 3D 打印的光漫射器，让这些立方体真正成为 360 度的体验。

L3D 魔方活动进展顺利，[肖恩和亚历克斯]接近翻番他们的 38，000 美元的目标。点击休息时间，查看他们的 Kickstarter 视频！

 <https://d2pq0u4uni88oo.cloudfront.net/projects/1475318/video-469625-h264_high.mp4?_=1>

[https://d2pq0u4uni88oo.cloudfront.net/projects/1475318/video-469625-h264_high.mp4](https://d2pq0u4uni88oo.cloudfront.net/projects/1475318/video-469625-h264_high.mp4)