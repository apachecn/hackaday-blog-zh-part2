# 蜡马达为您的项目增添活力

> 原文：<https://hackaday.com/2014/11/10/wax-motors-add-motion-to-your-projects/>

[electronicsNmore]上传了一个关于 wax motors 的[大拆和教程视频](https://www.youtube.com/watch?v=sApyrDEXGAI) (YouTube 链接)。电动[蜡马达](http://en.wikipedia.org/wiki/Wax_motor)在业余电子产品中并不常见，但在家电行业却很常见，这意味着这些马达通常可以从废弃的家电中廉价或免费获得。多年来，非电动蜡马达一直被用作[汽车冷却剂恒温器](http://en.wikipedia.org/wiki/Wax_thermostatic_element)。谁知道呢，这可能只是医生给你下一个项目下的订单。

正如[electronicsNmore]解释的那样，蜡马达是相当简单的设备。一小块蜡被密封在一个带有可移动活塞的金属容器中。加热时，蜡会膨胀，将活塞推出。一旦蜡冷却，一个弹簧帮助将活塞拉回。

真正的诀窍是制造一台无需烹饪就能加热的发动机。这是通过一个[正温度系数(PTC)热敏电阻](http://en.wikipedia.org/wiki/Thermistor#PTC)完成的。顾名思义，PTC 热敏电阻的电阻随着温度的升高而增大。这与我们通常用作温度传感器的负温度系数(NTC)热敏电阻正好相反。PTC 通常用于限制冲击电流的电源或小型加热系统，例如我们的蜡马达。

随着 PTC 加热，其电阻增加，直到停止加热。同时，蜡被加热，从而推出活塞。正如你所料，蜡马达并不是非常有效的设备。[electronics nmore]视频中的马达依靠 120 伏交流电运行。不过，它们确实比螺线管有一些优势。蜡马达提供平稳、缓慢的操作。由于它们是阻性器件，因此也不需要反激二极管，也不会产生螺线管会产生的射频噪声。

[https://www.youtube.com/embed/sApyrDEXGAI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/sApyrDEXGAI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)