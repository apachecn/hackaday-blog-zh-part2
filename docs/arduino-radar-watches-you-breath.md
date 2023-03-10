# Arduino 雷达观察你的呼吸

> 原文：<https://hackaday.com/2015/08/15/arduino-radar-watches-you-breath/>

我们可能都看过《星际迷航》的一集，并钦佩医务室诊断床上的集成水平。凭借其一套无线传感器和平板显示器，即使是 20 世纪 60 年代对未来的想象也摆脱了现代 ICU 入住的明显有线体验。但我们可能会更接近于[麦考伊博士]对这种基于雷达的呼吸探测器的体验。

[yvind]的构建将术语“试验板”的起源铭记于心，基于一种不便宜的 [Xethru 模块](https://www.xethru.com/shop/x4m200-respiration-sensor.html)，该模块似乎是为检测呼吸而专门构建的。超厚的 PC 板似乎在内部容纳了波导，这是一个巧妙的技巧，但可能会限制模块的部署。该模块需要一个 USB 接口和电平转换器，以便将模块的 2.8V 电平连接到 5V Arduino Uno。在下面的视频中，[yvind]的原型只是点亮了一个 RGB LED，以响应它检测到的胸部运动，但这里还有很多发展潜力。我们之前见过[基于激光的婴儿呼吸监测器](http://hackaday.com/2012/08/21/making-sure-a-baby-is-still-breathing-with-lasers-and-a-wiimote/)；也许这个系统可以用于同样的目的，而不会有弄瞎你的眼睛的危险。或者比在睡眠研究实验室度过一个打扰的夜晚更好的睡眠呼吸暂停患者诊断方法。

传感器板和 USB 接口的价格为 249 美元，这种设计不太适合心脏虚弱或钱包鼓鼓的人。但是作为一个现成的解决方案来满足一个特定的需求，同时也有相当多的黑客攻击的可能性，它可能正是某些人所需要的。当然，如果雷达是你的东西，你可能更愿意做大，造一些能穿墙的东西。

[https://www.youtube.com/embed/hx-wP4jU8a4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/hx-wP4jU8a4?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)