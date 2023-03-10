# hack let 47–热成像项目

> 原文：<https://hackaday.com/2015/05/15/hacklet-47-thermal-imaging-projects/>

热成像是将物体的热信号转换成人类可见图像的科学。绝对零度以上的任何东西都会散发出一些热量，热成像仪让我们能够看到这一点——即使房间里没有可见光。历史上，热成像系统体积庞大且价格昂贵。早期的系统需要液氮冷却它们的[测辐射热计](http://en.wikipedia.org/wiki/Bolometer "Bolometer")传感器。最近的电子技术进步已经将热成像系统的价格从平流层带到了 300 美元以下——这正是制造商和黑客可以涉足的领域。这正是 Flir 轻子模块和 Seek 热感相机所发生的事情。本周的 Hacklet 是关于 [Hackaday.io 上的热成像项目！](http://hackaday.io/)

[![](img/fa071afbc34a2543c0e8b89987517d32.png)](https://hackaday.io/project/3000) 我们先从【纯工程学】和 [Flir 轻子热感相机突围](https://hackaday.io/project/3000)说起。Flir 的轻子热感相机去年在 Flir One 热感 iPhone 相机中首次亮相时引起了不小的轰动。Flir One 中使用的轻子模块是一个很好的独立单元。接口只需要一个用于设置的 I2C 接口和一个用于图像数据传输的 SPI 接口。实际上使用轻子是一个更大的挑战，主要是因为它的包装。[纯工程]做了一个简单的分线板，使得使用轻子变得容易。它还兼容试验板，这在任何项目的早期阶段都是一个巨大的优势。

![grideye](img/79e60fa9aed17065ffffcd710abefad8.png)接下来是【又名】带[栅眼 BLE 功能的热感相机](https://hackaday.io/project/1389)。这个项目是一个蓝牙低能量(BLE)热感相机使用松下的网格眼 64 像素热传感器。64 像素听起来可能不多，但一个 8×8 的网格足以看到相当多的温度变化。如果你不相信，可以在项目页面上查看一段使用 Grid-EYE 机载有机发光二极管显示器的视频。Grid-EYE 是 2014 年 Hackaday 奖的半决赛选手，我们[去年在【AKA】上刊登了一篇传记。](http://hackaday.com/2014/09/13/thp-hacker-bio-aka/)建造你自己的网格眼唯一困难的部分是获得传感器本身。松下不会把它们卖给任何人，所以你可能要经过几道程序才能买到自己的。

[![pylepton](img/ec4193f8b868ec9f48c7f29607b4aabf.png)](https://hackaday.io/project/5359) 【库尔特·基弗】用[派尔普顿视频叠加](https://hackaday.io/project/5359-pylepton-video-overlay)把 FLIR 轻子带到了树莓派。该项目使用轻子将热数据与 Raspbery Pi 相机模块捕获的图像叠加。轻子通过 PI 的 GPIO 引脚上的 I2C 和 SPI 端口连接。结果是彩色相机图像上的一些黑白热视图的幽灵图像——非常适合您的下一次幽灵狩猎探险！整个项目都是用 Python 实现的，所以很容易在自己的项目中导入和使用 pylepton。[Kurt]甚至给出了一个仅用 5 行代码捕获图像的例子。干得好，[库尔特]！

[![wificam](img/60cb1a061f602d98d7bb3e8c2e026d2a.png)](https://hackaday.io/project/5452) 终于有了【埃里克·比尔】带 [WiFi 热感摄像头](https://hackaday.io/project/5452-wifi-thermal-camera)。[Eric]正在使用 82×62 二极管阵列来创建热图像。与微测辐射热计传感器不同，二极管/热电堆传感器不需要经常校准。它们也比基于微机电系统( [MEMS)](http://en.wikipedia.org/wiki/Microelectromechanical_systems) 的设备更坚固。这个特别的项目使用了来自 Heimann Sensor 的阵列。顾名思义，该传感器与 WiFi 无线电配对，这使得使用它来捕捉和显示数据变得很容易。[Erik]一定是在做正确的事情，因为 WiFi 热感相机刚刚完成了一次非常成功的 Kickstarter，在 4 万美元的初始目标上筹集了 143，126 美元。

你有灵感吗？热像仪可以用来检测建筑物中的热量损失，或者由电气故障产生的热量——这意味着这将是 2015 年[hack aday 奖的一个伟大项目！如果你想看更多的热成像项目，请查看](https://hackaday.io/prize)[热成像项目列表！](https://hackaday.io/list/5819)

这就是本周的 Hacklet，一如既往，下周见。同样的黑时间，同样的黑渠道，带给你最好的 [Hackaday.io！](http://hackaday.io/?utm_source=hackaday&utm_medium=29&utm_campaign=hacklet)