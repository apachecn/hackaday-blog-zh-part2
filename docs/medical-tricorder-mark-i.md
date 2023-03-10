# 医用三记录器标志 I

> 原文：<https://hackaday.com/2014/11/07/medical-tricorder-mark-i/>

一台手持三录仪是启动一个项目的最好理由。源自科幻小说的外形提供了一个在许多不同硬件开发领域工作的机会，如便携式电源、充电、传感器和微控制器之间的通信。当然，您需要一个用户界面，以便返回的值对用户有一定的意义。

[马库斯 B]在他的第一个医用三录仪版本中做得非常好。目前的设计有两个传感器，一个使用红外线测量皮肤温度，另一个是脉冲传感器。

对我们来说，不是传感器的数量使某样东西成为“三录仪”，而是设备使用这些传感器进行诊断的能力(或者给用户足够的提示以得出他们自己的结论)。[Marcus]也有类似的观点，因此他设计了一个实时时钟和一个 SD 卡插槽。这些可用于记录传感器数据随时间的变化，然后能够基于一组已知的常见诊断参数提示疾病。

看着上面的图片，你可能想知道哪个芯片是微控制器。这个建筑实际上是隐藏在下面的 Arduino 人的盾牌。

休息之后有一段演示视频。如果你觉得这令人印象深刻，你一定不想错过 2014 年 Hackaday 奖决赛选手之一的开源科学 Tricorder 。

[https://www.youtube.com/embed/A6dti7zWh9A?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/A6dti7zWh9A?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)