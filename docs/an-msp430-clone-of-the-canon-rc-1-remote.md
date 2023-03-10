# 佳能 RC-1 遥控器的 MSP430 克隆版

> 原文：<https://hackaday.com/2014/11/09/an-msp430-clone-of-the-canon-rc-1-remote/>

出于我们都同意和不能理解的原因，大多数“专业消费者”单反相机没有机械快门。相反，红外发光二极管被纳入组合，佳能 RC-1 遥控触发器是没有选择尼康的人的快门释放选择。[【维森特】克隆了佳能 RC-1](http://r6500.blogspot.com.es/2014/11/canon-ir-trigger.html) ，但他不是为了省钱才这么做的；这个项目有很多东西要学，制作自己的项目可以让他在未来扩展更多的功能。

在研究佳能 RC-1 的功能时，[Vicente]发现需要做出一些妥协。红外 LED 发射的总功率通常是其光束宽度的函数；波束宽度越小，意味着到达相机红外接收器的光子越多。这也意味着遥控器必须更准确地对准摄像机。最终，[Vicente]决定采用功率更高、光束宽度更窄的 LED，这略低于接收器的最佳波长。这完全是一种折衷的做法，但是其他组件也可以看到类似的性能。

选定 LED 后，[Vicente]继续构建实际的控制器。他选择了低功耗的 MSP430 微控制器，用手表电池和晶体管驱动 LED。放在一块原型板上，它实际上非常接近电视。一切都焊接好了，这足以在大约 5 米远的地方触发他相机的快门。未来的改进包括清理代码，使用晶振使时序更加精确，以及在 MSP430 上实现低功耗模式。