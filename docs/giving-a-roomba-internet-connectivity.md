# 为 Roomba 提供互联网连接

> 原文：<https://hackaday.com/2014/01/11/giving-a-roomba-internet-connectivity/>

![roombahack01_09](img/01f223fd0db0e49ca45fa780d4f3640c.png)

当[Arthur]决定给他的 Roomba 提供互联网连接时，原本应该是有趣的 1 天构建最终变成了充满千钧一发的 3 天旅程。

被[亚瑟]称为科林的 Roomba 已经服役几年了，一旦他得到了电动 Imp，他就有了这个项目的想法。凭借嵌入式 Wi-Fi 和 32 位处理器，所有这些都集成在 SD 卡外形中，电动 Imp 可以非常容易地将“物联网”添加到您能想到的任何东西中。[亚瑟]想要获得 Roomba 的控制权，所以他接入了 SCI ( [串行命令接口](http://www.irobot.cimg/consumer/hacker/Roomba_SCI_Spec_Manual.pdf))。现在，他可以读出 Roomba 的板载传感器数据，包括电池电压、电流消耗，甚至温度。

这是我们喜欢看到的那种走查，因为他是实时走查的，所以你可以体验一路上的所有“惊喜”。例如，他移除了一个外部充电端口，以便为添加的组件腾出空间，但这最终导致了坞站充电器的禁用。然后他发现当 Roomba 充电时，电动 Imp 分线板的输入电压太高，所以他必须引入一个中间电压调节器。但也许路上最大的颠簸是当他在通电时不小心擦过 Roomba 的控制板上的电动 Imp 分线板。幸运的是，损害被隔离到仅仅一个烟雾——一个简单的场效应晶体管。这个项目结果很棒，而且(今天)科林的数据实际上可以通过一个公共的 [Xively feed 看到。](https://xively.com/feeds/811473458)

[https://www.youtube.com/embed/kgPeDa4VdQI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/kgPeDa4VdQI?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)

[](https://arthurguy.co.uk/blog/2013/12/upgrading-colin)