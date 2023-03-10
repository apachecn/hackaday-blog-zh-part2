# 没有微控制器的自动植物护理

> 原文：<https://hackaday.com/2015/01/19/automatic-plant-care-minus-the-microcontroller/>

植物对大多数栖息地来说都是很好的补充。它们中的许多都有花朵或迷人的叶子，其中一些有助于过滤空气，其他的，如芦荟，有药用价值。虽然有些植物需要很少的护理，但它们在某些时候都需要一点水分。总的来说，植物护理有点复杂:浇水太多，会有根腐的风险；水太少，有脱水致死的危险。Hackaday 的校友凯文·达拉(Kevin Darrah)不愿意在这两种情况下冒险，所以在一个周末的时间里，他用手头的组件建造了一个太阳能自动植物浇水系统。

虽然他身边可能有一两个微控制器，但他没有用过。他的系统是一个金属氧化物半导体场效应晶体管系统，它从一个自动喷虫瓶中触发一个机动泵，从水库中抽水并浇灌植物。太阳能电池板给一组 6800 F 的电容器充电，这些电容器是[凯文]从一个旧接收器中取出的。当达到所需电量时，小型土壤传感器模块通电，评估湿度水平。如果水位低于微调电容器确定的阈值，来自电容器组的电能被转储到水泵，他的植物得到了饮用水。

[凯文]的设计很好地处理了太阳能可能存在的缺陷。他包括了一个 0.1 F 电容，以确保通过系统锁存，并添加了一个泄放电阻，使泵永远不会不必要地供电。运行几天后，他已经看到土壤中的水分调节。他完整的演示和操作理论是在休息之后。如果你对太阳能很感兴趣，但还没准备好放弃太阳能，看看这个由 Arduino 控制的解决口渴的西红柿的方案或者这个由 T2 PIC 供电的植物奶嘴。

[https://www.youtube.com/embed/yT0O2CAHOFU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent](https://www.youtube.com/embed/yT0O2CAHOFU?version=3&rel=1&showsearch=0&showinfo=1&iv_load_policy=1&fs=1&hl=en-US&autohide=2&wmode=transparent)