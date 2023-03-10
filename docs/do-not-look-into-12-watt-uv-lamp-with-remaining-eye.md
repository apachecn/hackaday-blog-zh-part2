# 不要用剩余的眼睛看 12 瓦的紫外线灯

> 原文：<https://hackaday.com/2012/11/07/do-not-look-into-12-watt-uv-lamp-with-remaining-eye/>

![](img/6f762485da6515c3f66f28b0d6bcfb57.png "PCB")

我们已经看到了一些用于曝光光敏 PCB 和擦除 EPROMs 的 UV 灯，但是 pcboard.ca 的[John]决定[如果值得做，就值得做得过分](http://pcboard.ca/info/pcb_uv_lamp/index.html)。他们设计了一个紫外线曝光板，使用 12 个 1 瓦的紫外线发光二极管，这是一种令人印象深刻的紫外线，你可能不应该看太久。

我们以前见过紫外线曝光箱，[通常由一束 5 毫米的紫外线发光二极管](http://hackaday.com/2012/11/06/ikea-provides-a-great-uv-exposure-box/)焊接在一块原板上制成。这些项目完成了它们的工作，但是曝光时间大约是几分钟。PCboard.ca 紫外灯可以在短短 20 秒内曝光 PCB。

从四块 1 英寸宽、1/8 英寸厚的铝条开始建造。12 个星形发光二极管用热粘合剂粘在这个棒上，作为一个相当大的散热器。

[John] [做了一个小测试](http://pcboard.ca/info/pcb_uv_lamp/expose.html)来确定这个巨大的紫外线源曝光 PCB 需要多长时间。通过复制 PCB 掩模四次并将其放置在未曝光的板上，[John]制作了曝光时间为 60、45、30 和 15 秒的 PCB。[在显影和蚀刻](http://pcboard.ca/info/pcb_uv_lamp/etching.html)之后，除了 15 秒的曝光时间之外，所有的都被完全蚀刻了，这是一个惊人的结果，可能会导致一些非常非常快速的原型制作。

更令人印象深刻的是，该版本仅使用了四个 1 瓦 LED 驱动器。没错，这个紫外灯实际上是以其最大额定值的四分之一工作，或者说每个 LED 大约 285 毫安。不管有没有护目镜，我们都不想看到这东西满负荷运转。