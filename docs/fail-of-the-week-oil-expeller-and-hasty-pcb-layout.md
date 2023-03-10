# 本周失败:石油驱逐者和仓促的 PCB 布局

> 原文：<https://hackaday.com/2014/02/06/fail-of-the-week-oil-expeller-and-hasty-pcb-layout/>

![fotw-oil-extractor-hasty-pcb-layout](img/cdb5b39607db80c509bd14619fe687bf.png)

本周的失败是一箭双雕。左边是[试图加热榨油机](http://www.waldeneffect.org/blog/How_not_to_heat_a_Rajkumar_oil_expeller/)的输出。葵花籽大丰收后，马克拿起榨油机来做自己的食用油。他试图使用焊枪作为热源，但仅仅几分钟后，它就熔化了烙铁的塑料外壳。他正在寻找一个替代热源，但我们想知道为什么他不能扔掉塑料，把它栓在一个散热器上？

右边是仓促 PCB 布局的产物。[Andrew]需要一个 USB 转 GPIO 转换器来配合他的 Android 棒使用。他以前已经制作了几个，自己蚀刻印刷电路板。但是现在他没有时间自己蚀刻，他想他可以设计一个板子的修订版，然后把它伪造出来。结果是[这并不是他所希望的节省时间的方式](http://ncrmnt.org/wp/2013/12/23/a-attiny2313-usb2gpio-adapter-fail/)。丝网标签的位置问题不是什么大问题，但他的 USB 连接器所在的电路板上的“V”字挡住了他试图插入的任何电缆。一点切割解决了这个问题，但他还必须处理弹簧端子，这些端子的引线不符合电路板上钻孔的直径。在提交给 fab house 之前，我们总是会打印出 Gerbers，并将足迹与我们的零件进行比较。但我们不确定这样做是否会发现 USB 电缆间隙问题。在提交你自己的板之前，你使用什么清单？

* * *

**[![2013-09-05-Hackaday-Fail-tips-tile](img/4ddcb45ba24697ecb36e5a2da073e8dc.png)](mailto:tips@hackaday.com?Subject=[Fail of the Week]) 每周失败是一个每周三运行的黑客专栏。通过写下你过去的失败和[给我们发送一个故事的链接](mailto:tips@hackaday.com?Subject=[Fail of the Week])，或者发送你在互联网旅行中发现的失败报道的链接，来帮助保持乐趣。**